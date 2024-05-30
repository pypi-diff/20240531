# Comparing `tmp/dagster-1.7.7.tar.gz` & `tmp/dagster-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.7.tar", last modified: Thu May 23 20:22:44 2024, max compression
+gzip compressed data, was "dagster-1.7.8.tar", last modified: Thu May 30 22:04:46 2024, max compression
```

## Comparing `dagster-1.7.7.tar` & `dagster-1.7.8.tar`

### file list

```diff
@@ -1,725 +1,737 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-23 20:22:18.000000 dagster-1.7.7/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:22:18.000000 dagster-1.7.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-23 20:22:18.000000 dagster-1.7.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-23 20:22:44.801151 dagster-1.7.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7214 2024-05-23 20:22:18.000000 dagster-1.7.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.681152 dagster-1.7.7/dagster/
--rw-r--r--   0 root         (0) root         (0)    30281 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52028 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.689152 dagster-1.7.7/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30233 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8271 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30627 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.689152 dagster-1.7.7/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.693152 dagster-1.7.7/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.693152 dagster-1.7.7/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11635 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)      806 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25411 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.713152 dagster-1.7.7/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7873 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     8848 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     9763 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)     4860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py
--rw-r--r--   0 root         (0) root         (0)     5543 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)    12582 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/utils.py
--rw-r--r--   0 root         (0) root         (0)     7493 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5628 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    20781 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)     6153 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    11507 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    30136 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6937 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7315 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    11171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    78592 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    14208 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    11580 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21722 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)    50929 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_impls.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    35407 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22967 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30236 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/README.md
--rw-r--r--   0 root         (0) root         (0)     1244 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2771 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    17161 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4889 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
--rw-r--r--   0 root         (0) root         (0)     4918 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
--rw-r--r--   0 root         (0) root         (0)     4473 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
--rw-r--r--   0 root         (0) root         (0)     2548 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
--rw-r--r--   0 root         (0) root         (0)    14325 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
--rw-r--r--   0 root         (0) root         (0)    10301 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py
--rw-r--r--   0 root         (0) root         (0)     9192 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
--rw-r--r--   0 root         (0) root         (0)     5132 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
--rw-r--r--   0 root         (0) root         (0)    10067 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    70075 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12656 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    29195 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9808 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_based_auto_materialize.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    54423 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8703 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    10018 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5848 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/metadata_set.py
--rw-r--r--   0 root         (0) root         (0)    31381 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/metadata_value.py
--rw-r--r--   0 root         (0) root         (0)     9938 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/source_code.py
--rw-r--r--   0 root         (0) root         (0)    12486 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57718 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27690 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.725151 dagster-1.7.7/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     9183 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    45639 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19238 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    22389 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   104499 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    16727 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11028 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.725151 dagster-1.7.7/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.729151 dagster-1.7.7/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    68093 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.729151 dagster-1.7.7/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/data_version_cache.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    49252 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    18608 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17062 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40877 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9768 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/run_metrics_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    15211 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132126 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5624 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    84694 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.749151 dagster-1.7.7/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.749151 dagster-1.7.7/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.761151 dagster-1.7.7/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3872 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/base_storage.py
--rw-r--r--   0 root         (0) root         (0)     3320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/batch_asset_record_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21051 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   123419 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    33038 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    18101 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14235 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25156 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19736 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     2728 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.773151 dagster-1.7.7/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29231 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    42160 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12950 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18725 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39411 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.681152 dagster-1.7.7/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.785151 dagster-1.7.7/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.785151 dagster-1.7.7/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    61307 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     2306 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42035 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8978 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    46494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.793151 dagster-1.7.7/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/datetime.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.797151 dagster-1.7.7/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    26684 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10818 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/aiodataloader.py
--rw-r--r--   0 root         (0) root         (0)     9782 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5536 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    45800 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    13054 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     1388 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/cronstring.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    32783 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36148 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     4978 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29940 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1483 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-23 20:22:44.809151 dagster-1.7.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6901 2024-05-23 20:22:18.000000 dagster-1.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.962787 dagster-1.7.8/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-30 22:04:21.000000 dagster-1.7.8/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:04:21.000000 dagster-1.7.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-30 22:04:21.000000 dagster-1.7.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-30 22:04:46.962787 dagster-1.7.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7214 2024-05-30 22:04:21.000000 dagster-1.7.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.854788 dagster-1.7.8/dagster/
+-rw-r--r--   0 root         (0) root         (0)    30281 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20880 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.862788 dagster-1.7.8/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.866788 dagster-1.7.8/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52666 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.870788 dagster-1.7.8/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30233 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30627 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.870788 dagster-1.7.8/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.870788 dagster-1.7.8/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.874788 dagster-1.7.8/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18114 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11635 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41311 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.874788 dagster-1.7.8/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.874788 dagster-1.7.8/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25411 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.874788 dagster-1.7.8/dagster/_core/blueprints/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/blueprints/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/blueprints/blueprint.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/blueprints/load_from_yaml.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.874788 dagster-1.7.8/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.890788 dagster-1.7.8/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.890788 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.890788 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     8848 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9763 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_factories/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7493 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    20781 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)     6153 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    11613 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    80214 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    14208 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11589 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21722 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    50929 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule_impls.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    35407 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22967 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30236 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.890788 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/README.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.894788 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    17161 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.894788 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4889 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.894788 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
+-rw-r--r--   0 root         (0) root         (0)    14325 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+-rw-r--r--   0 root         (0) root         (0)    10301 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.894788 dagster-1.7.8/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    66347 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8912 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    28850 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    29195 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9808 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/freshness_based_auto_materialize.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    54423 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8703 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.898788 dagster-1.7.8/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    10018 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/metadata/metadata_set.py
+-rw-r--r--   0 root         (0) root         (0)    32463 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/metadata/metadata_value.py
+-rw-r--r--   0 root         (0) root         (0)    10262 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/metadata/source_code.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57718 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    48442 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27690 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.898788 dagster-1.7.8/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    45639 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39579 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19238 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/step_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.898788 dagster-1.7.8/dagster/_core/definitions/tags/
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/tags/tag_set.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   107028 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    16727 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12404 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.898788 dagster-1.7.8/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.902788 dagster-1.7.8/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    68093 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    18379 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.902788 dagster-1.7.8/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/data_version_cache.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    49252 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    18612 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.906787 dagster-1.7.8/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40877 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9768 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/run_metrics_thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.906787 dagster-1.7.8/dagster/_core/execution/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/scripts/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/scripts/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15211 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.906787 dagster-1.7.8/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.910787 dagster-1.7.8/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.910787 dagster-1.7.8/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.910787 dagster-1.7.8/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132126 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.910787 dagster-1.7.8/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/loader.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.910787 dagster-1.7.8/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    38233 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    84694 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28819 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.914787 dagster-1.7.8/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.922788 dagster-1.7.8/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.922788 dagster-1.7.8/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.934787 dagster-1.7.8/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7307 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/base_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/batch_asset_record_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.934787 dagster-1.7.8/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    26328 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21051 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9417 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   123676 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    33038 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    18253 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14235 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.938787 dagster-1.7.8/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25156 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.942787 dagster-1.7.8/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.942787 dagster-1.7.8/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19736 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.942787 dagster-1.7.8/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.942787 dagster-1.7.8/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.942787 dagster-1.7.8/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29750 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12950 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39411 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.850788 dagster-1.7.8/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.946787 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    61307 2024-05-30 22:04:21.000000 dagster-1.7.8/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.950787 dagster-1.7.8/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42035 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    45851 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.954787 dagster-1.7.8/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/compat/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.958787 dagster-1.7.8/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    26684 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10818 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/aiodataloader.py
+-rw-r--r--   0 root         (0) root         (0)     9782 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    45800 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    13054 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/cronstring.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11253 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)    32783 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/source_position.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.962787 dagster-1.7.8/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36148 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.962787 dagster-1.7.8/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     5089 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     9418 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-30 22:04:22.000000 dagster-1.7.8/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:04:46.858788 dagster-1.7.8/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    30293 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:04:46.000000 dagster-1.7.8/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-30 22:04:46.962787 dagster-1.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6901 2024-05-30 22:04:22.000000 dagster-1.7.8/setup.py
```

### Comparing `dagster-1.7.7/COPYING` & `dagster-1.7.8/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/LICENSE` & `dagster-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/MANIFEST.in` & `dagster-1.7.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/PKG-INFO` & `dagster-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.7
+Version: 1.7.8
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.7/README.md` & `dagster-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/__init__.py` & `dagster-1.7.8/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_annotations.py` & `dagster-1.7.8/dagster/_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,19 +157,21 @@
         setattr(
             target,
             _DEPRECATED_ATTR_NAME,
             DeprecatedInfo(breaking_version, additional_warn_text, subject),
         )
 
         if emit_runtime_warning:
+            stack_level = _get_warning_stacklevel(__obj)
+            subject = subject or _get_subject(__obj)
             warning_fn = lambda: deprecation_warning(
-                subject or _get_subject(__obj),
+                subject,
                 breaking_version=breaking_version,
                 additional_warn_text=additional_warn_text,
-                stacklevel=_get_warning_stacklevel(__obj),
+                stacklevel=stack_level,
             )
             return apply_pre_call_decorator(__obj, warning_fn)
         else:
             return __obj
 
 
 def is_deprecated(obj: Annotatable) -> bool:
@@ -364,18 +366,20 @@
             emit_runtime_warning=emit_runtime_warning,
         )
     else:
         target = _get_annotation_target(__obj)
         setattr(target, _EXPERIMENTAL_ATTR_NAME, ExperimentalInfo(additional_warn_text, subject))
 
         if emit_runtime_warning:
+            stack_level = _get_warning_stacklevel(__obj)
+            subject = subject or _get_subject(__obj)
             warning_fn = lambda: experimental_warning(
-                subject or _get_subject(__obj),
+                subject,
                 additional_warn_text=additional_warn_text,
-                stacklevel=_get_warning_stacklevel(__obj),
+                stacklevel=stack_level,
             )
             return apply_pre_call_decorator(__obj, warning_fn)
         else:
             return __obj
 
 
 def is_experimental(obj: Annotatable) -> bool:
```

### Comparing `dagster-1.7.7/dagster/_api/get_server_id.py` & `dagster-1.7.8/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/list_repositories.py` & `dagster-1.7.8/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/notebook_data.py` & `dagster-1.7.8/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.8/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_job.py` & `dagster-1.7.8/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_partition.py` & `dagster-1.7.8/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_repository.py` & `dagster-1.7.8/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_schedule.py` & `dagster-1.7.8/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_api/snapshot_sensor.py` & `dagster-1.7.8/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_check/README.md` & `dagster-1.7.8/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_check/__init__.py` & `dagster-1.7.8/dagster/_check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -909,15 +909,17 @@
 def mapping_param(
     obj: Mapping[T, U],
     param_name: str,
     key_type: Optional[TypeOrTupleOfTypes] = None,
     value_type: Optional[TypeOrTupleOfTypes] = None,
     additional_message: Optional[str] = None,
 ) -> Mapping[T, U]:
-    if not isinstance(obj, collections.abc.Mapping):
+    ttype = type(obj)
+    # isinstance check against abc is costly, so try to handle common cases with cheapest check possible
+    if not (ttype is dict or isinstance(obj, collections.abc.Mapping)):
         raise _param_type_mismatch_exception(
             obj, (collections.abc.Mapping,), param_name, additional_message=additional_message
         )
 
     if not (key_type or value_type):
         return obj
 
@@ -1099,15 +1101,17 @@
 
 def sequence_param(
     obj: Sequence[T],
     param_name: str,
     of_type: Optional[TypeOrTupleOfTypes] = None,
     additional_message: Optional[str] = None,
 ) -> Sequence[T]:
-    if not isinstance(obj, collections.abc.Sequence):
+    ttype = type(obj)
+    # isinstance check against abc is costly, so try to handle common cases with cheapest check possible
+    if not (ttype is list or ttype is tuple or isinstance(obj, collections.abc.Sequence)):
         raise _param_type_mismatch_exception(
             obj, (collections.abc.Sequence,), param_name, additional_message
         )
 
     if not of_type:
         return obj
 
@@ -1116,17 +1120,19 @@
 
 def opt_sequence_param(
     obj: Optional[Sequence[T]],
     param_name: str,
     of_type: Optional[TypeOrTupleOfTypes] = None,
     additional_message: Optional[str] = None,
 ) -> Sequence[T]:
+    ttype = type(obj)
     if obj is None:
         return []
-    elif not isinstance(obj, collections.abc.Sequence):
+    # isinstance check against abc is costly, so try to handle common cases with cheapest check possible
+    elif not (ttype is list or ttype is tuple or isinstance(obj, collections.abc.Sequence)):
         raise _param_type_mismatch_exception(
             obj, (collections.abc.Sequence,), param_name, additional_message
         )
     elif of_type is not None:
         return _check_iterable_items(obj, of_type, "sequence")
     else:
         return obj
@@ -1169,15 +1175,17 @@
 
 def iterable_param(
     obj: Iterable[T],
     param_name: str,
     of_type: Optional[TypeOrTupleOfTypes] = None,
     additional_message: Optional[str] = None,
 ) -> Iterable[T]:
-    if not isinstance(obj, collections.abc.Iterable):
+    ttype = type(obj)
+    # isinstance check against abc is costly, so try to handle common cases with cheapest check possible
+    if not (ttype is list or ttype is tuple or isinstance(obj, collections.abc.Iterable)):
         raise _param_type_mismatch_exception(
             obj, (collections.abc.Iterable,), param_name, additional_message
         )
 
     if not of_type:
         return obj
```

### Comparing `dagster-1.7.7/dagster/_cli/__init__.py` & `dagster-1.7.8/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/api.py` & `dagster-1.7.8/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/asset.py` & `dagster-1.7.8/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/code_server.py` & `dagster-1.7.8/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/config_scaffolder.py` & `dagster-1.7.8/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/debug.py` & `dagster-1.7.8/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/dev.py` & `dagster-1.7.8/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/instance.py` & `dagster-1.7.8/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/job.py` & `dagster-1.7.8/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/load_handle.py` & `dagster-1.7.8/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/project.py` & `dagster-1.7.8/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/run.py` & `dagster-1.7.8/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/schedule.py` & `dagster-1.7.8/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/sensor.py` & `dagster-1.7.8/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/utils.py` & `dagster-1.7.8/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.8/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/__init__.py` & `dagster-1.7.8/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/config_schema.py` & `dagster-1.7.8/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/config_type.py` & `dagster-1.7.8/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/errors.py` & `dagster-1.7.8/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/evaluate_value_result.py` & `dagster-1.7.8/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/field.py` & `dagster-1.7.8/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/field_utils.py` & `dagster-1.7.8/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/post_process.py` & `dagster-1.7.8/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/primitive_mapping.py` & `dagster-1.7.8/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.8/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.8/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/config.py` & `dagster-1.7.8/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.8/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.8/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.8/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.8/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.8/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/snap.py` & `dagster-1.7.8/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/source.py` & `dagster-1.7.8/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/stack.py` & `dagster-1.7.8/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/traversal_context.py` & `dagster-1.7.8/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/type_printer.py` & `dagster-1.7.8/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_config/validate.py` & `dagster-1.7.8/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.8/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/assets.py` & `dagster-1.7.8/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/code_pointer.py` & `dagster-1.7.8/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/container_context/config.py` & `dagster-1.7.8/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/debug.py` & `dagster-1.7.8/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/decorator_utils.py` & `dagster-1.7.8/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/schema_change_checks.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/utils.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_factories/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.8/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.8/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.8/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.8/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.8/dagster/_core/definitions/asset_dep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from typing import Iterable, NamedTuple, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Iterable, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.asset_spec import AssetSpec
-from dagster._core.definitions.assets import AssetsDefinition
-from dagster._core.definitions.partition_mapping import PartitionMapping
+from dagster._core.definitions.partition_mapping import (
+    PartitionMapping,
+    warn_if_partition_mapping_not_builtin,
+)
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 
 from .events import (
     AssetKey,
     CoercibleToAssetKey,
 )
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.assets import AssetsDefinition
+
+
 CoercibleToAssetDep = Union[
-    CoercibleToAssetKey, AssetSpec, AssetsDefinition, SourceAsset, "AssetDep"
+    CoercibleToAssetKey, AssetSpec, "AssetsDefinition", SourceAsset, "AssetDep"
 ]
 
 
 class AssetDep(
     NamedTuple(
         "_AssetDep",
         [
@@ -50,18 +56,20 @@
                     )
                 ]
             )
     """
 
     def __new__(
         cls,
-        asset: Union[CoercibleToAssetKey, AssetSpec, AssetsDefinition, SourceAsset],
+        asset: Union[CoercibleToAssetKey, AssetSpec, "AssetsDefinition", SourceAsset],
         *,
         partition_mapping: Optional[PartitionMapping] = None,
     ):
+        from dagster._core.definitions.assets import AssetsDefinition
+
         if isinstance(asset, list):
             check.list_param(asset, "asset", of_type=str)
         else:
             check.inst_param(
                 asset, "asset", (AssetKey, str, AssetSpec, AssetsDefinition, SourceAsset)
             )
         if isinstance(asset, AssetsDefinition) and len(asset.keys) > 1:
@@ -71,14 +79,17 @@
                 " Instead, specify dependencies on the assets created by the multi_asset"
                 f" via AssetKeys or strings. For the multi_asset {asset.node_def.name}, the"
                 f" available keys are: {asset.keys}."
             )
 
         asset_key = _get_asset_key(asset)
 
+        if partition_mapping:
+            warn_if_partition_mapping_not_builtin(partition_mapping)
+
         return super().__new__(
             cls,
             asset_key=asset_key,
             partition_mapping=check.opt_inst_param(
                 partition_mapping,
                 "partition_mapping",
                 PartitionMapping,
@@ -88,14 +99,16 @@
     @staticmethod
     def from_coercible(arg: "CoercibleToAssetDep") -> "AssetDep":
         # if arg is AssetDep, return the original object to retain partition_mapping
         return arg if isinstance(arg, AssetDep) else AssetDep(asset=arg)
 
 
 def _get_asset_key(arg: "CoercibleToAssetDep") -> AssetKey:
+    from dagster._core.definitions.assets import AssetsDefinition
+
     if isinstance(arg, (AssetsDefinition, SourceAsset, AssetSpec)):
         return arg.key
     elif isinstance(arg, AssetDep):
         return arg.asset_key
     else:
         return AssetKey.from_coercible(arg)
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.8/dagster/_core/definitions/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,23 @@
 
     @property
     def is_executable(self) -> bool:
         return self.assets_def.is_executable
 
     @property
     def metadata(self) -> ArbitraryMetadataMapping:
-        return self.assets_def.metadata_by_key.get(self.key, {})
+        return self.assets_def.specs_by_key[self.key].metadata or {}
 
     @property
     def tags(self) -> Mapping[str, str]:
         return self.assets_def.tags_by_key.get(self.key, {})
 
     @property
     def owners(self) -> Sequence[str]:
-        return self.assets_def.owners_by_key.get(self.key, [])
+        return self.assets_def.specs_by_key[self.key].owners or []
 
     @property
     def is_partitioned(self) -> bool:
         return self.assets_def.partitions_def is not None
 
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
@@ -106,15 +106,15 @@
 
     @property
     def backfill_policy(self) -> Optional[BackfillPolicy]:
         return self.assets_def.backfill_policy
 
     @property
     def code_version(self) -> Optional[str]:
-        return self.assets_def.code_versions_by_key.get(self.key)
+        return self.assets_def.specs_by_key[self.key].code_version
 
     @property
     def check_keys(self) -> AbstractSet[AssetCheckKey]:
         return self._check_keys
 
     @property
     def execution_set_asset_keys(self) -> AbstractSet[AssetKey]:
@@ -137,14 +137,17 @@
     def execution_type(self) -> AssetExecutionType:
         return self.assets_def.execution_type
 
     @property
     def io_manager_key(self) -> str:
         return self.assets_def.get_io_manager_key_for_asset_key(self.key)
 
+    def to_asset_spec(self) -> AssetSpec:
+        return self.assets_def.specs_by_key[self.key]
+
 
 class AssetGraph(BaseAssetGraph[AssetNode]):
     _assets_defs_by_check_key: Mapping[AssetCheckKey, AssetsDefinition]
 
     def __init__(
         self,
         asset_nodes_by_key: Mapping[AssetKey, AssetNode],
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.8/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.8/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_in.py` & `dagster-1.7.8/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_job.py` & `dagster-1.7.8/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_key.py` & `dagster-1.7.8/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.8/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_out.py` & `dagster-1.7.8/dagster/_core/definitions/asset_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Any, Mapping, NamedTuple, Optional, Sequence, Type, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, experimental_param
+from dagster._core.definitions.asset_dep import AssetDep
+from dagster._core.definitions.asset_spec import AssetSpec
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.events import (
     AssetKey,
     CoercibleToAssetKey,
     CoercibleToAssetKeyPrefix,
 )
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.input import NoValueSentinel
 from dagster._core.definitions.output import Out
 from dagster._core.definitions.utils import DEFAULT_IO_MANAGER_KEY
 from dagster._core.types.dagster_type import DagsterType, resolve_dagster_type
+from dagster._utils.warnings import disable_dagster_warnings
 
 from .utils import validate_tags_strict
 
 
 @experimental_param(param="owners")
 @experimental_param(param="tags")
 class AssetOut(
@@ -131,7 +134,23 @@
             dagster_type=self.dagster_type,
             description=self.description,
             metadata=self.metadata,
             is_required=self.is_required,
             io_manager_key=self.io_manager_key,
             code_version=self.code_version,
         )
+
+    def to_spec(self, key: AssetKey, deps: Sequence[AssetDep]) -> AssetSpec:
+        with disable_dagster_warnings():
+            return AssetSpec(
+                key=key,
+                metadata=self.metadata,
+                description=self.description,
+                skippable=not self.is_required,
+                group_name=self.group_name,
+                code_version=self.code_version,
+                freshness_policy=self.freshness_policy,
+                auto_materialize_policy=self.auto_materialize_policy,
+                owners=self.owners,
+                tags=self.tags,
+                deps=deps,
+            )
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.8/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.8/dagster/_core/definitions/asset_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, NamedTuple, Optional, Sequence
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Sequence,
+)
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, experimental_param
 from dagster._serdes.serdes import whitelist_for_serdes
 
 from .auto_materialize_policy import AutoMaterializePolicy
 from .events import (
@@ -139,9 +147,9 @@
             ),
             auto_materialize_policy=check.opt_inst_param(
                 auto_materialize_policy,
                 "auto_materialize_policy",
                 AutoMaterializePolicy,
             ),
             owners=check.opt_sequence_param(owners, "owners", of_type=str),
-            tags=validate_tags_strict(tags),
+            tags=validate_tags_strict(tags) or {},
         )
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.8/dagster/_core/definitions/asset_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/assets.py` & `dagster-1.7.8/dagster/_core/definitions/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import warnings
+from collections import defaultdict
 from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
     Iterable,
@@ -18,14 +19,15 @@
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import experimental_param, public
 from dagster._core.definitions.asset_check_spec import AssetCheckKey, AssetCheckSpec
+from dagster._core.definitions.asset_dep import AssetDep
 from dagster._core.definitions.asset_layer import get_dep_node_handles_of_graph_backed_asset
 from dagster._core.definitions.asset_spec import (
     SYSTEM_METADATA_KEY_ASSET_EXECUTION_TYPE,
     SYSTEM_METADATA_KEY_AUTO_CREATED_STUB_ASSET,
     SYSTEM_METADATA_KEY_AUTO_OBSERVE_INTERVAL_MINUTES,
     AssetExecutionType,
 )
@@ -43,38 +45,40 @@
     RequiresResources,
     ResourceAddable,
     ResourceRequirement,
     merge_resource_defs,
 )
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
+from dagster._core.definitions.utils import normalize_group_name
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
 )
 from dagster._core.utils import is_valid_email
 from dagster._utils import IHasInternalInit
 from dagster._utils.merger import merge_dicts
 from dagster._utils.security import non_secure_md5_hash_str
-from dagster._utils.warnings import disable_dagster_warnings
+from dagster._utils.warnings import ExperimentalWarning, disable_dagster_warnings
 
+from .asset_spec import AssetSpec
 from .dependency import NodeHandle
 from .events import AssetKey, CoercibleToAssetKey, CoercibleToAssetKeyPrefix
 from .node_definition import NodeDefinition
 from .op_definition import OpDefinition
 from .partition import PartitionsDefinition
 from .partition_mapping import (
     PartitionMapping,
-    get_builtin_partition_mapping_types,
     infer_partition_mapping,
+    warn_if_partition_mapping_not_builtin,
 )
 from .resource_definition import ResourceDefinition
 from .source_asset import SourceAsset
-from .utils import DEFAULT_GROUP_NAME, normalize_group_name, validate_tags_strict
+from .utils import DEFAULT_GROUP_NAME, validate_tags_strict
 
 if TYPE_CHECKING:
     from .base_asset_graph import AssetKeyOrCheckKey
     from .graph_definition import GraphDefinition
 
 ASSET_SUBSET_INPUT_PREFIX = "__subset_input__"
 
@@ -82,35 +86,44 @@
 class AssetsDefinition(ResourceAddable, RequiresResources, IHasInternalInit):
     """Defines a set of assets that are produced by the same op or graph.
 
     AssetsDefinitions are typically not instantiated directly, but rather produced using the
     :py:func:`@asset <asset>` or :py:func:`@multi_asset <multi_asset>` decorators.
     """
 
+    # Constructor arguments that are redundant with the specs argument
+    _dagster_internal_init_excluded_args = {
+        "group_names_by_key",
+        "metadata_by_key",
+        "tags_by_key",
+        "freshness_policies_by_key",
+        "auto_materialize_policies_by_key",
+        "partition_mappings",
+        "descriptions_by_key",
+        "asset_deps",
+        "owners_by_key",
+    }
+
     _node_def: NodeDefinition
     _keys_by_input_name: Mapping[str, AssetKey]
     _keys_by_output_name: Mapping[str, AssetKey]
     _partitions_def: Optional[PartitionsDefinition]
+    # partition mappings are also tracked inside the AssetSpecs, but this enables faster access by
+    # upstream asset key
     _partition_mappings: Mapping[AssetKey, PartitionMapping]
-    _asset_deps: Mapping[AssetKey, AbstractSet[AssetKey]]
     _resource_defs: Mapping[str, ResourceDefinition]
-    _group_names_by_key: Mapping[AssetKey, str]
     _selected_asset_keys: AbstractSet[AssetKey]
     _can_subset: bool
-    _metadata_by_key: Mapping[AssetKey, ArbitraryMetadataMapping]
-    _tags_by_key: Mapping[AssetKey, Mapping[str, str]]
-    _freshness_policies_by_key: Mapping[AssetKey, FreshnessPolicy]
-    _auto_materialize_policies_by_key: Mapping[AssetKey, AutoMaterializePolicy]
     _backfill_policy: Optional[BackfillPolicy]
-    _code_versions_by_key: Mapping[AssetKey, Optional[str]]
-    _descriptions_by_key: Mapping[AssetKey, str]
     _selected_asset_check_keys: AbstractSet[AssetCheckKey]
     _is_subset: bool
-    _owners_by_key: Mapping[AssetKey, Sequence[str]]
 
+    _specs_by_key: Mapping[AssetKey, AssetSpec]
+
+    @experimental_param(param="specs")
     def __init__(
         self,
         *,
         keys_by_input_name: Mapping[str, AssetKey],
         keys_by_output_name: Mapping[str, AssetKey],
         node_def: NodeDefinition,
         partitions_def: Optional[PartitionsDefinition] = None,
@@ -121,19 +134,29 @@
         resource_defs: Optional[Mapping[str, object]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         tags_by_key: Optional[Mapping[AssetKey, Mapping[str, str]]] = None,
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
+        # descriptions by key is more accurately understood as _overriding_ the descriptions
+        # by key that are in the OutputDefinitions associated with the asset key.
+        # This is a dangerous construction liable for bugs. Instead there should be a
+        # canonical source of asset descriptions in AssetsDefinintion and if we need
+        # to create a memoized cached dictionary of asset keys for perf or something we do
+        # that in the `__init__` or on demand.
+        #
+        # This is actually an override. We do not override descriptions
+        # in OutputDefinitions in @multi_asset
         descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         check_specs_by_output_name: Optional[Mapping[str, AssetCheckSpec]] = None,
         selected_asset_check_keys: Optional[AbstractSet[AssetCheckKey]] = None,
         is_subset: bool = False,
         owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
+        specs: Optional[Sequence[AssetSpec]] = None,
         # if adding new fields, make sure to handle them in the with_attributes, from_graph,
         # from_op, and get_attributes_dict methods
     ):
         from dagster._core.execution.build_resources import wrap_resources_for_execution
 
         from .graph_definition import GraphDefinition
 
@@ -160,210 +183,180 @@
             key_type=str,
             value_type=AssetCheckSpec,
         )
 
         all_asset_keys = set(keys_by_output_name.values())
 
         self._partitions_def = partitions_def
-        self._partition_mappings = partition_mappings or {}
-        _validate_partition_mappings(
-            partition_mappings=self._partition_mappings,
-            input_asset_keys=set(keys_by_input_name.values()),
-            all_asset_keys=all_asset_keys,
-        )
+        if partition_mappings:
+            _validate_partition_mappings(
+                partition_mappings=partition_mappings,
+                input_asset_keys=set(keys_by_input_name.values()),
+                all_asset_keys=all_asset_keys,
+            )
 
-        self._asset_deps = asset_deps or {
-            out_asset_key: set(keys_by_input_name.values()) for out_asset_key in all_asset_keys
-        }
-        check.invariant(
-            set(self._asset_deps.keys()) == all_asset_keys,
-            "The set of asset keys with dependencies specified in the asset_deps argument must "
-            "equal the set of asset keys produced by this AssetsDefinition. \n"
-            f"asset_deps keys: {set(self._asset_deps.keys())} \n"
-            f"expected keys: {all_asset_keys}",
-        )
+        if asset_deps:
+            check.invariant(
+                set(asset_deps.keys()) == all_asset_keys,
+                "The set of asset keys with dependencies specified in the asset_deps argument must "
+                "equal the set of asset keys produced by this AssetsDefinition. \n"
+                f"asset_deps keys: {set(asset_deps.keys())} \n"
+                f"expected keys: {all_asset_keys}",
+            )
         self._resource_defs = wrap_resources_for_execution(
             check.opt_mapping_param(resource_defs, "resource_defs")
         )
 
-        group_names_by_key = (
-            check.mapping_param(group_names_by_key, "group_names_by_key")
-            if group_names_by_key
-            else {}
-        )
         self._selected_asset_keys, self._selected_asset_check_keys = _resolve_selections(
             all_asset_keys=all_asset_keys,
             all_check_keys={spec.key for spec in (check_specs_by_output_name or {}).values()},
             selected_asset_keys=selected_asset_keys,
             selected_asset_check_keys=selected_asset_check_keys,
         )
-        self._group_names_by_key = {}
-        # assets that don't have a group name get a DEFAULT_GROUP_NAME
-        for key in all_asset_keys:
-            group_name = group_names_by_key.get(key)
-            self._group_names_by_key[key] = normalize_group_name(group_name)
 
         self._check_specs_by_key = {
             spec.key: spec
             for spec in self._check_specs_by_output_name.values()
             if spec.key in self._selected_asset_check_keys
         }
 
         self._can_subset = can_subset
 
-        self._code_versions_by_key = {}
-        self._metadata_by_key = dict(
-            check.opt_mapping_param(
-                metadata_by_key, "metadata_by_key", key_type=AssetKey, value_type=dict
-            )
+        self._backfill_policy = check.opt_inst_param(
+            backfill_policy, "backfill_policy", BackfillPolicy
         )
 
-        for tags in (tags_by_key or {}).values():
-            validate_tags_strict(tags)
-        self._tags_by_key = tags_by_key or {}
+        if self._partitions_def is None:
+            # check if backfill policy is BackfillPolicyType.SINGLE_RUN if asset is not partitioned
+            check.param_invariant(
+                (
+                    backfill_policy.policy_type is BackfillPolicyType.SINGLE_RUN
+                    if backfill_policy
+                    else True
+                ),
+                "backfill_policy",
+                "Non partitioned asset can only have single run backfill policy",
+            )
+
+        self._is_subset = check.bool_param(is_subset, "is_subset")
+
+        if specs is not None:
+            check.invariant(group_names_by_key is None)
+            check.invariant(metadata_by_key is None)
+            check.invariant(tags_by_key is None)
+            check.invariant(freshness_policies_by_key is None)
+            check.invariant(auto_materialize_policies_by_key is None)
+            check.invariant(descriptions_by_key is None)
+            check.invariant(owners_by_key is None)
+            check.invariant(partition_mappings is None)
+            check.invariant(asset_deps is None)
+            resolved_specs = specs
 
-        self._descriptions_by_key = dict(
-            check.opt_mapping_param(
-                descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
+        else:
+            resolved_specs = _asset_specs_from_attr_key_params(
+                all_asset_keys=all_asset_keys,
+                keys_by_input_name=keys_by_input_name,
+                deps_by_asset_key=asset_deps,
+                partition_mappings=partition_mappings,
+                tags_by_key=tags_by_key,
+                owners_by_key=owners_by_key,
+                group_names_by_key=group_names_by_key,
+                freshness_policies_by_key=freshness_policies_by_key,
+                auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+                metadata_by_key=metadata_by_key,
+                descriptions_by_key=descriptions_by_key,
             )
-        )
-        for output_name, asset_key in keys_by_output_name.items():
-            output_def, _ = node_def.resolve_output_to_origin(output_name, None)
-            self._metadata_by_key[asset_key] = {
-                **output_def.metadata,
-                **self._metadata_by_key.get(asset_key, {}),
-            }
+
+        normalized_specs: List[AssetSpec] = []
+        output_names_by_key = {key: name for name, key in keys_by_output_name.items()}
+
+        for spec in resolved_specs:
+            if spec.owners:
+                for owner in spec.owners:
+                    validate_asset_owner(owner, spec.key)
+
+            group_name = normalize_group_name(spec.group_name)
+
+            output_def, _ = node_def.resolve_output_to_origin(output_names_by_key[spec.key], None)
+            metadata = {**output_def.metadata, **(spec.metadata or {})}
             # We construct description from three sources of truth here. This
             # highly unfortunate. See commentary in @multi_asset's call to dagster_internal_init.
-            description = (
-                self._descriptions_by_key.get(asset_key, output_def.description)
-                or node_def.description
-            )
-            if description:
-                self._descriptions_by_key[asset_key] = description
-            self._code_versions_by_key[asset_key] = output_def.code_version
+            description = spec.description or output_def.description or node_def.description
+            code_version = spec.code_version or output_def.code_version
 
-        for key, freshness_policy in (freshness_policies_by_key or {}).items():
-            check.param_invariant(
+            check.invariant(
                 not (
-                    freshness_policy
+                    spec.freshness_policy
                     and self._partitions_def is not None
                     and not isinstance(self._partitions_def, TimeWindowPartitionsDefinition)
                 ),
-                "freshness_policies_by_key",
                 "FreshnessPolicies are currently unsupported for assets with partitions of type"
                 f" {type(self._partitions_def)}.",
             )
 
-        self._freshness_policies_by_key = check.opt_mapping_param(
-            freshness_policies_by_key,
-            "freshness_policies_by_key",
-            key_type=AssetKey,
-            value_type=FreshnessPolicy,
-        )
+            normalized_specs.append(
+                spec._replace(
+                    group_name=group_name,
+                    code_version=code_version,
+                    metadata=metadata,
+                    description=description,
+                )
+            )
 
-        self._auto_materialize_policies_by_key = check.opt_mapping_param(
-            auto_materialize_policies_by_key,
-            "auto_materialize_policies_by_key",
-            key_type=AssetKey,
-            value_type=AutoMaterializePolicy,
+        self._partition_mappings = get_partition_mappings_from_deps(
+            {}, [dep for spec in normalized_specs for dep in spec.deps], node_def.name
         )
 
-        self._backfill_policy = check.opt_inst_param(
-            backfill_policy, "backfill_policy", BackfillPolicy
-        )
-
-        if self._partitions_def is None:
-            # check if backfill policy is BackfillPolicyType.SINGLE_RUN if asset is not partitioned
-            check.param_invariant(
-                (
-                    backfill_policy.policy_type is BackfillPolicyType.SINGLE_RUN
-                    if backfill_policy
-                    else True
-                ),
-                "backfill_policy",
-                "Non partitioned asset can only have single run backfill policy",
-            )
-
         _validate_self_deps(
             input_keys=[
                 key
                 # filter out the special inputs which are used for cases when a multi-asset is
                 # subsetted, as these are not the same as self-dependencies and are never loaded
                 # in the same step that their corresponding output is produced
                 for input_name, key in self._keys_by_input_name.items()
                 if not input_name.startswith(ASSET_SUBSET_INPUT_PREFIX)
             ],
             output_keys=self._selected_asset_keys,
             partition_mappings=self._partition_mappings,
             partitions_def=self._partitions_def,
         )
 
-        self._is_subset = check.bool_param(is_subset, "is_subset")
-
-        self._owners_by_key = check.opt_mapping_param(
-            owners_by_key, "owners_by_key", key_type=AssetKey, value_type=list
-        )
-        for key, owners in self._owners_by_key.items():
-            for owner in owners:
-                if is_valid_email(owner):
-                    continue
-                elif owner.startswith("team:") and len(owner) > 5:
-                    continue
-                else:
-                    raise DagsterInvalidDefinitionError(
-                        f"Invalid owner '{owner}' for asset '{key}'. Owner must be an email address or a team"
-                        " name prefixed with 'team:'."
-                    )
+        self._specs_by_key = {spec.key: spec for spec in normalized_specs}
 
     def dagster_internal_init(
         *,
         keys_by_input_name: Mapping[str, AssetKey],
         keys_by_output_name: Mapping[str, AssetKey],
         node_def: NodeDefinition,
         partitions_def: Optional[PartitionsDefinition],
-        partition_mappings: Optional[Mapping[AssetKey, PartitionMapping]],
-        asset_deps: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         selected_asset_keys: Optional[AbstractSet[AssetKey]],
         can_subset: bool,
         resource_defs: Optional[Mapping[str, object]],
-        group_names_by_key: Optional[Mapping[AssetKey, str]],
-        metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]],
-        tags_by_key: Optional[Mapping[AssetKey, Mapping[str, str]]],
-        freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]],
-        auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]],
         backfill_policy: Optional[BackfillPolicy],
-        descriptions_by_key: Optional[Mapping[AssetKey, str]],
         check_specs_by_output_name: Optional[Mapping[str, AssetCheckSpec]],
         selected_asset_check_keys: Optional[AbstractSet[AssetCheckKey]],
         is_subset: bool,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]],
+        specs: Optional[Sequence[AssetSpec]],
     ) -> "AssetsDefinition":
-        return AssetsDefinition(
-            keys_by_input_name=keys_by_input_name,
-            keys_by_output_name=keys_by_output_name,
-            node_def=node_def,
-            partitions_def=partitions_def,
-            partition_mappings=partition_mappings,
-            asset_deps=asset_deps,
-            selected_asset_keys=selected_asset_keys,
-            can_subset=can_subset,
-            resource_defs=resource_defs,
-            group_names_by_key=group_names_by_key,
-            metadata_by_key=metadata_by_key,
-            tags_by_key=tags_by_key,
-            freshness_policies_by_key=freshness_policies_by_key,
-            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
-            backfill_policy=backfill_policy,
-            descriptions_by_key=descriptions_by_key,
-            check_specs_by_output_name=check_specs_by_output_name,
-            selected_asset_check_keys=selected_asset_check_keys,
-            is_subset=is_subset,
-            owners_by_key=owners_by_key,
-        )
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=ExperimentalWarning)
+            return AssetsDefinition(
+                keys_by_input_name=keys_by_input_name,
+                keys_by_output_name=keys_by_output_name,
+                node_def=node_def,
+                partitions_def=partitions_def,
+                selected_asset_keys=selected_asset_keys,
+                can_subset=can_subset,
+                resource_defs=resource_defs,
+                backfill_policy=backfill_policy,
+                check_specs_by_output_name=check_specs_by_output_name,
+                selected_asset_check_keys=selected_asset_check_keys,
+                is_subset=is_subset,
+                specs=specs,
+            )
 
     def __call__(self, *args: object, **kwargs: object) -> object:
         from .composition import is_in_composition
         from .graph_definition import GraphDefinition
 
         # defer to GraphDefinition.__call__ for graph backed assets, or if invoked in composition
         if isinstance(self.node_def, GraphDefinition) or is_in_composition():
@@ -393,15 +386,15 @@
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
         check_specs: Optional[Sequence[AssetCheckSpec]] = None,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
+        owners_by_output_name: Optional[Mapping[str, Sequence[str]]] = None,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from a GraphDefinition.
 
         Args:
             graph_def (GraphDefinition): The GraphDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
                 names of the decorated graph to their corresponding asset keys. If not provided,
@@ -473,15 +466,15 @@
             metadata_by_output_name=metadata_by_output_name,
             tags_by_output_name=tags_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             backfill_policy=backfill_policy,
             can_subset=can_subset,
             check_specs=check_specs,
-            owners_by_key=owners_by_key,
+            owners_by_output_name=owners_by_output_name,
         )
 
     @public
     @staticmethod
     def from_op(
         op_def: OpDefinition,
         *,
@@ -593,15 +586,15 @@
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
         check_specs: Optional[Sequence[AssetCheckSpec]] = None,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
+        owners_by_output_name: Optional[Mapping[str, Sequence[str]]] = None,
     ) -> "AssetsDefinition":
         from dagster._core.definitions.decorators.asset_decorator import (
             _assign_output_names_to_check_specs,
             _validate_check_specs_target_relevant_asset_keys,
         )
 
         node_def = check.inst_param(node_def, "node_def", NodeDefinition)
@@ -676,78 +669,96 @@
                 asset_key: group_name for asset_key in keys_by_output_name_with_prefix.values()
             }
         elif group_names_by_output_name:
             group_names_by_key = _output_dict_to_asset_dict(group_names_by_output_name)
         else:
             group_names_by_key = None
 
-        return AssetsDefinition.dagster_internal_init(
+        specs = _asset_specs_from_attr_key_params(
+            all_asset_keys=set(keys_by_output_name_with_prefix.values()),
             keys_by_input_name=keys_by_input_name,
-            keys_by_output_name=keys_by_output_name_with_prefix,
-            node_def=node_def,
-            asset_deps=transformed_internal_asset_deps or None,
-            partitions_def=check.opt_inst_param(
-                partitions_def,
-                "partitions_def",
-                PartitionsDefinition,
-            ),
-            group_names_by_key=group_names_by_key,
-            resource_defs=resource_defs,
+            deps_by_asset_key=transformed_internal_asset_deps or None,
             partition_mappings=(
                 {
                     keys_by_input_name[input_name]: partition_mapping
                     for input_name, partition_mapping in partition_mappings.items()
                 }
                 if partition_mappings
                 else None
             ),
-            metadata_by_key=_output_dict_to_asset_dict(metadata_by_output_name),
             tags_by_key=_output_dict_to_asset_dict(tags_by_output_name),
+            owners_by_key=_output_dict_to_asset_dict(owners_by_output_name),
+            group_names_by_key=group_names_by_key,
             freshness_policies_by_key=_output_dict_to_asset_dict(freshness_policies_by_output_name),
             auto_materialize_policies_by_key=_output_dict_to_asset_dict(
                 auto_materialize_policies_by_output_name
             ),
+            metadata_by_key=_output_dict_to_asset_dict(metadata_by_output_name),
+            descriptions_by_key=_output_dict_to_asset_dict(descriptions_by_output_name),
+        )
+
+        return AssetsDefinition.dagster_internal_init(
+            keys_by_input_name=keys_by_input_name,
+            keys_by_output_name=keys_by_output_name_with_prefix,
+            node_def=node_def,
+            partitions_def=check.opt_inst_param(
+                partitions_def,
+                "partitions_def",
+                PartitionsDefinition,
+            ),
+            resource_defs=resource_defs,
             backfill_policy=check.opt_inst_param(
                 backfill_policy, "backfill_policy", BackfillPolicy
             ),
-            descriptions_by_key=_output_dict_to_asset_dict(descriptions_by_output_name),
             can_subset=can_subset,
             selected_asset_keys=None,  # node has no subselection info
             check_specs_by_output_name=check_specs_by_output_name,
             selected_asset_check_keys=None,
             is_subset=False,
-            owners_by_key=owners_by_key,
+            specs=specs,
         )
 
     @public
     @property
     def can_subset(self) -> bool:
         """bool: If True, indicates that this AssetsDefinition may materialize any subset of its
         asset keys in a given computation (as opposed to being required to materialize all asset
         keys).
         """
         return self._can_subset
 
+    @property
+    def specs(self) -> Iterable[AssetSpec]:
+        return self._specs_by_key.values()
+
+    @property
+    def specs_by_key(self) -> Mapping[AssetKey, AssetSpec]:
+        return self._specs_by_key
+
     @public
     @property
     def group_names_by_key(self) -> Mapping[AssetKey, str]:
         """Mapping[AssetKey, str]: Returns a mapping from the asset keys in this AssetsDefinition
         to the group names assigned to them. If there is no assigned group name for a given AssetKey,
         it will not be present in this dictionary.
         """
-        return self._group_names_by_key
+        return {key: check.not_none(spec.group_name) for key, spec in self._specs_by_key.items()}
 
     @public
     @property
     def descriptions_by_key(self) -> Mapping[AssetKey, str]:
         """Mapping[AssetKey, str]: Returns a mapping from the asset keys in this AssetsDefinition
         to the descriptions assigned to them. If there is no assigned description for a given AssetKey,
         it will not be present in this dictionary.
         """
-        return self._descriptions_by_key
+        return {
+            key: spec.description
+            for key, spec in self._specs_by_key.items()
+            if spec.description is not None
+        }
 
     @public
     @property
     def op(self) -> OpDefinition:
         """OpDefinition: Returns the OpDefinition that is used to materialize the assets in this
         AssetsDefinition.
         """
@@ -769,15 +780,17 @@
     @property
     def asset_deps(self) -> Mapping[AssetKey, AbstractSet[AssetKey]]:
         """Maps assets that are produced by this definition to assets that they depend on. The
         dependencies can be either "internal", meaning that they refer to other assets that are
         produced by this definition, or "external", meaning that they refer to assets that aren't
         produced by this definition.
         """
-        return self._asset_deps
+        return {
+            key: {dep.asset_key for dep in spec.deps} for key, spec in self._specs_by_key.items()
+        }
 
     @property
     def input_names(self) -> Iterable[str]:
         """Iterable[str]: The set of input names of the underlying NodeDefinition for this
         AssetsDefinition.
         """
         return self.keys_by_input_name.keys()
@@ -884,19 +897,27 @@
 
         return {
             name: key for name, key in self.node_keys_by_input_name.items() if key in upstream_keys
         }
 
     @property
     def freshness_policies_by_key(self) -> Mapping[AssetKey, FreshnessPolicy]:
-        return self._freshness_policies_by_key
+        return {
+            key: spec.freshness_policy
+            for key, spec in self._specs_by_key.items()
+            if spec.freshness_policy
+        }
 
     @property
     def auto_materialize_policies_by_key(self) -> Mapping[AssetKey, AutoMaterializePolicy]:
-        return self._auto_materialize_policies_by_key
+        return {
+            key: spec.auto_materialize_policy
+            for key, spec in self._specs_by_key.items()
+            if spec.auto_materialize_policy
+        }
 
     # Applies only to external observable assets. Can be removed when we fold
     # `auto_observe_interval_minutes` into auto-materialize policies.
     @property
     def auto_observe_interval_minutes(self) -> Optional[float]:
         value = self._get_external_asset_metadata_value(
             SYSTEM_METADATA_KEY_AUTO_OBSERVE_INTERVAL_MINUTES
@@ -914,45 +935,51 @@
         return (
             self._get_external_asset_metadata_value(SYSTEM_METADATA_KEY_AUTO_CREATED_STUB_ASSET)
             is not None
         )
 
     def _get_external_asset_metadata_value(self, metadata_key: str) -> object:
         first_key = next(iter(self.keys), None)
-        return self.metadata_by_key.get(first_key, {}).get(metadata_key) if first_key else None
+        if not first_key:
+            return None
+        return (self._specs_by_key[first_key].metadata or {}).get(metadata_key)
 
     @property
     def backfill_policy(self) -> Optional[BackfillPolicy]:
         return self._backfill_policy
 
     @public
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         """Optional[PartitionsDefinition]: The PartitionsDefinition for this AssetsDefinition (if any)."""
         return self._partitions_def
 
     @property
     def metadata_by_key(self) -> Mapping[AssetKey, ArbitraryMetadataMapping]:
-        return self._metadata_by_key
+        return {
+            key: spec.metadata
+            for key, spec in self._specs_by_key.items()
+            if spec.metadata is not None
+        }
 
     @property
     def tags_by_key(self) -> Mapping[AssetKey, Mapping[str, str]]:
-        return self._tags_by_key
+        return {key: spec.tags or {} for key, spec in self._specs_by_key.items()}
 
     @property
     def code_versions_by_key(self) -> Mapping[AssetKey, Optional[str]]:
-        return self._code_versions_by_key
+        return {key: spec.code_version for key, spec in self._specs_by_key.items()}
 
     @property
     def partition_mappings(self) -> Mapping[AssetKey, PartitionMapping]:
         return self._partition_mappings
 
     @property
     def owners_by_key(self) -> Mapping[AssetKey, Sequence[str]]:
-        return self._owners_by_key
+        return {key: spec.owners or [] for key, spec in self._specs_by_key.items()}
 
     @public
     def get_partition_mapping(self, in_asset_key: AssetKey) -> Optional[PartitionMapping]:
         """Returns the partition mapping between keys in this AssetsDefinition and a given input
         asset key (if any).
         """
         return self._partition_mappings.get(in_asset_key)
@@ -1082,155 +1109,94 @@
         )
         group_names_by_key = check.opt_mapping_param(
             group_names_by_key, "group_names_by_key", key_type=AssetKey, value_type=str
         )
 
         backfill_policy = check.opt_inst_param(backfill_policy, "backfill_policy", BackfillPolicy)
 
-        if group_names_by_key:
-            group_name_conflicts = [
-                asset_key
-                for asset_key in group_names_by_key
-                if asset_key in self.group_names_by_key
-                and self.group_names_by_key[asset_key] != DEFAULT_GROUP_NAME
-            ]
-            if group_name_conflicts:
-                raise DagsterInvalidDefinitionError(
-                    "Group name already exists on assets"
-                    f" {', '.join(asset_key.to_user_string() for asset_key in group_name_conflicts)}"
-                )
+        conflicts_by_attr_name: Dict[str, Set[AssetKey]] = defaultdict(set)
+        replaced_specs = []
 
-        replaced_group_names_by_key = {
-            output_asset_key_replacements.get(key, key): group_name
-            for key, group_name in self.group_names_by_key.items()
-        }
+        for key, spec in self._specs_by_key.items():
+            replace_dict = {}
 
-        if freshness_policy:
-            freshness_policy_conflicts = (
-                self.freshness_policies_by_key.keys()
-                if isinstance(freshness_policy, FreshnessPolicy)
-                else (freshness_policy.keys() & self.freshness_policies_by_key.keys())
-            )
-            if freshness_policy_conflicts:
-                raise DagsterInvalidDefinitionError(
-                    "FreshnessPolicy already exists on assets"
-                    f" {', '.join(key.to_string() for key in freshness_policy_conflicts)}"
-                )
+            def update_replace_dict_and_conflicts(
+                new_value: Union[Mapping[AssetKey, object], object],
+                attr_name: str,
+                default_value: object = None,
+            ) -> None:
+                if isinstance(new_value, Mapping):
+                    if key in new_value:
+                        replace_dict[attr_name] = new_value[key]
+                elif new_value:
+                    replace_dict[attr_name] = new_value
+
+                old_value = getattr(spec, attr_name)
+                if old_value and old_value != default_value and attr_name in replace_dict:
+                    conflicts_by_attr_name[attr_name].add(key)
 
-        replaced_freshness_policies_by_key = {}
-        for key in self.keys:
-            if isinstance(freshness_policy, FreshnessPolicy):
-                replaced_freshness_policy = freshness_policy
-            elif freshness_policy:
-                replaced_freshness_policy = freshness_policy.get(key)
-            else:
-                replaced_freshness_policy = self.freshness_policies_by_key.get(key)
-
-            if replaced_freshness_policy:
-                replaced_freshness_policies_by_key[output_asset_key_replacements.get(key, key)] = (
-                    replaced_freshness_policy
-                )
+            update_replace_dict_and_conflicts(
+                new_value=auto_materialize_policy, attr_name="auto_materialize_policy"
+            )
+            update_replace_dict_and_conflicts(
+                new_value=freshness_policy, attr_name="freshness_policy"
+            )
+            update_replace_dict_and_conflicts(new_value=tags_by_key, attr_name="tags")
+            update_replace_dict_and_conflicts(
+                new_value=group_names_by_key,
+                attr_name="group_name",
+                default_value=DEFAULT_GROUP_NAME,
+            )
 
-        if auto_materialize_policy:
-            auto_materialize_policy_conflicts = (
-                self.auto_materialize_policies_by_key.keys()
-                if isinstance(auto_materialize_policy, AutoMaterializePolicy)
-                else (auto_materialize_policy.keys() & self.auto_materialize_policies_by_key.keys())
-            )
-            if auto_materialize_policy_conflicts:
-                raise DagsterInvalidDefinitionError(
-                    "AutoMaterializePolicy already exists on assets"
-                    f" {', '.join(key.to_string() for key in auto_materialize_policy_conflicts)}"
-                )
+            if key in output_asset_key_replacements:
+                replace_dict["key"] = output_asset_key_replacements[key]
 
-        replaced_auto_materialize_policies_by_key = {}
-        for key in self.keys:
-            if isinstance(auto_materialize_policy, AutoMaterializePolicy):
-                replaced_auto_materialize_policy = auto_materialize_policy
-            elif auto_materialize_policy:
-                replaced_auto_materialize_policy = auto_materialize_policy.get(key)
-            else:
-                replaced_auto_materialize_policy = self.auto_materialize_policies_by_key.get(key)
-
-            if replaced_auto_materialize_policy:
-                replaced_auto_materialize_policies_by_key[
-                    output_asset_key_replacements.get(key, key)
-                ] = replaced_auto_materialize_policy
-
-        replaced_descriptions_by_key = {
-            output_asset_key_replacements.get(key, key): description
-            for key, description in self.descriptions_by_key.items()
-        }
+            if input_asset_key_replacements or output_asset_key_replacements:
+                new_deps = []
+                for dep in spec.deps:
+                    replacement_key = input_asset_key_replacements.get(
+                        dep.asset_key,
+                        output_asset_key_replacements.get(dep.asset_key),
+                    )
+                    if replacement_key is not None:
+                        new_deps.append(dep._replace(asset_key=replacement_key))
+                    else:
+                        new_deps.append(dep)
 
-        replaced_metadata_by_key = {
-            output_asset_key_replacements.get(key, key): metadata
-            for key, metadata in self.metadata_by_key.items()
-        }
+                replace_dict["deps"] = new_deps
 
-        replaced_tags_by_key = {
-            output_asset_key_replacements.get(key, key): tags
-            for key, tags in self.tags_by_key.items()
-        }
+            replaced_specs.append(spec._replace(**replace_dict))
 
-        replaced_owners_by_key = {
-            output_asset_key_replacements.get(key, key): owners
-            for key, owners in self.owners_by_key.items()
-        }
+        for attr_name, conflicting_asset_keys in conflicts_by_attr_name.items():
+            raise DagsterInvalidDefinitionError(
+                f"{attr_name} already exists on assets"
+                f" {', '.join(asset_key.to_user_string() for asset_key in conflicting_asset_keys)}"
+            )
 
         replaced_attributes = dict(
             keys_by_input_name={
                 input_name: input_asset_key_replacements.get(key, key)
                 for input_name, key in self._keys_by_input_name.items()
             },
             keys_by_output_name={
                 output_name: output_asset_key_replacements.get(key, key)
                 for output_name, key in self._keys_by_output_name.items()
             },
-            partition_mappings={
-                input_asset_key_replacements.get(key, key): partition_mapping
-                for key, partition_mapping in self._partition_mappings.items()
-            },
-            asset_deps={
-                # replace both the keys and the values in this mapping
-                output_asset_key_replacements.get(key, key): {
-                    input_asset_key_replacements.get(
-                        upstream_key,
-                        output_asset_key_replacements.get(upstream_key, upstream_key),
-                    )
-                    for upstream_key in value
-                }
-                for key, value in self.asset_deps.items()
-            },
             selected_asset_keys={
                 output_asset_key_replacements.get(key, key) for key in self._selected_asset_keys
             },
-            group_names_by_key={
-                **replaced_group_names_by_key,
-                **group_names_by_key,
-            },
-            metadata_by_key={
-                **self._metadata_by_key,
-                **replaced_metadata_by_key,
-            },
-            tags_by_key=replaced_tags_by_key,
-            owners_by_key=replaced_owners_by_key,
-            freshness_policies_by_key=replaced_freshness_policies_by_key,
-            auto_materialize_policies_by_key=replaced_auto_materialize_policies_by_key,
             backfill_policy=backfill_policy if backfill_policy else self.backfill_policy,
-            descriptions_by_key={
-                **self._descriptions_by_key,
-                **replaced_descriptions_by_key,
-            },
             is_subset=self.is_subset,
             check_specs_by_output_name=check_specs_by_output_name
             if check_specs_by_output_name
             else self._check_specs_by_output_name,
             selected_asset_check_keys=selected_asset_check_keys
             if selected_asset_check_keys
             else self._selected_asset_check_keys,
+            specs=replaced_specs,
         )
 
         merged_attrs = merge_dicts(self.get_attributes_dict(), replaced_attributes)
         return self.__class__.dagster_internal_init(**merged_attrs)
 
     def _subset_graph_backed_asset(
         self,
@@ -1308,47 +1274,48 @@
 
             subsetted_output_names = [output_def.name for output_def in subsetted_node.output_defs]
             subsetted_keys_by_output_name = {
                 key: value
                 for key, value in self.node_keys_by_output_name.items()
                 if key in subsetted_output_names
             }
+            selected_node_asset_keys = set(subsetted_keys_by_output_name.values())
 
             # An op within the graph-backed asset that yields multiple assets will be run
             # any time any of its output assets are selected. Thus, if an op yields multiple assets
             # and only one of them is selected, the op will still run and potentially unexpectedly
             # materialize the unselected asset.
             #
             # Thus, we include unselected assets that may be accidentally materialized in
             # keys_by_output_name and asset_deps so that the webserver can populate an warning when
             # this occurs. This is the same behavior as multi-asset subsetting.
 
-            subsetted_asset_deps = {
-                out_asset_key: set(self._keys_by_input_name.values())
-                for out_asset_key in subsetted_keys_by_output_name.values()
-            }
             replaced_attributes = dict(
                 keys_by_input_name=subsetted_keys_by_input_name,
                 keys_by_output_name=subsetted_keys_by_output_name,
                 node_def=subsetted_node,
-                asset_deps=subsetted_asset_deps,
                 selected_asset_keys=selected_asset_keys & self.keys,
                 selected_asset_check_keys=asset_check_subselection,
+                specs=[spec for spec in self.specs if spec.key in selected_node_asset_keys],
                 is_subset=True,
             )
 
-            return self.__class__(**merge_dicts(self.get_attributes_dict(), replaced_attributes))
+            return self.__class__.dagster_internal_init(
+                **merge_dicts(self.get_attributes_dict(), replaced_attributes)
+            )
         else:
             # multi_asset subsetting
             replaced_attributes = {
                 "selected_asset_keys": asset_subselection,
                 "selected_asset_check_keys": asset_check_subselection,
                 "is_subset": True,
             }
-            return self.__class__(**merge_dicts(self.get_attributes_dict(), replaced_attributes))
+            return self.__class__.dagster_internal_init(
+                **merge_dicts(self.get_attributes_dict(), replaced_attributes)
+            )
 
     @property
     def is_subset(self) -> bool:
         return self._is_subset
 
     @public
     def to_source_assets(self) -> Sequence[SourceAsset]:
@@ -1460,38 +1427,31 @@
     def with_resources(self, resource_defs: Mapping[str, ResourceDefinition]) -> "AssetsDefinition":
         attributes_dict = self.get_attributes_dict()
         attributes_dict["resource_defs"] = merge_resource_defs(
             old_resource_defs=self.resource_defs,
             resource_defs_to_merge_in=resource_defs,
             requires_resources=self,
         )
-        return self.__class__(**attributes_dict)
+        with disable_dagster_warnings():
+            return self.__class__(**attributes_dict)
 
     def get_attributes_dict(self) -> Dict[str, Any]:
         return dict(
             keys_by_input_name=self._keys_by_input_name,
             keys_by_output_name=self._keys_by_output_name,
             node_def=self._node_def,
             partitions_def=self._partitions_def,
-            partition_mappings=self._partition_mappings,
-            asset_deps=self.asset_deps,
             selected_asset_keys=self._selected_asset_keys,
             can_subset=self._can_subset,
             resource_defs=self._resource_defs,
-            group_names_by_key=self._group_names_by_key,
-            metadata_by_key=self._metadata_by_key,
-            freshness_policies_by_key=self._freshness_policies_by_key,
-            auto_materialize_policies_by_key=self._auto_materialize_policies_by_key,
             backfill_policy=self._backfill_policy,
-            descriptions_by_key=self._descriptions_by_key,
             check_specs_by_output_name=self._check_specs_by_output_name,
             selected_asset_check_keys=self._selected_asset_check_keys,
-            owners_by_key=self._owners_by_key,
-            tags_by_key=self._tags_by_key,
-            is_subset=self._is_subset,
+            specs=self.specs,
+            is_subset=self.is_subset,
         )
 
 
 def _infer_keys_by_input_names(
     node_def: NodeDefinition, keys_by_input_name: Mapping[str, AssetKey]
 ) -> Mapping[str, AssetKey]:
     all_input_names = [input_def.name for input_def in node_def.input_defs]
@@ -1626,37 +1586,106 @@
 
 
 def _validate_partition_mappings(
     partition_mappings: Mapping[AssetKey, PartitionMapping],
     input_asset_keys: AbstractSet[AssetKey],
     all_asset_keys: AbstractSet[AssetKey],
 ) -> None:
-    builtin_partition_mappings = get_builtin_partition_mapping_types()
     for asset_key, partition_mapping in partition_mappings.items():
-        if not isinstance(partition_mapping, builtin_partition_mappings):
-            warnings.warn(
-                f"Non-built-in PartitionMappings, such as {type(partition_mapping).__name__} "
-                "are deprecated and will not work with asset reconciliation. The built-in "
-                "partition mappings are "
-                + ", ".join(
-                    builtin_partition_mapping.__name__
-                    for builtin_partition_mapping in builtin_partition_mappings
-                )
-                + ".",
-                category=DeprecationWarning,
-            )
+        warn_if_partition_mapping_not_builtin(partition_mapping)
 
         if asset_key not in input_asset_keys:
             check.failed(
                 f"While constructing AssetsDefinition outputting {all_asset_keys}, received a"
                 f" partition mapping for {asset_key} that is not defined in the set of upstream"
                 f" assets: {input_asset_keys}"
             )
 
 
+def _asset_specs_from_attr_key_params(
+    all_asset_keys: AbstractSet[AssetKey],
+    keys_by_input_name: Mapping[str, AssetKey],
+    deps_by_asset_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]] = None,
+    partition_mappings: Optional[Mapping[AssetKey, PartitionMapping]] = None,
+    group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
+    metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
+    tags_by_key: Optional[Mapping[AssetKey, Mapping[str, str]]] = None,
+    freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
+    auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
+    descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
+    owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
+) -> Sequence[AssetSpec]:
+    validated_group_names_by_key = check.opt_mapping_param(
+        group_names_by_key, "group_names_by_key", key_type=AssetKey, value_type=str
+    )
+
+    validated_metadata_by_key = check.opt_mapping_param(
+        metadata_by_key, "metadata_by_key", key_type=AssetKey, value_type=dict
+    )
+
+    for tags in (tags_by_key or {}).values():
+        validate_tags_strict(tags)
+    validated_tags_by_key = tags_by_key or {}
+
+    validated_descriptions_by_key = check.opt_mapping_param(
+        descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
+    )
+
+    validated_freshness_policies_by_key = check.opt_mapping_param(
+        freshness_policies_by_key,
+        "freshness_policies_by_key",
+        key_type=AssetKey,
+        value_type=FreshnessPolicy,
+    )
+
+    validated_auto_materialize_policies_by_key = check.opt_mapping_param(
+        auto_materialize_policies_by_key,
+        "auto_materialize_policies_by_key",
+        key_type=AssetKey,
+        value_type=AutoMaterializePolicy,
+    )
+
+    validated_owners_by_key = check.opt_mapping_param(
+        owners_by_key, "owners_by_key", key_type=AssetKey, value_type=list
+    )
+
+    dep_keys_from_keys_by_input_name = set(keys_by_input_name.values())
+    dep_objs_from_keys_by_input_name = [
+        AssetDep(asset=key, partition_mapping=(partition_mappings or {}).get(key))
+        for key in dep_keys_from_keys_by_input_name
+    ]
+
+    result: List[AssetSpec] = []
+    for key in all_asset_keys:
+        if deps_by_asset_key:
+            dep_objs = [
+                AssetDep(asset=key, partition_mapping=(partition_mappings or {}).get(key))
+                for key in deps_by_asset_key.get(key, [])
+            ]
+        else:
+            dep_objs = dep_objs_from_keys_by_input_name
+
+        with disable_dagster_warnings():
+            result.append(
+                AssetSpec(
+                    key=key,
+                    description=validated_descriptions_by_key.get(key),
+                    metadata=validated_metadata_by_key.get(key),
+                    tags=validated_tags_by_key.get(key),
+                    freshness_policy=validated_freshness_policies_by_key.get(key),
+                    auto_materialize_policy=validated_auto_materialize_policies_by_key.get(key),
+                    owners=validated_owners_by_key.get(key),
+                    group_name=validated_group_names_by_key.get(key),
+                    deps=dep_objs,
+                )
+            )
+
+    return result
+
+
 def _validate_self_deps(
     input_keys: Iterable[AssetKey],
     output_keys: Iterable[AssetKey],
     partition_mappings: Mapping[AssetKey, PartitionMapping],
     partitions_def: Optional[PartitionsDefinition],
 ) -> None:
     output_keys_set = set(output_keys)
@@ -1701,7 +1730,37 @@
         if time_partition_mapping is None or not isinstance(
             time_partition_mapping.partition_mapping, TimeWindowPartitionMapping
         ):
             return None
 
         return time_partition_mapping.partition_mapping
     return None
+
+
+def validate_asset_owner(owner: str, key: AssetKey) -> None:
+    if not is_valid_email(owner) and not (owner.startswith("team:") and len(owner) > 5):
+        raise DagsterInvalidDefinitionError(
+            f"Invalid owner '{owner}' for asset '{key}'. Owner must be an email address or a team "
+            "name prefixed with 'team:'."
+        )
+
+
+def get_partition_mappings_from_deps(
+    partition_mappings: Dict[AssetKey, PartitionMapping], deps: Iterable[AssetDep], asset_name: str
+) -> Mapping[AssetKey, PartitionMapping]:
+    # Add PartitionMappings specified via AssetDeps to partition_mappings dictionary. Error on duplicates
+    for dep in deps:
+        if dep.partition_mapping is None:
+            continue
+        if partition_mappings.get(dep.asset_key, None) is None:
+            partition_mappings[dep.asset_key] = dep.partition_mapping
+            continue
+        if partition_mappings[dep.asset_key] == dep.partition_mapping:
+            continue
+        else:
+            raise DagsterInvalidDefinitionError(
+                f"Two different PartitionMappings for {dep.asset_key} provided for"
+                f" asset {asset_name}. Please use the same PartitionMapping for"
+                f" {dep.asset_key}."
+            )
+
+    return partition_mappings
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.8/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,8 +262,8 @@
 
     def __eq__(self, other) -> bool:
         # override the default NamedTuple __eq__ method to factor in types
         return type(self) == type(other) and super().__eq__(other)
 
     def __hash__(self) -> int:
         # override the default NamedTuple __hash__ method to factor in types
-        return hash(hash(type(self)) + super().__hash__())
+        return hash(hash(type(self).__name__) + super().__hash__())
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_impls.py` & `dagster-1.7.8/dagster/_core/definitions/auto_materialize_rule_impls.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.8/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.8/dagster/_core/definitions/base_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.8/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/composition.py` & `dagster-1.7.8/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/config.py` & `dagster-1.7.8/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/configurable.py` & `dagster-1.7.8/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/data_time.py` & `dagster-1.7.8/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/data_version.py` & `dagster-1.7.8/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/README.md` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             asset_slice_with_metadata
             for asset_slice_with_metadata in slices_with_metadata
             if not (
                 asset_slice_with_metadata.asset_slice.is_empty
                 or cast(
                     float,
                     asset_slice_with_metadata.metadata.get(
-                        _REQUEST_TIMESTAMP_METADATA_KEY, MetadataValue.float(0)
+                        _REQUEST_TIMESTAMP_METADATA_KEY, MetadataValue.float(0.0)
                     ).value,
                 )
                 < self._get_minimum_timestamp(context)
             )
         ]
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_context.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/serialized_objects.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/serialized_objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/utils.py` & `dagster-1.7.8/dagster/_core/definitions/declarative_scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,28 @@
 from dagster._config import UserConfigSchema
 from dagster._core.decorator_utils import get_function_params, get_valid_name_permutations
 from dagster._core.definitions.asset_dep import AssetDep, CoercibleToAssetDep
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.config import ConfigMapping
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping, RawMetadataMapping
-from dagster._core.definitions.partition_mapping import PartitionMapping
 from dagster._core.definitions.resource_annotation import (
     get_resource_args,
 )
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 from dagster._core.types.dagster_type import DagsterType
 from dagster._utils.warnings import (
     disable_dagster_warnings,
 )
 
 from ..asset_check_spec import AssetCheckSpec
 from ..asset_in import AssetIn
 from ..asset_out import AssetOut
 from ..asset_spec import AssetSpec
-from ..assets import ASSET_SUBSET_INPUT_PREFIX, AssetsDefinition
+from ..assets import ASSET_SUBSET_INPUT_PREFIX, AssetsDefinition, get_partition_mappings_from_deps
 from ..backfill_policy import BackfillPolicy, BackfillPolicyType
 from ..decorators.graph_decorator import graph
 from ..decorators.op_decorator import _Op
 from ..events import AssetKey, CoercibleToAssetKey, CoercibleToAssetKeyPrefix
 from ..input import GraphIn, In
 from ..output import GraphOut, Out
 from ..partition import PartitionsDefinition
@@ -458,58 +457,60 @@
                         if self.backfill_policy
                         else True
                     ),
                     "backfill_policy",
                     "Non partitioned asset can only have single run backfill policy",
                 )
 
-        keys_by_input_name = {
-            input_name: asset_key for asset_key, (input_name, _) in asset_ins.items()
-        }
-        partition_mappings = {
-            keys_by_input_name[input_name]: asset_in.partition_mapping
-            for input_name, asset_in in self.ins.items()
-            if asset_in.partition_mapping is not None
-        }
+            keys_by_input_name = {
+                input_name: asset_key for asset_key, (input_name, _) in asset_ins.items()
+            }
+            partition_mappings = {
+                keys_by_input_name[input_name]: asset_in.partition_mapping
+                for input_name, asset_in in self.ins.items()
+                if asset_in.partition_mapping is not None
+            }
 
-        partition_mappings = _get_partition_mappings_from_deps(
-            partition_mappings=partition_mappings, deps=self.deps, asset_name=asset_name
-        )
+            partition_mappings = get_partition_mappings_from_deps(
+                partition_mappings=partition_mappings, deps=self.deps, asset_name=asset_name
+            )
+
+        deps = [
+            AssetDep(asset=key, partition_mapping=partition_mappings.get(key))
+            for key in keys_by_input_name.values()
+        ]
+
+        with disable_dagster_warnings():
+            spec = AssetSpec(
+                key=out_asset_key,
+                freshness_policy=self.freshness_policy,
+                auto_materialize_policy=self.auto_materialize_policy,
+                group_name=self.group_name,
+                metadata=self.metadata,
+                tags=self.tags,
+                owners=self.owners,
+                # see comment in @multi_asset's call to dagster_internal_init for the gory details
+                # this is best understood as an _override_ which @asset does not support
+                description=None,
+                deps=deps,
+            )
 
         return AssetsDefinition.dagster_internal_init(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name={"result": out_asset_key},
             node_def=op,
             partitions_def=self.partitions_def,
-            partition_mappings=partition_mappings if partition_mappings else None,
             resource_defs=wrapped_resource_defs,
-            group_names_by_key=(
-                {out_asset_key: self.group_name} if self.group_name is not None else None
-            ),
-            freshness_policies_by_key=(
-                {out_asset_key: self.freshness_policy} if self.freshness_policy else None
-            ),
-            auto_materialize_policies_by_key=(
-                {out_asset_key: self.auto_materialize_policy}
-                if self.auto_materialize_policy
-                else None
-            ),
             backfill_policy=self.backfill_policy,
-            asset_deps=None,  # no asset deps in single-asset decorator
             selected_asset_keys=None,  # no subselection in decorator
             can_subset=False,
-            metadata_by_key={out_asset_key: self.metadata} if self.metadata else None,
-            tags_by_key={out_asset_key: self.tags} if self.tags else None,
-            # see comment in @multi_asset's call to dagster_internal_init for the gory details
-            # this is best understood as an _override_ which @asset does not support
-            descriptions_by_key=None,
             check_specs_by_output_name=check_specs_by_output_name,
             selected_asset_check_keys=None,  # no subselection in decorator
             is_subset=False,
-            owners_by_key={out_asset_key: self.owners} if self.owners else None,
+            specs=[spec],
         )
 
 
 @experimental_param(param="resource_defs")
 @deprecated_param(
     param="non_argument_deps", breaking_version="2.0.0", additional_warn_text="use `deps` instead."
 )
@@ -823,115 +824,63 @@
         partition_mappings = {
             keys_by_input_name[input_name]: asset_in.partition_mapping
             for input_name, asset_in in (ins or {}).items()
             if asset_in.partition_mapping is not None
         }
 
         if upstream_asset_deps:
-            partition_mappings = _get_partition_mappings_from_deps(
+            partition_mappings = get_partition_mappings_from_deps(
                 partition_mappings=partition_mappings, deps=upstream_asset_deps, asset_name=op_name
             )
 
         if specs:
-            props_by_asset_key: Mapping[AssetKey, Union[AssetSpec, AssetOut]] = {
-                spec.key: spec for spec in specs
+            resolved_specs = specs
+        else:
+            resolved_specs = []
+            input_deps_by_key = {
+                key: AssetDep(asset=key, partition_mapping=partition_mappings.get(key))
+                for key in keys_by_input_name.values()
             }
-            # Add PartitionMappings specified via AssetSpec.deps to partition_mappings dictionary. Error on duplicates
-            for spec in specs:
-                for dep in spec.deps:
-                    if dep.partition_mapping is None:
-                        continue
-                    if partition_mappings.get(dep.asset_key, None) is None:
-                        partition_mappings[dep.asset_key] = dep.partition_mapping
-                        continue
-                    if partition_mappings[dep.asset_key] == dep.partition_mapping:
-                        continue
-                    else:
-                        raise DagsterInvalidDefinitionError(
-                            f"Two different PartitionMappings for {dep.asset_key} provided for"
-                            f" multi_asset {op_name}. Please use the same PartitionMapping for"
-                            f" {dep.asset_key}."
+            input_deps = list(input_deps_by_key.values())
+            for output_name, asset_out in asset_out_map.items():
+                key = keys_by_output_name[output_name]
+                if internal_asset_deps:
+                    deps = [
+                        input_deps_by_key.get(
+                            dep_key,
+                            AssetDep(asset=dep_key, partition_mapping=partition_mappings.get(key)),
                         )
+                        for dep_key in internal_asset_deps.get(output_name, [])
+                    ]
+                else:
+                    deps = input_deps
 
-        else:
-            props_by_asset_key = {
-                keys_by_output_name[output_name]: asset_out
-                for output_name, asset_out in asset_out_map.items()
-            }
+                resolved_specs.append(asset_out.to_spec(key, deps=deps))
 
-        # handle properties defined ons AssetSpecs or AssetOuts
-        group_names_by_key = {
-            asset_key: props.group_name
-            for asset_key, props in props_by_asset_key.items()
-            if props.group_name is not None
-        }
         if group_name:
             check.invariant(
-                not group_names_by_key,
+                all(spec.group_name is None for spec in resolved_specs),
                 "Cannot set group_name parameter on multi_asset if one or more of the"
                 " AssetSpecs/AssetOuts supplied to this multi_asset have a group_name defined.",
             )
-            group_names_by_key = {asset_key: group_name for asset_key in props_by_asset_key}
-
-        freshness_policies_by_key = {
-            asset_key: props.freshness_policy
-            for asset_key, props in props_by_asset_key.items()
-            if props.freshness_policy is not None
-        }
-        auto_materialize_policies_by_key = {
-            asset_key: props.auto_materialize_policy
-            for asset_key, props in props_by_asset_key.items()
-            if props.auto_materialize_policy is not None
-        }
-        metadata_by_key = {
-            asset_key: props.metadata
-            for asset_key, props in props_by_asset_key.items()
-            if props.metadata is not None
-        }
-        tags_by_key = {
-            asset_key: props.tags
-            for asset_key, props in props_by_asset_key.items()
-            if props.tags is not None
-        }
-        owners_by_key = {
-            asset_key: props.owners
-            for asset_key, props in props_by_asset_key.items()
-            if props.owners is not None
-        }
+            resolved_specs = [spec._replace(group_name=group_name) for spec in resolved_specs]
 
         return AssetsDefinition.dagster_internal_init(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             node_def=op,
-            asset_deps=internal_deps,
             partitions_def=partitions_def,
-            partition_mappings=partition_mappings if partition_mappings else None,
             can_subset=can_subset,
             resource_defs=resource_defs,
-            group_names_by_key=group_names_by_key,
-            freshness_policies_by_key=freshness_policies_by_key,
-            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
             backfill_policy=backfill_policy,
             selected_asset_keys=None,  # no subselection in decorator
-            # descriptions by key is more accurately understood as _overriding_ the descriptions
-            # by key that are in the OutputDefinitions associated with the asset key.
-            # This is a dangerous construction liable for bugs. Instead there should be a
-            # canonical source of asset descriptions in AssetsDefinintion and if we need
-            # to create a memoized cached dictionary of asset keys for perf or something we do
-            # that in the `__init__` or on demand.
-            #
-            # This is actually an override. We do not override descriptions
-            # in OutputDefinitions in @multi_asset
-            descriptions_by_key=None,
-            metadata_by_key=metadata_by_key,
-            tags_by_key=tags_by_key,
             check_specs_by_output_name=check_specs_by_output_name,
             selected_asset_check_keys=None,  # no subselection in decorator
             is_subset=False,
-            owners_by_key=owners_by_key,
+            specs=resolved_specs,
         )
 
     return inner
 
 
 def get_function_params_without_context_or_config_or_resources(
     fn: Callable[..., Any],
@@ -1269,15 +1218,15 @@
         auto_materialize_policies_by_output_name=(
             {"result": auto_materialize_policy} if auto_materialize_policy else None
         ),
         backfill_policy=backfill_policy,
         descriptions_by_output_name={"result": description} if description else None,
         resource_defs=resource_defs,
         check_specs=check_specs,
-        owners_by_key={out_asset_key: owners} if owners else None,
+        owners_by_output_name={"result": owners} if owners else None,
     )
 
 
 def graph_multi_asset(
     *,
     outs: Mapping[str, AssetOut],
     name: Optional[str] = None,
@@ -1504,29 +1453,7 @@
 
 
 def _validate_and_assign_output_names_to_check_specs(
     check_specs: Optional[Sequence[AssetCheckSpec]], valid_asset_keys: Sequence[AssetKey]
 ) -> Mapping[str, AssetCheckSpec]:
     _validate_check_specs_target_relevant_asset_keys(check_specs, valid_asset_keys)
     return _assign_output_names_to_check_specs(check_specs)
-
-
-def _get_partition_mappings_from_deps(
-    partition_mappings: Dict[AssetKey, PartitionMapping], deps: Iterable[AssetDep], asset_name: str
-):
-    # Add PartitionMappings specified via AssetDeps to partition_mappings dictionary. Error on duplicates
-    for dep in deps:
-        if dep.partition_mapping is None:
-            continue
-        if partition_mappings.get(dep.asset_key, None) is None:
-            partition_mappings[dep.asset_key] = dep.partition_mapping
-            continue
-        if partition_mappings[dep.asset_key] == dep.partition_mapping:
-            continue
-        else:
-            raise DagsterInvalidDefinitionError(
-                f"Two different PartitionMappings for {dep.asset_key} provided for"
-                f" asset {asset_name}. Please use the same PartitionMapping for"
-                f" {dep.asset_key}."
-            )
-
-    return partition_mappings
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,49 +54,48 @@
     required_resource_keys: Optional[Set[str]] = None,
 ) -> Callable[[RawScheduleEvaluationFunction], ScheduleDefinition]:
     """Creates a schedule following the provided cron schedule and requests runs for the provided job.
 
     The decorated function takes in a :py:class:`~dagster.ScheduleEvaluationContext` as its only
     argument, and does one of the following:
 
-    1. Return a `RunRequest` object.
-    2. Return a list of `RunRequest` objects.
-    3. Return a `SkipReason` object, providing a descriptive message of why no runs were requested.
+    1. Return a :py:class:`~dagster.RunRequest` object.
+    2. Return a list of :py:class:`~dagster.RunRequest` objects.
+    3. Return a :py:class:`~dagster.SkipReason` object, providing a descriptive message of why no runs were requested.
     4. Return nothing (skipping without providing a reason)
     5. Return a run config dictionary.
-    6. Yield a `SkipReason` or yield one ore more `RunRequest` objects.
+    6. Yield a :py:class:`~dagster.SkipReason` or yield one ore more :py:class:`~dagster.RunRequest` objects.
 
     Returns a :py:class:`~dagster.ScheduleDefinition`.
 
     Args:
         cron_schedule (Union[str, Sequence[str]]): A valid cron string or sequence of cron strings
-            specifying when the schedule will run, e.g., ``'45 23 * * 6'`` for a schedule that runs
+            specifying when the schedule will run, e.g., ``45 23 * * 6`` for a schedule that runs
             at 11:45 PM every Saturday. If a sequence is provided, then the schedule will run for
             the union of all execution times for the provided cron strings, e.g.,
-            ``['45 23 * * 6', '30 9 * * 0]`` for a schedule that runs at 11:45 PM every Saturday and
+            ``['45 23 * * 6', '30 9 * * 0']`` for a schedule that runs at 11:45 PM every Saturday and
             9:30 AM every Sunday.
-        name (Optional[str]): The name of the schedule to create.
+        name (Optional[str]): The name of the schedule.
         tags (Optional[Dict[str, str]]): A dictionary of tags (string key-value pairs) to attach
             to the scheduled runs.
         tags_fn (Optional[Callable[[ScheduleEvaluationContext], Optional[Dict[str, str]]]]): A function
-            that generates tags to attach to the schedules runs. Takes a
+            that generates tags to attach to the schedule's runs. Takes a
             :py:class:`~dagster.ScheduleEvaluationContext` and returns a dictionary of tags (string
-            key-value pairs). You may set only one of ``tags`` and ``tags_fn``.
+            key-value pairs). **Note**: Either ``tags`` or ``tags_fn`` may be set, but not both.
         should_execute (Optional[Callable[[ScheduleEvaluationContext], bool]]): A function that runs at
             schedule execution time to determine whether a schedule should execute or skip. Takes a
             :py:class:`~dagster.ScheduleEvaluationContext` and returns a boolean (``True`` if the
             schedule should execute). Defaults to a function that always returns ``True``.
         execution_timezone (Optional[str]): Timezone in which the schedule should run.
             Supported strings for timezones are the ones provided by the
-            `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
+            `IANA time zone database <https://www.iana.org/time-zones>`_ - e.g. ``"America/Los_Angeles"``.
         description (Optional[str]): A human-readable description of the schedule.
         job (Optional[Union[GraphDefinition, JobDefinition, UnresolvedAssetJobDefinition]]): The job
-            that should execute when this schedule runs.
-        default_status (DefaultScheduleStatus): Whether the schedule starts as running or not. The default
-            status can be overridden from the Dagster UI or via the GraphQL API.
+            that should execute when the schedule runs.
+        default_status (DefaultScheduleStatus): If set to ``RUNNING``, the schedule will immediately be active when starting Dagster. The default status can be overridden from the `Dagster UI </concepts/webserver/ui>`_ or via the `GraphQL API </concepts/webserver/graphql>`_.
         required_resource_keys (Optional[Set[str]]): The set of resource keys required by the schedule.
     """
 
     def inner(fn: RawScheduleEvaluationFunction) -> ScheduleDefinition:
         from dagster._config.pythonic_config import validate_resource_annotated_function
 
         check.callable_param(fn, "fn")
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.8/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.8/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.8/dagster/_core/definitions/definitions_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import dagster._check as check
 from dagster._annotations import deprecated, experimental, public
 from dagster._config.pythonic_config import (
     attach_resource_id_to_key_mapping,
 )
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
 from dagster._core.definitions.asset_graph import AssetGraph
+from dagster._core.definitions.asset_spec import AssetSpec
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKey
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.execution.build_resources import wrap_resources_for_execution
 from dagster._core.execution.with_resources import with_resources
 from dagster._core.executor.base import Executor
@@ -248,25 +249,15 @@
     ] = None,
     sensors: Optional[Iterable[SensorDefinition]] = None,
     jobs: Optional[Iterable[Union[JobDefinition, UnresolvedAssetJobDefinition]]] = None,
     resources: Optional[Mapping[str, Any]] = None,
     executor: Optional[Union[ExecutorDefinition, Executor]] = None,
     loggers: Optional[Mapping[str, LoggerDefinition]] = None,
     asset_checks: Optional[Iterable[AssetChecksDefinition]] = None,
-):
-    check.opt_iterable_param(
-        assets, "assets", (AssetsDefinition, SourceAsset, CacheableAssetsDefinition)
-    )
-    check.opt_iterable_param(
-        schedules, "schedules", (ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition)
-    )
-    check.opt_iterable_param(sensors, "sensors", SensorDefinition)
-    check.opt_iterable_param(jobs, "jobs", (JobDefinition, UnresolvedAssetJobDefinition))
-
-    check.opt_inst_param(executor, "executor", (ExecutorDefinition, Executor))
+) -> RepositoryDefinition:
     executor_def = (
         executor
         if isinstance(executor, ExecutorDefinition) or executor is None
         else ExecutorDefinition.hardcoded_executor(executor)
     )
 
     # Generate a mapping from each top-level resource instance ID to its resource key
@@ -281,16 +272,14 @@
         }
         if resources
         else {}
     )
 
     resource_defs = wrap_resources_for_execution(resources_with_key_mapping)
 
-    check.opt_mapping_param(loggers, "loggers", key_type=str, value_type=LoggerDefinition)
-
     # Binds top-level resources to jobs and any jobs attached to schedules or sensors
     (
         jobs_with_resources,
         schedules_with_resources,
         sensors_with_resources,
     ) = _attach_resources_to_jobs_and_instigator_jobs(jobs, schedules, sensors, resource_defs)
 
@@ -411,14 +400,23 @@
       :py:func:`with_resources <with_resources>` as before.
     * The resources dictionary takes raw Python objects, not just instances
       of :py:class:`ResourceDefinition`. If that raw object inherits from
       :py:class:`IOManager`, it gets coerced to an :py:class:`IOManagerDefinition`.
       Any other object is coerced to a :py:class:`ResourceDefinition`.
     """
 
+    _assets: Iterable[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]
+    _schedules: Iterable[Union[ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition]]
+    _sensors: Iterable[SensorDefinition]
+    _jobs: Iterable[Union[JobDefinition, UnresolvedAssetJobDefinition]]
+    _resources: Mapping[str, Any]
+    _executor: Optional[Union[ExecutorDefinition, Executor]]
+    _loggers: Mapping[str, LoggerDefinition]
+    _asset_checks: Iterable[AssetChecksDefinition]
+
     def __init__(
         self,
         assets: Optional[
             Iterable[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]
         ] = None,
         schedules: Optional[
             Iterable[Union[ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition]]
@@ -426,26 +424,88 @@
         sensors: Optional[Iterable[SensorDefinition]] = None,
         jobs: Optional[Iterable[Union[JobDefinition, UnresolvedAssetJobDefinition]]] = None,
         resources: Optional[Mapping[str, Any]] = None,
         executor: Optional[Union[ExecutorDefinition, Executor]] = None,
         loggers: Optional[Mapping[str, LoggerDefinition]] = None,
         asset_checks: Optional[Iterable[AssetChecksDefinition]] = None,
     ):
+        self._assets = check.opt_iterable_param(
+            assets,
+            "assets",
+            (AssetsDefinition, SourceAsset, CacheableAssetsDefinition),
+        )
+        self._schedules = check.opt_iterable_param(
+            schedules,
+            "schedules",
+            (ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition),
+        )
+        self._sensors = check.opt_iterable_param(sensors, "sensors", SensorDefinition)
+        self._jobs = check.opt_iterable_param(
+            jobs, "jobs", (JobDefinition, UnresolvedAssetJobDefinition)
+        )
+        # Thee's a bug that means that sometimes it's Dagster's fault when AssetsDefinitions are
+        # passed here instead of AssetChecksDefinitions: https://github.com/dagster-io/dagster/issues/22064.
+        # After we fix the bug, we should remove AssetsDefinition from the set of accepted types.
+        self._asset_checks = check.opt_iterable_param(
+            asset_checks,
+            "asset_checks",
+            (AssetChecksDefinition, AssetsDefinition),
+        )
+        self._resources = check.opt_mapping_param(resources, "resources", key_type=str)
+        self._executor = check.opt_inst_param(executor, "executor", (ExecutorDefinition, Executor))
+        self._loggers = check.opt_mapping_param(
+            loggers, "loggers", key_type=str, value_type=LoggerDefinition
+        )
+
         self._created_pending_or_normal_repo = _create_repository_using_definitions_args(
             name=SINGLETON_REPOSITORY_NAME,
             assets=assets,
             schedules=schedules,
             sensors=sensors,
             jobs=jobs,
             resources=resources,
             executor=executor,
             loggers=loggers,
             asset_checks=asset_checks,
         )
 
+    @property
+    def assets(self) -> Iterable[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
+        return self._assets
+
+    @property
+    def schedules(
+        self,
+    ) -> Iterable[Union[ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition]]:
+        return self._schedules
+
+    @property
+    def sensors(self) -> Iterable[SensorDefinition]:
+        return self._sensors
+
+    @property
+    def jobs(self) -> Iterable[Union[JobDefinition, UnresolvedAssetJobDefinition]]:
+        return self._jobs
+
+    @property
+    def resources(self) -> Mapping[str, Any]:
+        return self._resources
+
+    @property
+    def executor(self) -> Optional[Union[ExecutorDefinition, Executor]]:
+        return self._executor
+
+    @property
+    def loggers(self) -> Mapping[str, LoggerDefinition]:
+        return self._loggers
+
+    @property
+    def asset_checks(self) -> Iterable[AssetChecksDefinition]:
+        return self._asset_checks
+
     @public
     def get_job_def(self, name: str) -> JobDefinition:
         """Get a job definition by name. If you passed in a an :py:class:`UnresolvedAssetJobDefinition`
         (return value of :py:func:`define_asset_job`) it will be resolved to a :py:class:`JobDefinition` when returned
         from this function.
         """
         check.str_param(name, "name")
@@ -569,7 +629,84 @@
         point is to defer that resolution until later.
         """
         return self._created_pending_or_normal_repo
 
     def get_asset_graph(self) -> AssetGraph:
         """Get the AssetGraph for this set of definitions."""
         return self.get_repository_def().asset_graph
+
+    @staticmethod
+    def merge(*def_sets: "Definitions") -> "Definitions":
+        """Merges multiple Definitions objects into a single Definitions object.
+
+        The returned Definitions object has the union of all the definitions in the input
+        Definitions objects.
+
+        Returns:
+            Definitions: The merged definitions.
+        """
+        check.sequence_param(def_sets, "def_sets", of_type=Definitions)
+
+        assets = []
+        schedules = []
+        sensors = []
+        jobs = []
+        asset_checks = []
+
+        resources = {}
+        resource_key_indexes: Dict[str, int] = {}
+        loggers = {}
+        logger_key_indexes: Dict[str, int] = {}
+        executor = None
+        executor_index: Optional[int] = None
+
+        for i, def_set in enumerate(def_sets):
+            assets.extend(def_set.assets or [])
+            asset_checks.extend(def_set.asset_checks or [])
+            schedules.extend(def_set.schedules or [])
+            sensors.extend(def_set.sensors or [])
+            jobs.extend(def_set.jobs or [])
+
+            for resource_key, resource_value in (def_set.resources or {}).items():
+                if resource_key in resources:
+                    raise DagsterInvariantViolationError(
+                        f"Definitions objects {resource_key_indexes[resource_key]} and {i} both have a "
+                        f"resource with key '{resource_key}'"
+                    )
+                resources[resource_key] = resource_value
+                resource_key_indexes[resource_key] = i
+
+            for logger_key, logger_value in (def_set.loggers or {}).items():
+                if logger_key in loggers:
+                    raise DagsterInvariantViolationError(
+                        f"Definitions objects {logger_key_indexes[logger_key]} and {i} both have a "
+                        f"logger with key '{logger_key}'"
+                    )
+                loggers[logger_key] = logger_value
+                logger_key_indexes[logger_key] = i
+
+            if def_set.executor is not None:
+                if executor is not None and executor != def_set.executor:
+                    raise DagsterInvariantViolationError(
+                        f"Definitions objects {executor_index} and {i} both have an executor"
+                    )
+
+                executor = def_set.executor
+                executor_index = i
+
+        return Definitions(
+            assets=assets,
+            schedules=schedules,
+            sensors=sensors,
+            jobs=jobs,
+            resources=resources,
+            executor=executor,
+            loggers=loggers,
+            asset_checks=asset_checks,
+        )
+
+    @public
+    @experimental
+    def get_all_asset_specs(self) -> Sequence[AssetSpec]:
+        """Returns an AssetSpec object for every asset contained inside the Definitions object."""
+        asset_graph = self.get_asset_graph()
+        return [asset_node.to_asset_spec() for asset_node in asset_graph.asset_nodes]
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/dependency.py` & `dagster-1.7.8/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/events.py` & `dagster-1.7.8/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/external_asset.py` & `dagster-1.7.8/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.8/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.8/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.8/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.8/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.8/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/inference.py` & `dagster-1.7.8/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/input.py` & `dagster-1.7.8/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.8/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/job_base.py` & `dagster-1.7.8/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/job_definition.py` & `dagster-1.7.8/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.8/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.8/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.8/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.8/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/materialize.py` & `dagster-1.7.8/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/metadata/metadata_set.py` & `dagster-1.7.8/dagster/_core/definitions/metadata/metadata_set.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,61 +7,39 @@
 from dagster import _check as check
 from dagster._model import DagsterModel
 from dagster._model.pydantic_compat_layer import model_fields
 from dagster._utils.typing_api import flatten_unions
 
 from .metadata_value import MetadataValue, TableColumnLineage, TableSchema
 
-T_NamespacedMetadataSet = TypeVar("T_NamespacedMetadataSet", bound="NamespacedMetadataSet")
-
-
 # Python types that have a MetadataValue types that directly wraps them
 DIRECTLY_WRAPPED_METADATA_TYPES = {
     str,
     float,
     int,
     bool,
     TableSchema,
     TableColumnLineage,
     type(None),
 }
 
-T_NamespacedMetadataSet = TypeVar("T_NamespacedMetadataSet", bound="NamespacedMetadataSet")
+T_NamespacedKVSet = TypeVar("T_NamespacedKVSet", bound="NamespacedKVSet")
 
 
 def is_raw_metadata_type(t: Type) -> bool:
     return issubclass(t, MetadataValue) or t in DIRECTLY_WRAPPED_METADATA_TYPES
 
 
-class NamespacedMetadataSet(ABC, DagsterModel):
-    """Extend this class to define a set of metadata fields in the same namespace.
+class NamespacedKVSet(ABC, DagsterModel):
+    """Base class for defining a set of key-value pairs in the same namespace.
 
-    Supports splatting to a dictionary that can be placed inside a metadata argument along with
-    other dictionary-structured metadata.
-
-    .. code-block:: python
+    Includes shared behavior between NamespacedMetadataSet and NamespacedTagSet.
 
-        my_metadata: NamespacedMetadataSet = ...
-        return MaterializeResult(metadata={**my_metadata, ...})
     """
 
-    def __init__(self, *args, **kwargs):
-        for field_name in model_fields(self).keys():
-            annotation_types = self._get_accepted_types_for_field(field_name)
-            invalid_annotation_types = {
-                annotation_type
-                for annotation_type in annotation_types
-                if not is_raw_metadata_type(annotation_type)
-            }
-            if invalid_annotation_types:
-                check.failed(
-                    f"Type annotation for field '{field_name}' includes invalid metadata type(s): {invalid_annotation_types}"
-                )
-        super().__init__(*args, **kwargs)
-
     @classmethod
     @abstractmethod
     def namespace(cls) -> str:
         raise NotImplementedError()
 
     @classmethod
     def _namespaced_key(cls, key: str) -> str:
@@ -80,46 +58,77 @@
         }
 
     def __getitem__(self, key: str) -> Any:
         # getattr returns the pydantic property on the subclass
         return getattr(self, self._strip_namespace_from_key(key))
 
     @classmethod
-    def extract(
-        cls: Type[T_NamespacedMetadataSet], metadata: Mapping[str, Any]
-    ) -> T_NamespacedMetadataSet:
-        """Extracts entries from the provided metadata dictionary into an instance of this class.
+    def extract(cls: Type[T_NamespacedKVSet], values: Mapping[str, Any]) -> T_NamespacedKVSet:
+        """Extracts entries from the provided dictionary into an instance of this class.
 
-        Ignores any entries in the metadata dictionary whose keys don't correspond to fields on this
+        Ignores any entries in the dictionary whose keys don't correspond to fields on this
         class.
 
         In general, the following should always pass:
 
         .. code-block:: python
 
-            class MyMetadataSet(NamedspacedMetadataSet):
+            class MyKVSet(NamespacedKVSet):
                 ...
 
-            metadata: MyMetadataSet  = ...
-            assert MyMetadataSet.extract(dict(metadata)) == metadata
+            metadata: MyKVSet  = ...
+            assert MyKVSet.extract(dict(metadata)) == metadata
 
         Args:
-            metadata (Mapping[str, Any]): A dictionary of metadata entries.
+            values (Mapping[str, Any]): A dictionary of entries to extract.
         """
         kwargs = {}
-        for namespaced_key, value in metadata.items():
+        for namespaced_key, value in values.items():
             splits = namespaced_key.split("/")
             if len(splits) == 2:
                 namespace, key = splits
                 if namespace == cls.namespace() and key in model_fields(cls):
                     kwargs[key] = cls._extract_value(field_name=key, value=value)
 
         return cls(**kwargs)
 
     @classmethod
+    @abstractmethod
+    def _extract_value(cls, field_name: str, value: Any) -> Any:
+        """Based on type annotation, potentially coerce the value to the expected type."""
+        ...
+
+
+class NamespacedMetadataSet(NamespacedKVSet):
+    """Extend this class to define a set of metadata fields in the same namespace.
+
+    Supports splatting to a dictionary that can be placed inside a metadata argument along with
+    other dictionary-structured metadata.
+
+    .. code-block:: python
+
+        my_metadata: NamespacedMetadataSet = ...
+        return MaterializeResult(metadata={**my_metadata, ...})
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        for field_name in model_fields(self).keys():
+            annotation_types = self._get_accepted_types_for_field(field_name)
+            invalid_annotation_types = {
+                annotation_type
+                for annotation_type in annotation_types
+                if not is_raw_metadata_type(annotation_type)
+            }
+            if invalid_annotation_types:
+                check.failed(
+                    f"Type annotation for field '{field_name}' includes invalid metadata type(s): {invalid_annotation_types}"
+                )
+        super().__init__(*args, **kwargs)
+
+    @classmethod
     def _extract_value(cls, field_name: str, value: Any) -> Any:
         """Based on type annotation, potentially coerce the metadata value to its inner value.
 
         E.g. if the annotation is Optional[float] and the value is FloatMetadataValue, construct
         the MetadataSet using the inner float.
         """
         if isinstance(value, MetadataValue):
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/metadata/metadata_value.py` & `dagster-1.7.8/dagster/_core/definitions/metadata/metadata_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,49 +2,51 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import (
     Any,
     Callable,
     Generic,
     Mapping,
+    NamedTuple,
     Optional,
     Sequence,
     Union,
 )
 
-from pydantic import Field
 from typing_extensions import Self, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._annotations import PublicAttr, experimental, public
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._core.errors import DagsterInvalidMetadata
-from dagster._model import DagsterModel
-from dagster._serdes import pack_value, whitelist_for_serdes
+from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
-    FieldSerializer,
-    JsonSerializableValue,
     PackableValue,
-    UnpackContext,
-    WhitelistMap,
 )
 
 from .table import (  # re-exported
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
     TableRecord as TableRecord,
     TableSchema as TableSchema,
 )
 
 T_Packable = TypeVar("T_Packable", bound=PackableValue, default=PackableValue, covariant=True)
-
+from dagster._serdes import pack_value
+from dagster._serdes.serdes import (
+    FieldSerializer,
+    JsonSerializableValue,
+    PackableValue,
+    UnpackContext,
+    WhitelistMap,
+)
 
 # ########################
 # ##### METADATA VALUE
 # ########################
 
 
 class MetadataValue(ABC, Generic[T_Packable]):
@@ -346,15 +348,15 @@
         Args:
             run_id (str): The ID of the run.
         """
         return DagsterRunMetadataValue(run_id)
 
     @public
     @staticmethod
-    def asset(asset_key: "AssetKey") -> "DagsterAssetMetadataValue":
+    def asset(asset_key: AssetKey) -> "DagsterAssetMetadataValue":
         """Static constructor for a metadata value referencing a Dagster asset, by key.
 
         For example:
 
         .. code-block:: python
 
             @op
@@ -509,112 +511,111 @@
 # for us because these static methods should never be called on instances.
 
 # NOTE: `XMetadataValue` classes are serialized with a storage name of `XMetadataEntryData` to
 # maintain backward compatibility. See docstring of `whitelist_for_serdes` for more info.
 
 
 @whitelist_for_serdes(storage_name="TextMetadataEntryData")
-class TextMetadataValue(DagsterModel, MetadataValue[str]):
+class TextMetadataValue(
+    NamedTuple(
+        "_TextMetadataValue",
+        [
+            ("text", PublicAttr[Optional[str]]),
+        ],
+    ),
+    MetadataValue[str],
+):
     """Container class for text metadata entry data.
 
     Args:
         text (Optional[str]): The text data.
     """
 
-    text_inner: Optional[str] = Field(..., alias="text")
-
-    def __init__(self, text: Optional[str]):
-        super().__init__(text=text or "")
-
-    @public
-    @property
-    def text(self) -> Optional[str]:
-        return self.text_inner
+    def __new__(cls, text: Optional[str]):
+        return super(TextMetadataValue, cls).__new__(
+            cls, check.opt_str_param(text, "text", default="")
+        )
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped text data."""
-        return self.text_inner
+        return self.text
 
 
 @whitelist_for_serdes(storage_name="UrlMetadataEntryData")
-class UrlMetadataValue(DagsterModel, MetadataValue[str]):
+class UrlMetadataValue(
+    NamedTuple(
+        "_UrlMetadataValue",
+        [
+            ("url", PublicAttr[Optional[str]]),
+        ],
+    ),
+    MetadataValue[str],
+):
     """Container class for URL metadata entry data.
 
     Args:
         url (Optional[str]): The URL as a string.
     """
 
-    url_inner: Optional[str] = Field(..., alias="url")
-
-    def __init__(self, url: Optional[str]):
-        super().__init__(url=url or "")
+    def __new__(cls, url: Optional[str]):
+        return super(UrlMetadataValue, cls).__new__(
+            cls, check.opt_str_param(url, "url", default="")
+        )
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped URL."""
-        return self.url_inner
-
-    @public
-    @property
-    def url(self) -> Optional[str]:
-        """Optional[str]: The wrapped URL."""
-        return self.url_inner
+        return self.url
 
 
 @whitelist_for_serdes(storage_name="PathMetadataEntryData")
-class PathMetadataValue(DagsterModel, MetadataValue[str]):
+class PathMetadataValue(
+    NamedTuple("_PathMetadataValue", [("path", PublicAttr[Optional[str]])]), MetadataValue[str]
+):
     """Container class for path metadata entry data.
 
     Args:
         path (Optional[str]): The path as a string or conforming to os.PathLike.
     """
 
-    path_inner: Optional[str] = Field(..., alias="path")
-
-    def __init__(self, path: Optional[Union[str, os.PathLike]]):
-        super().__init__(path=check.opt_path_param(path, "path", default=""))
-
-    @public
-    @property
-    def path(self) -> Optional[str]:
-        return self.path_inner
+    def __new__(cls, path: Optional[Union[str, os.PathLike]]):
+        return super(PathMetadataValue, cls).__new__(
+            cls, check.opt_path_param(path, "path", default="")
+        )
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped path."""
-        return self.path_inner
+        return self.path
 
 
 @whitelist_for_serdes(storage_name="NotebookMetadataEntryData")
-class NotebookMetadataValue(DagsterModel, MetadataValue[str]):
+class NotebookMetadataValue(
+    NamedTuple("_NotebookMetadataValue", [("path", PublicAttr[Optional[str]])]), MetadataValue[str]
+):
     """Container class for notebook metadata entry data.
 
     Args:
         path (Optional[str]): The path to the notebook as a string or conforming to os.PathLike.
     """
 
-    path_inner: Optional[str] = Field(..., alias="path")
-
-    def __init__(self, path: Optional[Union[str, os.PathLike]]):
-        super().__init__(path=check.opt_path_param(path, "path", default=""))
-
-    @public
-    @property
-    def path(self) -> Optional[str]:
-        return self.path_inner
+    def __new__(cls, path: Optional[Union[str, os.PathLike]]):
+        return super(NotebookMetadataValue, cls).__new__(
+            cls, check.opt_path_param(path, "path", default="")
+        )
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped path to the notebook as a string."""
-        return self.path_inner
+        return self.path
 
 
 class JsonDataFieldSerializer(FieldSerializer):
     def pack(
         self,
         mapping: JsonSerializableValue,
         whitelist_map: WhitelistMap,
@@ -634,235 +635,281 @@
         return pack_value(unpacked_value, whitelist_map=whitelist_map)
 
 
 @whitelist_for_serdes(
     storage_name="JsonMetadataEntryData",
     field_serializers={"data": JsonDataFieldSerializer},
 )
-class JsonMetadataValue(DagsterModel, MetadataValue[Union[Sequence[Any], Mapping[str, Any]]]):
+class JsonMetadataValue(
+    NamedTuple(
+        "_JsonMetadataValue",
+        [
+            ("data", PublicAttr[Optional[Union[Sequence[Any], Mapping[str, Any]]]]),
+        ],
+    ),
+    MetadataValue[Union[Sequence[Any], Mapping[str, Any]]],
+):
     """Container class for JSON metadata entry data.
 
     Args:
         data (Union[Sequence[Any], Dict[str, Any]]): The JSON data.
     """
 
-    data: PublicAttr[Optional[Union[Sequence[Any], Mapping[str, Any]]]]
-
-    def __init__(self, data: Optional[Union[Sequence[Any], Mapping[str, Any]]]):
+    def __new__(cls, data: Optional[Union[Sequence[Any], Mapping[str, Any]]]):
         data = check.opt_inst_param(data, "data", (Sequence, Mapping))
         try:
             # check that the value is JSON serializable
             seven.dumps(data)
         except TypeError:
             raise DagsterInvalidMetadata("Value is not JSON serializable.")
-        super().__init__(data=data)
+        return super(JsonMetadataValue, cls).__new__(cls, data)
 
     @public
     @property
     def value(self) -> Optional[Union[Sequence[Any], Mapping[str, Any]]]:
         """Optional[Union[Sequence[Any], Dict[str, Any]]]: The wrapped JSON data."""
         return self.data
 
 
 @whitelist_for_serdes(storage_name="MarkdownMetadataEntryData")
-class MarkdownMetadataValue(DagsterModel, MetadataValue[str]):
+class MarkdownMetadataValue(
+    NamedTuple(
+        "_MarkdownMetadataValue",
+        [
+            ("md_str", PublicAttr[Optional[str]]),
+        ],
+    ),
+    MetadataValue[str],
+):
     """Container class for markdown metadata entry data.
 
     Args:
         md_str (Optional[str]): The markdown as a string.
     """
 
-    md_str: PublicAttr[Optional[str]]
-
-    def __init__(self, md_str: Optional[str]):
-        super().__init__(md_str=md_str or "")
+    def __new__(cls, md_str: Optional[str]):
+        return super(MarkdownMetadataValue, cls).__new__(
+            cls, check.opt_str_param(md_str, "md_str", default="")
+        )
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped markdown as a string."""
         return self.md_str
 
 
 # This should be deprecated or fixed so that `value` does not return itself.
 @whitelist_for_serdes(storage_name="PythonArtifactMetadataEntryData")
-class PythonArtifactMetadataValue(DagsterModel, MetadataValue["PythonArtifactMetadataValue"]):
+class PythonArtifactMetadataValue(
+    NamedTuple(
+        "_PythonArtifactMetadataValue",
+        [
+            ("module", PublicAttr[str]),
+            ("name", PublicAttr[str]),
+        ],
+    ),
+    MetadataValue["PythonArtifactMetadataValue"],
+):
     """Container class for python artifact metadata entry data.
 
     Args:
         module (str): The module where the python artifact can be found
         name (str): The name of the python artifact
     """
 
-    module: PublicAttr[str]
-    name: PublicAttr[str]
-
-    def __init__(self, module: str, name: str):
-        super().__init__(module=module, name=name)
+    def __new__(cls, module: str, name: str):
+        return super(PythonArtifactMetadataValue, cls).__new__(
+            cls, check.str_param(module, "module"), check.str_param(name, "name")
+        )
 
     @public
     @property
     def value(self) -> Self:
         """PythonArtifactMetadataValue: Identity function."""
         return self
 
 
 @whitelist_for_serdes(storage_name="FloatMetadataEntryData")
-class FloatMetadataValue(DagsterModel, MetadataValue[float]):
+class FloatMetadataValue(
+    NamedTuple(
+        "_FloatMetadataValue",
+        [
+            ("value", PublicAttr[Optional[float]]),
+        ],
+    ),
+    MetadataValue[float],
+):
     """Container class for float metadata entry data.
 
     Args:
         value (Optional[float]): The float value.
     """
 
-    value_inner: Optional[float] = Field(..., alias="value")
-
-    def __init__(self, value: Optional[float]):
-        super().__init__(value=value)
-
-    @public
-    @property
-    def value(self) -> Optional[float]:
-        return self.value_inner
+    def __new__(cls, value: Optional[float]):
+        return super(FloatMetadataValue, cls).__new__(cls, check.opt_float_param(value, "value"))
 
 
 @whitelist_for_serdes(storage_name="IntMetadataEntryData")
-class IntMetadataValue(DagsterModel, MetadataValue[int]):
+class IntMetadataValue(
+    NamedTuple(
+        "_IntMetadataValue",
+        [
+            ("value", PublicAttr[Optional[int]]),
+        ],
+    ),
+    MetadataValue[int],
+):
     """Container class for int metadata entry data.
 
     Args:
         value (Optional[int]): The int value.
     """
 
-    value_inner: Optional[int] = Field(..., alias="value")
-
-    def __init__(self, value: Optional[int]):
-        super().__init__(value=value)
-
-    @public
-    @property
-    def value(self) -> Optional[int]:
-        return self.value_inner
+    def __new__(cls, value: Optional[int]):
+        return super(IntMetadataValue, cls).__new__(cls, check.opt_int_param(value, "value"))
 
 
 @whitelist_for_serdes(storage_name="BoolMetadataEntryData")
-class BoolMetadataValue(DagsterModel, MetadataValue[bool]):
+class BoolMetadataValue(
+    NamedTuple("_BoolMetadataValue", [("value", PublicAttr[Optional[bool]])]),
+    MetadataValue[bool],
+):
     """Container class for bool metadata entry data.
 
     Args:
         value (Optional[bool]): The bool value.
     """
 
-    value_inner: Optional[bool] = Field(..., alias="value")
-
-    def __init__(self, value: Optional[bool]):
-        super().__init__(value=value)
-
-    @public
-    @property
-    def value(self) -> Optional[bool]:
-        return self.value_inner
+    def __new__(cls, value: Optional[bool]):
+        return super(BoolMetadataValue, cls).__new__(cls, check.opt_bool_param(value, "value"))
 
 
 @whitelist_for_serdes
-class TimestampMetadataValue(DagsterModel, MetadataValue[float]):
+class TimestampMetadataValue(
+    NamedTuple(
+        "_DateTimeMetadataValue",
+        [("value", PublicAttr[float])],
+    ),
+    MetadataValue[float],
+):
     """Container class for metadata value that's a unix timestamp.
 
     Args:
         value (float): Seconds since the unix epoch.
     """
 
-    value_inner: Optional[float] = Field(..., alias="value")
-
-    def __init__(self, value: float):
-        super().__init__(value=value)
-
-    @public
-    @property
-    def value(self) -> Optional[float]:
-        return self.value_inner
+    def __new__(cls, value: float):
+        return super(TimestampMetadataValue, cls).__new__(cls, check.float_param(value, "value"))
 
 
 @whitelist_for_serdes(storage_name="DagsterPipelineRunMetadataEntryData")
-class DagsterRunMetadataValue(DagsterModel, MetadataValue[str]):
+class DagsterRunMetadataValue(
+    NamedTuple(
+        "_DagsterRunMetadataValue",
+        [
+            ("run_id", PublicAttr[str]),
+        ],
+    ),
+    MetadataValue[str],
+):
     """Representation of a dagster run.
 
     Args:
         run_id (str): The run id
     """
 
-    run_id: PublicAttr[str]
-
-    def __init__(self, run_id: str):
-        super().__init__(run_id=run_id)
+    def __new__(cls, run_id: str):
+        return super(DagsterRunMetadataValue, cls).__new__(cls, check.str_param(run_id, "run_id"))
 
     @public
     @property
     def value(self) -> str:
         """str: The wrapped run id."""
         return self.run_id
 
 
 @whitelist_for_serdes
-class DagsterJobMetadataValue(DagsterModel, MetadataValue["DagsterJobMetadataValue"]):
+class DagsterJobMetadataValue(
+    NamedTuple(
+        "_DagsterJobMetadataValue",
+        [
+            ("job_name", PublicAttr[str]),
+            ("location_name", PublicAttr[str]),
+            ("repository_name", PublicAttr[Optional[str]]),
+        ],
+    ),
+    MetadataValue["DagsterJobMetadataValue"],
+):
     """Representation of a dagster run.
 
     Args:
         job_name (str): The job's name
         location_name (str): The job's code location name
         repository_name (Optional[str]): The job's repository name. If not provided, the job is
             assumed to be in the same repository as this object.
     """
 
-    job_name: PublicAttr[str]
-    location_name: PublicAttr[str]
-    repository_name: PublicAttr[Optional[str]]
-
-    def __init__(
-        self,
+    def __new__(
+        cls,
         job_name: str,
         location_name: str,
         repository_name: Optional[str] = None,
     ):
-        super().__init__(
-            job_name=job_name,
-            location_name=location_name,
-            repository_name=repository_name,
+        return super(DagsterJobMetadataValue, cls).__new__(
+            cls,
+            check.str_param(job_name, "job_name"),
+            check.str_param(location_name, "location_name"),
+            check.opt_str_param(repository_name, "repository_name"),
         )
 
     @public
     @property
     def value(self) -> Self:
         return self
 
 
 @whitelist_for_serdes(storage_name="DagsterAssetMetadataEntryData")
-class DagsterAssetMetadataValue(DagsterModel, MetadataValue[AssetKey]):
+class DagsterAssetMetadataValue(
+    NamedTuple("_DagsterAssetMetadataValue", [("asset_key", PublicAttr[AssetKey])]),
+    MetadataValue[AssetKey],
+):
     """Representation of a dagster asset.
 
     Args:
         asset_key (AssetKey): The dagster asset key
     """
 
-    asset_key: PublicAttr[AssetKey]
+    def __new__(cls, asset_key: AssetKey):
+        from dagster._core.definitions.events import AssetKey
 
-    def __init__(self, asset_key: AssetKey):
-        super().__init__(asset_key=asset_key)
+        return super(DagsterAssetMetadataValue, cls).__new__(
+            cls, check.inst_param(asset_key, "asset_key", AssetKey)
+        )
 
     @public
     @property
-    def value(self) -> "AssetKey":
+    def value(self) -> AssetKey:
         """AssetKey: The wrapped :py:class:`AssetKey`."""
         return self.asset_key
 
 
 # This should be deprecated or fixed so that `value` does not return itself.
 @experimental
 @whitelist_for_serdes(storage_name="TableMetadataEntryData")
-class TableMetadataValue(DagsterModel, MetadataValue["TableMetadataValue"]):
+class TableMetadataValue(
+    NamedTuple(
+        "_TableMetadataValue",
+        [
+            ("records", PublicAttr[Sequence[TableRecord]]),
+            ("schema", PublicAttr[TableSchema]),
+        ],
+    ),
+    MetadataValue["TableMetadataValue"],
+):
     """Container class for table metadata entry data.
 
     Args:
         records (TableRecord): The data as a list of records (i.e. rows).
         schema (Optional[TableSchema]): A schema for the table.
 
     Example:
@@ -875,31 +922,28 @@
                 records=[
                     TableRecord({"column1": 5, "column2": "x"}),
                     TableRecord({"column1": 7, "column2": "y"}),
                 ]
             )
     """
 
-    records: PublicAttr[Sequence[TableRecord]]
-    schema_inner: TableSchema = Field(..., alias="schema")
-
     @public
     @staticmethod
     def infer_column_type(value: object) -> str:
         """str: Infer the :py:class:`TableSchema` column type that will be used for a value."""
         if isinstance(value, bool):
             return "bool"
         elif isinstance(value, int):
             return "int"
         elif isinstance(value, float):
             return "float"
         else:
             return "string"
 
-    def __init__(self, records: Sequence[TableRecord], schema: Optional[TableSchema] = None):
+    def __new__(cls, records: Sequence[TableRecord], schema: Optional[TableSchema]):
         check.sequence_param(records, "records", of_type=TableRecord)
         check.opt_inst_param(schema, "schema", TableSchema)
 
         if len(records) == 0:
             schema = check.not_none(schema, "schema must be provided if records is empty")
         else:
             columns = set(records[0].data.keys())
@@ -910,81 +954,78 @@
             schema = schema or TableSchema(
                 columns=[
                     TableColumn(name=k, type=TableMetadataValue.infer_column_type(v))
                     for k, v in records[0].data.items()
                 ]
             )
 
-        super().__init__(records=records, schema=schema)
-
-    @public
-    @property
-    def schema(self) -> TableSchema:
-        return self.schema_inner
+        return super(TableMetadataValue, cls).__new__(
+            cls,
+            records,
+            schema,
+        )
 
     @public
     @property
     def value(self) -> Self:
         """TableMetadataValue: Identity function."""
         return self
 
 
 @whitelist_for_serdes(storage_name="TableSchemaMetadataEntryData")
-class TableSchemaMetadataValue(DagsterModel, MetadataValue[TableSchema]):
+class TableSchemaMetadataValue(
+    NamedTuple("_TableSchemaMetadataValue", [("schema", PublicAttr[TableSchema])]),
+    MetadataValue[TableSchema],
+):
     """Representation of a schema for arbitrary tabular data.
 
     Args:
         schema (TableSchema): The dictionary containing the schema representation.
     """
 
-    schema_inner: TableSchema = Field(..., alias="schema")
-
-    def __init__(self, schema: TableSchema):
-        super().__init__(schema=schema)
+    def __new__(cls, schema: TableSchema):
+        return super(TableSchemaMetadataValue, cls).__new__(
+            cls, check.inst_param(schema, "schema", TableSchema)
+        )
 
     @public
     @property
     def value(self) -> TableSchema:
         """TableSchema: The wrapped :py:class:`TableSchema`."""
-        return self.schema_inner
-
-    @public
-    @property
-    def schema(self) -> TableSchema:
-        return self.schema_inner
+        return self.schema
 
 
 @whitelist_for_serdes
-class TableColumnLineageMetadataValue(DagsterModel, MetadataValue[TableColumnLineage]):
+class TableColumnLineageMetadataValue(
+    NamedTuple(
+        "_TableColumnLineageMetadataValue", [("column_lineage", PublicAttr[TableColumnLineage])]
+    ),
+    MetadataValue[TableColumnLineage],
+):
     """Representation of the lineage of column inputs to column outputs of arbitrary tabular data.
 
     Args:
         column_lineage (TableColumnLineage): The lineage of column inputs to column outputs
             for the table.
     """
 
-    column_lineage_inner: TableColumnLineage = Field(..., alias="column_lineage")
-
-    def __init__(self, column_lineage: TableColumnLineage):
-        super().__init__(column_lineage=column_lineage)
-
-    @public
-    @property
-    def column_lineage(self) -> TableColumnLineage:
-        return self.column_lineage_inner
+    def __new__(cls, column_lineage: TableColumnLineage):
+        return super(TableColumnLineageMetadataValue, cls).__new__(
+            cls, check.inst_param(column_lineage, "column_lineage", TableColumnLineage)
+        )
 
     @public
     @property
     def value(self) -> TableColumnLineage:
         """TableSpec: The wrapped :py:class:`TableSpec`."""
-        return self.column_lineage_inner
+        return self.column_lineage
 
 
 @whitelist_for_serdes(storage_name="NullMetadataEntryData")
-class NullMetadataValue(DagsterModel, MetadataValue[None]):
+class NullMetadataValue(NamedTuple("_NullMetadataValue", []), MetadataValue[None]):
     """Representation of null."""
 
     @public
     @property
     def value(self) -> None:
         """None: The wrapped null value."""
         return None
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/metadata/source_code.py` & `dagster-1.7.8/dagster/_core/definitions/metadata/source_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,22 @@
                 **metadata_by_key.get(key, {}),
                 **CodeReferencesMetadataSet(
                     code_references=CodeReferencesMetadataValue(code_references=sources_for_asset)
                 ),
             }
 
     return AssetsDefinition.dagster_internal_init(
-        **{**assets_def.get_attributes_dict(), "metadata_by_key": metadata_by_key}
+        **{
+            **assets_def.get_attributes_dict(),
+            **{
+                "specs": [
+                    spec._replace(metadata=metadata_by_key[spec.key]) for spec in assets_def.specs
+                ]
+            },
+        }
     )
 
 
 def convert_local_path_to_source_control_path(
     base_source_control_url: str,
     repository_root_absolute_path: str,
     local_path: LocalFileCodeReference,
@@ -195,15 +202,22 @@
             **metadata_by_key.get(key, {}),
             **CodeReferencesMetadataSet(
                 code_references=CodeReferencesMetadataValue(code_references=sources_for_asset)
             ),
         }
 
     return AssetsDefinition.dagster_internal_init(
-        **{**assets_def.get_attributes_dict(), "metadata_by_key": metadata_by_key}
+        **{
+            **assets_def.get_attributes_dict(),
+            **{
+                "specs": [
+                    spec._replace(metadata=metadata_by_key[spec.key]) for spec in assets_def.specs
+                ]
+            },
+        }
     )
 
 
 def _build_github_url(url: str, branch: str) -> str:
     return f"{url}/tree/{branch}"
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.8/dagster/_core/definitions/metadata/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping, NamedTuple, Optional, Sequence, Union, cast
+from typing import Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, experimental, public
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._serdes.serdes import (
     whitelist_for_serdes,
 )
@@ -204,22 +204,19 @@
         constraints: Optional["TableColumnConstraints"] = None,
     ):
         return super(TableColumn, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             type=check.str_param(type, "type"),
             description=check.opt_str_param(description, "description"),
-            constraints=cast(
-                "TableColumnConstraints",
-                check.opt_inst_param(
-                    constraints,
-                    "constraints",
-                    TableColumnConstraints,
-                    default=_DEFAULT_TABLE_COLUMN_CONSTRAINTS,
-                ),
+            constraints=check.opt_inst_param(
+                constraints,
+                "constraints",
+                TableColumnConstraints,
+                default=_DEFAULT_TABLE_COLUMN_CONSTRAINTS,
             ),
         )
 
 
 # ########################
 # ##### TABLE COLUMN CONSTRAINTS
 # ########################
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.8/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/node_container.py` & `dagster-1.7.8/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/node_definition.py` & `dagster-1.7.8/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/observe.py` & `dagster-1.7.8/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/op_definition.py` & `dagster-1.7.8/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.8/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/op_selection.py` & `dagster-1.7.8/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/output.py` & `dagster-1.7.8/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/partition.py` & `dagster-1.7.8/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.8/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.8/dagster/_core/definitions/partition_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import collections.abc
 import itertools
+import warnings
 from abc import ABC, abstractmethod, abstractproperty
 from collections import defaultdict
 from datetime import datetime
+from functools import lru_cache
 from typing import (
     Collection,
     Dict,
     List,
     Mapping,
     NamedTuple,
     Optional,
@@ -1123,20 +1125,37 @@
             return TimeWindowPartitionMapping()
         else:
             return IdentityPartitionMapping()
     else:
         return AllPartitionMapping()
 
 
+@lru_cache(maxsize=1)
 def get_builtin_partition_mapping_types() -> Tuple[Type[PartitionMapping], ...]:
     from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 
     return (
         AllPartitionMapping,
         IdentityPartitionMapping,
         LastPartitionMapping,
         SpecificPartitionsPartitionMapping,
         StaticPartitionMapping,
         TimeWindowPartitionMapping,
         MultiToSingleDimensionPartitionMapping,
         MultiPartitionMapping,
     )
+
+
+def warn_if_partition_mapping_not_builtin(partition_mapping: PartitionMapping) -> None:
+    builtin_partition_mappings = get_builtin_partition_mapping_types()
+    if not isinstance(partition_mapping, builtin_partition_mappings):
+        warnings.warn(
+            f"Non-built-in PartitionMappings, such as {type(partition_mapping).__name__} "
+            "are deprecated and will not work with asset reconciliation. The built-in "
+            "partition mappings are "
+            + ", ".join(
+                builtin_partition_mapping.__name__
+                for builtin_partition_mapping in builtin_partition_mappings
+            )
+            + ".",
+            category=DeprecationWarning,
+        )
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.8/dagster/_core/definitions/partitioned_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,21 +72,21 @@
     day_of_week: Optional[int] = None,
     day_of_month: Optional[int] = None,
     default_status: DefaultScheduleStatus = DefaultScheduleStatus.STOPPED,
     tags: Optional[Mapping[str, str]] = None,
     cron_schedule: Optional[str] = None,
     execution_timezone: Optional[str] = None,
 ) -> Union[UnresolvedPartitionedAssetScheduleDefinition, ScheduleDefinition]:
-    """Creates a schedule from a time window-partitioned job a job that targets
+    """Creates a schedule from a job that targets
     time window-partitioned or statically-partitioned assets. The job can also be
-    multipartitioned, as long as one of the partitions dimensions is time-partitioned.
+    multi-partitioned, as long as one of the partition dimensions is time-partitioned. Refer to the `Partitions API reference </_apidocs/partitions#partitioned-config>`_ for information about time-based run configuration.
 
-    The schedule executes at the cadence specified by the time partitioning of the job or assets.
+    The schedule executes at the cadence specified by the time partitioning of the job or assets. Refer to the `Partitions documentation </concepts/partitions-schedules-sensors/partitions>`_ for more information.
 
-    Examples:
+    **Example:**
         .. code-block:: python
 
             ######################################
             # Job that targets partitioned assets
             ######################################
 
             from dagster import (
@@ -143,14 +143,20 @@
         ),
         "Cannot provide both cron_schedule / execution_timezone parameters and"
         " day_of_month / day_of_week / hour_of_day / minute_of_hour parameters to"
         " build_schedule_from_partitioned_job.",
     )
 
     if isinstance(job, UnresolvedAssetJobDefinition) and job.partitions_def is None:
+        if cron_schedule or execution_timezone:
+            check.failed(
+                "Cannot provide cron_schedule or execution_timezone to"
+                " build_schedule_from_partitioned_job for a time-partitioned job."
+            )
+
         return UnresolvedPartitionedAssetScheduleDefinition(
             job=job,
             default_status=default_status,
             name=check.opt_str_param(name, "name", f"{job.name}_schedule"),
             description=check.opt_str_param(description, "description"),
             minute_of_hour=minute_of_hour,
             hour_of_day=hour_of_day,
@@ -246,15 +252,19 @@
             ]
 
     return schedule_fn
 
 
 def _check_valid_schedule_partitions_def(
     partitions_def: PartitionsDefinition,
-) -> Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition, StaticPartitionsDefinition]:
+) -> Union[
+    TimeWindowPartitionsDefinition,
+    MultiPartitionsDefinition,
+    StaticPartitionsDefinition,
+]:
     if not has_one_dimension_time_window_partitioning(partitions_def) and not isinstance(
         partitions_def, StaticPartitionsDefinition
     ):
         raise DagsterInvalidDefinitionError(
             "Tried to build a partitioned schedule from an asset job, but received an invalid"
             " partitions definition. The permitted partitions definitions are: \n1."
             " TimeWindowPartitionsDefinition\n2. MultiPartitionsDefinition with a single"
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/policy.py` & `dagster-1.7.8/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.8/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.8/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.8/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.8/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.8/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.8/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.8/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.8/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/result.py` & `dagster-1.7.8/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/run_config.py` & `dagster-1.7.8/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.8/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/run_request.py` & `dagster-1.7.8/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.8/dagster/_core/definitions/schedule_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,20 +141,20 @@
     if resource_args_from_kwargs:
         return context.merge_resources(resource_args_from_kwargs)
 
     return context
 
 
 class ScheduleEvaluationContext:
-    """The context object available as the first argument various functions defined on a :py:class:`dagster.ScheduleDefinition`.
+    """The context object available as the first argument to various functions defined on a :py:class:`dagster.ScheduleDefinition`.
 
-    A `ScheduleEvaluationContext` object is passed as the first argument to ``run_config_fn``, ``tags_fn``,
+    A ``ScheduleEvaluationContext`` object is passed as the first argument to ``run_config_fn``, ``tags_fn``,
     and ``should_execute``.
 
-    Users should not instantiate this object directly. To construct a `ScheduleEvaluationContext` for testing purposes, use :py:func:`dagster.build_schedule_context`.
+    **Users should not instantiate this object directly**. To construct a ``ScheduleEvaluationContext`` for testing purposes, use :py:func:`dagster.build_schedule_context`.
 
     Example:
         .. code-block:: python
 
             from dagster import schedule, ScheduleEvaluationContext
 
             @schedule
@@ -296,15 +296,15 @@
             },
             repository_def=self._repository_def,
         )
 
     @public
     @property
     def instance(self) -> "DagsterInstance":
-        """DagsterInstance: The current DagsterInstance."""
+        """DagsterInstance: The current :py:class:`~dagster.DagsterInstance`."""
         # self._instance_ref should only ever be None when this ScheduleEvaluationContext was
         # constructed under test.
         if not self._instance_ref:
             raise DagsterInvariantViolationError(
                 "Attempted to initialize dagster instance, but no instance reference was provided."
             )
         if not self._instance:
@@ -387,18 +387,18 @@
     resources: Optional[Mapping[str, object]] = None,
     repository_def: Optional["RepositoryDefinition"] = None,
     instance_ref: Optional["InstanceRef"] = None,
 ) -> ScheduleEvaluationContext:
     """Builds schedule execution context using the provided parameters.
 
     The instance provided to ``build_schedule_context`` must be persistent;
-    DagsterInstance.ephemeral() will result in an error.
+    :py:class:`DagsterInstance.ephemeral() <DagsterInstance>` will result in an error.
 
     Args:
-        instance (Optional[DagsterInstance]): The dagster instance configured to run the schedule.
+        instance (Optional[DagsterInstance]): The Dagster instance configured to run the schedule.
         scheduled_execution_time (datetime): The time in which the execution was scheduled to
             happen. May differ slightly from both the actual execution time and the time at which
             the run config is computed.
 
     Examples:
         .. code-block:: python
 
@@ -478,55 +478,51 @@
     breaking_version="2.0",
     additional_warn_text=(
         "It is no longer necessary. Schedules will have access to all environment variables set in"
         " the containing environment, and can safely be deleted."
     ),
 )
 class ScheduleDefinition(IHasInternalInit):
-    """Define a schedule that targets a job.
+    """Defines a schedule that targets a job.
 
     Args:
         name (Optional[str]): The name of the schedule to create. Defaults to the job name plus
-            "_schedule".
+            ``_schedule``.
         cron_schedule (Union[str, Sequence[str]]): A valid cron string or sequence of cron strings
-            specifying when the schedule will run, e.g., ``'45 23 * * 6'`` for a schedule that runs
+            specifying when the schedule will run, e.g., ``45 23 * * 6`` for a schedule that runs
             at 11:45 PM every Saturday. If a sequence is provided, then the schedule will run for
             the union of all execution times for the provided cron strings, e.g.,
             ``['45 23 * * 6', '30 9 * * 0]`` for a schedule that runs at 11:45 PM every Saturday and
             9:30 AM every Sunday.
-        execution_fn (Callable[ScheduleEvaluationContext]): The core evaluation function for the
-            schedule, which is run at an interval to determine whether a run should be launched or
-            not. Takes a :py:class:`~dagster.ScheduleEvaluationContext`.
+        execution_fn (Callable[ScheduleEvaluationContext]): The core evaluation function for the schedule, which is run at an interval to determine whether a run should be launched or not. Takes a :py:class:`~dagster.ScheduleEvaluationContext`.
 
-            This function must return a generator, which must yield either a single SkipReason
-            or one or more RunRequest objects.
+            This function must return a generator, which must yield either a single :py:class:`~dagster.SkipReason`
+            or one or more :py:class:`~dagster.RunRequest` objects.
         run_config (Optional[Mapping]): The config that parameterizes this execution,
             as a dict.
         run_config_fn (Optional[Callable[[ScheduleEvaluationContext], [Mapping]]]): A function that
-            takes a ScheduleEvaluationContext object and returns the run configuration that
-            parameterizes this execution, as a dict. You may set only one of ``run_config``,
-            ``run_config_fn``, and ``execution_fn``.
+            takes a :py:class:`~dagster.ScheduleEvaluationContext` object and returns the run configuration that
+            parameterizes this execution, as a dict. **Note**: Only one of the following may be set: You may set ``run_config``, ``run_config_fn``, or ``execution_fn``.
         tags (Optional[Mapping[str, str]]): A dictionary of tags (string key-value pairs) to attach
             to the scheduled runs.
         tags_fn (Optional[Callable[[ScheduleEvaluationContext], Optional[Mapping[str, str]]]]): A
-            function that generates tags to attach to the schedules runs. Takes a
+            function that generates tags to attach to the schedule's runs. Takes a
             :py:class:`~dagster.ScheduleEvaluationContext` and returns a dictionary of tags (string
-            key-value pairs). You may set only one of ``tags``, ``tags_fn``, and ``execution_fn``.
+            key-value pairs). **Note**: Only one of the following may be set:  ``tags``, ``tags_fn``, or ``execution_fn``.
         should_execute (Optional[Callable[[ScheduleEvaluationContext], bool]]): A function that runs
             at schedule execution time to determine whether a schedule should execute or skip. Takes
             a :py:class:`~dagster.ScheduleEvaluationContext` and returns a boolean (``True`` if the
             schedule should execute). Defaults to a function that always returns ``True``.
         execution_timezone (Optional[str]): Timezone in which the schedule should run.
             Supported strings for timezones are the ones provided by the
-            `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
+            `IANA time zone database <https://www.iana.org/time-zones>`_ - e.g. ``"America/Los_Angeles"``.
         description (Optional[str]): A human-readable description of the schedule.
         job (Optional[Union[GraphDefinition, JobDefinition]]): The job that should execute when this
             schedule runs.
-        default_status (DefaultScheduleStatus): Whether the schedule starts as running or not. The default
-            status can be overridden from the Dagster UI or via the GraphQL API.
+        default_status (DefaultScheduleStatus): If set to ``RUNNING``, the schedule will start as running. The default status can be overridden from the `Dagster UI </concepts/webserver/ui>`_ or via the `GraphQL API </concepts/webserver/graphql>`_.
         required_resource_keys (Optional[Set[str]]): The set of resource keys required by the schedule.
     """
 
     def with_updated_job(self, new_job: ExecutableDefinition) -> "ScheduleDefinition":
         """Returns a copy of this schedule with the job replaced.
 
         Args:
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.8/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/selector.py` & `dagster-1.7.8/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.8/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/source_asset.py` & `dagster-1.7.8/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.8/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/target.py` & `dagster-1.7.8/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.8/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.8/dagster/_core/definitions/time_window_partitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,14 +242,37 @@
     def is_empty(self) -> bool:
         return self.start == self.end
 
     @staticmethod
     def empty() -> "TimeWindow":
         return TimeWindow(start=datetime.max, end=datetime.max)
 
+    def subtract(self, other: "TimeWindow") -> Sequence["TimeWindow"]:
+        other_start_timestamp = other.start.timestamp()
+        start_timestamp = self.start.timestamp()
+        other_end_timestamp = other.end.timestamp()
+        end_timestamp = self.end.timestamp()
+
+        # Case where the two don't intersect at all - just return self
+        # Note that this assumes end is exclusive
+        if end_timestamp <= other_start_timestamp or other_end_timestamp <= start_timestamp:
+            return [self]
+
+        windows = []
+
+        if other_start_timestamp > start_timestamp:
+            windows.append(
+                TimeWindow(start=self.start, end=other.start),
+            )
+
+        if other_end_timestamp < end_timestamp:
+            windows.append(TimeWindow(start=other.end, end=self.end))
+
+        return windows
+
 
 @whitelist_for_serdes(
     field_serializers={"start": DatetimeFieldSerializer, "end": DatetimeFieldSerializer},
     is_pickleable=False,
 )
 class TimeWindowPartitionsDefinition(
     PartitionsDefinition,
@@ -367,84 +390,50 @@
     def get_current_timestamp(self, current_time: Optional[datetime] = None) -> float:
         return (
             pendulum.instance(current_time, tz=self.timezone)
             if current_time
             else pendulum.now(self.timezone)
         ).timestamp()
 
-    def _get_fast_num_partitions(self, current_time: Optional[datetime] = None) -> Optional[int]:
-        """Computes the total number of partitions quickly for common partition windows. Returns
-        None if the count cannot be computed quickly and must enumerate all partitions before
-        counting them.
-        """
-        last_partition_window = self.get_last_partition_window(current_time)
-        first_partition_window = self.get_first_partition_window(current_time)
-
-        if not last_partition_window or not first_partition_window:
-            return None
-
+    def get_num_partitions_in_window(self, time_window: TimeWindow) -> int:
         if self.is_basic_daily:
             return (
                 date(
-                    last_partition_window.start.year,
-                    last_partition_window.start.month,
-                    last_partition_window.start.day,
+                    time_window.end.year,
+                    time_window.end.month,
+                    time_window.end.day,
                 )
                 - date(
-                    first_partition_window.start.year,
-                    first_partition_window.start.month,
-                    first_partition_window.start.day,
+                    time_window.start.year,
+                    time_window.start.month,
+                    time_window.start.day,
                 )
-            ).days + 1
+            ).days
 
         fixed_minute_interval = get_fixed_minute_interval(self.cron_schedule)
         if fixed_minute_interval:
-            minutes_in_window = (
-                last_partition_window.start.timestamp() - first_partition_window.start.timestamp()
-            ) / 60
-            return int(minutes_in_window // fixed_minute_interval) + 1
+            minutes_in_window = (time_window.end.timestamp() - time_window.start.timestamp()) / 60
+            return int(minutes_in_window // fixed_minute_interval)
 
-        return None
+        return len(self.get_partition_keys_in_time_window(time_window))
 
     def get_num_partitions(
         self,
         current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> int:
-        # Method added for performance reasons.
-        # Fetching partition keys requires significantly more compute time to
-        # string format datetimes.
-
-        fast_num_partitions = self._get_fast_num_partitions(current_time)
-        if fast_num_partitions is not None:
-            return fast_num_partitions
-
-        current_timestamp = self.get_current_timestamp(current_time=current_time)
-
-        partitions_past_current_time = 0
-
-        num_partitions = 0
-        for time_window in self._iterate_time_windows(self.start):
-            if self.end and time_window.end.timestamp() > self.end.timestamp():
-                break
-            if (
-                time_window.end.timestamp() <= current_timestamp
-                or partitions_past_current_time < self.end_offset
-            ):
-                num_partitions += 1
-
-                if time_window.end.timestamp() > current_timestamp:
-                    partitions_past_current_time += 1
-            else:
-                break
+        last_partition_window = self.get_last_partition_window(current_time)
+        first_partition_window = self.get_first_partition_window(current_time)
 
-        if self.end_offset < 0:
-            num_partitions += self.end_offset
+        if not last_partition_window or not first_partition_window:
+            return 0
 
-        return num_partitions
+        return self.get_num_partitions_in_window(
+            TimeWindow(start=first_partition_window.start, end=last_partition_window.end)
+        )
 
     def get_partition_keys_between_indexes(
         self, start_idx: int, end_idx: int, current_time: Optional[datetime] = None
     ) -> List[str]:
         # Fetches the partition keys between the given start and end indices.
         # Start index is inclusive, end index is exclusive.
         # Method added for performance reasons, to only string format
@@ -1949,22 +1938,33 @@
         if self is other:
             return self
         return self.with_partition_keys(other.get_partition_keys())
 
     def __sub__(self, other: "PartitionsSubset") -> "PartitionsSubset":
         if self is other:
             return self.empty_subset(self.partitions_def)
-        return self.empty_subset(self.partitions_def).with_partition_keys(
+
+        empty_subset = self.empty_subset(self.partitions_def)
+
+        if other is empty_subset:
+            return self
+
+        return empty_subset.with_partition_keys(
             set(self.get_partition_keys()).difference(set(other.get_partition_keys()))
         )
 
     def __and__(self, other: "PartitionsSubset") -> "PartitionsSubset":
         if self is other:
             return self
-        return self.empty_subset(self.partitions_def).with_partition_keys(
+
+        empty_subset = self.empty_subset(self.partitions_def)
+        if other is empty_subset:
+            return empty_subset
+
+        return empty_subset.with_partition_keys(
             set(self.get_partition_keys()) & set(other.get_partition_keys())
         )
 
 
 class PartitionKeysTimeWindowPartitionsSubset(BaseTimeWindowPartitionsSubset):
     """A PartitionsSubset for a TimeWindowPartitionsDefinition, which internally represents the
     included partitions using strings.
@@ -2193,15 +2193,15 @@
         return self.included_time_windows[-1].end.timestamp() <= dt.timestamp()
 
     @cached_property
     def num_partitions(self) -> int:
         num_partitions_ = self._asdict()["num_partitions"]
         if num_partitions_ is None:
             return sum(
-                len(self.partitions_def.get_partition_keys_in_time_window(time_window))
+                self.partitions_def.get_num_partitions_in_window(time_window)
                 for time_window in self.included_time_windows
             )
         return num_partitions_
 
     @classmethod
     def _num_partitions_from_time_windows(
         cls, partitions_def: TimeWindowPartitionsDefinition, time_windows: Sequence[TimeWindow]
@@ -2252,14 +2252,76 @@
             num_partitions=self.num_partitions,
             included_time_windows=self.included_time_windows,
         )
 
     def __repr__(self) -> str:
         return f"TimeWindowPartitionsSubset({self.get_partition_key_ranges(self.partitions_def)})"
 
+    def __sub__(self, other: "PartitionsSubset") -> "PartitionsSubset":
+        if self is other:
+            return self.empty_subset(self.partitions_def)
+
+        empty_subset = self.empty_subset(self.partitions_def)
+
+        if other is empty_subset:
+            return self
+
+        if not isinstance(other, TimeWindowPartitionsSubset):
+            return empty_subset.with_partition_keys(
+                set(self.get_partition_keys()).difference(set(other.get_partition_keys()))
+            )
+
+        time_windows = sorted(self.included_time_windows, key=lambda tw: tw.start.timestamp())
+        other_time_windows = sorted(
+            other.included_time_windows, key=lambda tw: tw.start.timestamp()
+        )
+
+        next_time_window_index_to_process = 0
+        next_other_window_index_to_process = 0
+
+        # Slide through both sets of windows, moving to the next window once its start has passed
+        # the end of the window is it being compared to
+        while (next_time_window_index_to_process < len(time_windows)) and (
+            next_other_window_index_to_process < len(other_time_windows)
+        ):
+            time_window = time_windows[next_time_window_index_to_process]
+            other_time_window = other_time_windows[next_other_window_index_to_process]
+
+            # Perform the subtraction and splice the 0, 1, or 2 result windows
+            # back into the time_windows list
+
+            subtracted_time_windows = time_window.subtract(other_time_window)
+
+            time_windows[
+                next_time_window_index_to_process : next_time_window_index_to_process + 1
+            ] = subtracted_time_windows
+
+            if len(subtracted_time_windows) == 0:
+                # other_time_window fully consumed time_window
+                # next_time_window_index_to_process can stay the same since everything has shifted over one
+                pass
+            else:
+                updated_time_window = time_windows[next_time_window_index_to_process]
+                if updated_time_window.end <= other_time_window.start:
+                    # Current subtractor is too early to intersect, can advance
+                    next_time_window_index_to_process += 1
+                elif other_time_window.end <= updated_time_window.start:
+                    # current subtractee is too early to intersect, can advance
+                    next_other_window_index_to_process += 1
+                else:
+                    check.failed(
+                        "After subtraction, the new window should no longer intersect with the other window"
+                    )
+
+        return TimeWindowPartitionsSubset(
+            partitions_def=self.partitions_def,
+            num_partitions=None,
+            included_time_windows=time_windows,
+        )
+
     def to_serializable_subset(self) -> "TimeWindowPartitionsSubset":
         from dagster._core.remote_representation.external_data import (
             external_time_window_partitions_definition_from_def,
         )
 
         # in cases where we're dealing with (e.g.) HourlyPartitionsDefinition, we need to convert
         # this partitions definition into a raw TimeWindowPartitionsDefinition to make it
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.8/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/definitions/utils.py` & `dagster-1.7.8/dagster/_core/definitions/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     ]
     + list(keyword.kwlist)  # just disallow all python keywords
 )
 
 VALID_NAME_REGEX_STR = r"^[A-Za-z0-9_]+$"
 VALID_NAME_REGEX = re.compile(VALID_NAME_REGEX_STR)
 
+INVALID_TITLE_CHARACTERS_REGEX_STR = r"[\%\*\"]"
+INVALID_TITLE_CHARACTERS_REGEX = re.compile(INVALID_TITLE_CHARACTERS_REGEX_STR)
+MAX_TITLE_LENGTH = 100
+
 
 class NoValueSentinel:
     """Sentinel value to distinguish unset from None."""
 
 
 def has_valid_name_chars(name: str) -> bool:
     return bool(VALID_NAME_REGEX.match(name))
@@ -78,14 +82,54 @@
 
 def is_valid_name(name: str) -> bool:
     check.str_param(name, "name")
 
     return name not in DISALLOWED_NAMES and has_valid_name_chars(name)
 
 
+def is_valid_title_and_reason(title: Optional[str]) -> Tuple[bool, Optional[str]]:
+    check.opt_str_param(title, "title")
+
+    if title is None:
+        return True, None
+
+    if len(title) > MAX_TITLE_LENGTH:
+        return (
+            False,
+            f'"{title}" ({len(title)} characters) is not a valid title in Dagster. Titles must not be longer than {MAX_TITLE_LENGTH}.',
+        )
+
+    if not is_valid_title_chars(title):
+        return (
+            False,
+            f'"{title}" is not a valid title in Dagster. Titles must not contain regex {INVALID_TITLE_CHARACTERS_REGEX_STR}.',
+        )
+
+    return True, None
+
+
+def check_valid_title(title: Optional[str]) -> Optional[str]:
+    """A title is distinguished from a name in that the title is a descriptive string meant for display in the UI.
+    It is not used as an identifier for an object.
+    """
+    is_valid, reason = is_valid_title_and_reason(title)
+    if not is_valid:
+        raise DagsterInvariantViolationError(reason)
+
+    return title
+
+
+def is_valid_title(title: Optional[str]) -> bool:
+    return is_valid_title_and_reason(title)[0]
+
+
+def is_valid_title_chars(title: str):
+    return not bool(INVALID_TITLE_CHARACTERS_REGEX.search(title))
+
+
 def _kv_str(key: object, value: object) -> str:
     return f'{key}="{value!r}"'
 
 
 def struct_to_string(name: str, **kwargs: object) -> str:
     # Sort the kwargs to ensure consistent representations across Python versions
     props_str = ", ".join([_kv_str(key, value) for key, value in sorted(kwargs.items())])
```

### Comparing `dagster-1.7.7/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.8/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/errors.py` & `dagster-1.7.8/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/event_api.py` & `dagster-1.7.8/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/events/__init__.py` & `dagster-1.7.8/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/events/log.py` & `dagster-1.7.8/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/events/utils.py` & `dagster-1.7.8/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/api.py` & `dagster-1.7.8/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.8/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/backfill.py` & `dagster-1.7.8/dagster/_core/execution/backfill.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pendulum
 
 from dagster import _check as check
 from dagster._core.definitions import AssetKey
 from dagster._core.definitions.base_asset_graph import BaseAssetGraph
 from dagster._core.definitions.partition import PartitionsSubset
+from dagster._core.definitions.utils import check_valid_title
 from dagster._core.errors import DagsterDefinitionChangedDeserializationError
 from dagster._core.execution.bulk_actions import BulkActionType
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.remote_representation.origin import RemotePartitionSetOrigin
 from dagster._core.storage.tags import USER_TAG
 from dagster._core.workspace.workspace import IWorkspace
 from dagster._serdes import whitelist_for_serdes
@@ -45,14 +46,16 @@
             ("backfill_id", str),
             ("status", BulkActionStatus),
             ("from_failure", bool),
             ("tags", Mapping[str, str]),
             ("backfill_timestamp", float),
             ("error", Optional[SerializableErrorInfo]),
             ("asset_selection", Optional[Sequence[AssetKey]]),
+            ("title", Optional[str]),
+            ("description", Optional[str]),
             # fields that are only used by job backfills
             ("partition_set_origin", Optional[RemotePartitionSetOrigin]),
             ("partition_names", Optional[Sequence[str]]),
             ("last_submitted_partition_name", Optional[str]),
             ("reexecution_steps", Optional[Sequence[str]]),
             # only used by asset backfills
             ("serialized_asset_backfill_data", Optional[str]),
@@ -65,14 +68,16 @@
         backfill_id: str,
         status: BulkActionStatus,
         from_failure: bool,
         tags: Optional[Mapping[str, str]],
         backfill_timestamp: float,
         error: Optional[SerializableErrorInfo] = None,
         asset_selection: Optional[Sequence[AssetKey]] = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
         partition_set_origin: Optional[RemotePartitionSetOrigin] = None,
         partition_names: Optional[Sequence[str]] = None,
         last_submitted_partition_name: Optional[str] = None,
         reexecution_steps: Optional[Sequence[str]] = None,
         serialized_asset_backfill_data: Optional[str] = None,
         asset_backfill_data: Optional[AssetBackfillData] = None,
     ):
@@ -85,29 +90,43 @@
             check.invariant(partition_set_origin is None)
             check.invariant(partition_names is None)
             check.invariant(last_submitted_partition_name is None)
             check.invariant(reexecution_steps is None)
 
         return super(PartitionBackfill, cls).__new__(
             cls,
-            check.str_param(backfill_id, "backfill_id"),
-            check.inst_param(status, "status", BulkActionStatus),
-            check.bool_param(from_failure, "from_failure"),
-            check.opt_mapping_param(tags, "tags", key_type=str, value_type=str),
-            check.float_param(backfill_timestamp, "backfill_timestamp"),
-            check.opt_inst_param(error, "error", SerializableErrorInfo),
-            check.opt_nullable_sequence_param(asset_selection, "asset_selection", of_type=AssetKey),
-            check.opt_inst_param(
+            backfill_id=check.str_param(backfill_id, "backfill_id"),
+            status=check.inst_param(status, "status", BulkActionStatus),
+            from_failure=check.bool_param(from_failure, "from_failure"),
+            tags=check.opt_mapping_param(tags, "tags", key_type=str, value_type=str),
+            backfill_timestamp=check.float_param(backfill_timestamp, "backfill_timestamp"),
+            error=check.opt_inst_param(error, "error", SerializableErrorInfo),
+            asset_selection=check.opt_nullable_sequence_param(
+                asset_selection, "asset_selection", of_type=AssetKey
+            ),
+            title=check_valid_title(title),
+            description=check.opt_str_param(description, "description"),
+            partition_set_origin=check.opt_inst_param(
                 partition_set_origin, "partition_set_origin", RemotePartitionSetOrigin
             ),
-            check.opt_nullable_sequence_param(partition_names, "partition_names", of_type=str),
-            check.opt_str_param(last_submitted_partition_name, "last_submitted_partition_name"),
-            check.opt_nullable_sequence_param(reexecution_steps, "reexecution_steps", of_type=str),
-            check.opt_str_param(serialized_asset_backfill_data, "serialized_asset_backfill_data"),
-            check.opt_inst_param(asset_backfill_data, "asset_backfill_data", AssetBackfillData),
+            partition_names=check.opt_nullable_sequence_param(
+                partition_names, "partition_names", of_type=str
+            ),
+            last_submitted_partition_name=check.opt_str_param(
+                last_submitted_partition_name, "last_submitted_partition_name"
+            ),
+            reexecution_steps=check.opt_nullable_sequence_param(
+                reexecution_steps, "reexecution_steps", of_type=str
+            ),
+            serialized_asset_backfill_data=check.opt_str_param(
+                serialized_asset_backfill_data, "serialized_asset_backfill_data"
+            ),
+            asset_backfill_data=check.opt_inst_param(
+                asset_backfill_data, "asset_backfill_data", AssetBackfillData
+            ),
         )
 
     @property
     def selector_id(self):
         return self.partition_set_origin.get_selector_id() if self.partition_set_origin else None
 
     @property
@@ -286,14 +305,16 @@
             tags=self.tags,
             backfill_timestamp=self.backfill_timestamp,
             last_submitted_partition_name=self.last_submitted_partition_name,
             error=self.error,
             asset_selection=self.asset_selection,
             serialized_asset_backfill_data=self.serialized_asset_backfill_data,
             asset_backfill_data=self.asset_backfill_data,
+            title=self.title,
+            description=self.description,
         )
 
     def with_partition_checkpoint(self, last_submitted_partition_name):
         check.str_param(last_submitted_partition_name, "last_submitted_partition_name")
         return PartitionBackfill(
             status=self.status,
             backfill_id=self.backfill_id,
@@ -304,14 +325,16 @@
             tags=self.tags,
             backfill_timestamp=self.backfill_timestamp,
             last_submitted_partition_name=last_submitted_partition_name,
             error=self.error,
             asset_selection=self.asset_selection,
             serialized_asset_backfill_data=self.serialized_asset_backfill_data,
             asset_backfill_data=self.asset_backfill_data,
+            title=self.title,
+            description=self.description,
         )
 
     def with_error(self, error):
         check.opt_inst_param(error, "error", SerializableErrorInfo)
         return PartitionBackfill(
             status=self.status,
             backfill_id=self.backfill_id,
@@ -322,14 +345,16 @@
             tags=self.tags,
             backfill_timestamp=self.backfill_timestamp,
             last_submitted_partition_name=self.last_submitted_partition_name,
             error=error,
             asset_selection=self.asset_selection,
             serialized_asset_backfill_data=self.serialized_asset_backfill_data,
             asset_backfill_data=self.asset_backfill_data,
+            title=self.title,
+            description=self.description,
         )
 
     def with_asset_backfill_data(
         self,
         asset_backfill_data: AssetBackfillData,
         dynamic_partitions_store: DynamicPartitionsStore,
         asset_graph: BaseAssetGraph,
@@ -349,27 +374,31 @@
             asset_selection=self.asset_selection,
             serialized_asset_backfill_data=asset_backfill_data.serialize(
                 dynamic_partitions_store=dynamic_partitions_store, asset_graph=asset_graph
             )
             if is_backcompat
             else None,
             asset_backfill_data=asset_backfill_data if not is_backcompat else None,
+            title=self.title,
+            description=self.description,
         )
 
     @classmethod
     def from_asset_partitions(
         cls,
         backfill_id: str,
         asset_graph: BaseAssetGraph,
         partition_names: Optional[Sequence[str]],
         asset_selection: Sequence[AssetKey],
         backfill_timestamp: float,
         tags: Mapping[str, str],
         dynamic_partitions_store: DynamicPartitionsStore,
         all_partitions: bool,
+        title: Optional[str],
+        description: Optional[str],
     ) -> "PartitionBackfill":
         """If all the selected assets that have PartitionsDefinitions have the same partitioning, then
         the backfill will target the provided partition_names for all those assets.
 
         Otherwise, the backfill must consist of a partitioned "anchor" asset and a set of other
         assets that descend from it. In that case, the backfill will target the partition_names of
         the anchor asset, as well as all partitions of other selected assets that are downstream
@@ -388,25 +417,29 @@
             status=BulkActionStatus.REQUESTED,
             from_failure=False,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
             serialized_asset_backfill_data=None,
             asset_backfill_data=asset_backfill_data,
+            title=title,
+            description=description,
         )
 
     @classmethod
     def from_partitions_by_assets(
         cls,
         backfill_id: str,
         asset_graph: BaseAssetGraph,
         backfill_timestamp: float,
         tags: Mapping[str, str],
         dynamic_partitions_store: DynamicPartitionsStore,
         partitions_by_assets: Sequence[PartitionsByAssetSelector],
+        title: Optional[str],
+        description: Optional[str],
     ):
         asset_backfill_data = AssetBackfillData.from_partitions_by_assets(
             asset_graph=asset_graph,
             dynamic_partitions_store=dynamic_partitions_store,
             backfill_start_time=pendulum.from_timestamp(backfill_timestamp, tz="UTC"),
             partitions_by_assets=partitions_by_assets,
         )
@@ -415,8 +448,10 @@
             status=BulkActionStatus.REQUESTED,
             from_failure=False,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             serialized_asset_backfill_data=None,
             asset_backfill_data=asset_backfill_data,
             asset_selection=[selector.asset_key for selector in partitions_by_assets],
+            title=title,
+            description=description,
         )
```

### Comparing `dagster-1.7.7/dagster/_core/execution/build_resources.py` & `dagster-1.7.8/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/compute_logs.py` & `dagster-1.7.8/dagster/_core/execution/compute_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import tempfile
 import time
 import uuid
 import warnings
 from contextlib import contextmanager
 
-from dagster._core.execution import poll_compute_logs, watch_orphans
+from dagster._core.execution.scripts import poll_compute_logs, watch_orphans
 from dagster._serdes.ipc import interrupt_ipc_subprocess, open_ipc_subprocess
 from dagster._seven import IS_WINDOWS, wait_for_process
 from dagster._utils import ensure_file
 
 WIN_PY36_COMPUTE_LOG_DISABLED_MSG = """\u001b[33mWARNING: Compute log capture is disabled for the current environment. Set the environment variable `PYTHONLEGACYWINDOWSSTDIO` to enable.\n\u001b[0m"""
```

### Comparing `dagster-1.7.7/dagster/_core/execution/context/compute.py` & `dagster-1.7.8/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/data_version_cache.py` & `dagster-1.7.8/dagster/_core/execution/context/data_version_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/hook.py` & `dagster-1.7.8/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/init.py` & `dagster-1.7.8/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/input.py` & `dagster-1.7.8/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/invocation.py` & `dagster-1.7.8/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/logger.py` & `dagster-1.7.8/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/output.py` & `dagster-1.7.8/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context/system.py` & `dagster-1.7.8/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.8/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.8/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.8/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/execution_result.py` & `dagster-1.7.8/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/host_mode.py` & `dagster-1.7.8/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/job_backfill.py` & `dagster-1.7.8/dagster/_core/execution/job_backfill.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,17 @@
     )
     completed_partitions = set([run.tags.get(PARTITION_NAME_TAG) for run in backfill_runs])
     initial_checkpoint = (
         partition_names.index(checkpoint) + 1 if checkpoint and checkpoint in partition_names else 0
     )
     partition_names = partition_names[initial_checkpoint:]
 
-    partitions_def = partition_set.get_partitions_definition()
     backfill_policy = partition_set.backfill_policy
     if backfill_policy and backfill_policy.max_partitions_per_run != 1:
+        partitions_def = partition_set.get_partitions_definition()
         partitions_subset = partitions_def.subset_with_partition_keys(partition_names)
         partition_key_ranges = partitions_subset.get_partition_key_ranges(
             partitions_def, dynamic_partitions_store=instance
         )
         subdivided_ranges = [
             sr
             for r in partition_key_ranges
```

### Comparing `dagster-1.7.7/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.8/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/memoization.py` & `dagster-1.7.8/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/active.py` & `dagster-1.7.8/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/compute.py` & `dagster-1.7.8/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.8/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.8/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.8/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.8/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/handle.py` & `dagster-1.7.8/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.8/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.8/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.8/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/objects.py` & `dagster-1.7.8/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.8/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/plan.py` & `dagster-1.7.8/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/state.py` & `dagster-1.7.8/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/step.py` & `dagster-1.7.8/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/plan/utils.py` & `dagster-1.7.8/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.8/dagster/_core/execution/scripts/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.8/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/resources_init.py` & `dagster-1.7.8/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/retries.py` & `dagster-1.7.8/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.8/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/run_metrics_thread.py` & `dagster-1.7.8/dagster/_core/execution/run_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/stats.py` & `dagster-1.7.8/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.8/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/tags.py` & `dagster-1.7.8/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.8/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.8/dagster/_core/execution/scripts/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/execution/with_resources.py` & `dagster-1.7.8/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/base.py` & `dagster-1.7.8/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.8/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/in_process.py` & `dagster-1.7.8/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/init.py` & `dagster-1.7.8/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/multiprocess.py` & `dagster-1.7.8/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.8/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.8/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/instance/__init__.py` & `dagster-1.7.8/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/instance/config.py` & `dagster-1.7.8/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/instance/ref.py` & `dagster-1.7.8/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/instance_for_test.py` & `dagster-1.7.8/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/launcher/base.py` & `dagster-1.7.8/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.8/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.8/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/log_manager.py` & `dagster-1.7.8/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/nux.py` & `dagster-1.7.8/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.8/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/origin.py` & `dagster-1.7.8/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/pipes/client.py` & `dagster-1.7.8/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/pipes/context.py` & `dagster-1.7.8/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/pipes/subprocess.py` & `dagster-1.7.8/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/pipes/utils.py` & `dagster-1.7.8/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.8/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.8/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/external.py` & `dagster-1.7.8/dagster/_core/remote_representation/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -1029,16 +1029,23 @@
     def has_partition_name_data(self) -> bool:
         # Partition sets from older versions of Dagster as well as partition sets using
         # a DynamicPartitionsDefinition require calling out to user code to compute the partition
         # names
         return self._external_partition_set_data.external_partitions_data is not None
 
     def get_partitions_definition(self) -> PartitionsDefinition:
-        return (
-            self._external_partition_set_data.external_partitions_data.get_partitions_definition()  # type: ignore
-        )
+        partitions_data = self._external_partition_set_data.external_partitions_data
+        if partitions_data is None:
+            check.failed(
+                "Partition set does not have partition data, cannot get partitions definition"
+            )
+        return partitions_data.get_partitions_definition()
 
     def get_partition_names(self, instance: DagsterInstance) -> Sequence[str]:
-        check.invariant(self.has_partition_name_data())
+        partitions_data = self._external_partition_set_data.external_partitions_data
+        if partitions_data is None:
+            check.failed(
+                "Partition set does not have partition data, cannot get partitions definition"
+            )
         return self.get_partitions_definition().get_partition_keys(
             dynamic_partitions_store=instance
         )
```

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.8/dagster/_core/remote_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.8/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.8/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.8/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/handle.py` & `dagster-1.7.8/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/historical.py` & `dagster-1.7.8/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.8/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/origin.py` & `dagster-1.7.8/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/remote_representation/represented.py` & `dagster-1.7.8/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/run_coordinator/base.py` & `dagster-1.7.8/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.8/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.8/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/scheduler/__init__.py` & `dagster-1.7.8/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/scheduler/execution.py` & `dagster-1.7.8/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/scheduler/instigation.py` & `dagster-1.7.8/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.8/dagster/_core/scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,17 @@
         """
 
 
 DEFAULT_MAX_CATCHUP_RUNS = 5
 
 
 class DagsterDaemonScheduler(Scheduler, ConfigurableClass):
-    """Default scheduler implementation that submits runs from the `dagster-daemon`
-    long-lived process. Periodically checks each running schedule for execution times that don't
-    have runs yet and launches them.
+    """Default scheduler implementation that submits runs from the long-lived ``dagster-daemon``
+    process. Periodically checks each running schedule for execution times that don't yet
+    have runs and launches them.
     """
 
     def __init__(
         self,
         max_catchup_runs: int = DEFAULT_MAX_CATCHUP_RUNS,
         max_tick_retries: int = 0,
         inst_data: Optional[ConfigurableClassData] = None,
@@ -239,28 +239,27 @@
                 IntSource,
                 is_required=False,
                 default_value=DEFAULT_MAX_CATCHUP_RUNS,
                 description="""For partitioned schedules, controls the maximum number of past
             partitions for each schedule that will be considered when looking for missing
             runs . Generally this parameter will only come into play if the scheduler
             falls behind or launches after experiencing downtime. This parameter will not be checked for
-            schedules without partition sets (for example, schedules created using the @schedule
-            decorator) - only the most recent execution time will be considered for those schedules.
+            schedules without partition sets (for example, schedules created using the :py:func:`@schedule <dagster.schedule>` decorator) - only the most recent execution time will be considered for those schedules.
 
-            Note that no matter what this value is, the scheduler will never launch a run from a time
-            before the schedule was turned on (even if the start_date on the schedule is earlier) - if
-            you want to launch runs for earlier partitions, launch a backfill.
+            Note: No matter what this value is, the scheduler will never launch a run from a time
+            before the schedule was turned on, even if the schedule's ``start_date`` is earlier. If
+            you want to launch runs for earlier partitions, `launch a backfill </concepts/partitions-schedules-sensors/backfills>`_.
             """,
             ),
             "max_tick_retries": Field(
                 IntSource,
                 default_value=0,
                 is_required=False,
                 description=(
-                    "For each schedule tick that raises an error, how many times to retry that tick"
+                    "For each schedule tick that raises an error, the number of times to retry the tick."
                 ),
             ),
         }
 
     @classmethod
     def from_config_value(
         cls, inst_data: ConfigurableClassData, config_value: Mapping[str, Any]
```

### Comparing `dagster-1.7.7/dagster/_core/secrets/env_file.py` & `dagster-1.7.8/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/selector/subset_selector.py` & `dagster-1.7.8/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/__init__.py` & `dagster-1.7.8/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/dagster_types.py` & `dagster-1.7.8/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.8/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.8/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.8/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/mode.py` & `dagster-1.7.8/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/node.py` & `dagster-1.7.8/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.8/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.8/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/README.md` & `dagster-1.7.8/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/env.py` & `dagster-1.7.8/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.8/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.8/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.8/dagster/_core/storage/asset_value_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             resource_defs = merge_dicts(
                 {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
                 assets_def.resource_defs,
             )
             io_manager_key = assets_def.get_io_manager_key_for_asset_key(asset_key)
             io_manager_def = resource_defs[io_manager_key]
             name = assets_def.get_output_name_for_asset_key(asset_key)
-            output_definition_metadata = assets_def.metadata_by_key[asset_key]
+            output_definition_metadata = assets_def.specs_by_key[asset_key].metadata
             op_def = assets_def.get_op_def_for_asset_key(asset_key)
             asset_partitions_def = assets_def.partitions_def
         else:
             check.failed(f"Asset key {asset_key} not found")
 
         required_resource_keys = get_transitive_required_resource_keys(
             io_manager_def.required_resource_keys, resource_defs
```

### Comparing `dagster-1.7.7/dagster/_core/storage/base_storage.py` & `dagster-1.7.8/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/batch_asset_record_loader.py` & `dagster-1.7.8/dagster/_core/storage/batch_asset_record_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.8/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.8/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.8/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/config.py` & `dagster-1.7.8/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/dagster_run.py` & `dagster-1.7.8/dagster/_core/storage/dagster_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from datetime import datetime
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
+    Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Union,
 )
 
 from typing_extensions import Self
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, public
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.events import AssetKey
+from dagster._core.loader import InstanceLoadableBy
 from dagster._core.origin import JobPythonOrigin
 from dagster._core.storage.tags import PARENT_RUN_ID_TAG, ROOT_RUN_ID_TAG
 from dagster._core.utils import make_new_run_id
 from dagster._serdes.serdes import (
     NamedTupleSerializer,
     whitelist_for_serdes,
 )
@@ -33,14 +35,15 @@
     RESUME_RETRY_TAG,
     SCHEDULE_NAME_TAG,
     SENSOR_NAME_TAG,
     TICK_ID_TAG,
 )
 
 if TYPE_CHECKING:
+    from dagster._core.instance import DagsterInstance
     from dagster._core.remote_representation.external import ExternalSchedule, ExternalSensor
     from dagster._core.remote_representation.origin import RemoteJobOrigin
 
 
 @whitelist_for_serdes(storage_name="PipelineRunStatus")
 class DagsterRunStatus(Enum):
     """The status of run execution."""
@@ -576,15 +579,16 @@
             ("storage_id", int),
             ("dagster_run", DagsterRun),
             ("create_timestamp", datetime),
             ("update_timestamp", datetime),
             ("start_time", Optional[float]),
             ("end_time", Optional[float]),
         ],
-    )
+    ),
+    InstanceLoadableBy[str],
 ):
     """Internal representation of a run record, as stored in a
     :py:class:`~dagster._core.storage.runs.RunStorage`.
 
     Users should not invoke this class directly.
     """
 
@@ -604,14 +608,30 @@
             create_timestamp=check.inst_param(create_timestamp, "create_timestamp", datetime),
             update_timestamp=check.inst_param(update_timestamp, "update_timestamp", datetime),
             # start_time and end_time fields will be populated once the run has started and ended, respectively, but will be None beforehand.
             start_time=check.opt_float_param(start_time, "start_time"),
             end_time=check.opt_float_param(end_time, "end_time"),
         )
 
+    @classmethod
+    async def _batch_load(
+        cls,
+        keys: Iterable[str],
+        instance: "DagsterInstance",
+    ) -> Iterable[Optional["RunRecord"]]:
+        result_map: Dict[str, Optional[RunRecord]] = {run_id: None for run_id in keys}
+
+        # this should be replaced with an async DB call
+        records = instance.get_run_records(RunsFilter(run_ids=list(result_map.keys())))
+
+        for record in records:
+            result_map[record.dagster_run.run_id] = record
+
+        return result_map.values()
+
 
 @whitelist_for_serdes
 class RunPartitionData(
     NamedTuple(
         "_RunPartitionData",
         [
             ("run_id", str),
```

### Comparing `dagster-1.7.7/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.8/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/base.py` & `dagster-1.7.8/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.8/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.8/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.8/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.8/dagster/_core/storage/event_log/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     mysql_length={
         "asset_key": 64,
         "partition": 64,
         "check_name": 64,
     },
 )
 
+# This index doesn't enforce the uniqueness how we want it to because partition and run_id can be
+# null. Postgres and other dbms's consider each null value distinct.
 db.Index(
     "idx_asset_check_executions_unique",
     AssetCheckExecutionsTable.c.asset_key,
     AssetCheckExecutionsTable.c.check_name,
     AssetCheckExecutionsTable.c.run_id,
     AssetCheckExecutionsTable.c.partition,
     unique=True,
```

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.8/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from abc import abstractmethod
 from collections import OrderedDict, defaultdict
 from contextlib import contextmanager
 from datetime import datetime, timezone
+from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     Any,
     ContextManager,
     Dict,
     Iterable,
     Iterator,
@@ -2114,25 +2115,31 @@
                     db.and_(
                         DynamicPartitionsTable.c.partitions_def_name == partitions_def_name,
                         DynamicPartitionsTable.c.partition == partition_key,
                     )
                 )
             )
 
-    @property
+    @cached_property
     def supports_global_concurrency_limits(self) -> bool:
         return self.has_table(ConcurrencySlotsTable.name)
 
+    @cached_property
+    def has_concurrency_limits_table(self) -> bool:
+        # This table was added later, and to avoid forcing a migration
+        # we handle in the code if its been added or not.
+        return self.has_table(ConcurrencyLimitsTable.name)
+
     def _reconcile_concurrency_limits_from_slots(self) -> None:
         """Helper function that can be reconciles the concurrency limits table from the concurrency
         slots table.  This should only run when the concurrency limits table exists and is empty,
         since all of the slot configuration operations should keep them in sync.  We reconcile from
         the slots table because the initial implementation did not have the limits table.
         """
-        if not self.has_table(ConcurrencyLimitsTable.name):
+        if not self.has_concurrency_limits_table:
             return
 
         if not self._has_rows(ConcurrencySlotsTable) or self._has_rows(ConcurrencyLimitsTable):
             return
 
         with self.index_transaction() as conn:
             rows = conn.execute(
@@ -2163,15 +2170,15 @@
 
     def _has_rows(self, table) -> bool:
         with self.index_connection() as conn:
             row = conn.execute(db_select([True]).select_from(table).limit(1)).fetchone()
         return bool(row[0]) if row else False
 
     def initialize_concurrency_limit_to_default(self, concurrency_key: str) -> bool:
-        if not self.has_table(ConcurrencyLimitsTable.name):
+        if not self.has_concurrency_limits_table:
             return False
 
         self._reconcile_concurrency_limits_from_slots()
 
         if not self.has_instance:
             return False
 
@@ -2192,15 +2199,15 @@
                 pass
         return True
 
     def _upsert_and_lock_limit_row(self, conn, concurrency_key: str, num: int):
         """Helper function that can be overridden by each implementing sql variant which obtains a
         lock on the concurrency limits row for the given key and updates it to the given value.
         """
-        if not self.has_table(ConcurrencyLimitsTable.name):
+        if not self.has_concurrency_limits_table:
             # no need to grab the lock on the concurrency limits row if the table does not exist
             return None
 
         row = conn.execute(
             db_select([ConcurrencyLimitsTable.c.id])
             .select_from(ConcurrencyLimitsTable)
             .where(ConcurrencyLimitsTable.c.concurrency_key == concurrency_key)
@@ -2252,15 +2259,15 @@
         Args:
             concurrency_key (str): The key to delete.
         """
         # ensure that we have concurrency limits set for all keys
         self._reconcile_concurrency_limits_from_slots()
 
         with self.index_transaction() as conn:
-            if self.has_table(ConcurrencyLimitsTable.name):
+            if self.has_concurrency_limits_table:
                 conn.execute(
                     ConcurrencyLimitsTable.delete().where(
                         ConcurrencyLimitsTable.c.concurrency_key == concurrency_key
                     )
                 )
             self._allocate_concurrency_slots(conn, concurrency_key, 0)
 
@@ -2611,15 +2618,15 @@
             return ConcurrencySlotStatus.CLAIMED
 
     def get_concurrency_keys(self) -> Set[str]:
         self._reconcile_concurrency_limits_from_slots()
 
         """Get the set of concurrency limited keys."""
         with self.index_connection() as conn:
-            if self.has_table(ConcurrencyLimitsTable.name):
+            if self.has_concurrency_limits_table:
                 query = db_select([ConcurrencyLimitsTable.c.concurrency_key]).select_from(
                     ConcurrencyLimitsTable
                 )
             else:
                 query = (
                     db_select([ConcurrencySlotsTable.c.concurrency_key])
                     .select_from(ConcurrencySlotsTable)
```

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.8/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.8/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.8/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/file_manager.py` & `dagster-1.7.8/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/input_manager.py` & `dagster-1.7.8/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/io_manager.py` & `dagster-1.7.8/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.8/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.8/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.8/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/migration/utils.py` & `dagster-1.7.8/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.8/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/output_manager.py` & `dagster-1.7.8/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.8/dagster/_core/storage/partition_status_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -266,23 +266,20 @@
     )
     if not latest_storage_id:
         return None
 
     if not partitions_def or not is_cacheable_partition_type(partitions_def):
         return AssetStatusCacheValue(latest_storage_id=latest_storage_id)
 
-    failed_partitions: Set[str] = (
-        set(
-            partitions_def.deserialize_subset(
-                stored_cache_value.serialized_failed_partition_subset
-            ).get_partition_keys()
-        )
+    failed_subset = (
+        partitions_def.deserialize_subset(stored_cache_value.serialized_failed_partition_subset)
         if stored_cache_value and stored_cache_value.serialized_failed_partition_subset
-        else set()
+        else None
     )
+
     cached_in_progress_cursor = (
         (
             stored_cache_value.earliest_in_progress_materialization_event_id - 1
             if stored_cache_value.earliest_in_progress_materialization_event_id
             else stored_cache_value.latest_storage_id
         )
         if stored_cache_value
@@ -293,29 +290,37 @@
         # fetch the incremental new materialized partitions, and update the cached materialized
         # subset
         new_partitions = set()
         if (
             last_materialization_storage_id
             and last_materialization_storage_id > stored_cache_value.latest_storage_id
         ):
-            new_partitions = instance.get_materialized_partitions(
-                asset_key, after_cursor=stored_cache_value.latest_storage_id
+            new_partitions = get_validated_partition_keys(
+                dynamic_partitions_store,
+                partitions_def,
+                instance.get_materialized_partitions(
+                    asset_key, after_cursor=stored_cache_value.latest_storage_id
+                ),
             )
 
         materialized_subset: PartitionsSubset = (
             partitions_def.deserialize_subset(
                 stored_cache_value.serialized_materialized_partition_subset
             )
             if stored_cache_value.serialized_materialized_partition_subset
             else partitions_def.empty_subset()
-        ).with_partition_keys(
-            get_validated_partition_keys(dynamic_partitions_store, partitions_def, new_partitions)
         )
 
-        failed_partitions.difference_update(new_partitions)
+        if new_partitions:
+            materialized_subset = materialized_subset.with_partition_keys(new_partitions)
+
+        if failed_subset and new_partitions:
+            failed_subset = failed_subset - partitions_def.empty_subset().with_partition_keys(
+                new_partitions
+            )
 
     else:
         materialized_subset = partitions_def.empty_subset().with_partition_keys(
             get_validated_partition_keys(
                 dynamic_partitions_store,
                 partitions_def,
                 instance.get_materialized_partitions(asset_key),
@@ -328,15 +333,15 @@
         earliest_in_progress_materialization_event_id,
     ) = build_failed_and_in_progress_partition_subset(
         instance,
         asset_key,
         partitions_def,
         dynamic_partitions_store,
         last_planned_materialization_storage_id=last_planned_materialization_storage_id,
-        failed_partitions=failed_partitions,
+        failed_subset=failed_subset,
         after_storage_id=cached_in_progress_cursor,
     )
 
     return AssetStatusCacheValue(
         latest_storage_id=latest_storage_id,
         partitions_def_id=partitions_def.get_serializable_unique_identifier(
             dynamic_partitions_store=dynamic_partitions_store
@@ -350,31 +355,34 @@
 
 def build_failed_and_in_progress_partition_subset(
     instance: DagsterInstance,
     asset_key: AssetKey,
     partitions_def: PartitionsDefinition,
     dynamic_partitions_store: DynamicPartitionsStore,
     last_planned_materialization_storage_id: int,
-    failed_partitions: Optional[Set[str]] = None,
+    failed_subset: Optional[PartitionsSubset[str]] = None,
     after_storage_id: Optional[int] = None,
 ) -> Tuple[PartitionsSubset, PartitionsSubset, Optional[int]]:
-    failed_partitions = failed_partitions or set()
     in_progress_partitions: Set[str] = set()
 
     incomplete_materializations = {}
 
+    failed_subset = failed_subset or partitions_def.empty_subset()
+
     # Fetch incomplete materializations if there have been any planned materializations since the
     # cursor
     if last_planned_materialization_storage_id and (
         not after_storage_id or last_planned_materialization_storage_id > after_storage_id
     ):
         incomplete_materializations = instance.event_log_storage.get_latest_asset_partition_materialization_attempts_without_materializations(
             asset_key, after_storage_id=after_storage_id
         )
 
+    failed_partitions: Set[str] = set()
+
     cursor = None
     if incomplete_materializations:
         to_fetch = list(set([run_id for run_id, _event_id in incomplete_materializations.values()]))
         finished_runs = {}
         unfinished_runs = {}
 
         while to_fetch:
@@ -397,24 +405,23 @@
                 if cursor is None or event_id < cursor:
                     cursor = event_id
             else:
                 # Runs that are neither finished nor unfinished must have been deleted, so are
                 # considered neither in-progress nor failed
                 pass
 
-    return (
-        (
-            partitions_def.empty_subset().with_partition_keys(
-                get_validated_partition_keys(
-                    dynamic_partitions_store, partitions_def, failed_partitions
-                )
+    if failed_partitions:
+        failed_subset = failed_subset.with_partition_keys(
+            get_validated_partition_keys(
+                dynamic_partitions_store, partitions_def, failed_partitions
             )
-            if failed_partitions
-            else partitions_def.empty_subset()
-        ),
+        )
+
+    return (
+        failed_subset,
         (
             partitions_def.empty_subset().with_partition_keys(
                 get_validated_partition_keys(instance, partitions_def, in_progress_partitions)
             )
             if in_progress_partitions
             else partitions_def.empty_subset()
         ),
```

### Comparing `dagster-1.7.7/dagster/_core/storage/root.py` & `dagster-1.7.8/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/base.py` & `dagster-1.7.8/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.8/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/migration.py` & `dagster-1.7.8/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/schema.py` & `dagster-1.7.8/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.8/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.8/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.8/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/base.py` & `dagster-1.7.8/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.8/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.8/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.8/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.8/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.8/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/sql.py` & `dagster-1.7.8/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.8/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/sqlite.py` & `dagster-1.7.8/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.8/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/tags.py` & `dagster-1.7.8/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.8/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.8/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.8/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/system_config/objects.py` & `dagster-1.7.8/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/telemetry.py` & `dagster-1.7.8/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/telemetry_upload.py` & `dagster-1.7.8/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/test_utils.py` & `dagster-1.7.8/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.8/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/config_schema.py` & `dagster-1.7.8/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/dagster_type.py` & `dagster-1.7.8/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/decorator.py` & `dagster-1.7.8/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.8/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.8/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/python_dict.py` & `dagster-1.7.8/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/python_set.py` & `dagster-1.7.8/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/python_tuple.py` & `dagster-1.7.8/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/types/transform_typing.py` & `dagster-1.7.8/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/utility_ops.py` & `dagster-1.7.8/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/utils.py` & `dagster-1.7.8/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.8/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/config_schema.py` & `dagster-1.7.8/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/context.py` & `dagster-1.7.8/dagster/_core/workspace/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import threading
 import time
 import warnings
 from abc import ABC, abstractmethod
 from contextlib import ExitStack
 from itertools import count
-from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Sequence, Set, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Sequence, Set, Type, TypeVar, Union
 
 from typing_extensions import Self
 
 import dagster._check as check
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.errors import (
     DagsterCodeLocationLoadError,
@@ -36,16 +36,18 @@
     LocationStateSubscriber,
 )
 from dagster._core.remote_representation.origin import (
     GrpcServerCodeLocationOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
 from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
+from dagster._utils.aiodataloader import DataLoader
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
+from ..loader import LoadingContext
 from .load_target import WorkspaceLoadTarget
 from .permissions import (
     PermissionResult,
     get_location_scoped_user_permissions,
     get_user_permissions,
 )
 from .workspace import (
@@ -66,15 +68,15 @@
     )
 
 T = TypeVar("T")
 
 WEBSERVER_GRPC_SERVER_HEARTBEAT_TTL = 45
 
 
-class BaseWorkspaceRequestContext(IWorkspace):
+class BaseWorkspaceRequestContext(IWorkspace, LoadingContext):
     """This class is a request-scoped object that stores (1) a reference to all repository locations
     that exist on the `IWorkspaceProcessContext` at the start of the request and (2) a snapshot of the
     workspace at the start of the request.
 
     This object is needed because a process context and the repository locations on that context can
     be updated (for example, from a thread on the process context). If a request is accessing a
     repository location at the same time the repository location was being cleaned up, we would run
@@ -185,15 +187,21 @@
         return self.get_code_location_error(name) is not None
 
     def get_code_location_error(self, name: str) -> Optional[SerializableErrorInfo]:
         entry = self.get_location_entry(name)
         return entry.load_error if entry else None
 
     def has_code_location_name(self, name: str) -> bool:
-        return bool(self.get_location_entry(name))
+        # For some WorkspaceRequestContext subclasses, the CodeLocationEntry is more expensive
+        # than the CodeLocationStatusEntry, so use the latter for a faster check.
+        for status_entry in self.get_code_location_statuses():
+            if status_entry.location_name == name:
+                return True
+
+        return False
 
     def has_code_location(self, name: str) -> bool:
         location_entry = self.get_location_entry(name)
         return bool(location_entry and location_entry.code_location is not None)
 
     def is_reload_supported(self, name: str) -> bool:
         entry = self.get_location_entry(name)
@@ -335,16 +343,16 @@
         self._version = version
         self._source = source
         self._read_only = read_only
         self._read_only_locations = check.opt_mapping_param(
             read_only_locations, "read_only_locations"
         )
         self._checked_permissions: Set[str] = set()
-
         self._asset_record_loader = BatchAssetRecordLoader(self._instance, {})
+        self._loaders = {}
 
     @property
     def asset_record_loader(self) -> BatchAssetRecordLoader:
         return self._asset_record_loader
 
     @property
     def instance(self) -> DagsterInstance:
@@ -401,14 +409,18 @@
     @property
     def source(self) -> Optional[object]:
         """The source of the request this WorkspaceRequestContext originated from.
         For example in the webserver this object represents the web request.
         """
         return self._source
 
+    @property
+    def loaders(self) -> Dict[Type, DataLoader]:
+        return self._loaders
+
 
 class IWorkspaceProcessContext(ABC):
     """Class that stores process-scoped information about a webserver session.
     In most cases, you will want to create a `BaseWorkspaceRequestContext` to create a request-scoped
     object.
     """
```

### Comparing `dagster-1.7.7/dagster/_core/workspace/load.py` & `dagster-1.7.8/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/load_target.py` & `dagster-1.7.8/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/permissions.py` & `dagster-1.7.8/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_core/workspace/workspace.py` & `dagster-1.7.8/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/__init__.py` & `dagster-1.7.8/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/asset_daemon.py` & `dagster-1.7.8/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.8/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.8/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/backfill.py` & `dagster-1.7.8/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/cli/__init__.py` & `dagster-1.7.8/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/controller.py` & `dagster-1.7.8/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/daemon.py` & `dagster-1.7.8/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.8/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.8/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.8/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/sensor.py` & `dagster-1.7.8/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/types.py` & `dagster-1.7.8/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/utils.py` & `dagster-1.7.8/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_daemon/workspace.py` & `dagster-1.7.8/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_generate/download.py` & `dagster-1.7.8/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_generate/generate.py` & `dagster-1.7.8/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.8/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.8/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.8/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/__init__.py` & `dagster-1.7.8/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/client.py` & `dagster-1.7.8/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/compile.py` & `dagster-1.7.8/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/impl.py` & `dagster-1.7.8/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/protos/api.proto` & `dagster-1.7.8/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/proxy_server.py` & `dagster-1.7.8/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/server.py` & `dagster-1.7.8/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/server_watcher.py` & `dagster-1.7.8/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/types.py` & `dagster-1.7.8/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_grpc/utils.py` & `dagster-1.7.8/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_loggers/__init__.py` & `dagster-1.7.8/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_model/__init__.py` & `dagster-1.7.8/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.8/dagster/_model/pydantic_compat_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    List,
-    Optional,
-    Type,
-)
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Type
 
 import pydantic
-from pydantic import BaseModel
+from pydantic import BaseModel, ValidationError
 
 USING_PYDANTIC_1 = int(pydantic.__version__.split(".")[0]) == 1
 USING_PYDANTIC_2 = int(pydantic.__version__.split(".")[0]) >= 2
 
 PydanticUndefined = None
 if USING_PYDANTIC_2:
     from pydantic_core import PydanticUndefined as _PydanticUndefined  # type: ignore
@@ -137,7 +130,24 @@
                 else root_validator(post=False)(func)
             )
 
         return _decorate
 
 
 compat_model_validator = model_validator
+
+
+def build_validation_error(
+    base_error: ValidationError,
+    line_errors: List,
+    hide_input: bool,
+    input_type: Literal["python", "json"],
+) -> ValidationError:
+    if USING_PYDANTIC_1:
+        return ValidationError(errors=line_errors, model=base_error.model)  # type: ignore
+    else:
+        return ValidationError.from_exception_data(  # type: ignore
+            title=base_error.title,  # type: ignore
+            line_errors=line_errors,
+            input_type=input_type,
+            hide_input=hide_input,
+        )
```

### Comparing `dagster-1.7.7/dagster/_module_alias_map.py` & `dagster-1.7.8/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_scheduler/scheduler.py` & `dagster-1.7.8/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_scheduler/stale.py` & `dagster-1.7.8/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_serdes/__init__.py` & `dagster-1.7.8/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_serdes/config_class.py` & `dagster-1.7.8/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_serdes/ipc.py` & `dagster-1.7.8/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_serdes/serdes.py` & `dagster-1.7.8/dagster/_serdes/serdes.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,26 +187,14 @@
                 f"Multiple deserializers registered for storage name `{deserializer_name}`"
             )
         self.object_deserializers[deserializer_name] = serializer
         if old_storage_names:
             for old_storage_name in old_storage_names:
                 self.object_deserializers[old_storage_name] = serializer
 
-    def has_object_serializer(self, name: str) -> bool:
-        return name in self.object_serializers
-
-    def has_object_deserializer(self, name: str) -> bool:
-        return name in self.object_deserializers
-
-    def get_object_serializer(self, name: str) -> "ObjectSerializer":
-        return self.object_serializers[name]
-
-    def get_object_deserializer(self, name: str) -> "ObjectSerializer":
-        return self.object_deserializers[name]
-
     def register_enum(
         self,
         name: str,
         enum_class: Type[Enum],
         serializer_class: Optional[Type["EnumSerializer"]] = None,
         storage_name: Optional[str] = None,
         old_storage_names: Optional[AbstractSet[str]] = None,
@@ -219,20 +207,14 @@
         self.enum_serializers[name] = serializer
         if storage_name:
             self.enum_serializers[storage_name] = serializer
         if old_storage_names:
             for old_storage_name in old_storage_names:
                 self.enum_serializers[old_storage_name] = serializer
 
-    def has_enum_entry(self, name: str) -> bool:
-        return name in self.enum_serializers
-
-    def get_enum_entry(self, name: str) -> "EnumSerializer":
-        return self.enum_serializers[name]
-
     @staticmethod
     def create() -> "WhitelistMap":
         return WhitelistMap(object_serializers={}, object_deserializers={}, enum_serializers={})
 
 
 _WHITELIST_MAP: Final[WhitelistMap] = WhitelistMap.create()
 
@@ -429,15 +411,15 @@
     """Check if object has been decorated with `@whitelist_for_serdes`."""
     if (
         (isinstance(val, tuple) and hasattr(val, "_fields"))  # NamedTuple
         or (is_dataclass(val) and not isinstance(val, type))  # dataclass instance
         or isinstance(val, BaseModel)
     ):
         klass_name = val.__class__.__name__
-        return whitelist_map.has_object_serializer(klass_name)
+        return klass_name in whitelist_map.object_serializers
 
     return False
 
 
 ###################################################################################################
 # Serializers
 ###################################################################################################
@@ -565,15 +547,15 @@
                             value,
                             whitelist_map=whitelist_map,
                             context=context,
                         )
                     elif context.observed_unknown_serdes_values:
                         unpacked[loaded_name] = context.assert_no_unknown_values(value)
                     else:
-                        unpacked[loaded_name] = cast(PackableValue, value)
+                        unpacked[loaded_name] = value  # type: ignore # 2 hot 4 cast()
 
                 else:
                     context.clear_ignored_unknown_values(value)
 
             return self.klass(**unpacked)
         except Exception as exc:
             value = self.handle_unpack_error(exc, context, unpacked_dict)
@@ -829,15 +811,15 @@
     whitelist_map: WhitelistMap,
     object_handler: Callable[[SerializableObject, WhitelistMap, str], JsonSerializableValue],
     descent_path: str,
 ) -> JsonSerializableValue:
     # this is a hot code path so we handle the common base cases without isinstance
     tval = type(val)
     if tval in (int, float, str, bool) or val is None:
-        return cast(JsonSerializableValue, val)
+        return val  # type: ignore # 2 hot 4 cast()
     if tval is list:
         return [
             _transform_for_serialization(
                 item,
                 whitelist_map,
                 object_handler,
                 f"{descent_path}[{idx}]",
@@ -873,28 +855,28 @@
                 ]
                 for k, v in cast(dict, val).items()
             ]
         }
 
     if isinstance(val, Enum):
         klass_name = val.__class__.__name__
-        if not whitelist_map.has_enum_entry(klass_name):
+        if klass_name not in whitelist_map.enum_serializers:
             raise SerializationError(
                 "Can only serialize whitelisted Enums, received"
                 f" {klass_name}.\nDescent path: {descent_path}",
             )
-        enum_serializer = whitelist_map.get_enum_entry(klass_name)
+        enum_serializer = whitelist_map.enum_serializers[klass_name]
         return {"__enum__": enum_serializer.pack(val, whitelist_map, descent_path)}
     if (
         (isinstance(val, tuple) and hasattr(val, "_fields"))
         or isinstance(val, BaseModel)
         or (is_dataclass(val) and not isinstance(val, type))
     ):
         klass_name = val.__class__.__name__
-        if not whitelist_map.has_object_serializer(klass_name):
+        if klass_name not in whitelist_map.object_serializers:
             raise SerializationError(
                 "Can only serialize whitelisted namedtuples, received"
                 f" {val}.\nDescent path: {descent_path}",
             )
         return object_handler(
             cast(SerializableObject, val),
             whitelist_map,
@@ -958,15 +940,15 @@
 
 def _pack_object(
     obj: SerializableObject, whitelist_map: WhitelistMap, descent_path: str
 ) -> Mapping[str, JsonSerializableValue]:
     # the object_handler for _transform_for_serialization to produce dicts for objects
 
     klass_name = obj.__class__.__name__
-    serializer = whitelist_map.get_object_serializer(klass_name)
+    serializer = whitelist_map.object_serializers[klass_name]
     return dict(serializer.pack_items(obj, whitelist_map, _pack_object, descent_path))
 
 
 class _LazySerializationWrapper(dict):
     """An object used to allow us to drive serialization iteratively
     over the tree of objects via json.dumps, instead of having to create
     an entire tree of primitive objects to pass to json.dumps.
@@ -990,15 +972,15 @@
 
         # populate backing native dict to work around c fast path check
         # https://github.com/python/cpython/blob/0fb18b02c8ad56299d6a2910be0bab8ad601ef24/Modules/_json.c#L1542
         super().__init__({"__serdes": "wrapper"})
 
     def items(self) -> Iterator[Tuple[str, JsonSerializableValue]]:
         klass_name = self._obj.__class__.__name__
-        serializer = self._whitelist_map.get_object_serializer(klass_name)
+        serializer = self._whitelist_map.object_serializers[klass_name]
         yield from serializer.pack_items(
             self._obj, self._whitelist_map, _wrap_object, self._descent_path
         )
 
 
 def _wrap_object(
     obj: SerializableObject,
@@ -1080,39 +1062,39 @@
     def __init__(self, message: str, value: Mapping[str, UnpackedValue]):
         self.message = message
         self.value = value
 
 
 def _unpack_object(val: dict, whitelist_map: WhitelistMap, context: UnpackContext) -> UnpackedValue:
     if "__class__" in val:
-        klass_name = cast(str, val["__class__"])
-        if not whitelist_map.has_object_deserializer(klass_name):
+        klass_name = val["__class__"]
+        if klass_name not in whitelist_map.object_deserializers:
             return context.observe_unknown_value(
                 UnknownSerdesValue(
                     f'Attempted to deserialize class "{klass_name}" which is not in the whitelist.',
                     val,
                 )
             )
 
         val.pop("__class__")
-        deserializer = whitelist_map.get_object_deserializer(klass_name)
+        deserializer = whitelist_map.object_deserializers[klass_name]
         return deserializer.unpack(val, whitelist_map, context)
 
     if "__enum__" in val:
         enum = cast(str, val["__enum__"])
         name, member = enum.split(".")
-        if not whitelist_map.has_enum_entry(name):
+        if name not in whitelist_map.enum_serializers:
             return context.observe_unknown_value(
                 UnknownSerdesValue(
                     f"Attempted to deserialize enum {name} which was not in the whitelist.",
                     val,
                 )
             )
 
-        enum_serializer = whitelist_map.get_enum_entry(name)
+        enum_serializer = whitelist_map.enum_serializers[name]
         return enum_serializer.unpack(member)
 
     if "__set__" in val:
         items = cast(List[JsonSerializableValue], val["__set__"])
         return set(items)
 
     if "__frozenset__" in val:
```

### Comparing `dagster-1.7.7/dagster/_serdes/utils.py` & `dagster-1.7.8/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_seven/__init__.py` & `dagster-1.7.8/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_seven/abc.py` & `dagster-1.7.8/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_seven/compat/datetime.py` & `dagster-1.7.8/dagster/_seven/compat/datetime.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_seven/compat/pendulum.py` & `dagster-1.7.8/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/__init__.py` & `dagster-1.7.8/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/aiodataloader.py` & `dagster-1.7.8/dagster/_utils/aiodataloader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/alert.py` & `dagster-1.7.8/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/backoff.py` & `dagster-1.7.8/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/cached_method.py` & `dagster-1.7.8/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.8/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/concurrency.py` & `dagster-1.7.8/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/container.py` & `dagster-1.7.8/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/cronstring.py` & `dagster-1.7.8/dagster/_utils/cronstring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/dagster_type.py` & `dagster-1.7.8/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/env.py` & `dagster-1.7.8/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/error.py` & `dagster-1.7.8/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/external.py` & `dagster-1.7.8/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/forked_pdb.py` & `dagster-1.7.8/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/hosted_user_process.py` & `dagster-1.7.8/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/indenting_printer.py` & `dagster-1.7.8/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/internal_init.py` & `dagster-1.7.8/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/interrupts.py` & `dagster-1.7.8/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/log.py` & `dagster-1.7.8/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/merger.py` & `dagster-1.7.8/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/net.py` & `dagster-1.7.8/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/schedules.py` & `dagster-1.7.8/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/tags.py` & `dagster-1.7.8/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/temp_file.py` & `dagster-1.7.8/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/test/__init__.py` & `dagster-1.7.8/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/test/data_versions.py` & `dagster-1.7.8/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.8/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.8/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.8/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/timing.py` & `dagster-1.7.8/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/typed_dict.py` & `dagster-1.7.8/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/typing_api.py` & `dagster-1.7.8/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.7/dagster/_utils/warnings.py` & `dagster-1.7.8/dagster/_utils/warnings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import warnings
 from contextlib import contextmanager
+from contextvars import ContextVar
 from typing import Callable, Iterator, Optional, TypeVar
 
 import dagster._check as check
 from dagster._core.decorator_utils import (
     Decoratable,
     apply_context_manager_decorator,
 )
 
 T = TypeVar("T")
 
 # ########################
 # ##### DEPRECATED
 # ########################
 
+_warnings_on = ContextVar("_warnings_on", default=True)
+
 
 def normalize_renamed_param(
     new_val: T,
     new_arg: str,
     old_val: T,
     old_arg: str,
     coerce_old_to_new: Optional[Callable[[T], T]] = None,
@@ -55,14 +58,17 @@
 
 def deprecation_warning(
     subject: str,
     breaking_version: str,
     additional_warn_text: Optional[str] = None,
     stacklevel: int = 3,
 ):
+    if not _warnings_on.get():
+        return
+
     warnings.warn(
         f"{subject} is deprecated and will be removed in {breaking_version}."
         + ((" " + additional_warn_text) if additional_warn_text else ""),
         category=DeprecationWarning,
         stacklevel=stacklevel,
     )
 
@@ -82,14 +88,17 @@
 class ExperimentalWarning(Warning):
     pass
 
 
 def experimental_warning(
     subject: str, additional_warn_text: Optional[str] = None, stacklevel: int = 3
 ) -> None:
+    if not _warnings_on.get():
+        return
+
     extra_text = f" {additional_warn_text}" if additional_warn_text else ""
     warnings.warn(
         f"{subject} is experimental. It may break in future versions, even between dot"
         f" releases.{extra_text} {EXPERIMENTAL_WARNING_HELP}",
         ExperimentalWarning,
         stacklevel=stacklevel,
     )
@@ -124,18 +133,24 @@
 # ########################
 # ##### DISABLE DAGSTER WARNINGS
 # ########################
 
 
 @contextmanager
 def disable_dagster_warnings() -> Iterator[None]:
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=DeprecationWarning)
-        warnings.simplefilter("ignore", category=ExperimentalWarning)
-        yield
+    token = None
+    try:
+        token = _warnings_on.set(False)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=DeprecationWarning)
+            warnings.simplefilter("ignore", category=ExperimentalWarning)
+            yield
+    finally:
+        if token is not None:
+            _warnings_on.reset(token)
 
 
 T_Decoratable = TypeVar("T_Decoratable", bound=Decoratable)
 
 
 def suppress_dagster_warnings(__obj: T_Decoratable) -> T_Decoratable:
     """Mark a method/function as ignoring Dagster-generated warnings. This suppresses any
```

### Comparing `dagster-1.7.7/dagster.egg-info/PKG-INFO` & `dagster-1.7.8/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.7
+Version: 1.7.8
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.7/dagster.egg-info/SOURCES.txt` & `dagster-1.7.8/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -74,25 +74,29 @@
 dagster/_core/code_pointer.py
 dagster/_core/debug.py
 dagster/_core/decorator_utils.py
 dagster/_core/errors.py
 dagster/_core/event_api.py
 dagster/_core/instance_for_test.py
 dagster/_core/libraries.py
+dagster/_core/loader.py
 dagster/_core/log_manager.py
 dagster/_core/nux.py
 dagster/_core/op_concurrency_limits_counter.py
 dagster/_core/origin.py
 dagster/_core/telemetry.py
 dagster/_core/telemetry_upload.py
 dagster/_core/test_utils.py
 dagster/_core/utility_ops.py
 dagster/_core/utils.py
 dagster/_core/asset_graph_view/__init__.py
 dagster/_core/asset_graph_view/asset_graph_view.py
+dagster/_core/blueprints/__init__.py
+dagster/_core/blueprints/blueprint.py
+dagster/_core/blueprints/load_from_yaml.py
 dagster/_core/container_context/__init__.py
 dagster/_core/container_context/config.py
 dagster/_core/definitions/__init__.py
 dagster/_core/definitions/asset_check_evaluation.py
 dagster/_core/definitions/asset_check_result.py
 dagster/_core/definitions/asset_check_spec.py
 dagster/_core/definitions/asset_checks.py
@@ -233,14 +237,16 @@
 dagster/_core/definitions/metadata/table.py
 dagster/_core/definitions/repository_definition/__init__.py
 dagster/_core/definitions/repository_definition/caching_index.py
 dagster/_core/definitions/repository_definition/repository_data.py
 dagster/_core/definitions/repository_definition/repository_data_builder.py
 dagster/_core/definitions/repository_definition/repository_definition.py
 dagster/_core/definitions/repository_definition/valid_definitions.py
+dagster/_core/definitions/tags/__init__.py
+dagster/_core/definitions/tags/tag_set.py
 dagster/_core/events/__init__.py
 dagster/_core/events/log.py
 dagster/_core/events/utils.py
 dagster/_core/execution/__init__.py
 dagster/_core/execution/api.py
 dagster/_core/execution/asset_backfill.py
 dagster/_core/execution/backfill.py
@@ -251,26 +257,24 @@
 dagster/_core/execution/execute_in_process.py
 dagster/_core/execution/execute_in_process_result.py
 dagster/_core/execution/execution_result.py
 dagster/_core/execution/host_mode.py
 dagster/_core/execution/job_backfill.py
 dagster/_core/execution/job_execution_result.py
 dagster/_core/execution/memoization.py
-dagster/_core/execution/poll_compute_logs.py
 dagster/_core/execution/resolve_versions.py
 dagster/_core/execution/resources_init.py
 dagster/_core/execution/retries.py
 dagster/_core/execution/run_cancellation_thread.py
 dagster/_core/execution/run_metrics_thread.py
 dagster/_core/execution/stats.py
 dagster/_core/execution/submit_asset_runs.py
 dagster/_core/execution/tags.py
 dagster/_core/execution/telemetry.py
 dagster/_core/execution/validate_run_config.py
-dagster/_core/execution/watch_orphans.py
 dagster/_core/execution/with_resources.py
 dagster/_core/execution/context/__init__.py
 dagster/_core/execution/context/compute.py
 dagster/_core/execution/context/data_version_cache.py
 dagster/_core/execution/context/hook.py
 dagster/_core/execution/context/init.py
 dagster/_core/execution/context/input.py
@@ -292,14 +296,17 @@
 dagster/_core/execution/plan/objects.py
 dagster/_core/execution/plan/outputs.py
 dagster/_core/execution/plan/plan.py
 dagster/_core/execution/plan/resume_retry.py
 dagster/_core/execution/plan/state.py
 dagster/_core/execution/plan/step.py
 dagster/_core/execution/plan/utils.py
+dagster/_core/execution/scripts/__init__.py
+dagster/_core/execution/scripts/poll_compute_logs.py
+dagster/_core/execution/scripts/watch_orphans.py
 dagster/_core/executor/__init__.py
 dagster/_core/executor/base.py
 dagster/_core/executor/child_process_executor.py
 dagster/_core/executor/in_process.py
 dagster/_core/executor/init.py
 dagster/_core/executor/multiprocess.py
 dagster/_core/executor/step_delegating/__init__.py
@@ -615,16 +622,18 @@
 dagster/_utils/indenting_printer.py
 dagster/_utils/internal_init.py
 dagster/_utils/interrupts.py
 dagster/_utils/log.py
 dagster/_utils/merger.py
 dagster/_utils/net.py
 dagster/_utils/partitions.py
+dagster/_utils/pydantic_yaml.py
 dagster/_utils/schedules.py
 dagster/_utils/security.py
+dagster/_utils/source_position.py
 dagster/_utils/tags.py
 dagster/_utils/temp_file.py
 dagster/_utils/timing.py
 dagster/_utils/typed_dict.py
 dagster/_utils/types.py
 dagster/_utils/typing_api.py
 dagster/_utils/warnings.py
```

### Comparing `dagster-1.7.7/dagster.egg-info/requires.txt` & `dagster-1.7.8/dagster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
 filelock
-dagster-pipes==1.7.7
+dagster-pipes==1.7.8
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
@@ -75,15 +75,15 @@
 types-six
 types-sqlalchemy==1.4.53.34
 types-tabulate
 types-tzlocal
 types-toml
 
 [ruff]
-ruff==0.4.4
+ruff==0.4.5
 
 [test]
 buildkite-test-collector
 docker
 grpcio-tools>=1.44.0
 mock==3.0.5
 mypy-protobuf
```

### Comparing `dagster-1.7.7/setup.py` & `dagster-1.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
         "filelock",
-        "dagster-pipes==1.7.7",
+        "dagster-pipes==1.7.8",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
@@ -161,15 +161,15 @@
             "types-six",  # needed but not specified by grpcio
             "types-sqlalchemy==1.4.53.34",  # later versions introduce odd errors
             "types-tabulate",  # version will be resolved against tabulate
             "types-tzlocal",  # version will be resolved against tzlocal
             "types-toml",  # version will be resolved against toml
         ],
         "ruff": [
-            "ruff==0.4.4",
+            "ruff==0.4.5",
         ],
     },
     entry_points={
         "console_scripts": [
             "dagster = dagster.cli:main",
             "dagster-daemon = dagster.daemon.cli:main",
         ]
```

