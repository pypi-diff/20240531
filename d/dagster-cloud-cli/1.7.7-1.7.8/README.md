# Comparing `tmp/dagster-cloud-cli-1.7.7.tar.gz` & `tmp/dagster-cloud-cli-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.7.tar", last modified: Thu May 23 21:43:31 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.8.tar", last modified: Thu May 30 23:22:17 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.7.tar` & `dagster-cloud-cli-1.7.8.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.820963 dagster-cloud-cli-1.7.7/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-23 21:43:31.820963 dagster-cloud-cli-1.7.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    30031 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     3098 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17535 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1985 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      757 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18458 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12788 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/agent_queue.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    13801 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.816963 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    14436 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     8382 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6789 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20800 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.812963 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3066 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-23 21:43:31.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:43:31.820963 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16177 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_deps.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 21:43:31.820963 dagster-cloud-cli-1.7.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1283 2024-05-23 21:36:37.000000 dagster-cloud-cli-1.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.930572 dagster-cloud-cli-1.7.8/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-30 23:22:17.930572 dagster-cloud-cli-1.7.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.918572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.918572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    30031 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17535 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18458 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.922572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12788 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.926572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/agent_queue.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13801 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.926572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.926572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.930572 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13814 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     8382 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6789 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20800 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.918572 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3029 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-30 23:22:17.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:22:17.930572 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16177 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 23:22:17.930572 dagster-cloud-cli-1.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1283 2024-05-30 23:14:29.000000 dagster-cloud-cli-1.7.8/setup.py
```

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/ci/utils.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/ci/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/alert_types.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/artifacts.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/errors.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import os.path
 import re
 import subprocess
 import sys
 import tempfile
 from dataclasses import dataclass
-from typing import List, Mapping, Optional, Sequence, Tuple
+from typing import List, Optional, Tuple
 
 import click
 import pkg_resources
 from packaging import version
 
 from dagster_cloud_cli import ui
 from dagster_cloud_cli.core import docker_runner
@@ -184,44 +184,14 @@
         if self.stdout:
             lines.append("\nOutput:\n" + util.indent(self.stdout))
         if self.stderr:
             lines.append("\nError:\n" + util.indent(self.stderr))
         return "".join(lines)
 
 
-def get_and_check_dependency_versions_from_distributions(
-    distribution_names: Sequence[str],
-) -> Mapping[str, str]:
-    dep_names = ["dagster", "dagster_cloud", "dagster_plus"]
-    dep_versions = {}
-
-    # the distributions are named something like 'dagster-1.0.14-py3-none-any.whl'
-    # and 'dagster_cloud-1.1.7-py3-none-any.whl'
-    for name in distribution_names:
-        for dep_name in dep_names:
-            pattern = re.compile(f"{dep_name}-(.+?)-py")
-            match = pattern.match(name)
-            if match:
-                dep_versions[dep_name] = match.group(1)
-                break
-
-    if "dagster" not in dep_versions:
-        raise ValueError("The dagster package dependency was expected but not found.")
-    print(f"Found package dagster version {dep_versions['dagster']}.")
-
-    if "dagster_cloud" not in dep_versions and "dagster_plus" not in dep_versions:
-        raise ValueError(
-            "Either the dagster_cloud or dagster_plus package dependency was expected but not found."
-        )
-    for dep_name in ["dagster_cloud", "dagster_plus"]:
-        if dep_name in dep_versions:
-            print(f"Found package {dep_name} version {dep_versions[dep_name]}.")
-    return dep_versions
-
-
 def build_deps_from_requirements(
     requirements: DepsRequirements,
     output_directory: str,
     build_method: BuildMethod,
 ) -> Tuple[str, str]:
     os.makedirs(output_directory, exist_ok=True)
     deps_requirements_filename = f"deps-requirements-{requirements.hash}.txt"
@@ -281,15 +251,30 @@
     pex_info = util.get_pex_info(tmp_pex_path)
     pex_hash = pex_info["pex_hash"]
     final_pex_path = os.path.join(output_directory, f"deps-{pex_hash}.pex")
     os.rename(tmp_pex_path, final_pex_path)
     logging.info("Wrote deps pex: %r", final_pex_path)
 
     distribution_names = pex_info["distributions"].keys()
-    dep_versions = get_and_check_dependency_versions_from_distributions(distribution_names)
+    # the distributions are named something like 'dagster-1.0.14-py3-none-any.whl'
+    # and 'dagster_cloud-1.1.7-py3-none-any.whl'
+    dep_names = ["dagster", "dagster_cloud"]
+    dep_versions = {}
+    for name in distribution_names:
+        for dep_name in dep_names:
+            pattern = re.compile(f"{dep_name}-(.+?)-py")
+            match = pattern.match(name)
+            if match:
+                dep_versions[dep_name] = match.group(1)
+                break
+
+    for dep_name in dep_names:
+        if dep_name not in dep_versions:
+            raise ValueError(f"The {dep_name} package dependency was expected but not found.")
+        print(f"Found package {dep_name} version {dep_versions[dep_name]}.")
 
     return final_pex_path, dep_versions["dagster"]
 
 
 def build_deps_from_requirements_file(
     deps_requirements_path: str,
     output_pex_path: str,
```

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,10 +64,9 @@
 dagster_cloud_cli/core/pex_builder/selftest.py
 dagster_cloud_cli/core/pex_builder/source.py
 dagster_cloud_cli/core/pex_builder/util.py
 dagster_cloud_cli_tests/__init__.py
 dagster_cloud_cli_tests/conftest.py
 dagster_cloud_cli_tests/test_check.py
 dagster_cloud_cli_tests/test_ci_commands.py
-dagster_cloud_cli_tests/test_deps.py
 dagster_cloud_cli_tests/test_gql.py
 dagster_cloud_cli_tests/test_metrics.py
```

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.8/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.7/setup.py` & `dagster-cloud-cli-1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 setup(
     name="dagster-cloud-cli",
     version=get_version(),
     author_email="hello@elementl.com",
     packages=find_packages(exclude=["dagster_cloud.cli_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.7",
+        "dagster==1.7.8",
         "packaging>=20.9",
         "questionary",
         "requests",
         "typer>=0.4.1",
         "PyYAML>=5.1",
         "github3.py",
     ],
```

