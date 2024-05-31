# Comparing `tmp/dbt_af-0.5.1.tar.gz` & `tmp/dbt_af-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_af-0.5.1.tar", max compression
+gzip compressed data, was "dbt_af-0.5.2.tar", max compression
```

## Comparing `dbt_af-0.5.1.tar` & `dbt_af-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      193 2024-05-29 12:50:26.724213 dbt_af-0.5.1/AUTHORS
--rw-r--r--   0        0        0      580 2024-05-29 12:50:26.724213 dbt_af-0.5.1/LICENSE
--rw-r--r--   0        0        0     4722 2024-05-29 12:50:26.724213 dbt_af-0.5.1/README.md
--rw-r--r--   0        0        0       95 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/__init__.py
--rw-r--r--   0        0        0      809 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/backfill_dag_components.py
--rw-r--r--   0        0        0    16775 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/dag_components.py
--rw-r--r--   0        0        0    10831 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/dbt_af_builder.py
--rw-r--r--   0        0        0     2695 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/dbt_model_path_graph_builder.py
--rw-r--r--   0        0        0     5878 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/domain_dag.py
--rw-r--r--   0        0        0     1507 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/maintenance_dag_components.py
--rw-r--r--   0        0        0     4504 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/builder/task_dependencies.py
--rw-r--r--   0        0        0        0 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/common/__init__.py
--rw-r--r--   0        0        0      552 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/common/constants.py
--rw-r--r--   0        0        0     7473 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/common/scheduling.py
--rw-r--r--   0        0        0     1703 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/common/utils.py
--rw-r--r--   0        0        0      330 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/conf/__init__.py
--rw-r--r--   0        0        0    10498 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/conf/config.py
--rw-r--r--   0        0        0     4238 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/dags.py
--rw-r--r--   0        0        0        0 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/__init__.py
--rw-r--r--   0        0        0      200 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/mcd/__init__.py
--rw-r--r--   0        0        0      864 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/mcd/callbacks.py
--rw-r--r--   0        0        0     1610 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/mcd/dbt_core.py
--rw-r--r--   0        0        0      274 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/tableau/__init__.py
--rw-r--r--   0        0        0     1273 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/tableau/auth.py
--rw-r--r--   0        0        0      127 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/tableau/exceptions.py
--rw-r--r--   0        0        0     3612 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/integrations/tableau/extracts.py
--rw-r--r--   0        0        0        0 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/__init__.py
--rw-r--r--   0        0        0     9544 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/base.py
--rw-r--r--   0        0        0     1804 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/branch.py
--rw-r--r--   0        0        0     4865 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/kubernetes_pod.py
--rw-r--r--   0        0        0     6238 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/macros.py
--rw-r--r--   0        0        0     2416 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/run.py
--rw-r--r--   0        0        0    18787 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/sensors.py
--rw-r--r--   0        0        0     1021 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/operators/supplemental.py
--rw-r--r--   0        0        0        0 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/parser/__init__.py
--rw-r--r--   0        0        0    13514 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/parser/dbt_node_model.py
--rw-r--r--   0        0        0     1731 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/parser/dbt_profiles.py
--rw-r--r--   0        0        0     2023 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af/parser/dbt_source_model.py
--rw-r--r--   0        0        0       56 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/__init__.py
--rw-r--r--   0        0        0     2880 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/conftest.py
--rw-r--r--   0        0        0      791 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/main.py
--rw-r--r--   0        0        0      316 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/pyproject.toml
--rw-r--r--   0        0        0      923 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/test_af_wait_name_too_long.py
--rw-r--r--   0        0        0     2242 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/test_all_dbt_models_exist.py
--rw-r--r--   0        0        0      183 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/test_dbt_node_model.py
--rw-r--r--   0        0        0      924 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
--rw-r--r--   0        0        0      717 2024-05-29 12:50:26.724213 dbt_af-0.5.1/dbt_af_functional_tests/test_kubernetes_profiles.py
--rw-r--r--   0        0        0     2966 2024-05-29 12:50:26.744214 dbt_af-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 12:50:26.744214 dbt_af-0.5.1/scripts/__init__.py
--rw-r--r--   0        0        0     3492 2024-05-29 12:50:26.744214 dbt_af-0.5.1/scripts/mini_dbt_project_generator.py
--rw-r--r--   0        0        0     6400 1970-01-01 00:00:00.000000 dbt_af-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      193 2024-05-31 08:50:46.024286 dbt_af-0.5.2/AUTHORS
+-rw-r--r--   0        0        0      580 2024-05-31 08:50:46.024286 dbt_af-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-31 08:50:46.024286 dbt_af-0.5.2/README.md
+-rw-r--r--   0        0        0       95 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/backfill_dag_components.py
+-rw-r--r--   0        0        0    16775 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/dag_components.py
+-rw-r--r--   0        0        0    10831 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/dbt_af_builder.py
+-rw-r--r--   0        0        0     2695 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/dbt_model_path_graph_builder.py
+-rw-r--r--   0        0        0     5878 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/domain_dag.py
+-rw-r--r--   0        0        0     1507 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/maintenance_dag_components.py
+-rw-r--r--   0        0        0     4504 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/builder/task_dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/common/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/common/constants.py
+-rw-r--r--   0        0        0     7473 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/common/scheduling.py
+-rw-r--r--   0        0        0     1703 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/common/utils.py
+-rw-r--r--   0        0        0      330 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/conf/__init__.py
+-rw-r--r--   0        0        0    10498 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/conf/config.py
+-rw-r--r--   0        0        0     4238 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/dags.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/mcd/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/mcd/callbacks.py
+-rw-r--r--   0        0        0     1610 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/mcd/dbt_core.py
+-rw-r--r--   0        0        0      274 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/tableau/__init__.py
+-rw-r--r--   0        0        0     1273 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/tableau/auth.py
+-rw-r--r--   0        0        0      127 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/tableau/exceptions.py
+-rw-r--r--   0        0        0     3612 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/integrations/tableau/extracts.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/__init__.py
+-rw-r--r--   0        0        0     9544 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/base.py
+-rw-r--r--   0        0        0     1804 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/branch.py
+-rw-r--r--   0        0        0     4865 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0     6238 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/macros.py
+-rw-r--r--   0        0        0     2416 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/run.py
+-rw-r--r--   0        0        0    18787 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/sensors.py
+-rw-r--r--   0        0        0     1140 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/operators/supplemental.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:50:46.024286 dbt_af-0.5.2/dbt_af/parser/__init__.py
+-rw-r--r--   0        0        0    13514 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af/parser/dbt_node_model.py
+-rw-r--r--   0        0        0     1731 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af/parser/dbt_profiles.py
+-rw-r--r--   0        0        0     2023 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af/parser/dbt_source_model.py
+-rw-r--r--   0        0        0       56 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/conftest.py
+-rw-r--r--   0        0        0      791 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/main.py
+-rw-r--r--   0        0        0      316 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/test_af_wait_name_too_long.py
+-rw-r--r--   0        0        0     2242 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/test_all_dbt_models_exist.py
+-rw-r--r--   0        0        0      183 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/test_dbt_node_model.py
+-rw-r--r--   0        0        0      924 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
+-rw-r--r--   0        0        0      717 2024-05-31 08:50:46.028287 dbt_af-0.5.2/dbt_af_functional_tests/test_kubernetes_profiles.py
+-rw-r--r--   0        0        0     2966 2024-05-31 08:50:46.044287 dbt_af-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 08:50:46.044287 dbt_af-0.5.2/scripts/__init__.py
+-rw-r--r--   0        0        0     3492 2024-05-31 08:50:46.044287 dbt_af-0.5.2/scripts/mini_dbt_project_generator.py
+-rw-r--r--   0        0        0     6400 1970-01-01 00:00:00.000000 dbt_af-0.5.2/PKG-INFO
```

### Comparing `dbt_af-0.5.1/LICENSE` & `dbt_af-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/README.md` & `dbt_af-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/__init__.py` & `dbt_af-0.5.2/dbt_af/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/backfill_dag_components.py` & `dbt_af-0.5.2/dbt_af/builder/backfill_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/dag_components.py` & `dbt_af-0.5.2/dbt_af/builder/dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/dbt_af_builder.py` & `dbt_af-0.5.2/dbt_af/builder/dbt_af_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/dbt_model_path_graph_builder.py` & `dbt_af-0.5.2/dbt_af/builder/dbt_model_path_graph_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/domain_dag.py` & `dbt_af-0.5.2/dbt_af/builder/domain_dag.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/maintenance_dag_components.py` & `dbt_af-0.5.2/dbt_af/builder/maintenance_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/builder/task_dependencies.py` & `dbt_af-0.5.2/dbt_af/builder/task_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/common/constants.py` & `dbt_af-0.5.2/dbt_af/common/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/common/scheduling.py` & `dbt_af-0.5.2/dbt_af/common/scheduling.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/common/utils.py` & `dbt_af-0.5.2/dbt_af/common/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/conf/config.py` & `dbt_af-0.5.2/dbt_af/conf/config.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/dags.py` & `dbt_af-0.5.2/dbt_af/dags.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/integrations/mcd/callbacks.py` & `dbt_af-0.5.2/dbt_af/integrations/mcd/callbacks.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/integrations/mcd/dbt_core.py` & `dbt_af-0.5.2/dbt_af/integrations/mcd/dbt_core.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/integrations/tableau/auth.py` & `dbt_af-0.5.2/dbt_af/integrations/tableau/auth.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/integrations/tableau/extracts.py` & `dbt_af-0.5.2/dbt_af/integrations/tableau/extracts.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/base.py` & `dbt_af-0.5.2/dbt_af/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/branch.py` & `dbt_af-0.5.2/dbt_af/operators/branch.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/kubernetes_pod.py` & `dbt_af-0.5.2/dbt_af/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/macros.py` & `dbt_af-0.5.2/dbt_af/operators/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/run.py` & `dbt_af-0.5.2/dbt_af/operators/run.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/sensors.py` & `dbt_af-0.5.2/dbt_af/operators/sensors.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/operators/supplemental.py` & `dbt_af-0.5.2/dbt_af/operators/supplemental.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING
 
 from airflow.operators.python import PythonOperator
 
 from dbt_af.conf import Config
 from dbt_af.integrations.tableau import is_tableau_installed, tableau_extracts_refresh
 
 if TYPE_CHECKING:
     from dbt_af.parser.dbt_node_model import TableauRefreshTaskConfig
 
 
+def _tableau_extracts_refresh_dev(*args, **kwargs) -> None:
+    import logging
+
+    logging.info('tableau_extracts_refresh is disabled in dev mode.')
+    return None
+
+
 class TableauExtractsRefreshOperator(PythonOperator):
-    template_fields: Sequence[str] = ('tableau_refresh_tasks',)
-    template_fields_renderers = {'template_fields_renderers': 'py'}
+    template_fields = tuple()
 
     def __init__(self, tableau_refresh_tasks: 'list[TableauRefreshTaskConfig]', dbt_af_config: Config, **kwargs):
         if not is_tableau_installed():
             raise ImportError('tableauserverclient is not installed. Please install it to use this operator.')
 
         super().__init__(
-            python_callable=tableau_extracts_refresh,
+            python_callable=tableau_extracts_refresh if not dbt_af_config.is_dev else _tableau_extracts_refresh_dev,
             op_kwargs={
                 'tableau_refresh_tasks': tableau_refresh_tasks,
                 'dbt_af_config': dbt_af_config,
             },
             **kwargs,
         )
```

### Comparing `dbt_af-0.5.1/dbt_af/parser/dbt_node_model.py` & `dbt_af-0.5.2/dbt_af/parser/dbt_node_model.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/parser/dbt_profiles.py` & `dbt_af-0.5.2/dbt_af/parser/dbt_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af/parser/dbt_source_model.py` & `dbt_af-0.5.2/dbt_af/parser/dbt_source_model.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/conftest.py` & `dbt_af-0.5.2/dbt_af_functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/main.py` & `dbt_af-0.5.2/dbt_af_functional_tests/main.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/test_af_wait_name_too_long.py` & `dbt_af-0.5.2/dbt_af_functional_tests/test_af_wait_name_too_long.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/test_all_dbt_models_exist.py` & `dbt_af-0.5.2/dbt_af_functional_tests/test_all_dbt_models_exist.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py` & `dbt_af-0.5.2/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/dbt_af_functional_tests/test_kubernetes_profiles.py` & `dbt_af-0.5.2/dbt_af_functional_tests/test_kubernetes_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/pyproject.toml` & `dbt_af-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-af"
-version = "0.5.1"
+version = "0.5.2"
 description = "Distibuted dbt runs on Apache Airflow"
 authors = [
     "Nikita Yurasov <nikitayurasov@toloka.ai>",
     "Igor Safonov <igsaf@toloka.ai>",
     "Evgeny Ermakov <jkermakov@toloka.ai>",
     "Leonid Kozhinov <lkozhinov@toloka.ai>",
 ]
```

### Comparing `dbt_af-0.5.1/scripts/mini_dbt_project_generator.py` & `dbt_af-0.5.2/scripts/mini_dbt_project_generator.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.5.1/PKG-INFO` & `dbt_af-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-af
-Version: 0.5.1
+Version: 0.5.2
 Summary: Distibuted dbt runs on Apache Airflow
 Home-page: https://github.com/Toloka/dbt-af
 License: Apache-2.0
 Keywords: python,airflow,dbt
 Author: Nikita Yurasov
 Author-email: nikitayurasov@toloka.ai
 Requires-Python: >=3.10,<3.12
```

