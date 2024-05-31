# Comparing `tmp/river_core-1.6.0.tar.gz` & `tmp/river_core-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.6.0.tar", last modified: Mon May 27 16:57:57 2024, max compression
+gzip compressed data, was "dist/river_core-1.7.0.tar", last modified: Fri May 31 16:32:48 2024, max compression
```

## Comparing `river_core-1.6.0.tar` & `river_core-1.7.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 16:57:42.000000 river_core-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 16:57:42.000000 river_core-1.6.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 16:57:42.000000 river_core-1.6.0/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-27 16:57:42.000000 river_core-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-27 16:57:57.000000 river_core-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 16:57:42.000000 river_core-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-27 16:57:42.000000 river_core-1.6.0/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42985 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-27 16:57:57.000000 river_core-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-27 16:57:42.000000 river_core-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-31 16:32:37.000000 river_core-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 16:32:37.000000 river_core-1.7.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 16:32:37.000000 river_core-1.7.0/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-31 16:32:37.000000 river_core-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-31 16:32:48.000000 river_core-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-31 16:32:37.000000 river_core-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-31 16:32:37.000000 river_core-1.7.0/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-05-31 16:32:37.000000 river_core-1.7.0/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 16:32:48.000000 river_core-1.7.0/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-31 16:32:48.000000 river_core-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-31 16:32:37.000000 river_core-1.7.0/setup.py
```

### Comparing `river_core-1.6.0/CONTRIBUTING.rst` & `river_core-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/LICENSE.incore` & `river_core-1.7.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/LICENSE.tessolve` & `river_core-1.7.0/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/PKG-INFO` & `river_core-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.6.0
+Version: 1.7.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.6.0/examples/sample-config.ini` & `river_core-1.7.0/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/constants.py` & `river_core-1.7.0/river_core/constants.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/log.py` & `river_core-1.7.0/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/main.py` & `river_core-1.7.0/river_core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,21 @@
     help=
     'Toggle comparison between logs generated by the DuT and the Reference Plugin'
 )
 @click.option(
     '--coverage',
     is_flag=True,
     help='Enable collection of coverage statistics from the DuT plugin')
+@click.option(
+    '--nproc',
+    default=1,
+    help='Number of processes dedicated to rivercore framework')
 @cli.command()
 def compile(config, test_list, coverage, verbosity, dut_stage, ref_stage,
-            compare):
+            compare, nproc):
     '''
         subcommand to compile generated programs.
     '''
     logger.info(constants.header_temp.format(__version__))
     if not config:
         config = check_config()
     # Checking if the flags are ok
@@ -171,15 +175,15 @@
             logger.debug('Auto mode has disabled Ref Plugin')
             ref_stage = None
             if compare:
                 logger.warning(
                     'Compare is enabled\nThis will be generating incomplete reports'
                 )
     rivercore_compile(config, test_list, coverage, verbosity, dut_stage,
-                      ref_stage, compare)
+                      ref_stage, compare, nproc)
 
 
 @click.version_option(version=__version__)
 @click.option('-v',
               '--verbosity',
               default='info',
               help='Set the verbosity level for the framework')
```

### Comparing `river_core-1.6.0/river_core/rivercore.py` & `river_core-1.7.0/river_core/rivercore.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from cerberus import Validator
 from ruamel.yaml import YAML
 yaml = YAML(typ="rt")
 yaml.default_flow_style = False
 yaml.allow_unicode = True
 yaml.compact(seq_seq=False, seq_map=False)
 
+from multiprocessing import Pool
 
 # Misc Helper Functions
 def sanitise_pytest_json(json):
     '''
         Function to sanitise pytest JSONs, removes uncessary logs. 
 
         :param json: JSON to sanitise 
@@ -43,15 +44,14 @@
     for json_row in json:
         # NOTE: Playing with fire here, pytest developers could (potentially) change this
         if json_row.get('$report_type', None) == 'TestReport':
             return_data.append(json_row)
 
     return return_data
 
-
 def generate_coverage_report(output_dir, config, coverage_report,
                              coverage_rank_report, db_files):
     '''
         Function to generate coverage reports after merging databases. 
 
         :param json: JSON to sanitise 
 
@@ -408,15 +408,15 @@
                     "Opening test report for {0} in web-browser".format(suite))
                 webbrowser.open(report_html)
             except:
                 return 1
 
 
 def rivercore_compile(config_file, test_list, coverage, verbosity, dut_flags,
-                      ref_flags, compare):
+                      ref_flags, compare, process_count):
     '''
 
         Function to compile generated assembly programs using the plugin as configured in the config.ini.
 
         :param config_file: Config.ini file for generation
 
         :param test_list: Test List exported from generate sub-command 
@@ -615,67 +615,42 @@
                                 plugin_path=path_to_module)
                 refpm.hook.build()
                 ref_json = refpm.hook.run(module_dir=path_to_module)
             else:
                 logger.warning('Ref Plugin disabled')
 
         ## Comparing Dumps
-        success = True
         if compare:
             test_dict = utils.load_yaml(test_list)
             gen_json_data = []
             target_json_data = []
             ref_json_data = []
-            for test, attr in test_dict.items():
-                test_wd = attr['work_dir']
-                is_self_checking = attr['self_checking']
-                if not is_self_checking:
-                  if not os.path.isfile(test_wd + '/dut.dump'):
-                      logger.error(f'{test:<30} : DUT dump is missing')
-                      test_dict[test]['result'] = 'Unavailable'
-                      test_dict[test]['log'] = "DUT dump is missing"
-                      success = False
-                      continue
-                  if not os.path.isfile(test_wd + '/ref.dump'):
-                      logger.error(f'{test:<30} : REF dump is missing')
-                      test_dict[test]['result'] = 'Unavailable'
-                      test_dict[test]['log'] = "REF dump is missing"
-                      success = False
-                      continue
-                  result, log, insnsize = utils.compare_dumps(test_wd + '/dut.dump', test_wd + '/ref.dump')
-                else:
-                  if not os.path.isfile(test_wd + '/dut.signature'):
-                      logger.error(f'{test:<30} : DUT signature is missing')
-                      test_dict[test]['result'] = 'Unavailable'
-                      test_dict[test]['log'] = "DUT signature is missing"
-                      success = False
-                      continue
-                  result, log = utils.self_check(test_wd + '/dut.signature')
-                  insnsize = utils.get_file_size(test_wd + '/dut.dump')
-                test_dict[test]['num_instr'] = insnsize
-                test_dict[test]['result'] = result
-                test_dict[test]['log'] = log
-                if result == 'Passed':
-                    logger.info(f"{test:<30} : TEST {result.upper()}")
-                else:
-                    success = False
-                    logger.error(f"{test:<30} : TEST {result.upper()}")
-
+            # parallelized
+            success = True
+            items = test_dict.items()
+            with Pool(processes = process_count) as process_pool:
+                output = process_pool.map(logcomparison, items) #Collecting the return values from each process in the Pool
+            #Updating values
+            for i in output:
+                success = success and i[0]
+                test_dict[i[1]]['result'] = i[2]
+                test_dict[i[1]]['log'] = i[3]
+                test_dict[i[1]]['num_instr'] = i[4]
             utils.save_yaml(test_dict, output_dir+'/result_list.yaml')
             failed_dict = {}
             for test, attr in test_dict.items():
                 if attr['result'] == 'Failed' or 'Unavailable' in attr['result']:
                     failed_dict[test] = attr
+
             if len(failed_dict) != 0:
                 logger.error(f'Total Tests that Failed :{len(failed_dict)}')
                 failed_dict_file = output_dir+'/failed_list.yaml'
                 logger.error(f'Saving failed list of tests in {failed_dict_file}')
                 utils.save_yaml(failed_dict, failed_dict_file)
 
-
             # Start checking things after running the commands
             # Report generation starts here
             # Target
             # Move this into a function
             if target_json:
                 json_file = open(target_json[0] + '.json', 'r')
                 target_json_list = json_file.readlines()
@@ -957,15 +932,40 @@
         try:
             import webbrowser
             logger.info("Opening test report in web-browser")
             webbrowser.open(report_html)
         except:
             logger.info("Couldn't open the browser")
 
-
+#Helper function for parallel processing
+#Returns success,test,attr['result'],attr['log'],attr['numinstr']
+def logcomparison(item):
+    test, attr = item
+    test_wd = attr['work_dir']
+    is_self_checking = attr['self_checking']
+    if not is_self_checking:
+        if not os.path.isfile(test_wd + '/dut.dump'):
+            logger.error(f'{test:<30} : DUT dump is missing')
+            return False, test, 'Unavailable', "DUT dump is missing", None
+        if not os.path.isfile(test_wd + '/ref.dump'):
+            logger.error(f'{test:<30} : REF dump is missing')
+            return False, test, 'Unavailable', 'REF dump is missing', None
+        result, log, insnsize = utils.compare_dumps(test_wd + '/dut.dump', test_wd + '/ref.dump')
+    else:
+        if not os.path.isfile(test_wd + '/dut.signature'):
+            logger.error(f'{test:<30} : DUT signature is missing')
+            return False, test, 'Unavailable',"DUT signature is missing", None
+        result, log = utils.self_check(test_wd + '/dut.signature')
+        insnsize = utils.get_file_size(test_wd + '/dut.dump')
+    if result == 'Passed':
+        logger.info(f"{test:<30} : TEST {result.upper()}")
+        return True, test, result, log, insnsize
+    else:
+        logger.error(f"{test:<30} : TEST {result.upper()}")
+        return False, test, result, log, insnsize
 def rivercore_setup(config, dut, gen, ref, verbosity):
     '''
         Function to generate sample plugins 
 
         :param config: Flag to create a sample config.ini 
         
         :param dut: Flag to create a sample DuT plugin
@@ -1119,7 +1119,8 @@
 
         # Write the file out again
         with open(cwd + '/' + ref + '/' + 'conftest.py', 'w') as file:
             file.write(filedata)
 
         logger.info(
             'Created {0} Plugin in the current working directory'.format(ref))
+
```

### Comparing `river_core-1.6.0/river_core/sim_hookspecs.py` & `river_core-1.7.0/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/coverage_report.html` & `river_core-1.7.0/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/report.html` & `river_core-1.7.0/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.7.0/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.7.0/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.7.0/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.7.0/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.7.0/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.7.0/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/templates/style.css` & `river_core-1.7.0/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core/utils.py` & `river_core-1.7.0/river_core/utils.py`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/river_core.egg-info/PKG-INFO` & `river_core-1.7.0/river_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.6.0
+Version: 1.7.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.6.0/river_core.egg-info/SOURCES.txt` & `river_core-1.7.0/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.6.0/setup.py` & `river_core-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.6.0',
+    version='1.7.0',
     zip_safe=False,
 )
```

