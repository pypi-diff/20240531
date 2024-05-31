# Comparing `tmp/rai-workflow-manager-0.0.8.tar.gz` & `tmp/rai-workflow-manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai-workflow-manager-0.0.8.tar", last modified: Fri Sep  8 13:29:50 2023, max compression
+gzip compressed data, was "rai-workflow-manager-0.0.9.tar", last modified: Mon Sep 11 08:02:18 2023, max compression
```

## Comparing `rai-workflow-manager-0.0.8.tar` & `rai-workflow-manager-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.452294 rai-workflow-manager-0.0.8/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/cli/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/cli/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/cli/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-08 13:29:50.000000 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-08 13:29:50.000000 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:29:50.000000 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-08 13:29:50.000000 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-08 13:29:50.000000 rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rel/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rel/batch_config/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/batch_config.rel
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rel/batch_config/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/configure_sources.rel
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/export.rel
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/install_models.rel
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/invoke_solver.rel
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/load_data.rel
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/materialize.rel
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/batch_config/workflow/workflow.rel
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/rel/source_configs/
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/rel/source_configs/config.rel
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:29:50.456294 rai-workflow-manager-0.0.8/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22721 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/rai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-09-08 13:29:40.000000 rai-workflow-manager-0.0.8/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.845241 rai-workflow-manager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-11 08:02:18.845241 rai-workflow-manager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/cli/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/cli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/cli/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-11 08:02:18.000000 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-11 08:02:18.000000 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 08:02:18.000000 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-11 08:02:18.000000 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-11 08:02:18.000000 rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rel/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rel/batch_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/batch_config.rel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rel/batch_config/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/configure_sources.rel
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/export.rel
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/install_models.rel
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/invoke_solver.rel
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/load_data.rel
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/materialize.rel
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/batch_config/workflow/workflow.rel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/rel/source_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/rel/source_configs/config.rel
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 08:02:18.845241 rai-workflow-manager-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.841241 rai-workflow-manager-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 08:02:18.845241 rai-workflow-manager-0.0.9/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23244 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/rai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-09-11 08:02:11.000000 rai-workflow-manager-0.0.9/workflow/utils.py
```

### Comparing `rai-workflow-manager-0.0.8/LICENSE` & `rai-workflow-manager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/PKG-INFO` & `rai-workflow-manager-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-workflow-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: The RelationalAI Workflow Manager for batch runs
 Home-page: https://github.com/RelationalAI/rai-workflow-manager
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-workflow-manager-0.0.8/README.md` & `rai-workflow-manager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/cli/__init__.py` & `rai-workflow-manager-0.0.9/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/cli/args.py` & `rai-workflow-manager-0.0.9/cli/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parser.add_argument(
         "--start-date", help="Start date for model data. Format: 'YYYYmmdd'",
         required=False,
         type=str
     )
     parser.add_argument(
         "--end-date", help="End date for model data. Format: 'YYYYmmdd'",
-        required=True,
+        required=False,
         type=str
     )
     parser.add_argument(
         "--dev-data-dir", help="Directory containing dev data",
         required=False,
         default="../data",
         type=str
```

### Comparing `rai-workflow-manager-0.0.8/cli/runner.py` & `rai-workflow-manager-0.0.9/cli/runner.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/PKG-INFO` & `rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-workflow-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: The RelationalAI Workflow Manager for batch runs
 Home-page: https://github.com/RelationalAI/rai-workflow-manager
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-workflow-manager-0.0.8/rai_workflow_manager.egg-info/SOURCES.txt` & `rai-workflow-manager-0.0.9/rai_workflow_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/__init__.py` & `rai-workflow-manager-0.0.9/rel/__init__.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/batch_config/batch_config.rel` & `rai-workflow-manager-0.0.9/rel/batch_config/batch_config.rel`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/configure_sources.rel` & `rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/configure_sources.rel`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/batch_config/workflow/steps/export.rel` & `rai-workflow-manager-0.0.9/rel/batch_config/workflow/steps/export.rel`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/batch_config/workflow/workflow.rel` & `rai-workflow-manager-0.0.9/rel/batch_config/workflow/workflow.rel`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/rel/source_configs/config.rel` & `rai-workflow-manager-0.0.9/rel/source_configs/config.rel`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/setup.py` & `rai-workflow-manager-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/test/test_utils.py` & `rai-workflow-manager-0.0.9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/__init__.py` & `rai-workflow-manager-0.0.9/workflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version_info__ = (0, 0, 8)
+__version_info__ = (0, 0, 9)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `rai-workflow-manager-0.0.8/workflow/blob.py` & `rai-workflow-manager-0.0.9/workflow/blob.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/common.py` & `rai-workflow-manager-0.0.9/workflow/common.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/constants.py` & `rai-workflow-manager-0.0.9/workflow/constants.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/executor.py` & `rai-workflow-manager-0.0.9/workflow/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from workflow.utils import save_csv_output, format_duration, build_models, extract_date_range, build_relation_path, \
     get_common_model_relative_path
 from workflow.common import EnvConfig, RaiConfig, Source, BatchConfig, Export, FileType
 from workflow.manager import ResourceManager
 from workflow import query as q, paths, rai, constants
 from types import MappingProxyType
 
-
 CONFIGURE_SOURCES = 'ConfigureSources'
 INSTALL_MODELS = 'InstallModels'
 LOAD_DATA = 'LoadData'
 # not supported
 INVOKE_SOLVER = 'InvokeSolver'
 MATERIALIZE = 'Materialize'
 EXPORT = 'Export'
@@ -146,23 +145,35 @@
 
         self._inflate_sources(logger)
         rai.execute_query(logger, rai_config, q.populate_source_configs(self.sources), readonly=False)
 
     def _inflate_sources(self, logger: logging.Logger):
         for src in self.sources:
             logger.info(f"Inflating source: '{src.relation}'")
-            date_range = extract_date_range(logger, self.start_date, self.end_date, src.loads_number_of_days,
-                                            src.offset_by_number_of_days)
+            date_range = []
+            if src.is_date_partitioned:
+                date_range.extend(extract_date_range(logger, self.start_date, self.end_date, src.loads_number_of_days,
+                                                     src.offset_by_number_of_days))
+
             inflated_paths = self.paths_builder.build(logger, date_range, src.relative_path, src.extensions,
                                                       src.is_date_partitioned)
             src.paths = inflated_paths
 
 
 class ConfigureSourcesWorkflowStepFactory(WorkflowStepFactory):
 
+    def _validate_params(self, config: WorkflowConfig, step: dict) -> None:
+        super()._validate_params(config, step)
+        end_date = config.step_params[constants.END_DATE]
+        sources = self._parse_sources(step["sources"])
+        if not end_date:
+            for s in sources:
+                if s.is_date_partitioned:
+                    raise ValueError(f"End date is required for date partitioned source: {s.relation}")
+
     def _required_params(self, config: WorkflowConfig) -> List[str]:
         required_params = [constants.REL_CONFIG_DIR, constants.START_DATE, constants.END_DATE]
         if config.run_mode == WorkflowRunMode.LOCAL:
             required_params.append(constants.LOCAL_DATA_DIR)
         return required_params
 
     def _get_step(self, logger: logging.Logger, config: WorkflowConfig, idt, name, state, timing, engine_size,
@@ -178,15 +189,15 @@
         sources = self._parse_sources(step["sources"])
         start_date = config.step_params[constants.START_DATE]
         end_date = config.step_params[constants.END_DATE]
         return ConfigureSourcesWorkflowStep(idt, name, state, timing, engine_size, step["configFiles"], rel_config_dir,
                                             sources, paths_builder, start_date, end_date)
 
     @staticmethod
-    def _parse_sources(sources: List[Dict],) -> List[Source]:
+    def _parse_sources(sources: List[Dict]) -> List[Source]:
         result = []
         for source in sources:
             if "future" not in source or not source["future"]:
                 relation = source["relation"]
                 relative_path = source["relativePath"]
                 input_format = source["inputFormat"]
                 extensions = source.get("extensions", [input_format])
@@ -208,15 +219,15 @@
         return result
 
 
 class LoadDataWorkflowStep(WorkflowStep):
     collapse_partitions_on_load: bool
 
     def __init__(self, idt, name, state, timing, engine_size, collapse_partitions_on_load):
-        super().__init__(idt, name, state, timing, engine_size,)
+        super().__init__(idt, name, state, timing, engine_size)
         self.collapse_partitions_on_load = collapse_partitions_on_load
 
     def execute(self, logger: logging.Logger, env_config: EnvConfig, rai_config: RaiConfig):
         logger.info("Executing LoadData step..")
 
         missed_resources = rai.execute_relation_json(logger, rai_config, constants.MISSED_RESOURCES_REL)
```

### Comparing `rai-workflow-manager-0.0.8/workflow/manager.py` & `rai-workflow-manager-0.0.9/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/paths.py` & `rai-workflow-manager-0.0.9/workflow/paths.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/query.py` & `rai-workflow-manager-0.0.9/workflow/query.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/rai.py` & `rai-workflow-manager-0.0.9/workflow/rai.py`

 * *Files identical despite different names*

### Comparing `rai-workflow-manager-0.0.8/workflow/utils.py` & `rai-workflow-manager-0.0.9/workflow/utils.py`

 * *Files identical despite different names*

