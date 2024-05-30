# Comparing `tmp/dagster-graphql-1.7.6.tar.gz` & `tmp/dagster-graphql-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.7.6.tar", last modified: Thu May 16 19:28:10 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.7.tar", last modified: Thu May 23 20:23:17 2024, max compression
```

## Comparing `dagster-graphql-1.7.6.tar` & `dagster-graphql-1.7.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18338 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.180154 dagster-graphql-1.7.6/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    21152 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.180154 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14499 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12324 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7721 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    29547 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15166 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9069 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10352 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    14555 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9774 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.184154 dagster-graphql-1.7.6/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11998 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    55503 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    11078 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2592 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    22713 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    19024 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13742 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    12491 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28766 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.184154 dagster-graphql-1.7.6/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     6110 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17797 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11060 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39840 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1654 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32162 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    47162 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5092 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9135 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10196 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7078 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.220892 dagster-graphql-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-23 20:23:17.220892 dagster-graphql-1.7.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.204892 dagster-graphql-1.7.7/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.204892 dagster-graphql-1.7.7/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.208892 dagster-graphql-1.7.7/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    21499 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.208892 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12324 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7721 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    29547 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15166 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    14555 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.216892 dagster-graphql-1.7.7/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11998 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    55737 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    11078 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    22713 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    19024 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    14136 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    12491 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.216892 dagster-graphql-1.7.7/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     6298 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.216892 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39840 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.216892 dagster-graphql-1.7.7/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    47162 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.220892 dagster-graphql-1.7.7/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.220892 dagster-graphql-1.7.7/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:17.204892 dagster-graphql-1.7.7/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 20:23:17.000000 dagster-graphql-1.7.7/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-23 20:23:17.224892 dagster-graphql-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-05-23 20:22:18.000000 dagster-graphql-1.7.7/setup.py
```

### Comparing `dagster-graphql-1.7.6/LICENSE` & `dagster-graphql-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/PKG-INFO` & `dagster-graphql-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.6
+Version: 1.7.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/cli.py` & `dagster-graphql-1.7.7/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/client/client.py` & `dagster-graphql-1.7.7/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.7/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/client/query.py` & `dagster-graphql-1.7.7/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.7/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from dagster._core.definitions.asset_check_evaluation import AssetCheckEvaluationPlanned
 from dagster._core.definitions.metadata import (
     CodeReferencesMetadataValue,
     DagsterRunMetadataValue,
     MetadataValue,
     TableColumnLineageMetadataValue,
 )
+from dagster._core.definitions.metadata.source_code import LocalFileCodeReference
 from dagster._core.events import (
     DagsterEventType,
     HandledOutputData,
     LoadedInputData,
     StepExpectationResultData,
 )
 from dagster._core.events.log import EventLogEntry
@@ -60,14 +61,15 @@
         GraphenePythonArtifactMetadataEntry,
         GrapheneTableColumnLineageEntry,
         GrapheneTableColumnLineageMetadataEntry,
         GrapheneTableMetadataEntry,
         GrapheneTableSchemaMetadataEntry,
         GrapheneTextMetadataEntry,
         GrapheneTimestampMetadataEntry,
+        GrapheneUrlCodeReference,
         GrapheneUrlMetadataEntry,
     )
     from ..schema.table import GrapheneTable, GrapheneTableSchema
 
     check.mapping_param(metadata, "metadata", key_type=str)
     for key, value in metadata.items():
         if isinstance(value, PathMetadataValue):
@@ -154,20 +156,25 @@
                 jobName=value.job_name,
                 repositoryName=value.repository_name,
                 locationName=value.location_name,
             )
         elif isinstance(value, CodeReferencesMetadataValue):
             yield GrapheneCodeReferencesMetadataEntry(
                 label=key,
-                code_references=[
+                codeReferences=[
                     GrapheneLocalFileCodeReference(
                         filePath=reference.file_path,
                         lineNumber=reference.line_number,
                         label=reference.label,
                     )
+                    if isinstance(reference, LocalFileCodeReference)
+                    else GrapheneUrlCodeReference(
+                        url=reference.url,
+                        label=reference.label,
+                    )
                     for reference in value.code_references
                 ],
             )
         elif isinstance(value, TableMetadataValue):
             yield GrapheneTableMetadataEntry(
                 label=key,
                 table=GrapheneTable(
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/telemetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import TYPE_CHECKING
 
 from dagster._core.telemetry import log_action
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
@@ -14,15 +14,17 @@
     graphene_info: "ResolveInfo", action: str, client_time: str, client_id, metadata: str
 ) -> "GrapheneLogTelemetrySuccess":
     from ..schema.roots.mutation import GrapheneLogTelemetrySuccess
 
     instance = graphene_info.context.instance
     metadata = json.loads(metadata)
     assert isinstance(metadata, dict)
-    client_datetime = datetime.utcfromtimestamp(int(client_time) / 1000)
+    client_datetime = datetime.fromtimestamp(int(client_time) / 1000, timezone.utc).replace(
+        tzinfo=None
+    )
     log_action(
         instance=instance,
         action=action,
         client_time=client_datetime,
         elapsed_time=None,
         metadata={"client_id": client_id, **metadata},
     )
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.7/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/asset_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader, PartitionsDefinition
 from dagster._core.definitions.partition_mapping import PartitionMapping
 from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 from dagster._core.definitions.sensor_definition import (
     SensorType,
 )
 from dagster._core.errors import DagsterInvariantViolationError
-from dagster._core.event_api import EventRecordsFilter
+from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.events import DagsterEventType
 from dagster._core.remote_representation import CodeLocation, ExternalRepository
 from dagster._core.remote_representation.external import ExternalJob, ExternalSensor
 from dagster._core.remote_representation.external_data import (
     ExternalAssetNode,
     ExternalDynamicPartitionsDefinitionData,
     ExternalMultiPartitionsDefinitionData,
@@ -401,21 +401,28 @@
             ),
             assetKey=external_asset_node.asset_key,
             description=external_asset_node.op_description,
             opName=external_asset_node.op_name,
             opVersion=external_asset_node.code_version,
             groupName=external_asset_node.group_name,
             owners=[
-                GrapheneUserAssetOwner(email=owner)
-                if is_valid_email(owner)
-                else GrapheneTeamAssetOwner(team=owner)
+                self._graphene_asset_owner_from_owner_str(owner)
                 for owner in (external_asset_node.owners or [])
             ],
         )
 
+    def _graphene_asset_owner_from_owner_str(
+        self, owner_str: str
+    ) -> Union[GrapheneUserAssetOwner, GrapheneTeamAssetOwner]:
+        if is_valid_email(owner_str):
+            return GrapheneUserAssetOwner(email=owner_str)
+        else:
+            check.invariant(owner_str.startswith("team:"))
+            return GrapheneTeamAssetOwner(team=owner_str[5:])
+
     @property
     def repository_location(self) -> CodeLocation:
         return self._repository_location
 
     @property
     def external_repository(self) -> ExternalRepository:
         return self._external_repository
@@ -573,23 +580,22 @@
 
         # in the future, we can share this same CachingInstanceQueryer across all
         # GrapheneMaterializationEvent which share an external repository for improved performance
         instance_queryer = CachingInstanceQueryer(
             instance=graphene_info.context.instance, asset_graph=asset_graph
         )
         data_time_resolver = CachingDataTimeResolver(instance_queryer=instance_queryer)
-        event_records = instance.get_event_records(
-            EventRecordsFilter(
-                event_type=DagsterEventType.ASSET_MATERIALIZATION,
+        event_records = instance.fetch_materializations(
+            AssetRecordsFilter(
+                asset_key=asset_key,
                 before_timestamp=int(timestampMillis) / 1000.0 + 1,
                 after_timestamp=int(timestampMillis) / 1000.0 - 1,
-                asset_key=asset_key,
             ),
             limit=1,
-        )
+        ).records
 
         if not event_records:
             return []
 
         if not asset_graph.has_materializable_parents(asset_key):
             return []
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/asset_selections.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 class GrapheneRunsFilter(graphene.InputObjectType):
     runIds = graphene.List(graphene.String)
     pipelineName = graphene.InputField(graphene.String)
     tags = graphene.List(graphene.NonNull(GrapheneExecutionTag))
     statuses = graphene.List(graphene.NonNull(GrapheneRunStatus))
     snapshotId = graphene.InputField(graphene.String)
     updatedAfter = graphene.InputField(graphene.Float)
+    updatedBefore = graphene.InputField(graphene.Float)
     createdBefore = graphene.InputField(graphene.Float)
+    createdAfter = graphene.InputField(graphene.Float)
     mode = graphene.InputField(graphene.String)
 
     class Meta:
         description = """This type represents a filter on Dagster runs."""
         name = "RunsFilter"
 
     def to_selector(self):
@@ -54,25 +56,29 @@
             tags = None
 
         if self.statuses:
             statuses = [DagsterRunStatus[status.value] for status in self.statuses]
         else:
             statuses = None
 
+        updated_before = pendulum.from_timestamp(self.updatedBefore) if self.updatedBefore else None
         updated_after = pendulum.from_timestamp(self.updatedAfter) if self.updatedAfter else None
         created_before = pendulum.from_timestamp(self.createdBefore) if self.createdBefore else None
+        created_after = pendulum.from_timestamp(self.createdAfter) if self.createdAfter else None
 
         return RunsFilter(
             run_ids=self.runIds if self.runIds else None,
             job_name=self.pipelineName,
             tags=tags,
             statuses=statuses,
             snapshot_id=self.snapshotId,
+            updated_before=updated_before,
             updated_after=updated_after,
             created_before=created_before,
+            created_after=created_after,
         )
 
 
 class GrapheneStepOutputHandle(graphene.InputObjectType):
     stepKey = graphene.NonNull(graphene.String)
     outputName = graphene.NonNull(graphene.String)
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,29 +160,37 @@
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "JobMetadataEntry"
 
 
 class GrapheneLocalFileCodeReference(graphene.ObjectType):
     filePath = graphene.NonNull(graphene.String)
-    lineNumber = graphene.NonNull(graphene.Int)
+    lineNumber = graphene.Int()
     label = graphene.String()
 
     class Meta:
         name = "LocalFileCodeReference"
 
 
+class GrapheneUrlCodeReference(graphene.ObjectType):
+    url = graphene.NonNull(graphene.String)
+    label = graphene.String()
+
+    class Meta:
+        name = "UrlCodeReference"
+
+
 class GrapheneSourceLocation(graphene.Union):
     class Meta:
-        types = (GrapheneLocalFileCodeReference,)
+        types = (GrapheneLocalFileCodeReference, GrapheneUrlCodeReference)
         name = "SourceLocation"
 
 
 class GrapheneCodeReferencesMetadataEntry(graphene.ObjectType):
-    code_references = non_null_list(GrapheneSourceLocation)
+    codeReferences = non_null_list(GrapheneSourceLocation)
 
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "CodeReferencesMetadataEntry"
 
 
 class GrapheneNullMetadataEntry(graphene.ObjectType):
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/table.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.7/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.7/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.7/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.6
+Version: 1.7.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.6/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.7/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.6/setup.py` & `dagster-graphql-1.7.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.6",
+        "dagster==1.7.7",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

