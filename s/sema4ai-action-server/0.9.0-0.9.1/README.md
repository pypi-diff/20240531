# Comparing `tmp/sema4ai_action_server-0.9.0.tar.gz` & `tmp/sema4ai_action_server-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_action_server-0.9.0.tar", max compression
+gzip compressed data, was "sema4ai_action_server-0.9.1.tar", max compression
```

## Comparing `sema4ai_action_server-0.9.0.tar` & `sema4ai_action_server-0.9.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     4043 2024-05-16 19:42:04.658800 sema4ai_action_server-0.9.0/README.md
--rw-r--r--   0        0        0     2097 2024-05-16 19:42:04.658800 sema4ai_action_server-0.9.0/build.py
--rw-r--r--   0        0        0     1692 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      894 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/README.md
--rw-r--r--   0        0        0      128 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/__init__.py
--rw-r--r--   0        0        0      283 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/__main__.py
--rw-r--r--   0        0        0    20456 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_import.py
--rw-r--r--   0        0        0    20824 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_process_pool.py
--rw-r--r--   0        0        0    11418 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_run.py
--rw-r--r--   0        0        0     1263 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_run_helpers.py
--rw-r--r--   0        0        0     1237 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_action_package.py
--rw-r--r--   0        0        0     7722 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_run.py
--rw-r--r--   0        0        0     5664 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_secrets.py
--rw-r--r--   0        0        0     2623 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_app.py
--rw-r--r--   0        0        0      775 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_cli_helpers.py
--rw-r--r--   0        0        0    24297 2024-05-16 19:42:04.662800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_cli_impl.py
--rw-r--r--   0        0        0    21379 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_database.py
--rw-r--r--   0        0        0     1875 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_download_rcc.py
--rw-r--r--   0        0        0     8045 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_encryption.py
--rw-r--r--   0        0        0     3764 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_errors.py
--rw-r--r--   0        0        0      113 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_errors_action_server.py
--rw-r--r--   0        0        0      642 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_gen_ids.py
--rw-r--r--   0        0        0     5233 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_models.py
--rw-r--r--   0        0        0     2764 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_new_project.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/__init__.py
--rw-r--r--   0        0        0      714 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions.py
--rw-r--r--   0        0        0    10693 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py
--rw-r--r--   0        0        0     7857 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py
--rw-r--r--   0        0        0      691 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py
--rw-r--r--   0        0        0     4455 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_protocols.py
--rw-r--r--   0        0        0    13075 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_rcc.py
--rw-r--r--   0        0        0      426 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/auth.py
--rw-r--r--   0        0        0     1526 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/callback.py
--rw-r--r--   0        0        0     1282 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/constants.py
--rw-r--r--   0        0        0     1027 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/log_custom_handler.py
--rw-r--r--   0        0        0     1548 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/log_formatter.py
--rw-r--r--   0        0        0    19023 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/process.py
--rw-r--r--   0        0        0      692 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/run_in_thread.py
--rw-r--r--   0        0        0    13510 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/system_mutex.py
--rw-r--r--   0        0        0     4031 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_runs_state_cache.py
--rw-r--r--   0        0        0    16414 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_selftest.py
--rw-r--r--   0        0        0    11784 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server.py
--rw-r--r--   0        0        0    16734 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server_expose.py
--rw-r--r--   0        0        0    10275 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server_websockets.py
--rw-r--r--   0        0        0     6041 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_settings.py
--rw-r--r--   0        0        0     1650 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_slugify.py
--rw-r--r--   0        0        0   880128 2024-05-16 19:42:54.747024 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_static_contents.py
--rw-r--r--   0        0        0     2403 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/_whitelist.py
--rw-r--r--   0        0        0     1287 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/api.py
--rw-r--r--   0        0        0        6 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/bin/.gitignore
--rw-r--r--   0        0        0     1859 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/cli.py
--rw-r--r--   0        0        0      870 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/env/__init__.py
--rw-r--r--   0        0        0     5247 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/__init__.py
--rw-r--r--   0        0        0      408 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/migration_add_action_enabled.py
--rw-r--r--   0        0        0      375 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/migration_add_action_managed_params.py
--rw-r--r--   0        0        0      381 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/migration_add_action_options.py
--rw-r--r--   0        0        0      372 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/migration_add_is_consequential.py
--rw-r--r--   0        0        0      259 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/migration_initial.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/__init__.py
--rw-r--r--   0        0        0      468 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_ask_user.py
--rw-r--r--   0        0        0     7645 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_build.py
--rw-r--r--   0        0        0     7658 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_build_cli.py
--rw-r--r--   0        0        0     3387 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_metadata.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/py.typed
--rw-r--r--   0        0        0      349 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/README.md
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/__init__.py
--rw-r--r--   0        0        0    14982 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py
--rw-r--r--   0        0        0      157 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/action_package_handling/cli_errors.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/__init__.py
--rw-r--r--   0        0        0     1812 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py
--rw-r--r--   0        0        0     6112 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py
--rw-r--r--   0        0        0     1405 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py
--rw-r--r--   0        0        0     2333 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py
--rw-r--r--   0        0        0    23321 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py
--rw-r--r--   0        0        0    23813 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/__init__.py
--rw-r--r--   0        0        0      849 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
--rw-r--r--   0        0        0    11440 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
--rw-r--r--   0        0        0     9084 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
--rw-r--r--   0        0        0    13400 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
--rw-r--r--   0        0        0    25543 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
--rw-r--r--   0        0        0        0 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/__init__.py
--rw-r--r--   0        0        0     8976 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
--rw-r--r--   0        0        0     1431 2024-05-16 19:42:04.666800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
--rw-r--r--   0        0        0    14693 2024-05-16 19:42:04.670800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
--rw-r--r--   0        0        0     7245 2024-05-16 19:42:04.670800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py
--rw-r--r--   0        0        0      319 2024-05-16 19:42:04.670800 sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/termcolors/__init__.py
--rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 sema4ai_action_server-0.9.0/setup.py
--rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 sema4ai_action_server-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4043 2024-05-17 11:54:37.830413 sema4ai_action_server-0.9.1/README.md
+-rw-r--r--   0        0        0     2097 2024-05-17 11:54:37.830413 sema4ai_action_server-0.9.1/build.py
+-rw-r--r--   0        0        0     1692 2024-05-17 11:54:37.834413 sema4ai_action_server-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      894 2024-05-17 11:54:37.834413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/README.md
+-rw-r--r--   0        0        0      128 2024-05-17 11:54:37.834413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/__init__.py
+-rw-r--r--   0        0        0      283 2024-05-17 11:54:37.834413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/__main__.py
+-rw-r--r--   0        0        0    20456 2024-05-17 11:54:37.834413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_import.py
+-rw-r--r--   0        0        0    20824 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_process_pool.py
+-rw-r--r--   0        0        0    11418 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_run.py
+-rw-r--r--   0        0        0     1263 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_run_helpers.py
+-rw-r--r--   0        0        0     1237 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_action_package.py
+-rw-r--r--   0        0        0     7722 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_run.py
+-rw-r--r--   0        0        0     6005 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_secrets.py
+-rw-r--r--   0        0        0     2623 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_app.py
+-rw-r--r--   0        0        0      775 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_cli_helpers.py
+-rw-r--r--   0        0        0    24297 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_cli_impl.py
+-rw-r--r--   0        0        0    21379 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_database.py
+-rw-r--r--   0        0        0     1875 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_download_rcc.py
+-rw-r--r--   0        0        0     8045 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_encryption.py
+-rw-r--r--   0        0        0     3764 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_errors.py
+-rw-r--r--   0        0        0      113 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_errors_action_server.py
+-rw-r--r--   0        0        0      642 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_gen_ids.py
+-rw-r--r--   0        0        0     5233 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_models.py
+-rw-r--r--   0        0        0     2764 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_new_project.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions.py
+-rw-r--r--   0        0        0    10693 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py
+-rw-r--r--   0        0        0     7857 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py
+-rw-r--r--   0        0        0      691 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py
+-rw-r--r--   0        0        0     4455 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_protocols.py
+-rw-r--r--   0        0        0    13075 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_rcc.py
+-rw-r--r--   0        0        0      426 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/auth.py
+-rw-r--r--   0        0        0     1526 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/callback.py
+-rw-r--r--   0        0        0     1282 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/constants.py
+-rw-r--r--   0        0        0     1027 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/log_custom_handler.py
+-rw-r--r--   0        0        0     1548 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/log_formatter.py
+-rw-r--r--   0        0        0    19023 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/process.py
+-rw-r--r--   0        0        0      692 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/run_in_thread.py
+-rw-r--r--   0        0        0    13510 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/system_mutex.py
+-rw-r--r--   0        0        0     4031 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_runs_state_cache.py
+-rw-r--r--   0        0        0    16414 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_selftest.py
+-rw-r--r--   0        0        0    11784 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server.py
+-rw-r--r--   0        0        0    16734 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server_expose.py
+-rw-r--r--   0        0        0    10275 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server_websockets.py
+-rw-r--r--   0        0        0     6041 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_settings.py
+-rw-r--r--   0        0        0     1650 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_slugify.py
+-rw-r--r--   0        0        0   880128 2024-05-17 11:55:18.634274 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_static_contents.py
+-rw-r--r--   0        0        0     2403 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/_whitelist.py
+-rw-r--r--   0        0        0     1287 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/api.py
+-rw-r--r--   0        0        0        6 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/bin/.gitignore
+-rw-r--r--   0        0        0     1859 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/cli.py
+-rw-r--r--   0        0        0      870 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/env/__init__.py
+-rw-r--r--   0        0        0     5247 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/migration_add_action_enabled.py
+-rw-r--r--   0        0        0      375 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/migration_add_action_managed_params.py
+-rw-r--r--   0        0        0      381 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/migration_add_action_options.py
+-rw-r--r--   0        0        0      372 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/migration_add_is_consequential.py
+-rw-r--r--   0        0        0      259 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/migration_initial.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_ask_user.py
+-rw-r--r--   0        0        0     7645 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_build.py
+-rw-r--r--   0        0        0     7658 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_build_cli.py
+-rw-r--r--   0        0        0     3387 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/py.typed
+-rw-r--r--   0        0        0      349 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/__init__.py
+-rw-r--r--   0        0        0    14982 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/action_package_handling/cli_errors.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/__init__.py
+-rw-r--r--   0        0        0     1812 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py
+-rw-r--r--   0        0        0     6112 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py
+-rw-r--r--   0        0        0     1405 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py
+-rw-r--r--   0        0        0     2333 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py
+-rw-r--r--   0        0        0    23321 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py
+-rw-r--r--   0        0        0    23813 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-17 11:54:37.838413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
+-rw-r--r--   0        0        0    11440 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
+-rw-r--r--   0        0        0     9084 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
+-rw-r--r--   0        0        0    13400 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
+-rw-r--r--   0        0        0    25543 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/__init__.py
+-rw-r--r--   0        0        0     8976 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
+-rw-r--r--   0        0        0     1431 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
+-rw-r--r--   0        0        0    14693 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
+-rw-r--r--   0        0        0     7245 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py
+-rw-r--r--   0        0        0      319 2024-05-17 11:54:37.842413 sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/termcolors/__init__.py
+-rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 sema4ai_action_server-0.9.1/setup.py
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 sema4ai_action_server-0.9.1/PKG-INFO
```

### Comparing `sema4ai_action_server-0.9.0/README.md` & `sema4ai_action_server-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/build.py` & `sema4ai_action_server-0.9.1/build.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/pyproject.toml` & `sema4ai_action_server-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-action-server"
-version = "0.9.0"
+version = "0.9.1"
 description = """Sema4AI Action Server"""
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/sema4ai/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/README.md` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_import.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_import.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_process_pool.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_process_pool.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_run.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_run.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_actions_run_helpers.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_actions_run_helpers.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_action_package.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_action_package.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_run.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_run.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_api_secrets.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_api_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,22 @@
         raise ValueError("Expected the received secrets to be a dict.")
 
     for k, v in secrets.items():
         if not isinstance(k, str):
             raise ValueError("Expected the received secrets keys to be strings.")
 
         if not isinstance(v, str):
-            raise ValueError("Expected the received secrets values to be strings.")
+            if isinstance(v, dict):
+                if "access_token" not in v:
+                    raise ValueError(
+                        "When passing a dict for an OAuth2Secret, it's expected that the dict has at least the `access_token` key."
+                    )
+            else:
+                raise ValueError(
+                    "Expected the received secrets values to be strings or dicts."
+                )
 
     IN_MEMORY_SECRETS._update_secrets(
         typing.cast(dict[str, str], secrets),
         typing.cast(Literal["global"] | ActionPackageScopeTypedDict, scope),
     )
     return "ok"
```

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_app.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_app.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_cli_helpers.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_cli_impl.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_cli_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_database.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_database.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_download_rcc.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_download_rcc.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_encryption.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_encryption.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_errors.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_errors.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_gen_ids.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_gen_ids.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_models.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_models.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_new_project.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_new_project.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_protocols.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_rcc.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_rcc.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/callback.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/constants.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/constants.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/log_custom_handler.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/log_custom_handler.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/log_formatter.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/log_formatter.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/process.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/process.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/run_in_thread.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/run_in_thread.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_robo_utils/system_mutex.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_robo_utils/system_mutex.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_runs_state_cache.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_runs_state_cache.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_selftest.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_selftest.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server_expose.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server_expose.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_server_websockets.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_server_websockets.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_settings.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_settings.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_slugify.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_slugify.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_static_contents.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_static_contents.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/_whitelist.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/_whitelist.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/api.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/cli.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/env/__init__.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/env/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/migrations/__init__.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_build.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_build.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_build_cli.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_build_cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/package/_package_metadata.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/package/_package_metadata.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py` & `sema4ai_action_server-0.9.1/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.9.0/setup.py` & `sema4ai_action_server-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'websockets>=12.0,<13.0']
 
 entry_points = \
 {'console_scripts': ['action-server = sema4ai.action_server.cli:main']}
 
 setup_kwargs = {
     'name': 'sema4ai-action-server',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Sema4AI Action Server',
     'long_description': '# sema4ai-action-server\n\n[Sema4.ai Action Server](https://github.com/sema4ai/actions#readme) is a Python framework designed to simplify the deployment of actions (AI or otherwise).\n\nAn `action` in this case is defined as a Python function (which has inputs/outputs defined), which is served by the `Sema4.ai Action Server`.\n\nThe `Sema4.ai Action Server` automatically generates an OpenAPI spec for your Python code, enabling different AI/LLM Agents to understand and call your Action. It also manages the Action lifecycle and provides full traceability of what happened during runs.\n\n## 1. Install Action Server\n\nAction Server is available as a stand-alone fully signed executable and via `pip install sema4ai-action-server`.\n> We recommend the executable to prevent confusion in case you have multiple/crowded Python environments, etc.\n\n#### For macOS\n\n```sh\n# Install Sema4.ai Action Server\nbrew update\nbrew install sema4ai/tools/action-server \n```\n\n#### For Windows\n\n```sh\n# Download Sema4.ai Action Server\ncurl -o action-server.exe https://sema4.ai/cdn/downloads/action-server/releases/latest/windows64/action-server.exe\n\n# Add to PATH or move to a folder that is in PATH\nsetx PATH=%PATH%;%CD%\n```\n\n#### For Linux\n\n```sh\n# Download Sema4.ai Action Server\ncurl -o action-server https://sema4.ai/cdn/downloads/action-server/releases/latest/linux64/action-server\nchmod a+x action-server\n\n# Add to PATH or move to a folder that is in PATH\nsudo mv action-server /usr/local/bin/\n```\n\n## 2. Run your first Action\n\n```sh\n# Bootstrap a new project using this template.\n# You\'ll be prompted for the name of the project (directory):\naction-server new\n\n# Start Action Server \ncd my-project\naction-server start --expose\n```\n\n👉 You should now have an Action Server running locally at: [http://localhost:8080](http://localhost:8080), so open that in your browser and the web UI will guide you further.\n\n👉 Using the `--expose` -flag, you also get a public internet-facing URL (something like "https://twently-cuddly-dinosaurs.robocorp.link") and the related token. These are the details that you need to configure your AI Agent to have access to your Action\n\n## What do you need in your Action Package\n\nAn `Action Package` is currently defined as a local folder that contains at least one Python file containing an action entry point (a Python function marked with `@action` -decorator from `sema4ai.actions`).\n\nThe `package.yaml` file is required for specifying the Python environment and dependencies for your Action ([RCC](https://github.com/robocorp/rcc/) will be used to automatically bootstrap it and keep it updated given the `package.yaml` contents).\n\n> Note: the `package.yaml` is optional if the action server is not being used as a standalone (i.e.: if it was pip-installed it can use the same python environment where it\'s installed).\n\n### Bootstrapping a new Action\n\nStart new projects with:\n\n`action-server new`\n\nNote: the `action-server` executable should be automatically added to your python installation after `pip install sema4ai-action-server`, but if for some reason it wasn\'t pip-installed, it\'s also possible to use `python -m sema4ai.action_server` instead of `action-server`.\n\nAfter creating the project, it\'s possible to serve the actions under the current directory with:\n\n`action-server start`\n\nFor example: When running `action-server start`, the action server will scan for existing actions under the current directory, and it\'ll start serving those.\n\nAfter it\'s started, it\'s possible to access the following URLs:\n\n- `/index.html`: UI for the Action Server.\n- `/openapi.json`: Provides the openapi spec for the action server.\n- `/docs`: Provides access to the APIs available in the server and a UI to test it.\n\n## Documentation\n\nExplore our [docs](https://github.com/sema4ai/actions/tree/master/action_server/docs) for extensive documentation.\n\n## Changelog\n\nA list of releases and corresponding changes can be found in the [changelog](https://github.com/sema4ai/actions/blob/master/action_server/docs/CHANGELOG.md).\n',
     'author': 'Fabio Z.',
     'author_email': 'fabio@robocorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/sema4ai/actions/',
```

### Comparing `sema4ai_action_server-0.9.0/PKG-INFO` & `sema4ai_action_server-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-action-server
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sema4AI Action Server
 Home-page: https://github.com/sema4ai/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

