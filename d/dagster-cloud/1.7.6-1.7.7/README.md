# Comparing `tmp/dagster-cloud-1.7.6.tar.gz` & `tmp/dagster-cloud-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.6.tar", last modified: Thu May 16 20:18:25 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.7.tar", last modified: Thu May 23 21:43:24 2024, max compression
```

## Comparing `dagster-cloud-1.7.6.tar` & `dagster-cloud-1.7.7.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.464893 dagster-cloud-1.7.6/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      316 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)      826 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45896 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9443 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/defs.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/mutation.py
--rw-r--r--   0 root         (0) root         (0)     2245 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19251 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/artifacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     7964 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3234 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)     4194 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7254 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)    10624 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3808 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3215 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17294 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    22345 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.488893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.488893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.492893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.492893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2115 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17844 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12797 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.496893 dagster-cloud-1.7.6/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.496893 dagster-cloud-1.7.6/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.500893 dagster-cloud-1.7.6/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.500893 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.516893 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16377 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    46580 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      640 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.524893 dagster-cloud-1.7.6/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6742 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19554 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.524893 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7585 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.528893 dagster-cloud-1.7.6/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2778 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.528893 dagster-cloud-1.7.6/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.532893 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.532893 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12989 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.540893 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28867 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    28823 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.544893 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26266 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)     9855 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14260 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    85944 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4240 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      504 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3073 2024-05-16 20:06:43.000000 dagster-cloud-1.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.549021 dagster-cloud-1.7.7/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      826 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45896 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9443 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)    10624 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17294 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    22345 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.557021 dagster-cloud-1.7.7/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17185 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    48370 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      640 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19558 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.561021 dagster-cloud-1.7.7/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12989 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28867 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28823 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26266 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9855 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14260 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    85944 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:24.553021 dagster-cloud-1.7.7/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-23 21:43:24.000000 dagster-cloud-1.7.7/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4240 2024-05-23 21:43:24.000000 dagster-cloud-1.7.7/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:43:24.000000 dagster-cloud-1.7.7/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-23 21:43:24.000000 dagster-cloud-1.7.7/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-23 21:43:24.000000 dagster-cloud-1.7.7/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 21:43:24.565021 dagster-cloud-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3128 2024-05-23 21:36:37.000000 dagster-cloud-1.7.7/setup.py
```

### Comparing `dagster-cloud-1.7.6/PKG-INFO` & `dagster-cloud-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.6
+Version: 1.7.7
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.6/README.md` & `dagster-cloud-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/agent/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/agent/cli/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster-cloud-1.7.7/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/agent/queries.py` & `dagster-cloud-1.7.7/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/defs.py` & `dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/defs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/types.py` & `dagster-cloud-1.7.7/dagster_cloud/anomaly_detection/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/api/dagster_cloud_api.py` & `dagster-cloud-1.7.7/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/auth/constants.py` & `dagster-cloud-1.7.7/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/insights_utils.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/insights_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/metrics_utils.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/query.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/definitions.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py` & `dagster-cloud-1.7.7/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster-cloud-1.7.7/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/execution/utils/process.py` & `dagster-cloud-1.7.7/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/instance/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/client.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/compile.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/manager.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/registry.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/server.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/types.py` & `dagster-cloud-1.7.7/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/secrets/loader.py` & `dagster-cloud-1.7.7/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/serverless/io_manager.py` & `dagster-cloud-1.7.7/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/client.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/queries.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,38 @@
         assetEntry {
             ...AssetEntryFragment
         }
     }
     """
 )
 
+ASSET_CHECK_STATE_FRAGMENT = (
+    EVENT_LOG_ENTRY_FRAGMENT
+    + """
+    fragment AssetCheckSummaryRecordFragment on AssetCheckSummaryRecord {
+        assetCheckKey {
+            assetKey {
+                path
+            }
+            name
+        }
+        lastCheckExecutionRecord {
+            id
+            runId
+            status
+            event {
+                ...EventLogEntryFragment
+            }
+            createTimestamp
+        }
+        lastRunId 
+    } 
+"""
+)
+
 GET_RECORDS_FOR_RUN_QUERY = (
     EVENT_RECORD_FRAGMENT
     + """
     query getRecordsForRun($runId: String!, $cursor: String, $ofType: String, $ofTypes: [String!], $limit: Int) {
         eventLogs {
             getRecordsForRun(runId: $runId, cursor: $cursor, ofType: $ofType, ofTypes: $ofTypes, limit: $limit) {
                 records {
@@ -237,14 +261,27 @@
                 ...AssetRecordFragment
             }
         }
     }
     """
 )
 
+GET_ASSET_CHECK_STATE_QUERY = (
+    ASSET_CHECK_STATE_FRAGMENT
+    + """
+    query getAssetCheckSummaryRecord($assetCheckKeys: [String!]) {
+        eventLogs {
+            getAssetCheckSummaryRecord(assetCheckKeys: $assetCheckKeys) {
+                ...AssetCheckSummaryRecordFragment
+            }
+        }
+    }
+"""
+)
+
 GET_ALL_ASSET_KEYS_QUERY = """
     query getAllAssetKeys {
         eventLogs {
             getAllAssetKeys
         }
     }
     """
```

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/storage.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,21 @@
     EventRecordsResult,
     RunShardedEventsCursor,
     RunStatusChangeRecordsFilter,
 )
 from dagster._core.events import DagsterEvent, DagsterEventType
 from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, RunStepMarker, StepEventStatus
-from dagster._core.storage.asset_check_execution_record import AssetCheckExecutionRecord
+from dagster._core.storage.asset_check_execution_record import (
+    AssetCheckExecutionRecord,
+    AssetCheckExecutionRecordStatus,
+)
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.event_log.base import (
+    AssetCheckSummaryRecord,
     AssetEntry,
     AssetRecord,
     EventLogConnection,
     EventLogStorage,
     PlannedMaterializationInfo,
 )
 from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
@@ -80,14 +84,15 @@
     ENABLE_SECONDARY_INDEX_MUTATION,
     FETCH_MATERIALIZATIONS_QUERY,
     FETCH_OBSERVATIONS_QUERY,
     FETCH_PLANNED_MATERIALIZATIONS,
     FREE_CONCURRENCY_SLOT_FOR_STEP_MUTATION,
     FREE_CONCURRENCY_SLOTS_FOR_RUN_MUTATION,
     GET_ALL_ASSET_KEYS_QUERY,
+    GET_ASSET_CHECK_STATE_QUERY,
     GET_ASSET_RECORDS_QUERY,
     GET_CONCURRENCY_INFO_QUERY,
     GET_CONCURRENCY_KEYS_QUERY,
     GET_DYNAMIC_PARTITIONS_QUERY,
     GET_EVENT_RECORDS_QUERY,
     GET_EVENT_TAGS_FOR_ASSET,
     GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS,
@@ -359,14 +364,43 @@
     check.dict_param(graphene_asset_record, "graphene_asset_record")
     return AssetRecord(
         storage_id=graphene_asset_record["storageId"],
         asset_entry=_asset_entry_from_graphql(graphene_asset_record["assetEntry"]),
     )
 
 
+def _asset_check_execution_record_from_graphql(data: Dict):
+    return AssetCheckExecutionRecord(
+        id=data["id"],
+        run_id=data["runId"],
+        status=AssetCheckExecutionRecordStatus(data["status"]),
+        event=_event_log_entry_from_graphql(data["event"]),
+        create_timestamp=data["createTimestamp"],
+    )
+
+
+def _asset_check_summary_record_from_graphql(
+    graphene_asset_check_summary_record: Dict,
+) -> AssetCheckSummaryRecord:
+    check.dict_param(graphene_asset_check_summary_record, "graphene_asset_check_summary_record")
+    return AssetCheckSummaryRecord(
+        asset_check_key=AssetCheckKey.from_graphql_input(
+            graphene_asset_check_summary_record["assetCheckKey"]
+        ),
+        last_check_execution_record=(
+            _asset_check_execution_record_from_graphql(
+                graphene_asset_check_summary_record["lastCheckExecutionRecord"]
+            )
+            if graphene_asset_check_summary_record["lastCheckExecutionRecord"]
+            else None
+        ),
+        last_run_id=graphene_asset_check_summary_record["lastRunId"],
+    )
+
+
 def _event_records_result_from_graphql(graphene_event_records_result: Dict) -> EventRecordsResult:
     return EventRecordsResult(
         records=[
             _event_record_from_graphql(record)
             for record in graphene_event_records_result["records"]
         ],
         cursor=graphene_event_records_result["cursor"],
@@ -634,15 +668,14 @@
         limit: Optional[int] = None,
         ascending: Optional[bool] = False,
     ) -> Sequence[EventLogRecord]:
         check.opt_inst_param(event_records_filter, "event_records_filter", EventRecordsFilter)
         check.opt_int_param(limit, "limit")
         check.bool_param(ascending, "ascending")
 
-        print(_get_event_records_filter_input(event_records_filter))
         res = self._execute_query(
             GET_EVENT_RECORDS_QUERY,
             variables={
                 "eventRecordsFilter": _get_event_records_filter_input(event_records_filter),
                 "limit": limit,
                 "ascending": ascending,
             },
@@ -652,14 +685,28 @@
             for result in res["data"]["eventLogs"]["getEventRecords"]
         ]
 
     @property
     def asset_records_have_last_observation(self) -> bool:
         return True
 
+    def get_asset_check_summary_records(
+        self, asset_check_keys: Sequence[AssetCheckKey]
+    ) -> Mapping[AssetCheckKey, AssetCheckSummaryRecord]:
+        res = self._execute_query(
+            GET_ASSET_CHECK_STATE_QUERY,
+            variables={"assetCheckKeys": [key.to_user_string() for key in asset_check_keys]},
+        )
+        records = {}
+        for result in res["data"]["eventLogs"]["getAssetCheckSummaryRecord"]:
+            record = _asset_check_summary_record_from_graphql(result)
+            check_key = AssetCheckKey.from_graphql_input(result["assetCheckKey"])
+            records[check_key] = record
+        return records
+
     def get_asset_records(
         self, asset_keys: Optional[Sequence[AssetKey]] = None
     ) -> Iterable[AssetRecord]:
         res = self._execute_query(
             GET_ASSET_RECORDS_QUERY,
             variables={
                 "assetKeys": (
```

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/utils.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/runs/queries.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/runs/storage.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/runs/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunNotFoundError,
     DagsterSnapshotDoesNotExist,
 )
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
-from dagster._core.execution.types import RunTelemetryData
+from dagster._core.execution.telemetry import RunTelemetryData
 from dagster._core.remote_representation.origin import RemoteJobOrigin
 from dagster._core.snap import (
     ExecutionPlanSnapshot,
     JobSnapshot,
     create_execution_plan_snapshot_id,
     create_job_snapshot_id,
 )
```

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/schedules/queries.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/storage/schedules/storage.py` & `dagster-cloud-1.7.7/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/util/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/util/container_resources.py` & `dagster-cloud-1.7.7/dagster_cloud/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/docker.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/ecs.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/docker/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/client.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/launcher.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/service.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/utils.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/utils.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster-cloud-1.7.7/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.7/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.6
+Version: 1.7.7
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.6/dagster_cloud.egg-info/SOURCES.txt` & `dagster-cloud-1.7.7/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.6/setup.py` & `dagster-cloud-1.7.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.6",
-        "dagster-cloud-cli==1.7.6",
+        "dagster==1.7.7",
+        "dagster-cloud-cli==1.7.7",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
         "typer",
     ],
     extras_require={
         "tests": [
@@ -60,23 +60,23 @@
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
-            "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.23.6",
-            "dagster_k8s==0.23.6",
+            "dagster-dbt==0.23.7",
+            "dagster_k8s==0.23.7",
+            "requests<2.32.0",  # https://github.com/dagster-io/dagster/pull/21977
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.23.6"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.23.6"],
-        "ecs": ["dagster_aws==0.23.6", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.7"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.7"],
+        "ecs": ["dagster_aws==0.23.7", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

