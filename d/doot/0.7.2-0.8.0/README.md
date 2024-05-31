# Comparing `tmp/doot-0.7.2.tar.gz` & `tmp/doot-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doot-0.7.2.tar", last modified: Sat Apr 20 15:42:47 2024, max compression
+gzip compressed data, was "doot-0.8.0.tar", last modified: Fri May 31 20:27:47 2024, max compression
```

## Comparing `doot-0.7.2.tar` & `doot-0.8.0.tar`

### file list

```diff
@@ -1,185 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.842469 doot-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-20 15:42:41.000000 doot-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-20 15:42:47.838469 doot-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-20 15:42:41.000000 doot-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__data/
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__data/aliases.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__data/constants.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/basic_toml
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/stub_task_py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/tasks_toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__tests/test_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.818468 doot-0.7.2/doot/_abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/dbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.818468 doot-0.7.2/doot/_structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.822468 doot-0.7.2/doot/_structs/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_code_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_path_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_string_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_type_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_task_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/code_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/sname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/structured_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/task_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/toml_loc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/actions/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_queuing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_queuing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/speak.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/templater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/cmds/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/__tests/test_list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/base_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/clean_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/graph_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/help_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/locs_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/plugins_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/step_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/stub_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/control/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/control/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/base_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/step_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-20 15:42:41.000000 doot-0.7.2/doot/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-20 15:42:41.000000 doot-0.7.2/doot/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/loaders/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/task_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/fail_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/human_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/path_manip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/zipper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/parsers/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/__tests/test_flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/flexible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/reporters/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__tests/test_stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__tests/test_summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/basic_reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-20 15:42:41.000000 doot-0.7.2/doot/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/task/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/task/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/specialised_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot/utils/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/__tests/test_action_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/action_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/chain_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/check_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/mock_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/plugin_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/testing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/trace_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/url_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-20 15:42:41.000000 doot-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:42:47.842469 doot-0.7.2/setup.cfg
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.746801 doot-0.8.0/
+-rw-rw-r--   0 john      (1000) john      (1000)     1421 2023-12-10 00:45:10.000000 doot-0.8.0/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)    10281 2024-05-31 20:27:47.746801 doot-0.8.0/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     7341 2024-05-31 20:21:57.000000 doot-0.8.0/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.726801 doot-0.8.0/doot/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.726801 doot-0.8.0/doot/__data/
+-rw-rw-r--   0 john      (1000) john      (1000)     5212 2024-05-11 03:58:26.000000 doot-0.8.0/doot/__data/aliases.toml
+-rw-rw-r--   0 john      (1000) john      (1000)     3080 2024-05-31 20:04:24.000000 doot-0.8.0/doot/__data/constants.toml
+-rw-rw-r--   0 john      (1000) john      (1000)     6539 2024-05-31 20:21:57.000000 doot-0.8.0/doot/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4033 2024-05-31 20:04:24.000000 doot-0.8.0/doot/__main__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.726801 doot-0.8.0/doot/__templates/
+-rw-rw-r--   0 john      (1000) john      (1000)     2724 2024-05-31 20:04:24.000000 doot-0.8.0/doot/__templates/basic_config_toml
+-rw-rw-r--   0 john      (1000) john      (1000)     1988 2024-05-31 20:04:24.000000 doot-0.8.0/doot/__templates/stub_task_py
+-rw-rw-r--   0 john      (1000) john      (1000)      357 2023-12-09 23:29:38.000000 doot-0.8.0/doot/__templates/tasks_toml
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.726801 doot-0.8.0/doot/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)      996 2024-04-15 22:30:11.000000 doot-0.8.0/doot/__tests/test_basic.py
+-rw-rw-r--   0 john      (1000) john      (1000)      615 2024-04-15 22:30:11.000000 doot-0.8.0/doot/__tests/test_inits.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.726801 doot-0.8.0/doot/_abstract/
+-rw-rw-r--   0 john      (1000) john      (1000)      786 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1160 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3172 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/control.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1367 2023-10-17 22:05:44.000000 doot-0.8.0/doot/_abstract/dbm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 22:30:11.000000 doot-0.8.0/doot/_abstract/loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-04-15 22:30:11.000000 doot-0.8.0/doot/_abstract/overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1283 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/parser.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1004 2023-12-10 23:41:06.000000 doot-0.8.0/doot/_abstract/policy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5718 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/protocols.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1433 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/reporter.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2449 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_abstract/task.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.730801 doot-0.8.0/doot/_structs/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-12-09 23:29:38.000000 doot-0.8.0/doot/_structs/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.734801 doot-0.8.0/doot/_structs/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1338 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_action_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6392 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_artifact.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2255 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_code_ref.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3099 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_formatter.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13573 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8934 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2349 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key_multi.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7046 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key_path_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4423 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key_string_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3692 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_key_type_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2475 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_location.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5965 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3411 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_relation_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2482 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_structured_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4093 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_stub.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16130 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_task_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12096 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/__tests/test_task_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5997 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/action_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4337 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/artifact.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6322 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/code_ref.py
+-rw-rw-r--   0 john      (1000) john      (1000)    27478 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/key.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6520 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/location.py
+-rw-rw-r--   0 john      (1000) john      (1000)      172 2023-12-11 21:35:03.000000 doot-0.8.0/doot/_structs/log.doot
+-rw-rw-r--   0 john      (1000) john      (1000)     7332 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/logger_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12735 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7354 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/relation_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5174 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/structured_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8993 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/stub.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10227 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/task_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)    19063 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/task_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2240 2024-05-31 20:04:24.000000 doot-0.8.0/doot/_structs/trace.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.734801 doot-0.8.0/doot/actions/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.8.0/doot/actions/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.734801 doot-0.8.0/doot/actions/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1035 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_base_action.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1345 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_control_flow.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1345 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2908 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_job_actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3384 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_job_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4407 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_job_injection.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2869 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_job_queuing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1345 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_postbox.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1345 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1345 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/__tests/test_state.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1577 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/base_action.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5462 2024-04-15 22:30:11.000000 doot-0.8.0/doot/actions/compression.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5937 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/control_flow.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12967 2024-04-17 20:02:24.000000 doot-0.8.0/doot/actions/io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3061 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/job_actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5218 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/job_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6977 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/job_injection.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6254 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/job_queuing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3902 2024-04-15 22:30:11.000000 doot-0.8.0/doot/actions/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5683 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/postbox.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6896 2024-04-15 22:30:11.000000 doot-0.8.0/doot/actions/shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3315 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/speak.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4067 2024-05-31 20:04:24.000000 doot-0.8.0/doot/actions/state.py
+-rw-rw-r--   0 john      (1000) john      (1000)      939 2024-01-20 20:13:07.000000 doot-0.8.0/doot/actions/templater.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1973 2023-12-09 23:29:38.000000 doot-0.8.0/doot/actions/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/cmds/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.8.0/doot/cmds/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/cmds/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     6730 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/__tests/test_list_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2473 2024-04-15 22:30:11.000000 doot-0.8.0/doot/cmds/base_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2146 2024-04-15 22:30:11.000000 doot-0.8.0/doot/cmds/clean_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5141 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/graph_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6016 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/help_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8248 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/list_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2598 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/locs_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4215 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/plugins_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4876 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/run_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3775 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/step_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9365 2024-05-31 20:04:24.000000 doot-0.8.0/doot/cmds/stub_cmd.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/control/
+-rw-rwxr--   0 john      (1000) john      (1000)       10 2023-10-17 22:05:44.000000 doot-0.8.0/doot/control/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/control/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    14043 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/__tests/obsolete.py
+-rw-rw-r--   0 john      (1000) john      (1000)    33705 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/__tests/test_base_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8111 2024-05-04 01:22:58.000000 doot-0.8.0/doot/control/__tests/test_locations.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2887 2024-05-04 01:54:33.000000 doot-0.8.0/doot/control/__tests/test_overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6787 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/__tests/test_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14105 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/__tests/test_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7781 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/base_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    41144 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/base_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8363 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/locations.py
+-rw-rw-r--   0 john      (1000) john      (1000)      172 2023-11-03 03:34:45.000000 doot-0.8.0/doot/control/log.doot
+-rw-rw-r--   0 john      (1000) john      (1000)    11363 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11615 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8582 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/step_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14341 2024-05-31 20:04:24.000000 doot-0.8.0/doot/control/tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7784 2024-05-31 20:04:24.000000 doot-0.8.0/doot/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2904 2024-05-31 20:04:24.000000 doot-0.8.0/doot/errors.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/loaders/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.8.0/doot/loaders/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.738801 doot-0.8.0/doot/loaders/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1851 2024-04-15 22:30:11.000000 doot-0.8.0/doot/loaders/__tests/test_cmd_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1001 2024-04-15 22:30:11.000000 doot-0.8.0/doot/loaders/__tests/test_plugin_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7324 2024-05-31 20:04:24.000000 doot-0.8.0/doot/loaders/__tests/test_task_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2484 2023-12-10 23:41:06.000000 doot-0.8.0/doot/loaders/cmd_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6048 2024-05-12 04:15:19.000000 doot-0.8.0/doot/loaders/plugin_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11806 2024-05-31 20:04:24.000000 doot-0.8.0/doot/loaders/task_loader.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/mixins/
+-rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.8.0/doot/mixins/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2241 2024-05-31 20:04:24.000000 doot-0.8.0/doot/mixins/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1161 2024-04-15 22:30:11.000000 doot-0.8.0/doot/mixins/fail_handler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 22:30:11.000000 doot-0.8.0/doot/mixins/human_numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4557 2024-05-31 20:04:24.000000 doot-0.8.0/doot/mixins/importer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1155 2024-05-31 20:04:24.000000 doot-0.8.0/doot/mixins/param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7321 2024-04-15 22:30:11.000000 doot-0.8.0/doot/mixins/path_manip.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8963 2024-04-15 22:30:11.000000 doot-0.8.0/doot/mixins/zipper.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/parsers/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.8.0/doot/parsers/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/parsers/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    14130 2024-05-31 20:04:24.000000 doot-0.8.0/doot/parsers/__tests/test_flexible.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11270 2024-05-31 20:04:24.000000 doot-0.8.0/doot/parsers/flexible.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/reporters/
+-rw-r-xr--   0 john      (1000) john      (1000)        0 2023-10-05 00:53:38.000000 doot-0.8.0/doot/reporters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/reporters/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     4140 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/__tests/test_stack_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2074 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/__tests/test_summary_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2201 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/base_reporter.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1286 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/basic_reporters.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1585 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/stack_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3134 2024-05-31 20:04:24.000000 doot-0.8.0/doot/reporters/summary_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1175 2024-05-31 20:04:24.000000 doot-0.8.0/doot/structs.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/task/
+-rw-rw-r--   0 john      (1000) john      (1000)       89 2024-01-20 20:13:07.000000 doot-0.8.0/doot/task/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.742801 doot-0.8.0/doot/task/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1516 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/__tests/test_base_job.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4049 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/__tests/test_base_task.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1170 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/__tests/test_check_locs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3669 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/base_job.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8449 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/base_task.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2707 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/base_transformer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2245 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/check_locs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1767 2024-05-31 20:04:24.000000 doot-0.8.0/doot/task/specialised_jobs.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.746801 doot-0.8.0/doot/utils/
+-rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.8.0/doot/utils/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.746801 doot-0.8.0/doot/utils/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     6644 2024-04-17 20:02:24.000000 doot-0.8.0/doot/utils/__tests/test_action_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4368 2024-04-17 20:02:24.000000 doot-0.8.0/doot/utils/action_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1596 2024-04-15 22:30:11.000000 doot-0.8.0/doot/utils/chain_get.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1180 2023-10-17 22:05:44.000000 doot-0.8.0/doot/utils/check_protocol.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9018 2024-05-31 20:04:24.000000 doot-0.8.0/doot/utils/decorators.py
+-rw-rwxr--   0 john      (1000) john      (1000)     4525 2023-10-17 22:05:44.000000 doot-0.8.0/doot/utils/log_colour.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5050 2024-05-31 20:04:24.000000 doot-0.8.0/doot/utils/log_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-02-23 23:43:30.000000 doot-0.8.0/doot/utils/log_context.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4654 2024-05-31 20:04:24.000000 doot-0.8.0/doot/utils/mock_gen.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2530 2024-05-31 20:04:24.000000 doot-0.8.0/doot/utils/plugin_selector.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1841 2024-04-15 22:30:11.000000 doot-0.8.0/doot/utils/retrievers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1909 2024-02-23 23:43:30.000000 doot-0.8.0/doot/utils/signal_handler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1350 2024-04-15 22:30:11.000000 doot-0.8.0/doot/utils/testing_fixtures.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1787 2024-04-15 20:38:01.000000 doot-0.8.0/doot/utils/trace_helper.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1363 2023-10-17 22:05:44.000000 doot-0.8.0/doot/utils/url_expand.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:27:47.746801 doot-0.8.0/doot.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)    10281 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     4872 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       44 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      213 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        5 2024-05-31 20:27:47.000000 doot-0.8.0/doot.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     4259 2024-05-31 20:26:53.000000 doot-0.8.0/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-05-31 20:27:47.746801 doot-0.8.0/setup.cfg
```

### Comparing `doot-0.7.2/LICENSE` & `doot-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/PKG-INFO` & `doot-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.2
+Version: 0.8.0
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -57,25 +57,27 @@
 Requires-Dist: stackprinter>=0.2.10
 Requires-Dist: matplotlib
 Requires-Dist: sty
 Requires-Dist: boltons
 Requires-Dist: more_itertools
 Requires-Dist: decorator-validation>=3.0.0
 Requires-Dist: decorator>=5.0.0
-Requires-Dist: jgdv
+Requires-Dist: pydantic
+Requires-Dist: jgdv>=0.1.3
 Provides-Extra: test
 Requires-Dist: pytest<5.0.0; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
+<!-- <!--  README.md -*- mode: GFM -*-
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.2  
+Version : 0.8.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
@@ -97,23 +99,23 @@
 
 eg:
 ``` toml
 # -*- mode:conf-toml; -*-
 [settings.general]
 notify                   = { say-on-exit = false }
 loaders                  = { commands="default", task="default", parser="default"}
-location_check           = { make_missing = true, print_levels={action="WARN", execute="WARN" } }
+location_check           = { make_missing = true }
 
 [settings.tasks]
 sources = [".tasks"] # Files or directories where task specs can be loaded from, expanded according to [[locations]] keys
 code    = []         # Directories where task specific code can be imported from, expanded according to [[locations]] keys
 sleep   = { task=0.2, subtask=1, batch=1 }
 
 [logging]
-stream  = { level="WARN",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
+stream  = { level="WARNING",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
 file    = { level="DEBUG", allow=["doot"], format="{levelname:<8} : {message:<20} :|: (module:{module} line:{lineno} fn:{funcName})" }
 printer = { level="INFO", colour=true}
 
 [plugins]
 # Allows for defining shorthands
 command        = { other-run = "doot.cmds.run_cmd:RunCmd", tasks = "doot.cmds.list_cmd:ListCmd" }
 report-line    = {}
@@ -137,16 +139,16 @@
 
 ``` toml
 [[tasks.mygroup]] # mygroup is the group this task is part of
 name                 = "mytask" # combined together, this means this specific task is `mygroup::mytask`
 version              = "0.1"    # <str>
 ctor                 = "task"   # <type> the python class this task uses. See the plugins listed in 'doot plugins'
 doc                  = ["Text to help understand what this task does"] # <list[str]>
-required_for         = []                   # <list[DootTaskArtifact]> see below
-depends_on           = []                   # <list[DootTaskArtifact]> see below
+required_for         = []                   # <list[TaskArtifact]> see below
+depends_on           = []                   # <list[TaskArtifact]> see below
 actions              = []                   # <list[Any]> See below
 ```
 
 You can see what tasks are available by calling `doot list`.
 You can get help on a specific task by calling `doot {task} --help` or `doot help {task}`.
 You can run a task by calling `doot {task}` or `doot run {task}`.
 eg: `doot mygroup::mytask`
@@ -166,15 +168,15 @@
 - Action write! : doot.actions.io:WriteAction
 -- Declared kwargs for action: ['from_', 'to']
 
 -- Toml Form:
 { do="write!", args=[] }
 
 - For Custom Python Actions, implement the following in the .tasks director
-def custom_action(spec:DootActionSpec, task_state:dict) -> None|bool|dict:...
+def custom_action(spec:ActionSpec, task_state:dict) -> None|bool|dict:...
 ```
 
 When specifying values in toml you can use direct keys, or indirect keys.
 For example, the action:
 ``` toml
 { do="log", msg="This is a test", level="INFO" }
 ```
```

### Comparing `doot-0.7.2/README.md` & `doot-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+<!-- <!--  README.md -*- mode: GFM -*-
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.2  
+Version : 0.8.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
@@ -26,23 +27,23 @@
 
 eg:
 ``` toml
 # -*- mode:conf-toml; -*-
 [settings.general]
 notify                   = { say-on-exit = false }
 loaders                  = { commands="default", task="default", parser="default"}
-location_check           = { make_missing = true, print_levels={action="WARN", execute="WARN" } }
+location_check           = { make_missing = true }
 
 [settings.tasks]
 sources = [".tasks"] # Files or directories where task specs can be loaded from, expanded according to [[locations]] keys
 code    = []         # Directories where task specific code can be imported from, expanded according to [[locations]] keys
 sleep   = { task=0.2, subtask=1, batch=1 }
 
 [logging]
-stream  = { level="WARN",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
+stream  = { level="WARNING",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
 file    = { level="DEBUG", allow=["doot"], format="{levelname:<8} : {message:<20} :|: (module:{module} line:{lineno} fn:{funcName})" }
 printer = { level="INFO", colour=true}
 
 [plugins]
 # Allows for defining shorthands
 command        = { other-run = "doot.cmds.run_cmd:RunCmd", tasks = "doot.cmds.list_cmd:ListCmd" }
 report-line    = {}
@@ -66,16 +67,16 @@
 
 ``` toml
 [[tasks.mygroup]] # mygroup is the group this task is part of
 name                 = "mytask" # combined together, this means this specific task is `mygroup::mytask`
 version              = "0.1"    # <str>
 ctor                 = "task"   # <type> the python class this task uses. See the plugins listed in 'doot plugins'
 doc                  = ["Text to help understand what this task does"] # <list[str]>
-required_for         = []                   # <list[DootTaskArtifact]> see below
-depends_on           = []                   # <list[DootTaskArtifact]> see below
+required_for         = []                   # <list[TaskArtifact]> see below
+depends_on           = []                   # <list[TaskArtifact]> see below
 actions              = []                   # <list[Any]> See below
 ```
 
 You can see what tasks are available by calling `doot list`.
 You can get help on a specific task by calling `doot {task} --help` or `doot help {task}`.
 You can run a task by calling `doot {task}` or `doot run {task}`.
 eg: `doot mygroup::mytask`
@@ -95,15 +96,15 @@
 - Action write! : doot.actions.io:WriteAction
 -- Declared kwargs for action: ['from_', 'to']
 
 -- Toml Form:
 { do="write!", args=[] }
 
 - For Custom Python Actions, implement the following in the .tasks director
-def custom_action(spec:DootActionSpec, task_state:dict) -> None|bool|dict:...
+def custom_action(spec:ActionSpec, task_state:dict) -> None|bool|dict:...
 ```
 
 When specifying values in toml you can use direct keys, or indirect keys.
 For example, the action:
 ``` toml
 { do="log", msg="This is a test", level="INFO" }
 ```
```

### Comparing `doot-0.7.2/doot/__data/aliases.toml` & `doot-0.8.0/doot/__data/aliases.toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/__init__.py` & `doot-0.8.0/doot/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 #!/usr/bin/env python3
 """
 Doot : An Opinionated refactor of the Doit Task Runner.
 
 """
-##-- std imports
+
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
 import pathlib as pl
-from typing import Final, Any, assert_type
-from importlib.resources import files
 import sys
-##-- end std imports
+from collections import defaultdict
+from importlib.resources import files
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, assert_type, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-##-- imports
+# ##-- end stdlib imports
+
+# ##-- 3rd party imports
 import tomlguard as TG
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot.errors
 from doot.utils.check_protocol import check_protocol
-##-- end imports
+
+# ##-- end 1st party imports
 
 ##-- data
 data_path      = files("doot.__data")
 constants_file = data_path.joinpath("constants.toml")
 aliases_file   = data_path.joinpath("aliases.toml")
 ##-- end data
 
 ##-- logging
 logging         = logmod.getLogger(__name__)
 printer         = logmod.getLogger("doot._printer")
+setup_l         = printer.getChild("setup")
+fail_l          = printer.getChild("fail")
 ##-- end logging
 
+__all__ = []
+
 # Global, single points of truth:
-__version__          : Final[str]         = "0.7.2"
+__version__          : Final[str]         = "0.8.0"
 
+# Can't be in doot.constants, because that isn't loaded yet
 CONSTANT_PREFIX      : Final[str]         = "doot.constants"
 ALIAS_PREFIX         : Final[str]         = "doot.aliases"
 TOOL_PREFIX          : Final[str]         = "tool.doot"
 
 config               : TG.TomlGuard       = TG.TomlGuard() # doot config
 constants            : TG.TomlGuard       = TG.TomlGuard.load(constants_file).remove_prefix(CONSTANT_PREFIX)
 aliases              : TG.TomlGuard       = TG.TomlGuard()
 locs                 : DootLocData        = None # DootLocations(pl.Path()) # registered locations
 args                 : TG.TomlGuard       = TG.TomlGuard() # parsed arg access
-report               : Reporter_i         = None
+report               : Reporter_p         = None
 
 _configs_loaded_from : list[pl.Path]      = []
 
 def setup(targets:list[pl.Path]|False|None=None, prefix:str|None=TOOL_PREFIX) -> tuple[TG.TomlGuard, DootLocData]:
     """
       The core requirement to call before any other doot code is run.
       loads the config files, so everything else can retrieve values when imported.
@@ -65,47 +88,49 @@
         case list() if bool(targets):
             raise TypeError("Doot Config Targets should be pathlib.Path's", targets)
         case _:
             targets : list[pl.Path] = [pl.Path(x) for x in constants.paths.DEFAULT_LOAD_TARGETS]
 
     logging.debug("Loading Doot Config, version: %s targets: %s", __version__, targets)
     if bool(config):
-        printer.warning("doot.setup called even though doot is already set up")
+        setup_l.warning("doot.setup called even though doot is already set up")
 
     if bool(targets) and not any([x.exists() for x in targets]):
         raise doot.errors.DootMissingConfigError("No Doot data found")
 
     existing_targets       = [x for x in targets if x.exists()]
 
     try:
         config = TG.load(*existing_targets)
-    except OSError:
-        logging.error("Failed to Load Config Files: %s", existing_targets)
-        raise doot.errors.DootError()
+    except OSError as err:
+        fail_l.error("Failed to Load Config Files: %s", existing_targets)
+        raise doot.errors.DootError() from err
 
     config = config.remove_prefix(prefix)
     _load_constants()
     _load_aliases()
     _load_locations()
     _update_import_path()
 
     _configs_loaded_from   = existing_targets
 
     return config, locs
 
 def _load_constants():
     """ Load the override constants if the loaded base config specifies one"""
     global constants
+    setup_l.debug("Loading Constants")
     update_file = config.on_fail(None).settings.general.constants_file()
     if update_file:
         constants = TG.TomlGuard.load(pl.Path(update_file)).remove_prefix(CONSTANT_PREFIX)
 
 def _load_aliases():
     """ Load plugin aliases """
     global aliases
+    setup_l.debug("Loading Aliases")
     update_file = config.on_fail(aliases_file).settings.general.aliases_file()
     data        = TG.TomlGuard.load(pl.Path(update_file)).remove_prefix(ALIAS_PREFIX)
     # Flatten the lists
     flat = {}
     for key,val in data:
         flat[key] = {k:v for x in val for k,v in x.items()}
 
@@ -114,33 +139,51 @@
         flat[key].update(dict(val))
 
     aliases = TG.TomlGuard(flat)
 
 def _load_locations():
     """ Load and update the DootLocations db """
     global locs
+    setup_l.debug("Loading Locations")
+    # ##-- 1st party imports
     from doot.control.locations import DootLocations
+
+    # ##-- end 1st party imports
     locs   = DootLocations(pl.Path.cwd())
     # Load Initial locations
     for loc in config.on_fail([]).locations():
         locs.update(loc)
 
 def _update_import_path():
     """ Add locations to the python path for task local code importing  """
+    setup_l.debug("Updating Import Path")
     task_sources = config.on_fail([locs[".tasks"]], list).settings.tasks.sources(wrapper=lambda x: [locs[y] for y in x])
     task_code    = config.on_fail([locs[".tasks"]], list).settings.tasks.code(wrapper=lambda x: [locs[y] for y in x])
     for source in set(task_sources + task_code):
         if source.exists() and source.is_dir():
-            logging.debug("Adding task code directory to Import Path: %s", source)
+            setup_l.debug("Adding task code directory to Import Path: %s", source)
             sys.path.append(str(source))
 
+def _update_aliases(data:dict|TG.TomlGuard):
+    global aliases
+    if not bool(data):
+        return
+
+    setup_l.debug("Updating Aliases")
+    base = defaultdict(dict)
+    base.update(dict(aliases._table()))
+    for key,eps in data.items():
+        update = {x.name:x.value for x in eps}
+        base[key].update(update)
 
+    aliases = TG.TomlGuard(base)
 
 def _test_setup():
     """
-      Doesn't load anything but constants, for testing
+      Doesn't load anything but constants,
+      Used for initialising Doot when testing.
     """
     global config, _configs_loaded_from, locs
     config               = TG.TomlGuard()
     _configs_loaded_from = []
     locs                 = None
     setup(False)
```

### Comparing `doot-0.7.2/doot/__main__.py` & `doot-0.8.0/doot/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,120 @@
 #!/usr/bin/env python3
 """
 Alternative doot cli runner, to use the doot loader
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
 import abc
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
 import pathlib
 import pathlib as pl
 import sys
+from bdb import BdbQuit
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
+from importlib.resources import files
 from re import Pattern
 from sys import stderr, stdout
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
-##-- end imports
 
-logging         = logmod.root
-printer         = logmod.getLogger("doot._printer")
+# ##-- end stdlib imports
 
-from importlib.resources import files
+# ##-- 3rd party imports
 import sh
 import stackprinter
 import tomlguard as TG
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
-from bdb import BdbQuit
 from doot.utils.log_config import DootLogConfig
 
+# ##-- end 1st party imports
+
+##-- logging
+logging         = logmod.root
+printer         = logmod.getLogger("doot._printer")
+shutdown_l      = printer.getChild("shutdown")
+fail_l          = printer.getChild("fail")
+##-- end logging
+
 template_path      = files("doot.__templates")
 
 def main():
     result  = 1
     overlord = None
     try:
         log_config = DootLogConfig()
         # --- Setup
         if not bool(doot.config):
             doot.setup()
 
         log_config.setup()
 
-        logging.info("Called with: %s", sys.argv)
-        from doot.loaders.plugin_loader import DootPluginLoader
+        logging.info("Doot Calling Args: %s", sys.argv)
+        # ##-- 1st party imports
         from doot.control.overlord import DootOverlord
+        from doot.loaders.plugin_loader import DootPluginLoader
+
+        # ##-- end 1st party imports
         overlord  = DootOverlord(loaders={"plugin": DootPluginLoader().setup(sys.argv[:]) },
                                  config_filenames=[doot.constants.paths.DEFAULT_LOAD_TARGETS],
                                  log_config=log_config,
                                  args=sys.argv[:])
 
         # --- Do whatever thats been triggered
         result    = overlord()
 
     ##-- handle doot errors
     except (doot.errors.DootEarlyExit, BdbQuit):
-        printer.warning("Early Exit Triggered")
+        shutdown.warning("Early Exit Triggered")
         result = 0
     except doot.errors.DootMissingConfigError as err:
         result = 0
         # Handle missing files
         if pl.Path(doot.constants.on_fail(["doesntexist"]).paths.DEFAULT_LOAD_TARGETS()[0]).exists():
             pass
         elif input("No toml config data found, create stub doot.toml? _/n ") != "n":
             template = template_path.joinpath(doot.constants.paths.TOML_TEMPLATE)
             target = pl.Path(doot.constants.on_fail(["doot.toml"]).paths.DEFAULT_LOAD_TARGETS()[0])
             target.write_text(template.read_text())
-            logging.info("Stubbed")
+            shutdown.info("Doot Config File Stubbed: %s", target)
     except doot.errors.DootTaskError as err:
-        printer.error("%s : %s", err.general_msg, err.task_name)
-        printer.error("---- Source: %s", err.task_source)
-        printer.error("---- %s", str(err))
+        fail_prefix = doot.constants.printer.fail_prefix
+        fail_l.error("%s %s : %s", fail_prefix, err.general_msg, err.task_name)
+        fail_l.error("%s Source: %s", fail_prefix, err.task_source)
+        fail_l.error("%s %s", fail_prefix, str(err))
     except doot.errors.DootError as err:
-        printer.error("%s", err.general_msg)
-        printer.error("---- %s", str(err))
+        fail_prefix = doot.constants.printer.fail_prefix
+        fail_l.error("%s", err.general_msg)
+        fail_l.error("---- %s", str(err))
     ##-- end handle doot errors
     ##-- handle todo errors
     except NotImplementedError as err:
         logging.error(stackprinter.format())
-        printer.error("Not Implemented: %s", err)
+        fail_l.error("Not Implemented: %s", err)
     ##-- end handle todo errors
     ##-- handle general errors
     except Exception as err:
         logging.error(stackprinter.format())
-        # logging.error("Python Error: %s", err)
+        fail_l.error("Python Error: %s", err)
     ##-- end handle general errors
     finally: # --- final shutdown
         if overlord:
             overlord.shutdown()
 
         sys.exit(result)
```

### Comparing `doot-0.7.2/doot/__templates/stub_task_py` & `doot-0.8.0/doot/__templates/stub_task_py`

 * *Files 9% similar despite different names*

```diff
@@ -39,26 +39,26 @@
 
 printer = logmod.getLogger("doot._printer")
 
 import doot
 import doot.errors
 from doot.mixins.task.human_numbers import Human_M
 from doot.task.base_task import DootTask
-from doot.structs import DootActionSpec
+from doot.structs import ActionSpec
 
 class SimpleTaskExample(Human_M, DootTask):
     """
       A Simple example task that uses a mixin, and adds its own default actions
     """
 
     def __init__(self, spec, *, job=None, action_ctor=None, **kwargs):
         super().__init__(spec, job=job, **kwargs)
         self._extra_actions = []
-        self._extra_actions.append(DootActionSpec(do="custom head", fun=self._head))
-        self._extra_actions.append(DootActionSpec(do="custom tail", fun=self._tail))
+        self._extra_actions.append(ActionSpec(do="custom head", fun=self._head))
+        self._extra_actions.append(ActionSpec(do="custom tail", fun=self._tail))
 
     @property
     def actions(self):
         """ yield spec actions, plus a head and tail """
         yield self._extra_actions[0]
         yield from iter(self.spec.actions)
         yield self._extra_actions[1]
```

### Comparing `doot-0.7.2/doot/__tests/test_basic.py` & `doot-0.8.0/doot/__tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/__tests/test_inits.py` & `doot-0.8.0/doot/__tests/test_inits.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/_abstract/__init__.py` & `doot-0.8.0/doot/_abstract/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .loader import CommandLoader_p, PluginLoader_p, TaskLoader_p
 from .overlord import Overlord_p
 from .cmd import Command_i
 from .task import Action_p, Task_i, Job_i
 
 from .dbm import DBManager_p
 from .parser import ArgParser_i
-from .reporter import Reporter_i, ReportLine_i
+from .reporter import Reporter_p, ReportLine_p
 from .policy import FailPolicy_p
```

### Comparing `doot-0.7.2/doot/_abstract/cmd.py` & `doot-0.8.0/doot/_abstract/cmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import textwrap
 from typing import TYPE_CHECKING
 ##-- end imports
 
 from abc import abstractmethod
 from tomlguard import TomlGuard
 
-from doot._abstract.structs import ParamStruct_p
+from doot._abstract.protocols import ParamStruct_p
 
 class Command_i:
     """
     holds command information and performs it
     """
 
     _name : None|str       = None # if not specified uses the class name
```

### Comparing `doot-0.7.2/doot/_abstract/control.py` & `doot-0.8.0/doot/_abstract/control.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,74 +30,78 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from abc import abstractmethod
 from typing import Generator, NewType
 from collections import deque, defaultdict
 
-from doot.enums import TaskStateEnum
+from doot.enums import TaskStatus_e, ExecutionPolicy_e
 
-from doot._abstract.reporter import ReportLine_i, Reporter_i
+from doot._abstract.reporter import Reporter_p
 from doot._abstract.policy import FailPolicy_p
 from doot._abstract.task import Task_i
-from doot._abstract.structs import ArtifactStruct_p, SpecStruct_p
+from doot._abstract.protocols import ArtifactStruct_p, SpecStruct_p
+
+# ## Types
+AbstractId                     : TypeAlias                   = "TaskName|TaskArtifact"
+ConcreteId                     : TypeAlias                   = "TaskName|TaskArtifact"
+AnyId                          : TypeAlis                    = "TaskName|TaskArtifact"
+AbstractSpec                   : TypeAlias                   = "TaskSpec"
+ConcreteSpec                   : TypeAlias                   = "TaskSpec"
+AnySpec                        : TypeAlias                   = "TaskSpec"
+Depth                          : TypeAlias                   = int
+PlanEntry                      : TypeAlias                   = tuple[Depth, ConcreteId, str]
 
 class TaskTracker_i:
     """
     Track tasks that have run, need to run, are running,
     and have failed.
     Does not execute anything itself
     """
-    state_e : TypeAlias = TaskStateEnum
-
-    @abstractmethod
-    def __bool__(self) -> bool:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def __len__(self) -> int:
-        raise NotImplementedError()
 
     @abstractmethod
-    def __iter__(self) -> Generator:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def __contains__(self, target:str) -> bool:
-        raise NotImplementedError()
+    def register_spec(self, *specs:AnySpec)-> None:
+        pass
 
     @abstractmethod
-    def add_task(self, task:SpecStruct_p|Task_i):
-        raise NotImplementedError()
+    def queue_entry(self, name:str|AnyId|ConcreteSpec|Task_i, *, from_user:bool=False, status:None|TaskStatus_e=None) -> None|Node:
+        pass
 
     @abstractmethod
-    def queue_task(self, task:str) -> None:
-        raise NotImplementedError()
+    def get_status(self, task:ConcreteId) -> TaskStatus_e:
+        pass
 
     @abstractmethod
-    def update_state(self, task:str|DootTaskName|SpecStruct_p|Task_i|ArtifactStruct_p, state:TaskStateEnum) -> None:
-        raise notimplementederror()
+    def set_status(self, task:ConcreteId|Task_i, state:TaskStatus_e) -> bool:
+        pass
 
     @abstractmethod
-    def next_for(self, target:str) -> Task_i|ArtifactStruct_p|None:
-        raise NotImplementedError()
+    def next_for(self, target:None|str|ConcreteId=None) -> None|Task_i|"TaskArtifact":
+        pass
 
     @abstractmethod
-    def declared_set(self) -> set[str]:
-        raise NotImplementedError()
+    def build_network(self) -> None:
+        pass
 
     @abstractmethod
-    def defined_set(self) -> set[str]:
-        raise NotImplementedError()
+    def generate_plan(self, *, policy:None|ExecutionPolicy_e=None) -> list[PlanEntry]:
+        pass
 
 class TaskRunner_i:
     """
     Run tasks, actions, and jobs
     """
+    @abstractmethod
+    def __enter__(self) -> Any:
+        pass
 
     @abstractmethod
-    def __init__(self, *, tracker:TaskTracker_i, reporter:Reporter_i, policy:FailPolicy_p|None=None):
+    def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
+        pass
+
+    @abstractmethod
+    def __init__(self, *, tracker:TaskTracker_i, reporter:Reporter_p, policy:FailPolicy_p|None=None):
         pass
 
     @abstractmethod
     def __call__(self, *tasks:str) -> bool:
-        raise NotImplementedError()
+        pass
```

### Comparing `doot-0.7.2/doot/_abstract/dbm.py` & `doot-0.8.0/doot/_abstract/dbm.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/_abstract/loader.py` & `doot-0.8.0/doot/_abstract/loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/_abstract/overlord.py` & `doot-0.8.0/doot/_abstract/overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/_abstract/parser.py` & `doot-0.8.0/doot/_structs/trace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 #!/usr/bin/env python3
 """
 
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
-import types
-import abc
+# import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
-from copy import deepcopy
+import types
+import weakref
+# from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+                    cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
-from weakref import ref
 
-##-- end imports
+##-- end builtin imports
+
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from abc import abstractmethod
+from pydantic import BaseModel, Field, model_validator, field_validator
+import importlib
 from tomlguard import TomlGuard
+import doot.errors
+from doot.enums import TaskFlags, ReportEnum
+
+
+class TraceRecord(BaseModel):
+    message : str
+    flags   : ReportEnum
+    args    : list[Any]                = []
+    time    : datetime.datetime        = Field(default_factory=datetime.datetime.now)
+
+    @field_validator("flags", mode="before")
+    def _valdiate_flags(cls, val):
+        match val:
+            case None:
+                return ReportEnum.default
+            case str() | list():
+                return ReportEnum.build(val)
+            case ReportEnum():
+                return val
+            case _:
+                raise ValueError("Bad flags for TraceRecord", val)
+
+
+    def __str__(self):
+        match self.message:
+            case str():
+                return self.message.format(*self.args)
+            case TaskSpec():
+                return str(self.message.name)
+            case _:
+                return str(self.message)
+
+    def __contains__(self, other:ReportEnum) -> bool:
+        return all([x in self.flags for x in other])
 
-from doot._abstract.structs import ParamStruct_p
+    def __eq__(self, other:ReportEnum) -> bool:
+        return self.flags == other
 
-@dataclass
-class _RegexEqual(str):
-    """ https://martinheinz.dev/blog/78 """
-    string : str
-    match :  re.Match = None
-
-    def __eq__(self, pattern):
-        self.match = re.search(pattern, self.string)
-        return self.match is not None
-
-    def __getitem__(self, group):
-        return self.match[group]
-
-class ArgParser_i:
-    """
-    A Single standard process point for turning the list of passed in args,
-    into a dict, into a tomlguard,
-    along the way it determines the cmds and tasks that have been chosne
-    """
-
-    def __init__(self):
-        self.specs = []
-
-    def add_param_specs(self, specs:list):
-        self.specs += specs
-
-    @abstractmethod
-    def parse(self, args:list[str], doot_arg_specs:list[ParamStruct_p], cmds:TomlGuard, tasks:TomlGuard) -> TomlGuard:
-        raise NotImplementedError()
+    def some(self, other:reportPositionEnum) -> bool:
+        return any([x in self.flags for x in other])
```

### Comparing `doot-0.7.2/doot/_abstract/policy.py` & `doot-0.8.0/doot/_abstract/policy.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/_abstract/reporter.py` & `doot-0.8.0/doot/_abstract/reporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,35 +28,34 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from tomlguard import TomlGuard
 from doot.enums import ReportEnum
-from doot._structs.trace import DootTraceRecord
 
-class Reporter_i:
+class Reporter_p(abc.ABC):
     """
-      Holds ReportLine_i's, and stores DootTraceRecords
+      Holds ReportLine_i's, and stores TraceRecords
     """
 
-    def __init__(self, reporters:list[ReportLine_i]=None):
-        self._full_trace     : list[DootTraceRecord]       = []
-        self._reporters      : list[ReportLine_i] = list(reporters or [self._default_formatter])
-
-    def _default_formatter(self, trace:DootTraceRecord) -> str:
-        return str(trace)
-
-    def __str__(self):
-        raise NotImplementedError()
+    @abc.abstractmethod
+    def __init__(self, reporters:list[ReportLine_p]=None):
+        pass
+
+    @abc.abstractmethod
+    def _default_formatter(self, trace:"TraceRecord") -> str:
+        pass
 
+    @abc.abstractmethod
     def add_trace(self, msg, *args, flags=None):
-        self._full_trace.append(DootTraceRecord(msg, flags, args))
+        pass
 
 
-class ReportLine_i:
+class ReportLine_p(abc.ABC):
     """
     Reporters, like loggers, are stacked, and each takes the flags and data and maybe runs.
     """
 
-    def __call__(self, trace:DootTraceRecord) -> None|str:
-        raise NotImplementedError(self.__class__, "call")
+    @abc.abstractmethod
+    def __call__(self, trace:"TraceRecord") -> None|str:
+        pass
```

### Comparing `doot-0.7.2/doot/_abstract/structs.py` & `doot-0.8.0/doot/utils/testing_fixtures.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 """
-
-
-See EOF for license/metadata/notes as applicable
+Pytest testing fixtures
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
-import abc
+# import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
@@ -25,37 +23,34 @@
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
-##-- lib imports
-# import more_itertools as mitz
-# from boltons import
-##-- end lib imports
-
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import tomlguard
-
-class SpecStruct_p(abc.ABC):
-    """ Base class for specs, for type matching """
-
-    @property
-    @abc.abstractmethod
-    def params(self) -> dict|tomlguard.TomlGuard:
-        pass
-
-class ArtifactStruct_p(abc.ABC):
-    """ Base class for artifacts, for type matching """
-    pass
-
-class StubStruct_p(abc.ABC):
-    """ Base class for stubs, for type matching """
-    pass
-
-class ParamStruct_p(abc.ABC):
-    """ Base class for param specs, for type matching """
-    pass
+import pytest
+import os
+import doot
+
+@pytest.fixture
+def wrap_tmp(tmp_path):
+    """ create a new temp directory, and change cwd to it,
+      returning to original cwd after the test
+      """
+    logging.debug("Moving to temp dir")
+    orig     = pl.Path().cwd()
+    new_base = tmp_path / "test_root"
+    new_base.mkdir()
+    with doot.locs(new_base):
+        yield new_base
+    logging.debug("Returning to original dir")
+
+
+@pytest.fixture
+def wrap_locs():
+    logging.debug("Activating temp locs")
+    with doot.locs() as temp:
+        yield temp
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_action_spec.py` & `doot-0.8.0/doot/_structs/__tests/test_action_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,44 +13,40 @@
 
 import pytest
 logging = logmod.root
 
 import tomlguard
 import doot
 doot._test_setup()
-from doot import structs
+from doot._structs.action_spec import ActionSpec
 
 class TestActionSpec:
 
     def test_initial(self):
-        obj = structs.DootActionSpec()
-        assert(isinstance(obj, structs.DootActionSpec))
-
+        obj = ActionSpec()
+        assert(isinstance(obj, ActionSpec))
 
     def test_build_from_dict(self):
-        obj = structs.DootActionSpec.build({"do":"test"})
-        assert(isinstance(obj, structs.DootActionSpec))
-        assert(obj.do == "test")
-
+        obj = ActionSpec.build({"do":"basic"})
+        assert(isinstance(obj, ActionSpec))
+        assert(str(obj.do) == doot.aliases.action['basic'])
 
     def test_build_from_list(self):
-        obj = structs.DootActionSpec.build({"do":"test"})
-        assert(isinstance(obj, structs.DootActionSpec))
-        assert(obj.do == "test")
-
+        obj = ActionSpec.build({"do":"basic"})
+        assert(isinstance(obj, ActionSpec))
+        assert(str(obj.do) == doot.aliases.action['basic'])
 
     def test_build_nop(self):
-        obj = structs.DootActionSpec.build([])
-        obj2 = structs.DootActionSpec.build(obj)
+        obj = ActionSpec.build([])
+        obj2 = ActionSpec.build(obj)
         assert(obj is obj2)
 
-
     def test_call(self, mocker):
         fun_mock = mocker.Mock()
-        obj = structs.DootActionSpec(fun=fun_mock)
+        obj = ActionSpec(fun=fun_mock)
 
         obj({})
         fun_mock.assert_called_once()
 
-
+    @pytest.mark.xfail
     def test_set_function(self):
-        pass
+        raise NotImplementedError()
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_formatter.py` & `doot-0.8.0/doot/_structs/__tests/test_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,73 +27,73 @@
 
 ##-- end pytest reminder
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 
-from doot.structs import DootActionSpec
+from doot.structs import ActionSpec
 from doot._structs.key import DootFormatter
 
 class TestDootFormatter:
 
     @pytest.fixture(scope="function")
     def setup_locs(self, mocker):
         new_locs = TomlGuard({"p1": "test1", "p2": "test2/sub"})
         return mocker.patch.object(doot.locs, "_data", new_locs)
 
     def test_initial(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=ActionSpec)
         result = fmt.format("{a}", _spec=spec, _state={})
         assert(result == "blah")
 
     def test_missing(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=ActionSpec)
         result = fmt.format("{b}", _spec=spec, _state={})
         assert(result == "{b}")
 
 
     def test_multi(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=ActionSpec)
         state = {"b": "aweg"}
         result = fmt.format("{a}:{b}", _spec=spec, _state=state)
         assert(result == "blah:aweg")
 
 
     def test_indirect(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=ActionSpec)
         state = {"b": "aweg"}
         result = fmt.format("{a}", _spec=spec, _state=state)
         assert(result == "blah")
 
 
     def test_recursive(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=ActionSpec)
         state = {"b": "aweg {c}", "c": "blah"}
         result = fmt.format("{a}", _spec=spec, _state=state, _rec=True)
         assert(result == "this is a aweg blah")
 
 
     def test_recursive_missing(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=ActionSpec)
         state = {"b": "aweg {c}", "c": "blah {d}"}
         result = fmt.format("{a}", _spec=spec, _state=state, _rec=True)
         assert(result == "this is a aweg blah {d}")
 
 
     @pytest.mark.xfail
     def test_not_str_fails(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=ActionSpec)
         state = {"b": "aweg {c}", "c": [1,2,3]}
         with pytest.raises(TypeError):
             fmt.format("{a}", _spec=spec, _state=state, _rec=True)
 
 
     def test_empty_format(self):
         fmt = DootFormatter()
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key.py` & `doot-0.8.0/doot/_structs/__tests/test_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 logging = logmod.root
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
 
@@ -68,15 +68,15 @@
         assert(isinstance(obj, DootKey))
         assert(isinstance(obj, dkey.DootMultiKey))
 
 class TestSimpleGet:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo", "a": 2}))
+        return ActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo", "a": 2}))
 
     def test_initial(self, spec):
         key = DootKey.build("z_")
         result = key.basic(spec, {})
         assert(str(key) == "z_")
         assert(result == "bloo")
 
@@ -138,147 +138,147 @@
         assert(name.endswith("_"))
         obj = dkey.DootSimpleKey(name)
         assert(not obj.indirect.endswith("__"))
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_redirect(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{name}_": "blah"}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{name}_": "blah"}, spec=ActionSpec)
         assert(obj.indirect in spec.params)
         result        = obj.redirect(spec)
         assert(isinstance(result, DootKey))
         assert(result == "blah")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_redirect_to_list_fail(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{name}_": ["blah", "bloo"]}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{name}_": ["blah", "bloo"]}, spec=ActionSpec)
         assert(obj.indirect in spec.params)
         with pytest.raises(TypeError):
             result        = obj.redirect(spec)
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{name}_": ["blah", "bloo"]}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{name}_": ["blah", "bloo"]}, spec=ActionSpec)
         assert(obj.indirect in spec.params)
         result        = obj.redirect_multi(spec)
         assert(isinstance(result, list))
         assert(all((isinstance(x, DootKey) for x in result)))
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_expand_from_spec(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{obj}": "blah"}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{obj}": "blah"}, spec=ActionSpec)
         result        = obj.expand(spec, {})
         assert(result == "blah")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_expand_from_state(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {f"{obj}": "blah"}
         result        = obj.expand(spec, state)
         assert(result == "blah")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_expansion_prefers_spec_over_state(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{obj}": "bloo"}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{obj}": "bloo"}, spec=ActionSpec)
         state         = {f"{obj}": "blah"}
         result        = obj.expand(spec, state)
         assert(result == "bloo")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_expansion_prefers_redirect_over_other(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={"aweg": "bloo", obj.indirect : "aweg"}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={"aweg": "bloo", obj.indirect : "aweg"}, spec=ActionSpec)
         state         = {f"{obj}": "blah"}
         result        = obj.expand(spec, state)
         assert(result == "bloo")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_expansion_of_missing_returns_form(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {}
         result        = obj.expand(spec, state)
         assert(result == obj.form)
 
     @pytest.mark.parametrize("name", KEY_BASES)
     def test_recursive_expansion(self, mocker, name):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={f"{name}": dkey.DootSimpleKey("key1")}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={f"{name}": dkey.DootSimpleKey("key1")}, spec=ActionSpec)
         state         = {"key1": dkey.DootSimpleKey("key2"), "key2": "aweg"}
         result        = obj.expand(spec, state)
         assert(result == "aweg")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     @pytest.mark.parametrize("value,type", [([1,2,3], list)])
     def test_expansion_flattening(self, mocker, name, value, type):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {name: value}
         result        = obj.expand(spec, state)
         assert(isinstance(result, str))
         assert(result == str(value))
 
     @pytest.mark.parametrize("name", KEY_BASES)
     @pytest.mark.parametrize("value,type", [([1,2,3], list)])
     def test_to_type_expansion(self, mocker, name, value, type):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {name: value}
         result        = obj.to_type(spec, state)
         assert(isinstance(result, type))
         assert(result == value)
 
     @pytest.mark.parametrize("name", KEY_BASES)
     @pytest.mark.parametrize("value,type", [([1,2,3], list)])
     def test_to_type_on_fail(self, mocker, name, value, type):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {}
         result        = obj.to_type(spec, state, on_fail="blah")
         # assert(isinstance(result, type))
         assert(result == "blah")
 
     @pytest.mark.parametrize("name", KEY_BASES)
     @pytest.mark.parametrize("value,type", [([1,2,3], list)])
     def test_to_type_on_fail_nop(self, mocker, name, value, type):
         obj           = dkey.DootSimpleKey(name)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {name : value}
         result        = obj.to_type(spec, state, on_fail="blah")
         # assert(isinstance(result, type))
         assert(result == value)
 
     @pytest.mark.parametrize("key,target", [("blah", "./doot")])
     def test_to_path_expansion(self, mocker, key, target):
         mocker.patch.dict("doot.__dict__", locs=TEST_LOCS)
         obj           = DootKey.build(key)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {}
         result        = obj.to_path(spec, state)
         assert(isinstance(result, pl.Path))
         assert(result == pl.Path(target).expanduser().resolve())
 
     @pytest.mark.parametrize("name", MULTI_KEYS + NON_PATH_MUTI_KEYS)
     def test_set_default_expansion(self, name):
-        spec  = DootActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
+        spec  = ActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
         state = {"a": "bloo", "b_": "blee"}
         obj   = dkey.DootKey.build(name, strict=False)
         obj.set_expansion_hint("str")
         assert(isinstance(obj(spec, state), str))
 
 class TestKeySimple:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
+        return ActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
 
     @pytest.fixture(scope="function")
     def state(self):
         return {"a": "bloo", "b_": "blee"}
 
     def test_basic_expand(self):
         example = DootKey.build("blah")
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key_decorators.py` & `doot-0.8.0/doot/_structs/__tests/test_key_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logging = logmod.root
 
 import decorator
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 from doot.utils.decorators import DootDecorator as DDec, DecorationUtils as DecU
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
@@ -33,15 +33,15 @@
 TEST_LOCS               : Final[DootLocations] = DootLocations(pl.Path.cwd()).update({"blah": "doot"})
 
 class TestKeyDecorators:
     """ Test the key decorators """
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
+        return ActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
 
     @pytest.fixture(scope="function")
     def state(self):
         return {"a": "bloo", "b_": "blee", "c": "awegg"}
 
     def test_verify_signature_basic_with_self(self):
 
@@ -120,15 +120,15 @@
 
         assert(not DecU.verify_action_signature(an_action, ["z"]))
 
 class TestKeyDecoratorsCalls:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
+        return ActionSpec(kwargs=TomlGuard({"x": "aweg", "y_": "a"}))
 
     @pytest.fixture(scope="function")
     def state(self):
         return {"a": "bloo", "b_": "blee", "c": "awegg"}
 
     def test_basic_annotate(self):
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key_multi.py` & `doot-0.8.0/doot/_structs/__tests/test_key_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 logging = logmod.root
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
 
@@ -36,21 +36,21 @@
         obj           = DootKey.build(key, strict=False)
         assert(obj.keys() == set(targets))
 
     @pytest.mark.parametrize("key,target", [("{blah}/bloo", "./doot/bloo"), ("{blah}/bloo/{aweg}", "./doot/bloo/qqqq") ])
     def test_to_path_expansion(self, mocker, key, target):
         mocker.patch.dict("doot.__dict__", locs=TEST_LOCS)
         obj           = DootKey.build(key, strict=False)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {"aweg": "qqqq"}
         result        = obj.to_path(spec, state)
         assert(isinstance(result, pl.Path))
         assert(result == pl.Path(target).expanduser().resolve())
 
     @pytest.mark.parametrize("key,target", [("{blah}/bloo", "doot/bloo"), ("test !!! {blah}", "test !!! doot"), ("{aweg}-{blah}", "BOO-doot") ])
     def test_expansion(self, mocker, key, target):
         obj           = DootKey.build(key, strict=False)
-        spec          = mocker.Mock(params={}, spec=DootActionSpec)
+        spec          = mocker.Mock(params={}, spec=ActionSpec)
         state         = {"blah": "doot", "aweg": "BOO"}
         result        = obj.expand(spec, state)
         assert(isinstance(result, str))
         assert(result == target)
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key_path_expansion.py` & `doot-0.8.0/doot/_structs/__tests/test_key_path_expansion.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 logging = logmod.root
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
 
 TEST_LOCS               : Final[DootLocations] = DootLocations(pl.Path.cwd()).update({"blah": "doot"})
 
 class TestPathExpansion:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
+        return ActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
 
     @pytest.fixture(scope="function")
     def setup_locs(self, mocker):
         with doot.locs:
             doot.locs.update({"p1": "test1", "p2": "test2/sub"})
             yield
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key_string_expansion.py` & `doot-0.8.0/doot/_structs/__tests/test_key_string_expansion.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 logging = logmod.root
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
 
 TEST_LOCS               : Final[DootLocations] = DootLocations(pl.Path.cwd()).update({"blah": "doot"})
 
 class TestStringExpansion:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
+        return ActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
 
     @pytest.fixture(scope="function")
     def setup_locs(self, mocker):
         with doot.locs:
             doot.locs.update({"p1": "test1", "p2": "test2/sub"})
             yield
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_key_type_expansion.py` & `doot-0.8.0/doot/_structs/__tests/test_key_type_expansion.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 logging = logmod.root
 
 from tomlguard import TomlGuard
 import doot
 doot._test_setup()
 from doot.control.locations import DootLocations
-from doot.structs import DootKey, DootActionSpec
+from doot.structs import DootKey, ActionSpec
 from doot._structs import key as dkey
 
 KEY_BASES               : Final[str] = ["bob", "bill", "blah", "other"]
 MULTI_KEYS              : Final[str] = ["{bob}/{bill}", "{blah}/{bloo}", "{blah}/{bloo}"]
 NON_PATH_MUTI_KEYS      : Final[str] = ["{bob}_{bill}", "{blah} <> {bloo}", "! {blah}! {bloo}!"]
 KEY_INDIRECTS           : Final[str] = ["bob_", "bill_", "blah_", "other_"]
 
 TEST_LOCS               : Final[DootLocations] = DootLocations(pl.Path.cwd()).update({"blah": "doot"})
 
 class TestTypeExpansion:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
+        return ActionSpec(kwargs=TomlGuard({"y": "aweg", "z_": "bloo"}))
 
     @pytest.fixture(scope="function")
     def setup_locs(self, mocker):
         new_locs = TomlGuard({"p1": "test1", "p2": "test2/sub"})
         return mocker.patch.object(doot.locs, "_data", new_locs)
 
     def test_to_any_basic(self, spec, mocker, setup_locs):
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_param_spec.py` & `doot-0.8.0/doot/_structs/__tests/test_param_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,192 +14,193 @@
 ##-- end imports
 logging = logmod.root
 
 import pytest
 import doot
 doot._test_setup()
 import doot.errors
-from doot.structs import DootParamSpec, DootTaskSpec
+from doot.structs import ParamSpec, TaskSpec
 
 class TestParamSpec:
 
     def test_paramspec(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
-        assert(isinstance(example, DootParamSpec))
+        assert(isinstance(example, ParamSpec))
 
     def test_equal(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         assert(example == "test=blah")
         assert(example == "-test")
         assert(example == "-test=blah")
         assert(example == "-t")
         assert(example == "-t=blah")
 
     def test_equal_fail(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
         assert(example != "atest")
         assert(example != "--test")
         assert(example != "-tw")
 
     def test_consume_bool(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : "bool",
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-test"], data)
         assert('test' in data)
         assert(bool(data['test']))
 
     def test_consume_short_bool(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-t"], data)
         assert('test' in data)
         assert(bool(data['test']))
 
     def test_fail_on_assign_wrong_prefix(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         with pytest.raises(doot.errors.DootParseError):
             example.maybe_consume(["-t=blah"], {})
 
     def test_consume_inverse_bool(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-no-test"], data)
         assert('test' in data)
         assert(not bool(data['test']))
 
     def test_consume_list(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
           })
         assert(example == "test")
         data = {'test': []}
         example.maybe_consume(["-test", "bloo"], data)
         assert('test' in data)
         assert(data['test'] == ["bloo"])
 
     def test_consume_list_multi(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
             "positional": True
           })
         assert(example == "test")
         data = {'test': []}
         example.maybe_consume(["bloo", "blah"], data)
         assert('test' in data)
         assert(data['test'] == ["bloo", "blah"])
 
     @pytest.mark.xfail
     def test_consume_list_multi_joined(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
           })
         assert(example == "test")
         data = {'test': []}
         args = ["-test", "bloo", "-test", "blah"]
         example.maybe_consume(args, data)
         example.maybe_consume(args, data)
         assert('test' in data)
         assert(data['test'] == ["bloo", "blah"])
 
     @pytest.mark.xfail
     def test_consume_set_multi_joined(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name"    : "test",
             "type"    : set,
             "default" : set(),
           })
         assert(example == "test")
         data = {'test': set()}
         example.maybe_consume(["-test", "bloo"], data)
         example.maybe_consume(["-test", "bloo"], data)
         example.maybe_consume(["-test", "blah"], data)
         assert('test' in data)
         assert(data['test'] == {"bloo", "blah"})
 
     def test_consume_str(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : str,
             "default" : "",
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-test", "bloo,blah"], data)
         assert('test' in data)
         assert(data['test'] == "bloo,blah")
 
     def test_consume_str_multi_set_fail(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : str,
             "default" : "",
           })
         assert(example == "test")
         data = {} # <---
         example.maybe_consume(["-test", "bloo", "blah"], data)
         with pytest.raises(Exception):
             example.maybe_consume(data, "-test=aweg")
 
+    @pytest.mark.xfail
     def test_consume_custom_value(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : lambda x: int(x) + 2,
             "default" : 5,
           })
         assert(example == "test")
         data = {} # <---
         example.maybe_consume(["-test", "2"], data)
         assert(example == "test")
         assert(data['test'] == 4)
 
     def test_positional(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "positional" : True
             })
         assert(example.positional is True)
 
     def test_invisible_str(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "invisible" : True,
             })
         assert(str(example) == "")
 
     def test_not_invisible_str(self):
-        example = DootParamSpec.build({
+        example = ParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "invisible" : False,
             })
         assert(str(example) != "")
```

### Comparing `doot-0.7.2/doot/_structs/__tests/test_stub.py` & `doot-0.8.0/doot/_structs/__tests/test_stub.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,98 +13,103 @@
 
 import pytest
 logging = logmod.root
 
 import tomlguard
 import doot
 doot._test_setup()
-from doot import structs
+from doot._structs import stub
+from doot._structs.task_name import TaskName
 
 class TestTaskStub:
 
     def test_initial(self):
-        obj = structs.TaskStub(dict)
-        assert(isinstance(obj, structs.TaskStub))
-        assert(obj.ctor == dict)
-        assert(str(obj['name'].default) == "basic::stub")
+        obj = stub.TaskStub.build()
+        assert(isinstance(obj, stub.TaskStub))
+        assert(obj.ctor == "doot.task.base_task:DootTask")
+        assert(obj['name'].default == "basic::stub")
+
+    def test_add_field(self):
+        obj = stub.TaskStub.build()
+        assert("blah" not in obj)
+        obj['blah'].default = "bloo"
+        assert("blah" in obj)
 
     def test_default_keys(self):
         """ check a stub has the default components of a TaskSpec  """
-        obj = structs.TaskStub(dict)
-        default_keys = set(structs.DootTaskSpec.__annotations__.keys())
-        default_keys -= set(structs.TaskStub.skip_parts)
+        obj = stub.TaskStub.build()
+
+        default_keys = set(stub.TaskSpec.model_fields.keys())
+
+        default_keys -= set(stub.TaskStub.skip_parts)
+
         default_keys.add("name")
+
         default_keys.add("version")
         assert(set(obj.parts.keys()) == default_keys)
 
     def test_to_toml(self):
         """ check a stub has the default components of a TaskSpec  """
-        obj = structs.TaskStub(dict)
+        obj = stub.TaskStub.build()
         as_str = obj.to_toml().split("\n")
         assert(len(as_str) > 10)
 
-
     def test_to_toml_reparse(self):
         """ check a stub has the default components of a TaskSpec  """
-        obj = structs.TaskStub(dict)
+        obj = stub.TaskStub.build()
         as_str = obj.to_toml()
         loaded = tomlguard.read(as_str)
 
-
+    @pytest.mark.xfail
     def test_toml_reparse_to_spec(self):
         """ check a stub has the default components of a TaskSpec  """
-        obj    = structs.TaskStub()
+        obj    = stub.TaskStub.build()
         as_str = obj.to_toml()
         loaded = tomlguard.read(as_str)
-        spec   = structs.DootTaskSpec.build(loaded.tasks.basic[0])
-
-
-
+        # FIXME: currently splits the name so its not basic::stub, but 'stub', so fails building
+        spec   = stub.TaskSpec.build(loaded.tasks.basic[0])
 
 class TestTaskStubPart:
 
     def test_stub_initial(self):
-        obj = structs.TaskStubPart("test", type="list", default=[1,2,3], comment="a simple stub part")
-        assert(isinstance(obj, structs.TaskStubPart))
+        obj = stub.TaskStubPart(key="test", type_="list", default=[1,2,3], comment="a simple stub part")
+        assert(isinstance(obj, stub.TaskStubPart))
         assert(obj.key == "test")
-        assert(obj.type == "list")
+        assert(obj.type_ == "list")
         assert(obj.default == [1,2,3])
         assert(obj.comment == "a simple stub part")
 
-
     def test_name_reduce(self):
-        obj = structs.TaskStubPart("name", default=structs.DootTaskName.build("blah::bloo"))
+        obj = stub.TaskStubPart(key="name", default=TaskName.build("blah::bloo"))
         res_s = str(obj).split("\n")
         assert(res_s[0] == "[[tasks.blah]]")
         assert(res_s[1] == f"{'name':<20} = \"bloo\"")
 
-
     def test_num_reduce(self):
-        obj = structs.TaskStubPart("amount", default=10, type="int")
+        obj = stub.TaskStubPart(key="amount", default=10, type="int")
         result_str     = str(obj)
         result_tomlguard  = tomlguard.read(result_str)
         assert(result_tomlguard.amount == 10)
 
     def test_str_reduce_with_comment(self):
-        obj = structs.TaskStubPart("blah", default="a test", comment="a simple comment")
+        obj = stub.TaskStubPart(key="blah", default="a test", comment="a simple comment")
         as_toml = str(obj)
-        assert(as_toml == f"{'blah':<20} = \"a test\"             # <str>                a simple comment")
+        assert(as_toml == f"{'blah':<20} = \"a test\"             # <str>                # a simple comment")
 
     def test_stub_part_list_reduce(self):
-        obj = structs.TaskStubPart("test", type="list", default=[1,2,3], comment="a simple stub part")
+        obj = stub.TaskStubPart(key="test", type="list", default=[1,2,3], comment="a simple stub part")
         result_str     = str(obj)
         result_tomlguard  = tomlguard.read(result_str)
 
         assert(result_tomlguard.test == [1,2,3])
 
     def test_stub_part_str_reduce(self):
-        obj = structs.TaskStubPart("test", type="str", default="test", comment="a simple stub part")
+        obj = stub.TaskStubPart(key="test", type="str", default="test", comment="a simple stub part")
         result_str     = str(obj)
         result_tomlguard  = tomlguard.read(result_str)
         assert(result_tomlguard.test == "test")
 
-
     def test_stub_part_bool_reduce(self):
-        obj = structs.TaskStubPart("test", type="bool", default=False, comment="a simple stub part")
+        obj = stub.TaskStubPart(key="test", type="bool", default=False, comment="a simple stub part")
         result_str     = str(obj)
         result_tomlguard  = tomlguard.read(result_str)
         assert(result_tomlguard.test == False)
```

### Comparing `doot-0.7.2/doot/_structs/action_spec.py` & `doot-0.8.0/doot/_structs/action_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,67 +32,83 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from pydantic import BaseModel, Field, model_validator, field_validator
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
 from doot.enums import TaskFlags, ReportEnum
-from doot._abstract.structs import SpecStruct_p
+from doot._abstract.protocols import SpecStruct_p
+from doot._structs.code_ref import CodeReference
 
-PAD           : Final[int] = 15
-TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
+ALIASES = doot.aliases.action
 
-@dataclass
-class DootActionSpec(SpecStruct_p):
+class ActionSpec(BaseModel, arbitrary_types_allowed=True):
     """
       When an action isn't a full blown class, it gets wrapped in this,
       which passes the action spec to the callable.
 
       TODO: recogise arg prefixs and convert to correct type.
       eg: path:a/relative/path  -> Path(./a/relative/path)
       path:/usr/bin/python  -> Path(/usr/bin/python)
 
     """
-    do         : None|str                   = field(default=None)
-    args       : list[Any]                  = field(default_factory=list)
-    kwargs     : TomlGuard                  = field(default_factory=TomlGuard)
-    inState    : set[str]                   = field(default_factory=set)
-    outState   : set[str]                   = field(default_factory=set)
-    fun        : None|Callable              = field(default=None)
+    do         : None|CodeReference               = None
+    args       : list[Any]                            = []
+    kwargs     : TomlGuard                            = Field(default_factory=TomlGuard)
+    inState    : set[str]                             = set()
+    outState   : set[str]                             = set()
+    fun        : None|Callable                        = None
 
     @staticmethod
-    def build(data:dict|list|TomlGuard|DootActionSpec, *, fun=None) -> DootActionSpec:
+    def build(data:dict|list|TomlGuard|ActionSpec, *, fun=None) -> ActionSpec:
         match data:
-            case DootActionSpec():
+            case ActionSpec():
                 return data
             case list():
-                action_spec = DootActionSpec(
+                action_spec = ActionSpec(
                     args=data,
                     fun=fun if callable(fun) else None
                     )
                 return action_spec
 
             case dict() | TomlGuard():
-                kwargs = TomlGuard({x:y for x,y in data.items() if x not in DootActionSpec.__dataclass_fields__.keys()})
-                action_spec = DootActionSpec(
-                    do=data['do'],
+                kwargs = TomlGuard({x:y for x,y in data.items() if x not in ActionSpec.model_fields})
+                fun    = data.get('fun', fun)
+                action_spec = ActionSpec(
+                    do=data.get('do', None),
                     args=data.get('args',[]),
                     kwargs=kwargs,
                     inState=set(data.get('inState', set())),
                     outState=set(data.get('outState', set())),
-                    fun=fun if callable(fun) else None
+                    fun=fun,
                     )
                 return action_spec
             case _:
                 raise doot.errors.DootActionError("Unrecognized specification data", data)
 
+    @field_validator("do", mode="before")
+    def _validate_do(cls, val):
+        match val:
+            case None:
+                return None
+            case str() if val in ALIASES:
+                return CodeReference.build(ALIASES[val])
+            case str():
+                return CodeReference.build(val)
+            case CodeReference():
+                return val
+            case _:
+                raise TypeError("Unrecognized action spec do type", val)
+
     def __str__(self):
         result = []
         if isinstance(self.do, str):
             result.append(f"do={self.do}")
         elif self.do and hasattr(self.do, '__qualname__'):
             result.append(f"do={self.do.__qualname__}")
         elif self.do:
@@ -119,15 +135,15 @@
             raise doot.errors.DootActionError("Action Spec has not been finalised with a function", self)
 
         return self.fun(self, task_state)
 
     def set_function(self, fun:Action_p|Callable):
         """
           Sets the function of the action spec.
-          if given a class, the class it built,
+          if given a class, the class is built,
           if given a callable, that is used directly.
 
         """
         # if the function/class has an inState/outState attribute, add those to the spec's fields
         if hasattr(fun, 'inState') and isinstance(getattr(fun, 'inState'), list):
             self.inState.update(getattr(fun, 'inState'))
```

### Comparing `doot-0.7.2/doot/_structs/artifact.py` & `doot-0.8.0/doot/_structs/artifact.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,131 +32,119 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from pydantic import BaseModel, field_validator, model_validator
 import importlib
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.enums import TaskFlags, ReportEnum, LocationMeta
-from doot._structs.toml_loc import TomlLocation
+from doot._structs.location import Location, GLOB, SOLO, REC_GLOB
 from doot._structs.key import DootKey
 
-PAD           : Final[int]   = 15
-ARTIFACT      : Final[str]   = "!!Artifact!!"
-
-@dataclass
-class DootTaskArtifact:
+class TaskArtifact(Location, arbitrary_types_allowed=True):
     """
-      Wraps a toml defined location into an artifact
+      An concrete or abstract artifact a task can produce or consume.
 
-      Describes an artifact a task can produce or consume.
-    Artifacts can be Definite (concrete path) or indefinite (glob path)
-    """
-    base     : TomlLocation = field()
-    key      : DootKey      = field()
+      Tasks can depend on both concrete and abstract:
+      depends_on=['file:>/a/file.txt', 'file:>*.txt', 'file:>?.txt']
+      and can be a requirement for concrete or *solo* abstract artifacts:
+      required_for=['file:>a/file.txt', 'file:>?.txt']
 
-    @staticmethod
-    def build(data:str|dict|pl.Path) -> DootTaskArtifact:
-        match data:
-            case str() if data.startswith(doot.constants.patterns.FILE_DEP_PREFIX):
-                base = TomlLocation.build(ARTIFACT, data.removeprefix(doot.constants.patterns.FILE_DEP_PREFIX))
-                base.meta |= LocationMeta.file
-                key = DootKey.build(base.base)
-                return DootTaskArtifact(base, key)
-            case str():
-                base = TomlLocation.build(ARTIFACT, data)
-                key  = DootKey.build(base.base)
-                return DootTaskArtifact(base, key)
-            case dict():
-                base = TomlLocation.build(ARTIFACT, data)
-                if "*" in str(base.base):
-                    base.meta |= LocationMeta.indefinite
-                key = DootKey.build(base.base)
-                return DootTaskArtifact(base, key)
-            case pl.Path():
-                base = TomlLocation.build(ARTIFACT, data)
-                if "*" in str(base.base):
-                    base.meta |= LocationMeta.indefinite
-                key = DootKey.build(base.base)
-                return DootTaskArtifact(base, key)
-            case _:
-                raise TypeError("Unknown Type to build Artifact from: %s", data)
+
+    """
 
     def __repr__(self):
-        return f"<TaskArtifact: {self.key} : {self.base.meta}>"
+        return f"<TaskArtifact: {self.path} : {self.meta}>"
 
     def __str__(self):
-        return str(self.base.base)
+        return str(self.path)
 
     def __hash__(self):
         return hash(str(self))
 
-    def __eq__(self, other:DootTaskArtifact|Any):
+    def __eq__(self, other:str|pl.Path|TaskArtifact|Any):
         match other:
-            case DootTaskArtifact():
-                return self.base == other.base
+            case str() | pl.Path():
+                return pl.Path(other) == self.path
+            case TaskArtifact():
+                return self.path == other.path
             case _:
                 return False
 
     def __bool__(self):
-        return self.exists
+        return self.exists()
 
-    def __contains__(self, other):
-        """ whether a definite artifact is matched by self, an indefinite artifact
-          a/b/c.py ∈ a/b/*.py
-          ________ ∈ a/*/c.py
-          ________ ∈ a/b/c.*
-          ________ ∈ a/*/c.*
-          ________ ∈ **/c.py
+    @ftz.cached_property
+    def is_concrete(self):
+        return not self.check(LocationMeta.abstract)
 
-        """
-        if not self.check(LocationMeta.indefinite):
-            return False
-
-        for x,y in zip(self.parent.parts, other.parent.parts):
-            if x == "**" or y == "**":
-                break
-            if x == "*" or y == "*":
-                continue
-            if x != y:
-                return False
-
-        suffix      = (not self._definite_suffix) or self.base.base.suffix == other.base.base.suffix
-        stem        = (not self._definite_stem)    or self.base.base.stem == other.base.base.stem
-        return  suffix and stem
-
-    @property
-    def exists(self):
-        if not self.is_definite:
-            return False
-        as_path = self.key.to_path(None, None)
-        return as_path.exists()
-
-    @property
-    def is_definite(self):
-        """ tests the entire artifact path """
-        return not self.check(LocationMeta.indefinite)
-
-    @property
-    def _definite_stem(self):
-        """ tests the stem of the artifact """
-        return "*" not in self.base.base.stem
-
-    @property
-    def _definite_suffix(self):
-        """ tests the suffix of the artifact """
-        return "*" not in self.base.base.suffix
-
-    @property
+    @ftz.cached_property
     def parent(self):
-        return self.base.base.parent
+        return self.path.parent
 
     def is_stale(self) -> bool:
         """ whether the artifact itself is stale """
         raise NotImplementedError('TODO')
 
-    def check(self, meta:LocationMeta) -> bool:
-        return self.base.check(meta)
+
+    def match_with(self, other:pl.Path|TaskArtifact) -> None|TaskArtifact:
+        """ An abstract location, given a concrete other location,
+          will apply parts of it onto itself, where it has wildcards
+
+          To match, the stem *must* be a wildcard, at least.
+
+          This is for instantiating task transformers.
+
+          eg: a/*/?.blah + a/blah/file.txt -> a/blah/file.blah
+          a/**/?.blah + a/b/c/d.txt -> a/b/c/d.blah
+
+        """
+        if LocationMeta.abstract not in self:
+            return None
+
+        a_path, a_stem, a_suff = self.abstracts
+
+        if not a_stem:
+            return None
+
+        match other:
+            case Location():
+                match_on = other.path.parent.parts
+                stem     = other.path.stem
+                suff     = other.path.suffix
+            case pl.Path():
+                match_on = other.parent.parts
+                stem     = other.stem
+                suffix   = other.suffix
+            case _:
+                raise ValueError("Location can't match against a non-Location or path", other)
+
+        result = []
+        rest_of = False
+
+        if a_path:
+            for i, (x,y) in enumerate(zip(self.path.parent.parts, match_on)):
+                if x in [GLOB, SOLO]:
+                    result.append(y)
+                elif x == REC_GLOB:
+                    result += match_on[i:]
+                elif x == y:
+                    result.append(x)
+                else:
+                    return None
+        else:
+            result += self.path.parents
+
+        result.append(stem)
+
+        base = pl.Path().joinpath(*result)
+        if a_suff:
+            return TaskArtifact(path=base.with_suffix(suffix),
+                                    key=self.key)
+
+        return TaskArtifact(path=base.with_suffix(self.path.suffix),
+                                key=self.key)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `doot-0.7.2/doot/_structs/code_ref.py` & `doot-0.8.0/doot/_structs/code_ref.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,115 +32,102 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from pydantic import field_validator, model_validator
 import importlib
 from importlib.metadata import EntryPoint
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot._structs.structured_name import StructuredName
 
-@dataclass(eq=False, slots=True)
-class DootCodeReference(StructuredName):
+class CodeReference(StructuredName):
     """
       A reference to a class or function. can be created from a string (so can be used from toml),
       or from the actual object (from in python)
     """
-    separator : str                              = field(default=doot.constants.patterns.IMPORT_SEP, kw_only=True)
-    _mixins   : list[DootCodeReference]          = field(default_factory=list, kw_only=True)
-    _type     : None|type                        = field(default=None, kw_only=True)
+    _mixins   : list[CodeReference]          = []
+    _type     : None|type                        = None
+
+    _separator : ClassVar[str]                    = doot.constants.patterns.IMPORT_SEP
 
     @classmethod
     def build(cls, name:str|type|EntryPoint):
         match name:
+            case str() if cls._separator not in name:
+                raise ValueError("a separator needs to be used", name, cls._separator)
             case str():
-                return cls._from_str(name)
+                groupHead_r, taskHead_r = name.split(cls._separator)
+                return cls(head=[groupHead_r], tail=[taskHead_r])
             case type():
-                groupHead = name.__module__
-                codeHead  = name.__name__
-                ref = cls(groupHead, codeHead, _type=name)
+                group, code = name.__module__, name.__name__
+                ref = cls(head=[group], tail=[code], _type=name)
                 return ref
             case EntryPoint():
-                loaded = ctor.load()
-                groupHead = loaded.__module__
-                codeHead  = loaded.__name__
-                ref = cls(groupHead, codeHead, _type=loaded)
+                loaded      = ctor.load()
+                group, code = loaded.__module__, loaded.__name__
+                ref         = cls(head=[group], tail=[code], _type=loaded)
                 return ref
-
-    @classmethod
-    def _from_str(cls, name:str):
-        if doot.constants.patterns.TASK_SEP in name:
-            raise doot.errors.DootError("Code References should use a single colon, not double")
-
-        if ":" in name:
-            try:
-                groupHead_r, taskHead_r = name.split(":")
-                groupHead = groupHead_r.split(".")
-                taskHead = taskHead_r.split(".")
-            except ValueError:
-                raise doot.errors.DootConfigError("Code ref can't be split correctly, ensure its of the form x.y.z:ClassName", name)
-        else:
-            groupHead = None
-            taskHead  = name
-
-        return DootCodeReference(groupHead, taskHead)
+            case _:
+                raise ValueError("Bad Value used to try to build a coderef", name)
 
     @staticmethod
-    def from_alias(alias:str, group:str, plugins:TomlGuard) -> DootCodeReference:
+    def from_alias(alias:str, group:str, plugins:TomlGuard) -> CodeReference:
         if group not in plugins:
-            return DootCodeReference._from_str(alias)
+            raise ValueError("Plugin Group not found for CodeRef dealiasing", group, alias, plugins)
+
         match [x for x in plugins[group] if x.name == alias]:
             case [x, *xs]:
-                return DootCodeReference._from_str(x.value)
+                return CodeReference.build(x.value)
             case _:
-                return DootCodeReference._from_str(alias)
+                return CodeReference.build(alias)
 
     def __str__(self) -> str:
-        return "{}{}{}".format(self.module, self.separator, self.value)
+        return "{}{}{}".format(self.module, self._separator, self.value)
 
     def __repr__(self) -> str:
         code_path = str(self)
         mixins    = ", ".join(str(x) for x in self._mixins)
         return f"<CodeRef: {code_path} Mixins: {mixins}>"
 
     def __hash__(self):
         return hash(str(self))
 
     def __iter__(self):
         return iter(self._mixins)
 
-    @property
+    @ftz.cached_property
     def module(self):
-        return self.subseparator.join(self.head)
+        return self._subseparator.join(self.head)
 
-    @property
+    @ftz.cached_property
     def value(self):
-        return self.subseparator.join(self.tail)
+        return self._subseparator.join(self.tail)
 
-    def add_mixins(self, *mixins:str|DootCodeReference|type, plugins:TomlGuard=None) -> DootCodeReference:
+    def add_mixins(self, *mixins:str|CodeReference|type, plugins:TomlGuard=None) -> CodeReference:
         to_add = self._mixins[:]
         for mix in mixins:
             match mix:
-                case DootCodeReference():
+                case CodeReference():
                     ref = mix
                 case str() if plugins is not None:
-                    ref = DootCodeReference.from_alias(mix, "mixin", plugins)
+                    ref = CodeReference.from_alias(mix, "mixin", plugins)
                 case str() | type():
-                    ref = DootCodeReference.build(mix)
+                    ref = CodeReference.build(mix)
                 case _:
                     raise TypeError("Unrecognised mixin type", mix)
 
             if ref not in to_add:
                 to_add.append(ref)
 
-        new_ref = DootCodeReference(head=self.head[:], tail=self.tail[:], _mixins=to_add, _type=self._type)
+        new_ref = CodeReference(head=self.head[:], tail=self.tail[:], _mixins=to_add, _type=self._type)
         return new_ref
 
     def try_import(self, ensure:type=Any) -> Any:
         try:
             if self._type is not None:
                 curr = self._type
             else:
@@ -149,15 +136,15 @@
                 for name in self.tail:
                     curr = getattr(curr, name)
 
             if bool(self._mixins):
                 mixins = []
                 for mix in self._mixins:
                     match mix:
-                        case DootCodeReference():
+                        case CodeReference():
                             mixins.append(mix.try_import())
                         case type():
                             mixins.append(mix)
                 curr = type(f"DootGenerated:{curr.__name__}", tuple(mixins + [curr]), {})
 
             if ensure is not Any and not (isinstance(curr, ensure) or issubclass(curr, ensure)):
                 raise ImportError("Imported Code Reference is not of correct type", self, ensure)
@@ -177,18 +164,18 @@
         if group != "mixins":
             mixins = [x.to_aliases("mixins", plugins)[0] for x in  self._calculate_minimal_mixins(plugins)]
         else:
             mixins = []
 
         return base_alias, mixins
 
-    def _calculate_minimal_mixins(self, plugins:TomlGuard) -> list[DootCodeReference]:
+    def _calculate_minimal_mixins(self, plugins:TomlGuard) -> list[CodeReference]:
         found          = set()
         minimal_mixins = []
         for mixin in reversed(sorted(map(lambda x: x.try_import(), self), key=lambda x:  len(x.mro()))):
             if mixin in found:
                 continue
 
             found.update(mixin.mro())
             minimal_mixins.append(mixin)
 
-        return [DootCodeReference.build(x) for x in minimal_mixins]
+        return [CodeReference.build(x) for x in minimal_mixins]
```

### Comparing `doot-0.7.2/doot/_structs/key.py` & `doot-0.8.0/doot/_structs/key.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,22 +33,23 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
+from pydantic import BaseModel, Field, model_validator, field_validator
 import decorator
 import abc
 import string
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._structs.code_ref import DootCodeReference
-from doot._abstract.structs import SpecStruct_p
+from doot._structs.code_ref import CodeReference
+from doot._abstract.protocols import SpecStruct_p
 from doot.utils.chain_get import DootKeyGetter
 from doot.utils.decorators import DootDecorator, DecorationUtils
 
 KEY_PATTERN                                = doot.constants.patterns.KEY_PATTERN
 MAX_KEY_EXPANSIONS                         = doot.constants.patterns.MAX_KEY_EXPANSIONS
 STATE_TASK_NAME_K                          = doot.constants.patterns.STATE_TASK_NAME_K
 
@@ -167,16 +168,16 @@
 
     def format(self, fmt:str|DootKey|pl.Path, /, *args, **kwargs) -> str:
         """ expand and coerce keys """
         self._depth = 0
         match kwargs.get(self.SPEC, None):
             case None:
                 kwargs['_spec'] = {}
-            case SpecStruct_p():
-                kwargs['_spec'] = kwargs[self.SPEC].params
+            case x if hasattr(x, "params"):
+                kwargs['_spec'] = x.params
             case x:
                 raise TypeError("Bad Spec Type in Format Call", x)
 
         match fmt:
             case DootKey():
                 fmt = fmt.form
                 result = self.vformat(fmt, args, kwargs)
@@ -229,16 +230,17 @@
 
       DootSimpleKeys are strings, wrapped in {} when used in toml.
       so DootKey.build("blah") -> DootSimpleKey("blah") -> DootSimpleKey('blah').form =="{blah}" -> [toml] aValue = "{blah}"
 
       DootMultiKeys are containers of a string `value`, and a list of SimpleKeys the value contains.
       So DootKey.build("{blah}/{bloo}") -> DootMultiKey("{blah}/{bloo}", [DootSimpleKey("blah", DootSimpleKey("bloo")]) -> .form == "{blah}/{bloo}"
     """
-    dec   = KeyDecorator
-    kwrap = KeyDecorator
+    dec      : ClassVar[type]      = KeyDecorator
+    kwrap    : ClassVar[type]      = KeyDecorator
+    _pattern : ClassVar[re.Pattern] = PATTERN
 
     @staticmethod
     def build(s:str|DootKey|pl.Path|dict, *, strict=False, explicit=False, exp_hint:str|dict=None, help=None) -> DootKey:
         """ Make an appropriate DootKey based on input value
           Can only create MultiKeys if strict = False,
           if explicit, only keys wrapped in {} are made, everything else is returned untouched
           if strict, then only simple keys can be returned
@@ -314,20 +316,20 @@
             case {"expansion": "redirect_multi"}:
                 return self.redirect_multi(spec)
             case {"expansion": "coderef"}:
                 return self.to_coderef(spec, state)
             case x:
                 raise doot.errors.DootKeyError("Key Called with Bad Key Expansion Type", self, x)
 
-    @property
+    @ftz.cached_property
     def form(self) -> str:
         return str(self)
 
-    @property
-    def direct(self):
+    @ftz.cached_property
+    def direct(self) -> str:
         return str(self).removesuffix("_")
 
     @property
     def is_indirect(self) -> bool:
         return False
 
     def redirect(self, spec=None) -> DootKey:
@@ -381,28 +383,28 @@
     def to_type(self, spec, state, type_=Any, chain:list[DootKey]=None, on_fail=Any, **kwargs) -> Any:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs:DootLocations=None, **kwargs) -> str:
         pass
 
-    def to_coderef(self, spec:None|SpecStruct_p, state) -> None|DootCodeReference:
+    def to_coderef(self, spec:None|SpecStruct_p, state) -> None|CodeReference:
         match spec:
-            case SpecStruct_p():
+            case _ if hasattr(spec, "params"):
                 kwargs = spec.params
             case None:
                 kwargs = {}
 
         redir = self.redirect(spec)
 
         if redir not in kwargs and redir not in state:
             return None
         try:
             expanded = self.expand(spec, state)
-            ref = DootCodeReference.build(expanded)
+            ref = CodeReference.build(expanded)
             return ref
         except doot.errors.DootError:
             return None
 
 class DootNonKey(str, DootKey):
     """
       Just a string, not a key. But this lets you call no-ops for key specific methods
@@ -424,17 +426,17 @@
     def within(self, other:str|dict|TomlGuard) -> bool:
         match other:
             case str():
                 return self.form in other
             case dict() | TomlGuard():
                 return self in other
             case _:
-                raise TypeError("Uknown DootKey target for within", other)
+                raise TypeError("Unknown DootKey target for within", other)
 
-    @property
+    @ftz.cached_property
     def indirect(self) -> DootKey:
         if not self.is_indirect:
             return DootSimpleKey("{}_".format(super().__str__()))
         return self
 
     @property
     def is_indirect(self):
@@ -471,25 +473,25 @@
     def __eq__(self, other):
         match other:
             case DootKey() | str():
                 return str(self) == str(other)
             case _:
                 return False
 
-    @property
+    @ftz.cached_property
     def indirect(self):
         if not self.is_indirect:
             return DootSimpleKey("{}_".format(super().__str__()))
         return self
 
-    @property
+    @ftz.cached_property
     def is_indirect(self):
         return str(self).endswith("_")
 
-    @property
+    @ftz.cached_property
     def form(self):
         """ Return the key in its use form, ie: wrapped in braces """
         return "{{{}}}".format(str(self))
 
     def within(self, other:str|dict|TomlGuard) -> bool:
         match other:
             case str():
@@ -515,17 +517,17 @@
         """
           If the indirect form of the key is found in the spec, use that as a key instead
         """
         if not spec:
             return self
 
         match spec:
-            case SpecStruct_p():
+            case _ if hasattr(spec, "params"):
                 kwargs = spec.params
-            case None:
+            case _:
                 kwargs = {}
 
         match kwargs.get(self.indirect, self):
             case str() as x if x == self.indirect:
                 return self
             case str() as x:
                 return DootKey.build(x)
@@ -536,15 +538,15 @@
 
     def redirect_multi(self, spec:None|SpecStruct_p=None) -> list[DootKey]:
         """ redirect an indirect key to a *list* of keys """
         if not spec:
             return [self]
 
         match spec:
-            case SpecStruct_p():
+            case _ if hasattr(spec, "params"):
                 kwargs = spec.params
             case None:
                 kwargs = {}
 
         match kwargs.get(self.indirect, self):
             case str() as x if x == self:
                 return [self]
@@ -555,15 +557,15 @@
 
         return [self]
 
     def to_type(self, spec:None|SpecStruct_p=None, state=None, type_=Any, chain:list[DootKey]=None, on_fail=Any) -> Any:
         target            = self.redirect(spec)
 
         match spec:
-            case SpecStruct_p():
+            case _ if hasattr(spec, "params"):
                 kwargs = spec.params
             case None:
                 kwargs = {}
 
         task_name = state.get(STATE_TASK_NAME_K, None) if state else None
         match (replacement:=DootKeyGetter.chained_get(target, kwargs, state)):
             case None if bool(chain):
@@ -630,15 +632,15 @@
     """ A Key representing all of an action spec's kwargs """
 
     def __repr__(self):
         return "<DootArgsKey>"
 
     def to_type(self, spec:None|SpecStruct_p=None, state=None, *args, **kwargs) -> dict:
         match spec:
-            case SpecStruct_p():
+            case _ if hasattr(spec, "params"):
                 return spec.params
             case None:
                 return {}
 
 class DootMultiKey(DootKey):
     """ A string or path of multiple keys """
 
@@ -661,15 +663,15 @@
                 return str(self) == str(other)
             case _:
                 return False
 
     def keys(self) -> set(DootSimpleKey):
         return self._keys
 
-    @property
+    @ftz.cached_property
     def form(self):
         """ Return the key in its use form """
         return str(self)
 
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs=None, **kwargs) -> str:
         try:
             return DootFormatter.fmt(self.value, _spec=spec, _state=state, _rec=rec, _insist=insist, _locs=locs)
@@ -710,10 +712,10 @@
             case {"expansion": "redirect_multi"}:
                 return self.redirect_multi(spec)
             case x:
                 raise doot.errors.DootKeyError("Key Called with Bad Key Expansion Type", self, x)
 
 class DootImportKey(DootSimpleKey):
     """ a key to specify a key is used for importing
-    ie: str expands -> DootCodeReference.build -> .try_import
+    ie: str expands -> CodeReference.build -> .try_import
     """
     pass
```

### Comparing `doot-0.7.2/doot/_structs/param_spec.py` & `doot-0.8.0/doot/_structs/param_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,149 @@
 #!/usr/bin/env python3
 """
 
 See EOF for license/metadata/notes as applicable
 """
 
-##-- builtin imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
 # import abc
 import datetime
 import enum
 import functools as ftz
+import importlib
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+from types import GenericAlias
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 
-##-- end builtin imports
+# ##-- end stdlib imports
 
-##-- lib imports
+# ##-- 3rd party imports
 import more_itertools as mitz
-##-- end lib imports
+from pydantic import (BaseModel, Field, InstanceOf,
+                      field_validator, model_validator)
+from tomlguard import TomlGuard
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end 3rd party imports
 
-import importlib
-from tomlguard import TomlGuard
+# ##-- 1st party imports
 import doot
 import doot.errors
-from doot.enums import TaskFlags, ReportEnum
-from doot._abstract.structs import ParamStruct_p
+from doot._abstract.protocols import ParamStruct_p
+from doot.enums import ReportEnum, TaskFlags
+
+# ##-- end 1st party imports
 
-PAD           : Final[int] = 15
-TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
+##-- logging
+logging = logmod.getLogger(__name__)
+##-- end logging
 
-@dataclass
-class DootParamSpec(ParamStruct_p):
+class ParamSpec(BaseModel, arbitrary_types_allowed=True):
     """ Describes a command line parameter to use in the parser
       When `positional`, will not match against a string starting with `prefix`
       consumed in doot._abstract.parser.ArgParser_i's
       produced using doot._abstract.parser.ParamSpecMaker_m classes,
       like tasks, and jobs
     """
-    name              : str                       = field()
-    type              : type                      = field(default=bool)
 
-    prefix            : str                       = field(default="-")
+    name               : str
+    type_              : InstanceOf[type]|Callable = Field(default=bool, alias="type")
 
-    default           : Any                       = field(default=False)
-    desc              : str                       = field(default="An undescribed parameter")
-    constraints       : list                      = field(default_factory=list)
-    invisible         : bool                      = field(default=False)
-    positional        : bool|int                  = field(default=False)
-    _short            : None|str                  = field(default=None)
-
-    _repeatable_types : ClassVar[list[Any]]       = [list, int]
-
-    separator         : str                       = field(default="=")
-    _consumed         : int                       = field(default=0)
+    default            : Any                       = False
+    desc               : str                       = "An undescribed parameter"
+    constraints        : list                      = []
+    invisible          : bool                      = False
+    positional         : bool|int                  = False
+    prefix             : str                       = "-"
+    separator          : str                       = "="
+
+    _short             : None|str                  = None
+    _consumed          : int                       = 0
+    _repeatable_types  : ClassVar[list[Any]]       = [list, int]
+    _pad               : ClassVar[int]             = 15
 
     @classmethod
-    def build(cls, data:TomlGuard|dict) -> DootParamSpec:
-        param =  cls(**data)
-        match param:
-            case DootParamSpec(type="int"):
-                param.type = int
-            case DootParamSpec(type="float"):
-                param.type = float
-            case DootParamSpec(type="bool"):
-                param.type = bool
-            case DootParamSpec(type="str"):
-                param.type = str
-            case DootParamSpec(type="list"):
-                param.type = list
-
-        if param.default == "None":
-            param.default = None
-
+    def build(cls:BaseModel, data:TomlGuard|dict) -> ParamSpec:
+        param =  cls.model_validate(data)
         return param
 
     @staticmethod
     def key_func(x):
         return (x.positional != 0, x.prefix)
 
-    @property
+    @field_validator("type_", mode="before")
+    def validate_type(cls, val):
+        match val:
+            case "int":
+                return int
+            case "float":
+                return float
+            case "bool":
+                return bool
+            case "str":
+                return str
+            case "list":
+                return list
+            case type():
+                return val
+            case _:
+                return Any
+
+    @field_validator("default")
+    def validate_default(cls, val):
+        match val:
+            case "None":
+                return None
+            case _:
+                 return val
+
+    @ftz.cached_property
     def short(self):
         if self.positional:
             return self.name
 
         if self._short:
             return self._short
 
         return self.name[0]
 
-    @property
+    @ftz.cached_property
     def inverse(self):
         return f"no-{self.name}"
 
-    @property
+    @ftz.cached_property
     def repeatable(self):
-        return self.type in DootParamSpec._repeatable_types and not self.positional
+        return self.type_ in ParamSpec._repeatable_types and not self.positional
 
-    @property
+    @ftz.cached_property
     def key_str(self):
         if self.invisible or self.positional:
             return ""
 
         if self.prefix == doot.constants.patterns.PARAM_ASSIGN_PREFIX:
             return f"{self.prefix}{self.name}{self.separator}"
 
         return f"{self.prefix}{self.name}"
 
-    @property
+    @ftz.cached_property
     def short_key_str(self):
         if self.invisible or self.positional:
             return ""
 
         if self.prefix == doot.constants.patterns.PARAM_ASSIGN_PREFIX:
             return f"{self.prefix}{self.name[0]}{self.separator}"
 
@@ -144,15 +160,15 @@
 
     def __eq__(self, val) -> bool:
         """ test to see if a cli argument matches this param """
         if 0 < self.positional <= self._consumed:
             return False
 
         match val, self.positional:
-            case DootParamSpec(), _:
+            case ParamSpec(), _:
                 return val is self
             case str(), False:
                 [head, *_] = self._split_name_from_value(val)
                 return head in [self.name, self.short, self.inverse]
             case str(), True:
                 return not val.startswith(self.prefix)
             case str(), int():
@@ -162,17 +178,17 @@
 
     def __str__(self):
         if self.invisible:
             return ""
 
         parts = [self.key_str or f"[{self.name}]"]
 
-        parts.append(" " * (PAD-len(parts[0])))
-        match self.type:
-            case type() if self.type == bool:
+        parts.append(" " * (self._pad - len(parts[0])))
+        match self.type_:
+            case type() if self.type_ == bool:
                 parts.append(f"{'(bool)': <10}:")
             case str() if bool(self.default):
                 parts.append(f"{'(str)': <10}:")
             case str():
                 parts.append(f"{'(str)': <10}:")
             case _:
                 pass
@@ -201,22 +217,27 @@
         prefixed      = focus.startswith(self.prefix) # form of -param
         is_assign     = self.separator in focus       # form of --param=arg
         key, vals     = None, []
 
         # Figure out the key and value
         match prefixed, is_assign:
             case _, True if self.prefix != doot.constants.patterns.PARAM_ASSIGN_PREFIX:
-                raise doot.errors.DootParseError("Assignment parameters should be prefixed with the PARAM_ASSIGN_PREFIX", doot.constants.patterns.PARAM_ASSIGN_PREFIX)
-            case True, False if self.type.__name__ != "bool" and not bool(args):
-                raise doot.errors.DootParseError("key lacks a following value", focus, self.type.__name__)
+                raise doot.errors.DootParseError(
+                    "Assignment parameters should be prefixed with the PARAM_ASSIGN_PREFIX",
+                    doot.constants.patterns.PARAM_ASSIGN_PREFIX,
+                )
+            case True, False if self.type_.__name__ != "bool" and not bool(args):
+                raise doot.errors.DootParseError(
+                    "key lacks a following value", focus, self.type_.__name__
+                )
             case True, True: # --key=val
                 key, val = focus.split(self.separator)
                 key = key.removeprefix(self.prefix)
                 vals.append(val)
-            case True, False if self.type.__name__ == "bool": # --key
+            case True, False if self.type_.__name__ == "bool": # --key
                 key = focus.removeprefix(self.prefix)
             case True, False: # -key val
                 key = focus.removeprefix(self.prefix)
                 vals.append(args[1])
                 pop_count = 2
 
         return key, vals, pop_count
@@ -224,71 +245,88 @@
     def _add_non_positional_value(self, data:dict, *, key:str=None, vals:list[str]=None) -> bool:
         """ if the given value is suitable, add it into the given data
         takes separated key, values,
         and the key has had the prefix stripped
         """
         vals = vals or []
         # TODO if constraints, check against them
-        logging.debug("Matching: %s : %s : %s", self.type.__name__, key, vals)
+        logging.debug("Matching: %s : %s : %s", self.type_.__name__, key, vals)
 
         # Use type.__name__ because you can't match on type. ("case str" fails, expecting "case str()")
-        match self.type.__name__:
+        match self.type_.__name__:
             case "list":
                 if self.name not in data or data[self.name] == self.default:
                     data[self.name] = []
                 data[self.name] += vals
             case "set":
                 if self.name not in data or data[self.name] == self.default:
                     data[self.name] = set()
                 data[self.name].update(vals)
+            case "Any":
+                data[self.name] = vals[0]
             case _ if data.get(self.name, self.default) != self.default:
-                raise doot.errors.DootParseError("Trying to re-set an arg already set: %s : %s", self.name, vals)
+                raise doot.errors.DootParseError(
+                    "Trying to re-set an arg already set: %s : %s", self.name, vals
+                )
             ##-- handle bools and inversion
             case "bool" if bool(vals):
-                raise doot.errors.DootParseError("Bool Arguments shouldn't have values: %s : %s", self.name, vals)
+                raise doot.errors.DootParseError(
+                    "Bool Arguments shouldn't have values: %s : %s", self.name, vals
+                )
             case "bool" if key == self.inverse:
                 data[self.name] = False
             case "bool":
                 data[self.name] = True
             ##-- end handle bools and inversion
             case _ if not bool(vals):
-                raise doot.errors.DootParseError("Non-Bool Arguments should have values: %s : %s", self.name, vals)
+                raise doot.errors.DootParseError(
+                    "Non-Bool Arguments should have values: %s : %s", self.name, vals
+                )
             case _ if len(vals) == 1:
-                data[self.name] = self.type(vals[0])
+                data[self.name] = self.type_(vals[0])
             case _:
                 raise doot.errors.DootParseError("Can't understand value: %s : %s", self.name, vals)
 
         return data[self.name] != self.default
 
     def _add_positional_value(self, data, *, key:str=None, vals:list[str]=None) -> int:
         pop_count = 1
         end_index = None if "--" not in vals else vals.index("--")
 
         match self.positional:
-            case True if self.type != list:
+            case True if self.type_ != list:
                 data[self.name] = vals[0]
             case True:
                 consume_these      = vals[:end_index]
                 pop_count          = len(consume_these)
                 data[self.name]    = consume_these
             case 1:
-                data[self.name] = self.type(vals[0])
+                data[self.name] = self.type_(vals[0])
                 pop_count = 1
             case x:
                 t = min(x, end_index or len(vals))
                 consume_these      = vals[:t]
                 pop_count          = len(consume_these)
                 data[self.name]    = consume_these
 
         if 1 < pop_count < self.positional:
-            raise doot.errors.DootParseError("Not Enough positional args provided", self.name, self.positional, vals)
+            raise doot.errors.DootParseError(
+                "Not Enough positional args provided", self.name, self.positional, vals
+            )
         elif 1 < self.positional < pop_count:
-            raise doot.errors.DootParseError("Too Many positional args provided", self.name, self.positional, vals)
-        elif 1 < pop_count and self.type != list:
-            raise doot.errors.DootParseError("Multi positional args should be of type list", self.name, self.positional, self.type)
+            raise doot.errors.DootParseError(
+                "Too Many positional args provided", self.name, self.positional, vals
+            )
+        elif 1 < pop_count and self.type_ != list:
+            raise doot.errors.DootParseError(
+                "Multi positional args should be of type list",
+                self.name,
+                self.positional,
+                self.type_,
+            )
 
         return pop_count
 
     def maybe_consume(self, args:list[str], data:dict) -> int:
         """
           Given a list of args, possibly add a value to the data.
           operates *in place* on both the args list and the data.
```

### Comparing `doot-0.7.2/doot/_structs/sname.py` & `doot-0.8.0/doot/actions/job_actions.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,63 +15,83 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-from dataclasses import InitVar, dataclass, field
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
-import importlib
+
+import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot.enums import TaskFlags, ReportEnum
-from doot._structs.structured_name import StructuredName
-from doot._structs.task_name import DootTaskName
-from doot._structs.code_ref import DootCodeReference
-
-PAD           : Final[int] = 15
-TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
-
-@dataclass(eq=False, slots=True)
-class DootStructuredName(StructuredName):
-    """ A Complex name class for identifying tasks and classes.
+from doot.structs import DootKey, TaskSpec, TaskName, CodeReference
+from doot.actions.base_action import DootBaseAction
+from doot.actions.job_expansion import JobGenerate, JobExpandAction, JobMatchAction
+from doot.actions.job_injection import JobPrependActions, JobAppendActions, JobInjector, JobInjectPathParts, JobInjectShadowAction, JobSubNamer
+from doot.actions.job_queuing import JobQueueAction, JobQueueHead, JobChainer
+from doot.mixins.path_manip import Walker_m
+
+
+class JobWalkAction(Walker_m, DootBaseAction):
+    """
+      Triggers a directory walk to build tasks from
+    """
+
+    @DootKey.dec.types("roots", "exts")
+    @DootKey.dec.types("recursive", hint={"type_": bool|None})
+    @DootKey.dec.references("fn")
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, roots, exts, recursive, fn, _update):
+        exts    = {y for x in (exts or []) for y in [x.lower(), x.upper()]}
+        rec     = recursive or False
+        roots   = [DootKey.build(x).to_path(spec, state) for x in roots]
+        match fn:
+            case CodeReference():
+                accept_fn = fn.try_import()
+            case None:
+                accept_fn = lambda x: True
 
-      Classes are the standard form used in importlib: "module.path:ClassName"
-      Tasks use a double colon to separate head from tail name: "group.name::TaskName"
+        results = [x for x in self.walk_all(roots, exts, rec=rec, fn=accept_fn)]
+        return { _update : results }
+
+class JobLimitAction(DootBaseAction):
+    """
+      Limits a list to an amount, overwriting the 'from' key,
+      'method' defaults to a random sample,
+      or a coderef of type callable[[spec, state, list[taskspec]], list[taskspec]]
 
     """
-    head            : list[str]          = field(default_factory=list)
-    tail            : list[str]          = field(default_factory=list)
 
-    separator       : str                = field(default=doot.constants.patterns.TASK_SEP, kw_only=True)
-    subseparator    : str                = field(default=".", kw_only=True)
+    @DootKey.dec.types("from_", "count")
+    @DootKey.dec.references("method")
+    @DootKey.dec.redirects("from_")
+    def __call__(self, spec, state, _from, count, method, _update):
+        if count == -1:
+            return
+
+        match method:
+            case None:
+                limited = random.sample(_from, count)
+            case CodeReference():
+                fn      = method.try_import()
+                limited = fn(spec, state, _from)
 
-    @staticmethod
-    def build(name:str|DootStructuredName|type) -> DootStructuredName:
-        match name:
-            case DootStructuredName():
-                return name
-            case type():
-                return DootCodeReference.build(name)
-            case str() if doot.constants.patterns.TASK_SEP in name:
-                return DootTaskName.build(name)
-            case str() if doot.constants.patterns.IMPORT_SEP in name:
-                return DootTaskName.build(name)
-            case _:
-                raise doot.errors.DootError("Tried to build a name from a bad value", name)
+        return { _update : limited }
```

### Comparing `doot-0.7.2/doot/_structs/structured_name.py` & `doot-0.8.0/doot/_structs/structured_name.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,102 +32,136 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from pydantic import BaseModel, Field, field_validator
 import importlib
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.enums import TaskFlags, ReportEnum
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
+TailEntry     : TypeAlias  = str|int|UUID
 
-def aware_splitter(x, sep="."):
+def aware_splitter(x, sep=".") -> list[str]:
     match x:
         case str():
             return x.split(sep)
         case _:
             return [x]
 
-@dataclass(eq=False, slots=True)
-class StructuredName:
+class StructuredName(BaseModel):
     """ A Complex name class for identifying tasks and classes.
 
       Classes are the standard form used in importlib: "module.path:ClassName"
       Tasks use a double colon to separate head from tail name: "group.name::TaskName"
 
     """
-    head            : list[str]          = field(default_factory=list)
-    tail            : list[str|UUID]     = field(default_factory=list)
+    head             : list[str]              = []
+    tail             : list[TailEntry]        = []
 
-    separator       : str                = field(default=doot.constants.patterns.TASK_SEP, kw_only=True)
-    subseparator    : str                = field(default=".", kw_only=True)
+    _separator       : ClassVar[str]          = doot.constants.patterns.TASK_SEP
+    _subseparator    : ClassVar[str]          = "."
 
-    def __post_init__(self):
-        sub_split = ftz.partial(aware_splitter, sep=self.subseparator)
-        match self.head:
+    @staticmethod
+    def build(val:str) -> StructuredName:
+        match val.split(StructuredName._separator):
+            case [head, tail]:
+                return StructuredName(head=[head], tail=[tail])
+            case _:
+                raise ValueError("Bad value for building a name from", val)
+
+    @field_validator("head", mode="before")
+    def _process_head(cls, head):
+        sub_split = ftz.partial(aware_splitter, sep=cls._subseparator)
+        match head:
             case None | []:
-                self.head = ["default"]
+                head = ["default"]
             case ["tasks", x] if x.startswith('"') and x.endswith('"'):
-                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, x[1:-1]))
+                head = ftz.reduce(lambda x, y: x + y, map(sub_split, x[1:-1]))
             case ["tasks", *xs]:
-                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, xs))
+                head = ftz.reduce(lambda x, y: x + y, map(sub_split, xs))
             case list():
-                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, self.head))
-            case str():
-                self.head = self.head.split(self.subseparator)
+                head = ftz.reduce(lambda x, y: x + y, map(sub_split, head))
             case _:
-                self.head = [self.head]
+                raise ValueError("Bad Head Value", head)
+
+        return head
 
-        match self.tail:
+    @field_validator("tail", mode="before")
+    def _process_tail(cls, tail):
+        sub_split = ftz.partial(aware_splitter, sep=cls._subseparator)
+        match tail:
             case None | []:
-                self.tail = ["default"]
+                tail = ["default"]
             case list():
-                self.tail = ftz.reduce(lambda x, y: x + y, map(sub_split, self.tail))
-            case str():
-                self.tail = self.tail.split(self.subseparator)
+                tail = ftz.reduce(lambda x, y: x + y, map(sub_split, tail))
             case _:
-                self.tail = [self.tail]
+                raise ValueError("Bad Tail Value", tail)
+        return tail
 
     def __hash__(self):
         return hash(str(self))
 
     def __str__(self):
-        return self.head_str + self.separator + self.tail_str
+        return self._separator.join([self.head_str(), self.tail_str()])
+
+    def __eq__(self, other):
+        return str(self) == str(other)
 
     def __lt__(self, other) -> bool:
-        """ Compare two names, return true if other is a subname of this name
-        eg: a.b.c < a.b.c.d
+        """ test for hierarhical ordering of names
+        eg: self(a.b.c) < other(a.b.c.d)
+        ie: other ∈ self
         """
         match other:
             case str():
                 other = StructuredName.build(other)
             case StructuredName():
                 pass
             case _:
                 return False
 
+        if len(self.head) != len(other.head):
+            return False
+        if len(self.tail) >= len(other.tail):
+            return False
+
         for x,y in zip(self.head, other.head):
             if x != y:
                 return False
 
         for x,y in zip(self.tail, other.tail):
             if x != y:
                 return False
 
         return True
 
-    def __contains__(self, other:str):
-        return str(other) in str(self)
+    def __le__(self, other) -> bool:
+        return (self == other) or (self < other)
 
-    def __eq__(self, other):
-        return str(self) == str(other)
+    def __contains__(self, other) -> bool:
+        """ test for conceptual containment of names
+        other(a.b.c) ∈ self(a.b) ?
+        ie: self < other
+        """
+        match other:
+            case str():
+                return other in str(self)
+            case StructuredName() if len(self.tail) > len(other.tail):
+                # a.b.c.d is not in a.b
+                return False
+            case StructuredName():
+                head_matches = all(x==y for x,y in zip(self.head, other.head))
+                tail_matches = all(x==y for x,y in zip(self.tail, other.tail))
+                return head_matches and tail_matches
 
-    def tail_str(self):
-        return self.subseparator.join(str(x) for x in self.tail)
+    def tail_str(self) -> str:
+        return self._subseparator.join(str(x) for x in self.tail)
 
-    def head_str(self):
-        return self.subseparator.join(str(x) for x in self.head)
+    def head_str(self) -> str:
+        return self._subseparator.join(str(x) for x in self.head)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doot-0.7.2/doot/_structs/stub.py` & `doot-0.8.0/doot/_structs/stub.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,63 +32,82 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from typing import GenericAlias
+from pydantic import BaseModel, Field, model_validator, field_validator, InstanceOf
 import importlib
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.enums import TaskFlags, ReportEnum, LocationMeta, TaskQueueMeta
-from doot._structs.task_name import DootTaskName
-from doot._structs.code_ref import DootCodeReference
-from doot._structs.task_spec import DootTaskSpec
-from doot._abstract.structs import StubStruct_p
+from doot._structs.task_name import TaskName
+from doot._structs.code_ref import CodeReference
+from doot._structs.task_spec import TaskSpec
+from doot._abstract.protocols import StubStruct_p
 
-PAD           : Final[int]               = 15
 TaskFlagNames : Final[str]               = [x.name for x in TaskFlags]
-DEFAULT_CTOR  : Final[DootCodeReference] = DootCodeReference.build(doot.aliases.task[doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS])
 
-@dataclass
-class TaskStub(StubStruct_p):
+DEFAULT_CTOR  : Final[CodeReference] = CodeReference.build(doot.aliases.task[doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS])
+
+class TaskStub(BaseModel, arbitrary_types_allowed=True):
     """ Stub Task Spec for description in toml
-    Automatically Adds default keys from DootTaskSpec
+    Automatically Adds default keys from TaskSpec
 
     This essentially wraps a dict, adding toml stubs parts as you access keys.
     eg:
     obj = TaskStub()
     ob["blah"].type = "int"
 
     # str(obj) -> will now generate toml, including a "blah" key
 
     """
-    ctor       : str|DootCodeReference|type                     = field(default=DEFAULT_CTOR)
-    parts      : dict[str, TaskStubPart]                        = field(default_factory=dict, kw_only=True)
+    ctor       : str|CodeReference|type                     = DEFAULT_CTOR
+    parts      : dict[str, TaskStubPart]                        = {}
 
-    # Don't copy these from DootTaskSpec blindly
+    # Don't copy these from TaskSpec blindly
     skip_parts : ClassVar[set[str]]          = set(["name", "extra", "ctor", "source", "version"])
 
-    def __post_init__(self):
-        self['name'].default     = DootTaskName.build(doot.constants.names.DEFAULT_STUB_TASK_NAME)
+    @classmethod
+    def build(cls, data:None|dict=None):
+        match data:
+            case None:
+                return TaskStub()
+            case _:
+                return TaskStub.model_validate(data)
+
+    @model_validator(mode="after")
+    def initial_values(self):
+        self['name'].default     = TaskName.build(doot.constants.names.DEFAULT_STUB_TASK_NAME)
         self['version'].default  = "0.1"
         # Auto populate the stub with what fields are defined in a TaskSpec:
-        for dcfield in DootTaskSpec.__dataclass_fields__.values():
-            if dcfield.name in TaskStub.skip_parts:
+        for dcfield, data in TaskSpec.model_fields.items():
+            if dcfield in TaskStub.skip_parts:
                 continue
-            self.parts[dcfield.name] = TaskStubPart(key=dcfield.name, type=dcfield.type)
-            if dcfield.default != MISSING:
-                self.parts[dcfield.name].default = dcfield.default
+
+            self.parts[dcfield] = TaskStubPart(key=dcfield, type_=data.annotation)
+            if data.default_factory is not None:
+                self.parts[dcfield].default = data.default_factory()
+            else:
+                self.parts[dcfield].default= data.default
+
+
+        return self
 
     def __getitem__(self, key):
         if key not in self.parts:
-            self.parts[key] = TaskStubPart(key)
+            self.parts[key] = TaskStubPart(key=key)
         return self.parts[key]
 
+    def __contains__(self, key):
+        return key in self.parts
+
     def __iadd__(self, other):
         match other:
             case [head, val] if head in self.parts:
                 self.parts[head].default = val
             case [head, val]:
                 self.parts[head] = TaskStubPart(head, default=val)
             case { "name" : name, "type": type, "default": default, "doc": doc, }:
@@ -108,17 +127,17 @@
         parts = []
         parts.append(self.parts['name'])
         parts.append(self.parts['version'])
         parts.append(self.parts['doc'])
         if 'ctor' in self.parts:
             parts.append(self.parts['ctor'])
         elif isinstance(self.ctor, type):
-            parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor.__module__}{doot.constants.patterns.IMPORT_SEP}{self.ctor.__name__}\""))
+            parts.append(TaskStubPart(key="ctor", type_="type", default=f"\"{self.ctor.__module__}{doot.constants.patterns.IMPORT_SEP}{self.ctor.__name__}\""))
         else:
-            parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor}\""))
+            parts.append(TaskStubPart(key="ctor", type_="type", default=f"\"{self.ctor}\""))
 
         delayed_actions = []
         for key, part in sorted(self.parts.items(), key=lambda x: x[1]):
             if key in ["name", "version", "ctor", "doc"]:
                 continue
             if 'actions' in key:
                 delayed_actions.append(part)
@@ -127,87 +146,99 @@
 
         # Actions always go at the end
         for part in delayed_actions:
             parts.append(part)
 
         return "\n".join(map(str, parts))
 
-@dataclass
-class TaskStubPart:
+class TaskStubPart(BaseModel, arbitrary_types_allowed=True):
     """ Describes a single part of a stub task in toml """
-    key      : str      = field()
-    type     : str      = field(default="str")
-    prefix   : str      = field(default="")
-
-    default  : Any      = field(default="")
-    comment  : str      = field(default="")
-    priority : int      = field(default=0)
+    key       : str
+    type_     : str|InstanceOf[type]|Any       = "str"
+    prefix    : str                            = ""
+
+    default   : Any                            = Field(default="Undefined")
+    comment   : str                            = ""
+    priority  : int                            = 0
+
 
     def __lt__(self, other):
         return self.priority < other.priority
 
     def __str__(self) -> str:
         """
           the main conversion method of a stub part -> toml string
           the match statement handles the logic of different types.
           eg: lowercasing the python bool from False to false for toml
         """
         # shortcut on being the name:
-        if isinstance(self.default, DootTaskName) and self.key == "name":
+        if isinstance(self.default, TaskName) and self.key == "name":
             return f"[[tasks.{self.default.group}]]\n{'name':<20} = \"{self.default.task}\""
 
-        key_str     = f"{self.key:<20}"
-        type_str    = f"<{self.type}>"
-        comment_str = f"{self.comment}"
-        val_str     = None
+        key_str     = self._key_str()
+        type_str    = self._type_str()
+        comment_str = self._comment_str()
+        val_str     = self._default_str()
+
+        return f"{self.prefix}{key_str} = {val_str:<20} # {type_str:<20} # {comment_str}"
 
+    def set(self, **kwargs):
+        self.type_     = kwargs.get('type_', self.type_)
+        self.prefix    = kwargs.get('prefix', self.prefix)
+        self.default   = kwargs.get('default', self.default)
+        self.comment   = kwargs.get('comment', self.comment)
+        self.priority  = kwargs.get('priority', self.priority)
+
+    def _key_str(self) -> str:
+        return f"{self.key:<20}"
+
+    def _type_str(self) -> str:
+        match type(self.type_), self.type_:
+            case x, t if x == GenericAlias and bool(t.__args__) and hasattr(t.__args__[0], "__args__"):
+                args = self.type_.__args__[0].__args__
+                args_s = " | ".join(arg.__name__ for arg in args)
+                return f"<{self.type_.__name__}[{args_s}]>"
+            case _, t if hasattr(t, "__name__"):
+                return f"<{self.type_.__name__}>"
+            case _, _:
+                return f"<{self.type_}>"
+
+    def _comment_str(self) -> str:
+        return f"{self.comment}"
+
+    def _default_str(self) -> str:
         match self.default:
-            case TaskFlags() | LocationMeta():
+            case "" if isinstance(self.type_, enum.EnumMeta):
+                val_str = f'[ "{self.type_.default.name}" ]'
+            case enum.Flag(): # TaskFlags() | LocationMeta():
                 parts = [x.name for x in TaskFlags if x in self.default]
                 joined = ", ".join(map(lambda x: f"\"{x}\"", parts))
                 val_str = f"[ {joined} ]"
             case TaskQueueMeta():
                 val_str = '"{}"'.format(self.default.name)
-            case "" if self.type == "TaskFlags":
-                val_str = f"[ \"{TaskFlags.TASK.name}\" ]"
             case bool():
                 val_str = str(self.default).lower()
-            case str() if self.type == "type":
+            case str() if self.type_ == "type":
                 val_str = self.default
-            case list() if "Flags" in self.type:
-                parts = ", ".join([f"\"{x}\"" for x in self.default])
-                val_str = f"[{parts}]"
-            case list() if all(isinstance(x, (int, float)) for x in self.default):
-
-                def_str = ", ".join(str(x) for x in self.default)
-                val_str = f"[{def_str}]"
-            case list():
-
-                def_str = ", ".join([f'"{x}"' for x in self.default])
-                val_str = f"[{def_str}]"
-            case dict():
-                val_str = "{}"
-            case _ if "list" in self.type:
-
-                def_str = ", ".join(str(x) for x in self.default)
-                val_str = f"[{def_str}]"
-            case _ if "dict" in self.type:
-                val_str = f"{{{self.default}}}"
             case int() | float():
                 val_str = f"{self.default}"
             case str() if "\n" in self.default:
                 flat = self.default.replace("\n", "\\n")
-                val_str = f"\"{flat}\""
+                val_str = f'"{flat}"'
             case str():
-                val_str = f"\"{self.default}\""
-
-        if val_str is None:
-            raise TypeError("Unknown stub part reduction:", self)
+                val_str = f'"{self.default}"'
+            case list() if all(isinstance(x, (int, float)) for x in self.default):
 
-        return f"{self.prefix}{key_str} = {val_str:<20} # {type_str:<20} {comment_str}"
+                def_str = ", ".join(str(x) for x in self.default)
+                val_str = f"[{def_str}]"
+            case list():
+                parts = ", ".join([f'"{x}"' for x in self.default])
+                val_str = f"[{parts}]"
+            case dict() | TomlGuard() if not bool(self.default):
+                val_str = "{}"
+            case _:
+                logging.debug("Unknown stub part reduction: %s : %s : %s", self.key, self.type_, self.default)
+                breakpoint()
+                pass
+                val_str = '"unknown"'
 
-    def set(self, **kwargs):
-        self.type     = kwargs.get('type', self.type)
-        self.prefix   = kwargs.get('prefix', self.prefix)
-        self.default  = kwargs.get('default', self.default)
-        self.comment  = kwargs.get('comment', self.comment)
-        self.priority = kwargs.get('priority', self.priority)
+        return val_str
```

### Comparing `doot-0.7.2/doot/_structs/task_spec.py` & `doot-0.8.0/doot/control/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,272 @@
 #!/usr/bin/env python3
 """
 
-See EOF for license/metadata/notes as applicable
 """
-
-##-- builtin imports
+# Imports:
 from __future__ import annotations
 
-# import abc
+# ##-- stdlib imports
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
-# from copy import deepcopy
-from dataclasses import InitVar, dataclass, field, _MISSING_TYPE
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+from collections import defaultdict
+from contextlib import nullcontext
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Self, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 
-##-- end builtin imports
+# ##-- end stdlib imports
 
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+# ##-- 3rd party imports
+import networkx as nx
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end 3rd party imports
 
-import importlib
-from importlib.metadata import EntryPoint
-from tomlguard import TomlGuard
+# ##-- 1st party imports
 import doot
 import doot.errors
-from doot.enums import TaskFlags, ReportEnum, TaskQueueMeta
-from doot._structs.sname import DootTaskName, DootCodeReference
-from doot._structs.action_spec import DootActionSpec
-from doot._structs.artifact import DootTaskArtifact
-from doot._structs.toml_loc import TomlLocation
-from doot._abstract.structs import SpecStruct_p
-
-PAD           : Final[int] = 15
-
-# TODO: taskspec.setup, taskspec.cleanup, taskspec.on_fail
-
-def _separate_into_core_and_extra(data) -> tuple[dict, dict]:
-    core_keys   = list(DootTaskSpec.__dataclass_fields__.keys())
-    core_data, extra_data = dict(), dict()
-    # Integrate extras, normalize keys
-    for key, val in data.items():
-        if "-" in key:
-            key = key.replace("-","_")
-        match key:
-            case "extra" if val is not None:
-                extra_data.update(dict(val))
-            case "extra":
-                pass
-            case "print_levels":
-                core_data["print_levels"] = TomlGuard(val)
-            case "required_for":
-                processed = _prepare_deps(val)
-                core_data["required_for"] = processed
-            case "depends_on":
-                processed = _prepare_deps(val)
-                core_data["depends_on"] = processed
-            case "setup":
-                processed = _prepare_deps(val)
-                core_data["setup"] = processed
-            case "cleanup":
-                processed = _prepare_deps(val)
-                core_data["cleanup"] = processed
-            case "on_fail":
-                processed = _prepare_deps(val)
-                core_data["on_fail"] = processed
-            case "queue_behaviour":
-                as_enum = TaskQueueMeta.build(val)
-                core_data["queue_behaviour"] = as_enum
-            case x if x in core_keys:
-                core_data[x] = val
-            case x if x not in ["name", "group"]:
-                extra_data[key] = val
-
-    return core_data, extra_data
-
-def _prepare_deps(deps:None|list[str], source=None) -> list[DootTaskArtifact|DootTaskName]:
-    """
-      Prepares dependencies, converting from strings to Artifacts (ie:files), or Task Names
-      # TODO handle callables?
-    """
-    if deps is None:
-        return []
-
-    results = []
-    for x in deps:
-        match x:
-            case { "do": action  }:
-                results.append(DootActionSpec.build(x))
-            case { "loc": filename }:
-                results.append(DootTaskArtifact.build(x))
-            case str() if x.startswith(doot.constants.patterns.FILE_DEP_PREFIX):
-                results.append(DootTaskArtifact.build(x))
-            case str() if doot.constants.patterns.TASK_SEP in x:
-                results.append(DootTaskName.build(x))
-            case DootTaskName() | DootTaskArtifact() | DootActionSpec():
-                results.append(x)
-            case _:
-                raise doot.errors.DootInvalidConfig(f"Unrecognised task pre/post dependency form. (Remember: files are prefixed with `{doot.constants.patterns.FILE_DEP_PREFIX}`, tasks are in the form group::name)", x, source)
-
-    return results
+from doot._abstract import (Action_p, FailPolicy_p, Job_i, Reporter_p, Task_i,
+                            TaskRunner_i, TaskTracker_i)
+from doot._structs.relation_spec import RelationSpec
+from doot.control.base_runner import BaseRunner, logctx
+from doot.enums import ActionResponseEnum as ActRE
+from doot.enums import ReportEnum
+from doot.structs import ActionSpec, TaskArtifact, TaskName, TaskSpec
+from doot.utils.signal_handler import SignalHandler
 
-def _prepare_ctor(ctor, mixins) -> DootTaskName|DootCodeReference:
-    match ctor:
-        case None:
-            default_alias = doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS
-            coderef_str   = doot.aliases.task[default_alias]
-            return DootCodeReference.build(coderef_str).add_mixins(*mixins)
-        case EntryPoint():
-            return DootCodeReference.build(ctor).add_mixins(*mixins)
-        case DootTaskName() if bool(mixins):
-            raise TypeError("Task name ctor can't take mixins")
-        case DootTaskName():
-            return ctor
-        case DootCodeReference() if not bool(ctor._mixins):
-            return ctor.add_mixins(*mixins)
-        case DootCodeReference():
-            return ctor
-        case type():
-            return DootCodeReference.build(ctor).add_mixins(*mixins)
-        case str():
-            return DootCodeReference.build(ctor).add_mixins(*mixins)
-        case _:
-            return DootCodeReference.build(ctor).add_mixins(*mixins)
-
-@dataclass
-class DootTaskSpec(SpecStruct_p):
-    """ The information needed to describe a generic task.
-    Optional things are shoved into 'extra', so things can use .on_fail on the tomlguard
-
-    the cli parser can understand cli=[{}] specs
-    actions                      : list[ [args] | {do="", args=[], **kwargs} ]
-
-    """
-    name                         : DootTaskName                                                            = field()
-    doc                          : list[str]                                                               = field(default_factory=list)
-    source                       : DootTaskName|str|None                                                   = field(default=None)
-    actions                      : list[DootActionSpec]                                                    = field(default_factory=list)
-
-    required_for                 : list[DootTaskName|DootTaskArtifact]                                     = field(default_factory=list)
-    depends_on                   : list[DootTaskName|DootTaskArtifact|DootActionSpec]                      = field(default_factory=list)
-    setup                        : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
-    cleanup                      : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
-    on_fail                      : list[DootTaskName|DootAcitonSpec]                                       = field(default_factory=list)
-    priority                     : int                                                                     = field(default=10)
-    ctor                         : DootTaskName|DootCodeReference                                          = field(default=None)
-    # Any additional information:
-    version                      : str                                                                     = field(default=doot.__version__)
-    # TODO version               : dict                                                                    = field(default_factory=dict)
-    print_levels                 : TomlGuard                                                               = field(default_factory=TomlGuard)
-    flags                        : TaskFlags                                                               = field(default=TaskFlags.TASK)
-
-    extra                        : TomlGuard                                                               = field(default_factory=TomlGuard)
-
-    queue_behaviour              : TaskQueueMeta                                                 = field(default=TaskQueueMeta.default)
-
-    @staticmethod
-    def build(data:TomlGuard|dict|DootTaskName|str):
-        match data:
-            case TomlGuard() | dict():
-                return DootTaskSpec.from_dict(data)
-            case DootTaskName():
-                return DootTaskSpec.from_name(data)
-            case str():
-                return DootTaskSpec.from_name(DootTaskName.build(data))
-
-    @staticmethod
-    def from_dict(data:TomlGuard|dict):
-        """ builds a task spec from a raw dict
-          able to handle a name:str = "group::task" form,
-          able to convert TaskFlag str's into an or'd enum value
-          """
-        core_data, extra_data = _separate_into_core_and_extra(data)
+# ##-- end 1st party imports
 
-        core_data['name']     = DootTaskName.build(data)
-        core_data['flags']    = TaskFlags.build(core_data.get("flags", []))
+##-- logging
+logging       = logmod.getLogger(__name__)
+printer       = logmod.getLogger("doot._printer")
+fail_l        = printer.getChild("fail")
+skip_l        = printer.getChild("skip")
+task_header_l = printer.getChild("task_header")
+actgrp_l      = printer.getChild("action_group")
+queue_l       = printer.getChild("queue")
+actexec_l     = printer.getChild("action_exec")
+state_l       = printer.getChild("task_state")
+##-- end logging
 
-        # Prepare constructor
-        core_data['ctor'] = _prepare_ctor(data.get("ctor",None), [])
+head_level              : Final[str] = doot.constants.printer.DEFAULT_HEAD_LEVEL
+build_level             : Final[str] = doot.constants.printer.DEFAULT_BUILD_LEVEL
+action_level            : Final[str] = doot.constants.printer.DEFAULT_ACTION_LEVEL
+sleep_level             : Final[str] = doot.constants.printer.DEFAULT_SLEEP_LEVEL
+execute_level           : Final[str] = doot.constants.printer.DEFAULT_EXECUTE_LEVEL
+skip_msg                : Final[str] = doot.constants.printer.skip_by_condition_msg
+actgrp_prefix           : Final[str] = doot.constants.printer.action_group_prefix
+fail_prefix             : Final[str] = doot.constants.printer.fail_prefix
+max_steps               : Final[str] = doot.config.on_fail(100_000).settings.tasks.max_steps()
+
+@doot.check_protocol
+class DootRunner(BaseRunner, TaskRunner_i):
+    """ The simplest single threaded task runner """
+
+    def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_p):
+        super().__init__(tracker=tracker, reporter=reporter)
+        self.teardown_list  = []                     # list of tasks to teardown
+
+    def __call__(self, *tasks:str, handler=None):
+        """ tasks are initial targets to run.
+          so loop on the tracker, getting the next task,
+          running its actions,
+          and repeating,
+          until done
 
-        # prep actions
-        core_data['actions'] = [DootActionSpec.build(x) for x in core_data.get('actions', [])]
-
-        task = DootTaskSpec(**core_data, extra=TomlGuard(extra_data))
-        return task
-
-    @staticmethod
-    def from_name(name:DootTaskName):
-        match name:
-            case DootTaskName() if bool(name.args):
-                spec_dict = name.args.copy()
-                spec_dict['name'] = str(name)
-                return DootTaskSpec.from_dict(spec_dict)
-            case DootTaskName():
-                return DootTaskSpec.from_dict({"name": name})
+          if task is a job, it is expanded and added into the tracker
+          """
+        match handler:
+            case None | True:
+                handler = SignalHandler()
+            case type() as x:
+                handler = x()
+            case x if hasattr(x, "__enter__"):
+                handler = x
             case _:
-                raise TypeError("Bad Type used to build a task spec", name)
+                handler = nullcontext()
+
+        with handler:
+            while bool(self.tracker) and self.step < max_steps:
+                self._run_next_task()
 
-    def specialize_from(self, data:DootTaskSpec) -> DootTaskSpec:
+    def _run_next_task(self):
         """
-          Specialize an existing task spec, with additional data
+          Get the next task from the tracker, expand/run it,
+          and handle the result/failure
         """
-        if not self.name == data.ctor:
-            raise doot.errors.DootTaskTrackingError("Tried to specialize a task that isn't based on this task", str(data.name), str(self.name))
-        specialized = {}
-        for field in DootTaskSpec.__annotations__.keys():
-            match field:
-                case "name":
-                    specialized[field] = data.name.specialize()
-                case "extra":
-                   specialized[field] = TomlGuard.merge(data.extra, self.extra, shadow=True)
-                case "ctor":
-                    specialized[field] = self.ctor
-                case "actions":
-                    specialized[field] = self.actions + data.actions
-                case "depends_on":
-                    specialized["depends_on"] = self.depends_on[:] + data.depends_on[:]
-                case "required_for":
-                    specialized["required_for"] = self.required_for[:] + data.required_for[:]
-                case "cleanup":
-                    specialized["cleanup"] = self.cleanup[:] + data.cleanup[:]
-                case "on_fail":
-                    specialized["on_fail"] = self.on_fail[:] + data.on_fail[:]
-                case "setup":
-                    specialized["setup"] = self.setup[:] + data.setup[:]
+        task = None
+        try:
+            match (task:=self.tracker.next_for()):
+                case None:
+                    pass
+                case TaskArtifact():
+                    self._notify_artifact(task)
+                    raise doot.errors.DootTaskFailed("Artifact resolutely does not exist", task=task)
+                case Job_i() if self._test_conditions(task):
+                    self._expand_job(task)
+                case Task_i() if self._test_conditions(task):
+                    self._execute_task(task)
+                case Task_i():
+                    # test_conditions failed, so skip
+                    skip_l.info(skip_msg, self.step, task.shortname)
                 case _:
-                    # prefer the newest data, then the unspecialized data, then the default
-                    field_data         = DootTaskSpec.__dataclass_fields__.get(field)
-                    match getattr(data,field), field_data.default, field_data.default_factory:
-                        case x, _MISSING_TYPE(), y if y == TomlGuard:
-                            value = TomlGuard.merge(getattr(data,field), getattr(self, field), shadow=True)
-                        case x, _MISSING_TYPE(), _MISSING_TYPE():
-                            value = x or getattr(self, field)
-                        case x, y, _MISSING_TYPE() if x == y:
-                            value = getattr(self, field)
-                        case x, _, _MISSING_TYPE():
-                            value = x
-                        case x, _MISSING_TYPE(), _ if bool(x):
-                            value = x
-                        case x, _MISSING_TYPE(), _:
-                            value = getattr(self, field)
-                        case x, y, z:
-                            raise TypeError("Unknown Task Spec Specialization field types", field, x, y, z)
-
-                    specialized[field] = value
-
-        logging.debug("Specialized Task: %s on top of: %s", data.name.readable, self.name)
-        return DootTaskSpec.build(specialized)
-
-    def make(self, ensure=Any) -> Task_i:
-        """ Create actual task instance """
-        task_ctor = self.ctor.try_import(ensure=ensure)
-        return task_ctor(self)
-
-    def check(self, ensure=Any):
-        if self.ctor.module == "default":
-            return True
-        self.ctor.try_import(ensure=ensure)
-        return True
-
-    def __hash__(self):
-        return hash(str(self.name))
-
-    @property
-    def params(self):
-        return self.extra
-
-    @property
-    def action_groups(self):
-        return [self.depends_on, self.setup, self.actions, self.cleanup, self.on_fail]
+                    pass
+        except doot.errors.DootError as err:
+            self._handle_failure(task, err)
+        except Exception as err:
+            fail_l.exception("Unknown, non-Doot failure occurred: %s", err)
+            self.tracker.clear_queue()
+            raise err
+        else:
+            self._handle_task_success(task)
+            self._sleep(task)
+            self.step += 1
+
+    def _expand_job(self, job:Job_i) -> None:
+        """ turn a job into all of its tasks, including teardowns """
+        try:
+            logmod.debug("-- Expanding Job %s: %s", self.step, job.shortname)
+            task_header_l.info("> Job %s: %s", self.step, job.shortname, extra={"colour":"magenta"})
+            # TODO queue $head$ ?
+
+            self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.INIT)
+
+            self._execute_action_group(job.spec.setup, job, group="setup")
+            self._execute_action_group(job.spec.actions, job, allow_queue=True, group="actions")
+
+        except doot.errors.DootError as err:
+            self._execute_action_group(job.spec.on_fail, job, group="on_fail")
+            raise err
+        finally:
+            # cleanup actions are *not* run here, as they've been added to the auto-gen $head$ and queued
+            job.state.clear()
+            self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.SUCCEED)
+            task_header_l.info("< Job %s: %s", self.step, job.shortname, extra={"colour":"magenta"})
+
+    def _execute_task(self, task:Task_i) -> None:
+        """ execute a single task's actions """
+        try:
+            task_header_l.info("> Task %s :  %s", self.step, task.shortname, extra={"colour":"magenta"})
+            self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.INIT)
+
+            self._execute_action_group(task.spec.setup, task, group="setup")
+            self._execute_action_group(task.spec.actions, task, group="action")
+            self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.SUCCEED)
+        except doot.errors.DootError as err:
+            self._execute_action_group(task.spec.on_fail, task, group="on_fail")
+            raise err
+        finally:
+            # Cleanup Actions *are* run here, because tasks don't have subtasks they setup for
+            self._execute_action_group(task.spec.cleanup, task, group="cleanup")
+            task.state.clear()
+            task_header_l.debug("< Task: %s", task.shortname, extra={"colour":"cyan"})
+
+    def _execute_action_group(self, actions:list, task:Task_i, allow_queue=False, group=None) -> tuple[int, ActRE]:
+        """ Execute a group of actions, possibly queue any task specs they produced,
+        and return a count of the actions run + the result
+        """
+        actgrp_l.info("%s Action Group %s (%s) for : %s", actgrp_prefix, group, len(actions), task.shortname)
+        group_result     = ActRE.SUCCESS
+        to_queue         = []
+        executed_count   = 0
+
+        for action in actions:
+            result : None|bool|list = None
+            match action:
+                case RelationSpec():
+                    pass
+                case ActionSpec():
+                    result = self._execute_action(executed_count, action, task)
+                case _:
+                    self.reporter.add_trace(task.spec, flags=ReportEnum.FAIL | ReportEnum.TASK)
+                    raise doot.errors.DootTaskError("Task %s Failed: Produced a bad action: %s", task.shortname, repr(action), task=task.spec)
+
+            match result:
+                case True:
+                    continue
+                case False:
+                    group_result = ActRE.FAIL
+                    break
+                case None:
+                    continue
+                case list():
+                    to_queue += result
+                case ActRE.SKIP:
+                    skip_l.warning("------ Remaining Task Actions skipped by Action Result")
+                    group_result = ActRE.SKIP
+                    break
+
+            executed_count += 1
+
+        else: # runs only if no 'break'
+            match to_queue:
+                case []:
+                    pass
+                case [*xs] if not allow_queue:
+                    fail_l.warning("%s Tried to Queue additional tasks from a bad action group: %s", fail_prefix, task)
+                    group_result = ActRE.FAIL
+                case [*xs]:
+                    for spec in xs:
+                        self.tracker.queue_entry(spec)
+                    self.tracker.build_network()
+                    queue_l.info("Queued %s Subtasks for %s", len(xs), task.shortname)
+
+        return executed_count, group_result
+
+    def _execute_action(self, count, action, task) -> ActRE|list:
+        """ Run the given action of a specific task.
+
+          returns either a list of specs to (potentially) queue,
+          or an ActRE describing the action result.
+
+        """
+        result                     = None
+        task.state['_action_step'] = count
+        self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.INIT)
+        actexec_l.info( "Action %s.%s: %s", self.step, count, action.do or action.fun, extra={"colour":"cyan"})
+
+        actexec_l.debug("Action Executing for Task: %s", task.shortname)
+        actexec_l.debug("Action State: %s.%s: args=%s kwargs=%s. state(size)=%s", self.step, count, action.args, dict(action.kwargs), len(task.state.keys()))
+        action.verify(task.state)
+        result = action(task.state)
+        actexec_l.debug("Action Result: %s", result)
+
+        match result:
+            case ActRE.SKIP:
+                # result will be returned, and expand_job/execute_task will handle it
+                pass
+            case None | True:
+                result = ActRE.SUCCESS
+            case dict(): # update the task's state
+                state_l.info("Updating Task State: %s keys", len(result))
+                task.state.update({str(k):v for k,v in result.items()})
+                result = ActRE.SUCCESS
+            case list() if all(isinstance(x, (TaskName, TaskSpec)) for x in result):
+                pass
+            case False | ActRE.FAIL:
+                self.reporter.add_trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
+                raise doot.errors.DootTaskFailed("Task %s: Action Failed: %s", task.shortname, action.do, task=task.spec)
+            case _:
+                self.reporter.add_trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
+                raise doot.errors.DootTaskError("Task %s: Action %s Failed: Returned an unplanned for value: %s", task.shortname, action.do, result, task=task.spec)
+
+        action.verify_out(task.state)
+        self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.SUCCEED)
+        return result
+
+    def _test_conditions(self, task:Task_i) -> bool:
+        """ run a task's depends_on group, coercing to a bool """
+        match self._execute_action_group(task.spec.depends_on, task, group="depends_on"):
+            case _, ActRE.SKIP | ActRE.FAIL:
+                return False
+            case _, _:
+                return True
```

### Comparing `doot-0.7.2/doot/_structs/trace.py` & `doot-0.8.0/doot/task/specialised_jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 #!/usr/bin/env python3
 """
 
-See EOF for license/metadata/notes as applicable
 """
-
-##-- builtin imports
+##-- imports
 from __future__ import annotations
 
 # import abc
-import datetime
-import enum
+# import datetime
+# import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
 # from copy import deepcopy
-from dataclasses import InitVar, dataclass, field
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
-from uuid import UUID, uuid1
-
-##-- end builtin imports
+                    cast, final, overload, runtime_checkable)
+# from uuid import UUID, uuid1
+# from weakref import ref
 
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import importlib
-from tomlguard import TomlGuard
-import doot.errors
-from doot.enums import TaskFlags, ReportEnum
-
-PAD           : Final[int] = 15
-TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
-
-@dataclass
-class DootTraceRecord:
-    message : str                      = field()
-    flags   : None|ReportEnum          = field()
-    args    : list[Any]                = field(default_factory=list)
-    time    : datetime.datetime        = field(default_factory=datetime.datetime.now)
+import doot
+from doot.task.base_job import DootJob
 
-    def __str__(self):
-        match self.message:
-            case str():
-                return self.message.format(*self.args)
-            case DootTaskSpec():
-                return str(self.message.name)
-            case _:
-                return str(self.message)
 
-    def __contains__(self, other:ReportEnum) -> bool:
-        return all([x in self.flags for x in other])
+@doot.check_protocol
+class GroupJob(DootJob):
+    """ A Group of task specs, none of which require params """
+
+    def __init__(self, spec:TaskSpec):
+        super().__init__(spec)
+        self.name       = name.replace(" ", "_")
+        self.tasks      = list(args)
+        self.as_creator = as_creator
+
+    def __str__(self):
+        return f"group:{self.name}({len(self)})"
 
-    def __eq__(self, other:ReportEnum) -> bool:
-        return self.flags == other
+    def __len__(self):
+        return len(self.tasks)
 
-    def some(self, other:reportPositionEnum) -> bool:
-        return any([x in self.flags for x in other])
+    def __iadd__(self, other):
+        self.tasks.append(other)
+        return self
+
+    def to_dict(self):
+        # this can add jobs to the namespace,
+        # but doesn't help for dicts
+        return {f"doot_{self.name}_{id(x)}": x for x in self.tasks}
+
+    def add_tasks(self, *other):
+        for x in other:
+            self.tasks.append(other)
+
+@doot.check_protocol
+class WatchJob(DootJob):
+    """
+    Job that watches for conditions, *then*
+    generates tasks.
+    eg: a file watcher
+    """
+    pass
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_base_action.py` & `doot-0.8.0/doot/actions/__tests/test_base_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,12 +30,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_control_flow.py` & `doot-0.8.0/doot/actions/__tests/test_control_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_io.py` & `doot-0.8.0/doot/actions/__tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_job_actions.py` & `doot-0.8.0/doot/actions/__tests/test_job_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
                     TypeVar, cast)
 import warnings
 import pytest
 
 import doot
 doot._test_setup()
 import doot.errors
-from doot.structs import DootKey, DootTaskSpec, DootActionSpec, DootTaskName
+from doot.structs import DootKey, TaskSpec, ActionSpec, TaskName
 import doot.actions.job_actions as JA
 
 printer = logmod.getLogger("doot._printer")
 logging = logmod.root
 
 class TestJobActions:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     @pytest.fixture(scope="function")
     def cleanup(self):
         pass
 
     def test_initial(self, spec, state):
         jqa    = JA.JobQueueAction()
@@ -41,41 +41,41 @@
         assert(isinstance(result, list))
 
     def test_basic(self, spec, state):
         jqa    = JA.JobQueueAction()
         result = jqa(spec, state)
         assert(isinstance(result, list))
         assert(len(result) == 2)
-        assert(all(isinstance(x, DootTaskSpec) for x in result))
+        assert(all(isinstance(x, TaskSpec) for x in result))
 
     def test_basic_expander(self, spec, state):
-        state.update(dict(_task_name=DootTaskName.build("basic"),
+        state.update(dict(_task_name=TaskName.build("agroup::basic"),
                           inject={"replace":["aKey"]},
                           base="base::task"))
 
         state['from'] = ["first", "second", "third"]
         jqa    = JA.JobExpandAction()
         result = jqa(spec, state)
         assert(isinstance(result, dict))
         assert("specs" in result)
-        assert(all(isinstance(x, DootTaskSpec) for x in result['specs']))
+        assert(all(isinstance(x, TaskSpec) for x in result['specs']))
         assert(all(x.extra['aKey'] in ["first", "second", "third"] for x in result['specs']))
         assert(len(result['specs']) == 3)
 
     def test_expander_with_dict_injection(self, spec, state):
-        state.update(dict(_task_name=DootTaskName.build("basic"),
+        state.update(dict(_task_name=TaskName.build("agroup::basic"),
                           inject={"replace": ["aKey"], "copy":{"other":"blah"}},
                           base="base::task"))
 
         state['from']          = ["first", "second", "third"]
         jqa    = JA.JobExpandAction()
         result = jqa(spec, state)
         assert(isinstance(result, dict))
         assert("specs" in result)
-        assert(all(isinstance(x, DootTaskSpec) for x in result['specs']))
+        assert(all(isinstance(x, TaskSpec) for x in result['specs']))
         assert(all(x.extra['aKey'] in ["first", "second", "third"] for x in result['specs']))
         assert(all('other' in x.extra for x in result['specs']))
         assert(len(result['specs']) == 3)
 
 
 class TestJobWalker:
     @pytest.mark.skip
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_job_expansion.py` & `doot-0.8.0/doot/actions/__tests/test_job_expansion.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 logging = logmod.root
 
 import doot
 doot._test_setup()
 from doot.actions.job_expansion import JobExpandAction, JobMatchAction
 import doot.errors
-from doot.structs import DootKey, DootActionSpec, DootTaskName
+from doot.structs import DootKey, ActionSpec, TaskName
 
 class TestJobExpansion:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "expand", "args":[], "update_":"specs"})
+        return ActionSpec.build({"do": "job.expand", "args":[], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self, spec, state):
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(len(result['specs']) == 1)
@@ -53,51 +53,51 @@
         state['inject'] = {"replace": ['target']}
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(len(result['specs']) == 3)
         for spec, expect in zip(result['specs'], args):
-            assert(spec.extra.target == expect)
+            assert(spec.target == expect)
 
     def test_action_template(self, spec, state):
         state['template'] = "test::task"
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
-        assert(result['specs'][0].ctor == "test::task")
+        assert(result['specs'][0].sources == ["test::task"])
         assert(len(result['specs'][0].actions) == 0)
 
     def test_taskname_template(self, spec, state):
-        state['template'] = [{"do":"aweg"}, {"do":"blah"}, {"do":"jioj"}]
+        state['template'] = [{"do":"basic"}, {"do":"basic"}, {"do":"basic"}]
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(len(result['specs'][0].actions) == 3)
 
 class TestJobMatcher:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self):
         pass
 
 class TestJobGenerate:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self):
         pass
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_job_injection.py` & `doot-0.8.0/doot/actions/__tests/test_job_injection.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 logging = logmod.root
 
 import doot
 doot._test_setup()
 from doot.actions import job_injection as ji
 import doot.errors
-from doot.structs import DootKey, DootActionSpec, DootTaskName
+from doot.structs import DootKey, ActionSpec, TaskName
 
 class TestJobInjection:
     """
 
     """
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_copy(self, spec, state):
         """ the injection copies the value over directly """
         state.update({"a": 2})
         inj = ji.JobInjector()
         injection = inj.build_injection(spec, state, dict(copy=["a"]))
         assert("a" in injection)
@@ -95,19 +95,19 @@
         assert("a" in injection)
         assert(injection['a'] == 10)
 
 class TestPathInjection:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self, spec ,state):
         obj = ji.JobInjectPathParts()
         # build task specs
         # set roots
         # Call:
         result = obj(spec, state)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_job_queuing.py` & `doot-0.8.0/doot/actions/__tests/test_job_queuing.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,58 +15,58 @@
 
 logging = logmod.root
 
 import doot
 doot._test_setup()
 from doot.actions.job_queuing import JobQueueAction, JobQueueHead, JobChainer
 import doot.errors
-from doot.structs import DootKey, DootActionSpec, DootTaskName, DootTaskSpec
+from doot.structs import DootKey, ActionSpec, TaskName, TaskSpec
 
 class TestJobQueue:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self, spec, state):
         obj = JobQueueAction()
         result = obj(spec, state)
         assert(isinstance( result, list ))
 
     def test_from_arg(self, spec, state):
         obj = JobQueueAction()
         result = obj(spec, state)
         assert(isinstance( result, list ))
-        assert(all(isinstance(x, DootTaskSpec) for x in result))
+        assert(all(isinstance(x, TaskSpec) for x in result))
 
     def test_from_multi_arg(self, spec, state):
         obj = JobQueueAction()
         result = obj(spec, state)
         assert(isinstance( result, list ))
-        assert(all(isinstance(x, DootTaskSpec) for x in result))
+        assert(all(isinstance(x, TaskSpec) for x in result))
 
     def test_args(self, spec, state):
         obj = JobQueueAction()
         result = obj(spec, state)
         assert(isinstance( result, list ))
-        assert(all(isinstance(x, DootTaskSpec) for x in result))
+        assert(all(isinstance(x, TaskSpec) for x in result))
 
 class TestJobQueueHead:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
     def test_initial(self, spec, state):
         obj = JobQueueHead()
         result = obj(spec, state)
         assert(isinstance( result, list ))
 
 
@@ -81,18 +81,18 @@
         result = obj(spec, state)
         assert(isinstance( result, list ))
 
 class TestJobChainer:
 
     @pytest.fixture(scope="function")
     def spec(self):
-        return DootActionSpec.build({"do": "action", "args":["test::simple", "test::other"], "update_":"specs"})
+        return ActionSpec.build({"do": "basic", "args":["test::simple", "test::other"], "update_":"specs"})
 
     @pytest.fixture(scope="function")
     def state(self):
-        return {"_task_name": DootTaskName.build("basic")}
+        return {"_task_name": TaskName.build("agroup::basic")}
 
 
     def test_initial(self, spec, state):
         obj = JobChainer()
         result = obj(spec, state)
         assert(result is None)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_postbox.py` & `doot-0.8.0/doot/actions/__tests/test_postbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_shell.py` & `doot-0.8.0/doot/actions/__tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/__tests/test_state.py` & `doot-0.8.0/doot/actions/__tests/test_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     def test_initial(self):
         action = DootBaseAction()
         assert(isinstance(action, DootBaseAction))
 
     def test_call_action(self, caplog, mocker):
         action = DootBaseAction()
         state  = { "count" : 0  }
-        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec   = mocker.Mock(spec=doot.structs.ActionSpec)
         spec.args = []
         result = action(spec, state)
         assert(result['count'] == 1)
         assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.7.2/doot/actions/base_action.py` & `doot-0.8.0/doot/actions/base_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 ## base_action.py -*- mode: Py -*-
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
-# import datetime
-# import enum
+# ##-- stdlib imports
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-##-- end imports
-
-printer = logmod.getLogger("doot._printer")
+# ##-- end stdlib imports
 
+# ##-- 1st party imports
 import doot
-from doot.errors import DootTaskError, DootTaskFailed
-from doot.structs import DootActionSpec
 from doot._abstract import Action_p
 from doot.enums import ActionResponseEnum
+from doot.errors import DootTaskError, DootTaskFailed
+from doot.structs import ActionSpec
+
+# ##-- end 1st party imports
+
+##-- logging
+printer = logmod.getLogger("doot._printer")
+
+##-- end logging
 
 class DootBaseAction(Action_p):
     """
     The basic action, which just prints that the action was called
     Subclass this and override __call__ for your own actions.
     The arguments of the action are held in the passed in spec
     __call__ is passed a *copy* of the task's state dictionary
     """
     ActRE = ActionResponseEnum
 
-
     def __str__(self):
         return f"Base Action"
 
-    def __call__(self, spec:DootActionSpec, state:dict) -> dict|bool|None:
+    def __call__(self, spec:ActionSpec, state:dict) -> dict|bool|None:
         printer.debug("Base Action Called: %s", state.get("count", 0))
         printer.info(" ".join(spec.args))
         return { "count" : state.get("count", 0) + 1 }
```

### Comparing `doot-0.7.2/doot/actions/compression.py` & `doot-0.8.0/doot/actions/compression.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/actions/control_flow.py` & `doot-0.8.0/doot/actions/control_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 from time import sleep
 import sh
 import shutil
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 
-from doot.structs import DootKey, DootCodeReference
+from doot.structs import DootKey, CodeReference
 from doot.mixins.path_manip import PathManip_m
 from doot.actions.base_action import DootBaseAction
 from doot.utils.action_decorators import ControlFlow
 
 @ControlFlow()
 class PredicateCheck(DootBaseAction):
     """
@@ -137,15 +137,15 @@
                         return
         except ValueError:
             return result
 
 class LogAction(DootBaseAction):
 
     @DootKey.dec.types("level", hint={"type_":str, "on_fail":"INFO"})
-    @DootKey.dec.expands("msg")
+    @DootKey.dec.expands("msg", hint={"rec":True})
     def __call__(self, spec, state, level, msg):
         level        = logmod.getLevelName(level)
         printer.log(level, "%s", msg)
 
 @ControlFlow()
 class StalenessCheck(DootBaseAction):
     """ Skip the rest of the task if old hasn't been modified since new was modifed """
```

### Comparing `doot-0.7.2/doot/actions/io.py` & `doot-0.8.0/doot/actions/io.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/actions/job_expansion.py` & `doot-0.8.0/doot/actions/job_expansion.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot.structs import DootKey, DootTaskSpec, DootTaskName, DootCodeReference
+from doot.structs import DootKey, TaskSpec, TaskName, CodeReference
 from doot.actions.base_action import DootBaseAction
 from doot.actions.job_injection import JobInjector
 
 class JobGenerate(DootBaseAction):
     """ Run a custom function to generate task specs
-      Function is in the form: fn(spec, state) -> list[DootTaskSpec]
+      Function is in the form: fn(spec, state) -> list[TaskSpec]
     """
 
     @DootKey.dec.references("fn")
     @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _fn_ref, _update):
         fn = _fn_ref.try_import()
         return { _update : list(fn(spec, state)) }
@@ -59,77 +59,85 @@
 class JobExpandAction(JobInjector):
     """
       Takes a template taskname/list[actionspec] and builds one new subtask for each entry in a list
 
       'inject' provides an injection dict, with $arg$ being the entry from the source list
     """
 
-    @DootKey.dec.types("from", "inject", "template", "print_levels")
+    @DootKey.dec.types("from", "inject", "template")
     @DootKey.dec.expands("prefix")
     @DootKey.dec.redirects("update_")
     @DootKey.dec.taskname
-    def __call__(self, spec, state, _from, inject, template, _printL, prefix, _update, _basename):
+    def __call__(self, spec, state, _from, inject, template, prefix, _update, _basename):
         match prefix:
             case "{prefix}":
                 prefix = "{Anon}"
             case _:
                 pass
 
         result          = []
         build_queue     = []
-        base_head       = _basename.task_head()
-        actions, base   = self._prep_base(template)
+        root            = _basename.root()
+        base_head       = root.job_head()
+        actions, sources = self._prep_base(template)
         match _from:
             case int():
                 build_queue += range(_from)
             case list():
                 build_queue += _from
             case None:
                 build_queue += [1]
             case _:
                 printer.warning("Tried to expand a non-list of args")
                 return self.ActRE.FAIL
 
         for i, arg in enumerate(build_queue):
-                injection = self.build_injection(spec, state, inject, replacement=arg)
-                new_spec  = DootTaskSpec.build(dict(name=_basename.subtask(prefix, i),
-                                                    ctor=base,
-                                                    actions = actions or [],
-                                                    required_for=[base_head],
-                                                    extra=injection,
-                                                    print_levels=_printL or {},
-                                                    ))
+                # TODO change job subtask naming scheme
+                base_dict = dict(name=root.subtask(prefix, i),
+                                 sources=sources,
+                                 actions = actions or [],
+                                 required_for=[base_head],
+                                 )
+                match self.build_injection(spec, state, inject, replacement=arg):
+                    case None:
+                        pass
+                    case dict() as val:
+                        base_dict.update(val)
+
+                new_spec  = TaskSpec.build(base_dict)
                 result.append(new_spec)
 
         return { _update : result }
 
-    def _prep_base(self, base:DootTaskName|list[DootActionSpec]) -> tuple[list, DootTaskName|None]:
+    def _prep_base(self, base:TaskName|list[ActionSpec]) -> tuple[list, TaskName|None]:
         """
           base can be the literal name of a task (base="group::task") to build off,
           or an indirect key to a list of actions (base_="sub_actions")
 
           This handles those possibilities and returns a list of actions and maybe a task name
 
         """
         match base:
             case list():
-                actions = base
-                base    = None
-            case DootTaskName():
+                assert(all(isinstance(x, (dict, TomlGuard)) for x in base))
+                actions  = base
+                sources  = [None]
+            case TaskName():
                 actions = []
+                sources = [base]
             case str():
                 actions = []
-                base    = DootTaskName.build(base)
+                sources = [TaskName.build(base)]
             case None:
                 actions = []
-                base    = None
+                sources = [None]
             case _:
                 raise doot.errors.DootActionError("Unrecognized base type", base)
 
-        return actions, base
+        return actions, sources
 
 class JobMatchAction(DootBaseAction):
     """
       Take a mapping of {pattern -> task} and a list,
       and build a list of new subtasks
 
       use `prepfn` to get a value from a taskspec to match on.
@@ -140,16 +148,16 @@
     @DootKey.dec.types("onto_")
     @DootKey.dec.references("prepfn")
     @DootKey.dec.types("mapping")
     def __call__(self, spec, state, _onto, prepfn, mapping):
         match prepfn:
             case None:
                 fn = lambda x: x.extra.fpath.suffix
-            case DootCodeReference():
+            case CodeReference():
                 fn = prepfn.try_import()
 
         for x in _onto:
             match fn(x):
                 case str() as key if key in mapping:
-                    x.ctor = DootTaskName.build(mapping[key])
+                    x.ctor = TaskName.build(mapping[key])
                 case _:
                     pass
```

### Comparing `doot-0.7.2/doot/actions/job_injection.py` & `doot-0.8.0/doot/actions/job_injection.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ##-- end logging
 
 import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot._abstract import Action_p
-from doot.structs import DootKey, DootTaskSpec, DootTaskName, DootCodeReference
+from doot.structs import DootKey, TaskSpec, TaskName, CodeReference
 from doot.mixins.path_manip import PathManip_m
 
 class JobInjector(Action_p):
     """
       Inject data into task specs.
       "inject" = {copy=X, expand=Y, replace=Z}
       'copy'   : redirects, and copies without expansion : [a_,x] -> {a:2, x:{q}}
@@ -62,17 +62,17 @@
 
     @DootKey.dec.types("onto", "inject")
     def __call__(self, spec, state, onto, inject):
         injection = self.build_injection(spec, state, inject)
         match onto:
             case list():
                 for x in onto:
-                    x.extra = TomlGuard(dict(**x.extra, **injection))
-            case DootTaskSpec():
-                onto.extra = TomlGuard(dict(**x.extra, **injection))
+                    x.model_extra.update(dict(**x.extra, **injection))
+            case TaskSpec():
+                onto.model_extra.update(dict(**x.extra, **injection))
 
     def build_injection(self, spec, state, inject, replacement=None, post:dict|None=None) -> None|TomlGuard:
         match inject:
             case dict():
                 copy    = inject.get("copy", [])
                 expand  = inject.get("expand", {})
                 replace = inject.get("replace", [])
@@ -118,24 +118,24 @@
 
         return injection_dict
 
 class JobPrependActions(Action_p):
 
     @DootKey.dec.types("_onto", "add_actions")
     def __call__(self, spec, state, _onto, _actions):
-        action_specs = [DootActionSpec.build(x) for x in _actions]
+        action_specs = [ActionSpec.build(x) for x in _actions]
         for x in _onto:
             actions = action_specs + x.actions
             x.actions = actions
 
 class JobAppendActions(Action_p):
 
     @DootKey.dec.types("_onto", "add_actions")
     def __call__(self, spec, state, _onto, _actions):
-        actions_specs = [DootActionSpec.build(x) for x in _actions]
+        actions_specs = [ActionSpec.build(x) for x in _actions]
         for x in _onto:
             x.actions += action_specs
 
 class JobInjectPathParts(PathManip_m):
     """
       Map lpath, fstem, fparent, fname, fext onto each
       taskspec in the `onto` list, using each spec's `key`
@@ -144,21 +144,21 @@
     @DootKey.dec.types("onto", "roots")
     @DootKey.dec.redirects("key_")
     def __call__(self, spec, state, _onto, roots, _key):
         root_paths = self._build_roots(spec, state, roots)
         match _onto:
             case list():
                 for x in _onto:
-                    data = dict(x.extra)
+                    data = x.params
                     data.update(self._calc_path_parts(x.extra[_key], root_paths))
-                    x.extra = TomlGuard(data)
-            case DootTaskSpec():
+                    x.model_extra.update(data)
+            case TaskSpec():
                 data = dict(x.extra)
                 data.update(self._calc_path_parts(onto.extra[_key], root_paths))
-                _onto.extra = TomlGuard(data)
+                _onto.model_extra.update(data)
 
 class JobInjectShadowAction(PathManip_m):
     """
       Inject a shadow path into each task entry, using the target key which points to the relative path to shadow
       returns the *directory* of the shadow target
     """
 
@@ -166,18 +166,18 @@
     @DootKey.dec.paths("shadow_root")
     @DootKey.dec.redirects("key_")
     def __call__(self, spec, state, _onto, _shadow, _key):
         match _onto:
             case list():
                 for x in _onto:
                     rel_path = self._shadow_path(x.extra[_key], _shadow)
-                    x.extra = TomlGuard(dict(**x.extra, **{"shadow_path": rel_path}))
-            case DootTaskSpec():
+                    x.model_extra.update(dict(**x.extra, **{"shadow_path": rel_path}))
+            case TaskSpec():
                 rel_path = self._shadow_path(onto.extra[_key], _shadow)
-                onto.extra = TomlGuard(dict(**onto.extra, **{"shadow_path": rel_path}))
+                onto.model_extra.update(dict(**onto.extra, **{"shadow_path": rel_path}))
 
 class JobSubNamer(Action_p):
     """
       Apply the name {basename}.{i}.{key} to each taskspec in {onto}
     """
 
     @DootKey.dec.taskname
@@ -185,15 +185,15 @@
     @DootKey.dec.types("onto")
     def __call__(self, spec, state, _basename, _key, _onto):
         match _onto:
             case list():
                 for i,x in enumerate(_onto):
                     val = x.extra[_key]
                     x.name = _basename.subtask(i, self._gen_subname(val))
-            case DootTaskSpec():
+            case TaskSpec():
                 onto.name = _basename.subtask(self._gen_subname(val))
 
     def _gen_subname(self, val):
         match val:
             case pl.Path():
                 return val.stem
             case str():
```

### Comparing `doot-0.7.2/doot/actions/job_queuing.py` & `doot-0.8.0/doot/actions/job_queuing.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,112 +38,114 @@
 ##-- end logging
 
 import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot._abstract import Action_p
-from doot.structs import DootKey, DootTaskSpec, DootTaskName, DootCodeReference
+from doot.structs import DootKey, TaskSpec, TaskName, CodeReference
 
 class JobQueueAction(Action_p):
     """
       Queues a list of tasks into the tracker.
 
       1) Queue Named Tasks: {do='job.queue', args=['group::task'] }
       2) Queue Expanded TaskSpecs: {do='job.queue', from_="state_key" }
     """
 
     @DootKey.dec.args
-    @DootKey.dec.types("from_", hint={"type_":list|DootTaskSpec|None})
+    @DootKey.dec.types("from_", hint={"type_":list|TaskSpec|None})
     @DootKey.dec.redirects_many("from_multi_")
-    @DootKey.dec.types("after", hint={"type_":list|DootTaskName|str|None, "on_fail":None})
+    @DootKey.dec.types("after", hint={"type_":list|TaskName|str|None, "on_fail":None})
     @DootKey.dec.taskname
     def __call__(self, spec, state, _args, _from, _from_multi, _after, _basename) -> list:
         # TODO maybe expand args
         subtasks                   = []
-        queue : list[DootTaskSpec] = []
+        queue : list[TaskSpec] = []
         _after                     = self._expand_afters(_after, _basename)
 
         if _args:
             queue += self._build_args(_basename, _args)
 
         if _from:
             queue += self._build_from(_basename, _from)
 
         if _from_multi:
             queue += self._build_from_multi(_basename, _from_multi, spec, state)
 
         for sub in queue:
             match sub:
-                case DootTaskSpec():
+                case TaskSpec():
                     sub.depends_on += _after
                     subtasks.append(sub)
                 case x:
-                    raise doot.errors.DootActionError("Tried to queue a not DootTaskSpec", x)
+                    raise doot.errors.DootActionError("Tried to queue a not TaskSpec", x)
 
         return subtasks
 
     def _expand_afters(self, afters, base):
         result = []
         match afters:
             case None:
                 return []
             case "$head$":
                 return [base.head_task()]
             case str():
-                return [DootTaskName.build(afters)]
+                return [TaskName.build(afters)]
             case list():
                 for x in afters:
                     if x == "$head$":
                         result.append(base.head_task())
                     else:
-                        result.append(DootTaskName.build(x))
+                        result.append(TaskName.build(x))
 
         return result
 
 
 
     def _build_args(self, base, args) -> list:
         result = []
-        head   = base.task_head()
+        root   = base.root()
+        head   = base.job_head()
         for i,x in enumerate(args):
-            sub = DootTaskSpec.build(dict(
-                name=base.subtask(i),
-                ctor=DootTaskName.build(x),
+            sub = TaskSpec.build(dict(
+                name=root.subtask(i),
+                sources=[TaskName.build(x)],
                 required_for=[head],
                 depends_on=[],
                 ))
             result.append(sub)
 
         return result
 
     def _build_from_multi(self, base, froms, spec, state) -> list:
         result  = []
-        head    = base.task_head()
+        root    = base.root()
+        head    = base.job_head()
         as_keys = []
         match froms:
             case None:
                 pass
             case [*xs]:
                 as_keys += [DootKey.build(x) for x in xs]
 
         for key in as_keys:
-            match key.to_type(spec, state, type_=list|DootTaskSpec|None):
+            match key.to_type(spec, state, type_=list|TaskSpec|None):
                 case None:
                     pass
                 case list() as l:
                     result += l
-                case DootTaskSpec() as s:
+                case TaskSpec() as s:
                     result.append(s)
 
         return result
 
     def _build_from(self, base, _from) -> list:
         result = []
-        head = base.task_head()
+        head = base.job_head()
         match _from:
             case None:
                 pass
             case list() as l:
                 result += l
 
         return result
@@ -151,32 +153,33 @@
 class JobQueueHead(Action_p):
     """ Queue the head/on_completion task of this job"""
 
     @DootKey.dec.types("base")
     @DootKey.dec.types("inject")
     @DootKey.dec.taskname
     def __call__(self, spec, state, base, inject, _basename):
-        head_name       = _basename.task_head()
+        root            = _basename.root()
+        head_name       = _basename.job_head()
         head            = []
 
         match base:
-            case str() | DootTaskName():
-                head += [DootTaskSpec.build(dict(name=head_name,
+            case str() | TaskName():
+                head += [TaskSpec.build(dict(name=head_name,
                                                  actions=[],
                                                  queue_behaviour="auto")),
-                         DootTaskSpec.build(dict(name=head_name.subtask("1"),
-                                                 ctor=DootTaskName.build(base),
+                         TaskSpec.build(dict(name=root.job_head().subtask("1"),
+                                                 sources=[TaskName.build(base)],
                                                  depends_on=[head_name],
                                                  extra=inject or {},
                                                  queue_behaviour="auto"))
                     ]
             case list():
-                head += [DootTaskSpec.build(dict(name=head_name, actions=base, extra=inject or {}, queue_behaviour="auto"))]
+                head += [TaskSpec.build(dict(name=head_name, actions=base, extra=inject or {}, queue_behaviour="auto"))]
             case None:
-                head += [DootTaskSpec.build(dict(name=head_name, queue_behaviour="auto"))]
+                head += [TaskSpec.build(dict(name=head_name, queue_behaviour="auto"))]
 
         return head
 
 class JobChainer(Action_p):
     """
       Add dependencies to task specs, from left to right, by key
       ie: task -> task -> task
@@ -190,10 +193,10 @@
     def __call__(self, spec, state, kwargs):
         for k,v in kwargs.items():
             match DootKey.build(k).to_type(spec, state):
                 case list() as l:
                     for x in l:
                         x.required_for += []
 
-                case DootTaskSpec() as s:
+                case TaskSpec() as s:
                     s.required_for += []
                     pass
```

### Comparing `doot-0.7.2/doot/actions/json.py` & `doot-0.8.0/doot/actions/json.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/actions/postbox.py` & `doot-0.8.0/doot/actions/postbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from collections import defaultdict
 from time import sleep
 import sh
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
-from doot.structs import DootKey, DootTaskName
+from doot.structs import DootKey, TaskName
 
 printer = logmod.getLogger("doot._printer")
 STATE_TASK_NAME_K : Final[str] = doot.constants.patterns.STATE_TASK_NAME_K
 
 ##-- expansion keys
 UPDATE      : Final[DootKey] = DootKey.build("update_")
 TASK_NAME   : Final[DootKey] = DootKey.build(STATE_TASK_NAME_K)
@@ -51,32 +51,30 @@
       Postboxes are lists, values are appended to it
     """
 
     boxes : ClassVar[dict[str,list[Any]]] = defaultdict(lambda: defaultdict(list))
     default_subkey                        = "_default"
 
     @staticmethod
-    def put(key:DootTaskName, val):
+    def put(key:TaskName, val):
         subbox = str(key.last())
         box    = str(key.root())
         match val:
             case None | [] | {} | dict() if not bool(val):
                 pass
             case list() | set():
                 _DootPostBox.boxes[box][subbox] += val
             case _:
                 _DootPostBox.boxes[box][subbox].append(val)
 
     @staticmethod
-    def get(key:DootTaskName, subkey=Any) -> list|dict:
+    def get(key:TaskName, subkey=Any) -> list|dict:
         box    = str(key.root())
         subbox = str(key.last())
         match subbox:
-            case "" | "-":
-                return _DootPostBox.boxes[box][_DootPostBox.default_subkey][:]
             case x if x == Any:
                 return _DootPostBox.boxes[box][_DootPostBox.default_subkey][:]
             case "*" | None:
                 return _DootPostBox.boxes[box].copy()
             case _:
                 return _DootPostBox.boxes[box][subbox]
 
@@ -95,29 +93,28 @@
 class PutPostAction(Action_p):
     """
     push data to the inter-task postbox of this task tree
     The arguments of the action are held in self.spec
     'args' are pushed to the default subbox
     'kwargs' are pushed to the kwarg specific subbox
 
-    eg: {do="post.put", args=["{key}", "{key}"], subbox="{key}"}
+    eg: {do="post.put", args=["{key}", "{key}"], "group::task.sub..subbox"="{key}"}
     """
 
     @DootKey.dec.args
     @DootKey.dec.kwargs
     @DootKey.dec.taskname
     def __call__(self, spec, state, args, kwargs, _basename) -> dict|bool|None:
         target = _basename.root().subtask(_DootPostBox.default_subkey)
         for statekey in args:
             data = DootKey.build(statekey).to_type(spec, state)
             _DootPostBox.put(target, data)
 
-        root = _basename.root()
-        for subbox,statekey in kwargs.items():
-            box  = root.subtask(subbox)
+        for box_str,statekey in kwargs.items():
+            box = TaskName.build(box_str)
             match statekey:
                 case str():
                     data = DootKey.build(statekey).to_type(spec, state)
                     _DootPostBox.put(box, data)
                 case [*xs]:
                     for x in statekey:
                         data = DootKey.build(x).to_type(spec, state)
@@ -125,48 +122,48 @@
 
 
 class GetPostAction(Action_p):
     """
       Read data from the inter-task postbox of a task tree
       The arguments of the action are held in self.spec
 
-      stateKey="group::task.{subbox}"
-      eg: data="bib::format.-"
+      stateKey="group::task.sub..{subbox}"
+      eg: data="bib::format..-"
     """
 
     @DootKey.dec.kwargs
     def __call__(self, spec, state, kwargs) -> dict|bool|None:
         updates = {}
-        for key,subkey in kwargs.items():
+        for key,box_str in kwargs.items():
             state_key          = DootKey.build(key, explicit=True).expand(spec, state)
-            target_box         = DootTaskName.build(subkey)
+            target_box         = TaskName.build(box_str)
             updates[state_key] = _DootPostBox.get(target_box)
 
         return updates
 
 class ClearPostAction(Action_p):
     """
       Clear your postbox
     """
     @DootKey.dec.expands("key", hint={"on_fail":Any})
     @DootKey.dec.taskname
     def __call__(self, spec, state, key, _basename):
-        from_task = _basename.root().subtask(key)
+        from_task = _basename.root(top=True).subtask(key)
         _DootPostBox.clear_box(from_task)
         return
 
 
 class SummarizePostAction(Action_p):
     """
       print a summary of this task tree's postbox
       The arguments of the action are held in self.spec
     """
     @DootKey.dec.types("from", hint={"type_":str|None})
     @DootKey.dec.types("full", hint={"type_":bool, "on_fail":False})
     def __call__(self, spec, state, _from, full) -> dict|bool|None:
-        from_task = _from or TASK_NAME.to_type(spec, state).root()
+        from_task = _from or TASK_NAME.to_type(spec, state).root(top=True)
         data   = _DootPostBox.get(from_task)
         if full:
             for x in data:
                 printer.info("Postbox %s: Item: %s", from_task, str(x))
 
         printer.info("Postbox %s: Size: %s", from_task, len(data))
```

### Comparing `doot-0.7.2/doot/actions/shell.py` & `doot-0.8.0/doot/actions/shell.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/actions/speak.py` & `doot-0.8.0/doot/actions/speak.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 ## base_action.py -*- mode: python -*-
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
+# ##-- stdlib imports
 import datetime
-# import enum
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
+import sys
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-##-- end imports
+from time import sleep
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-printer = logmod.getLogger("doot._printer")
+# ##-- end stdlib imports
 
-from time import sleep
-import sys
+# ##-- 3rd party imports
 import sh
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
-from doot.structs import DootKey
-from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
+from doot.errors import DootTaskError, DootTaskFailed
+from doot.structs import DootKey
+
+# ##-- end 1st party imports
+
+##-- logging
+printer = logmod.getLogger("doot._printer")
+cmd_l   = printer.getChild("cmd")
+fail_l  = printer.getChild("fail")
+##-- end logging
 
 class SpeakTimeAction(Action_p):
     """
     A Simple Action that announces the time
     Subclass this and override __call__ for your own actions.
     The arguments of the action are held in self.spec
 
@@ -53,18 +65,18 @@
                 case "linux":
                     return self._say_linux(spec, state)
                 case "darwin":
                     return self._say_mac(spec, state)
                 case _:
                     return False
         except sh.CommandNotFound as err:
-            printer.error("Shell Commmand '%s' Not Action: %s", err.args[0], args)
+            fail_l.error("Shell Commmand '%s' Not Action: %s", err.args[0], args)
             return False
         except sh.ErrorReturnCode:
-            printer.error("Shell Command '%s' exited with code: %s for args: %s", args[0], result.exit_code, args)
+            fail_l.error("Shell Command '%s' exited with code: %s for args: %s", args[0], result.exit_code, args)
             return False
 
 
     def _say_linux(self, spec, state:dict):
         cmd    = sh.espeak
         args   = (spec.args or self.mac_announce_args) + [self._current_time()]
         if spec.kwargs.on_fail(False, bool).wait():
```

### Comparing `doot-0.7.2/doot/actions/state.py` & `doot-0.8.0/doot/actions/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 ## base_action.py -*- mode: python -*-
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
+# ##-- stdlib imports
 import datetime
-# import enum
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
+import shutil
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
-
-##-- end imports
+from time import sleep
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-printer = logmod.getLogger("doot._printer")
+# ##-- end stdlib imports
 
-from time import sleep
-import datetime
+# ##-- 3rd party imports
 import sh
-import shutil
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
-from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
-from doot.mixins.importer import Importer_m
+from doot.actions.job_injection import (JobInjectPathParts,
+                                        JobInjectShadowAction)
+from doot.errors import DootTaskError, DootTaskFailed
 from doot.mixins.path_manip import PathManip_m
-from doot.structs import DootCodeReference, DootKey
-from doot.actions.job_injection import JobInjectPathParts, JobInjectShadowAction
+from doot.structs import CodeReference, DootKey
+
+# ##-- end 1st party imports
+
+printer = logmod.getLogger("doot._printer")
 
 ##-- expansion keys
 UPDATE : Final[DootKey] = DootKey.build("update_")
 FORMAT : Final[DootKey] = DootKey.build("format")
 FROM   : Final[DootKey] = DootKey.build("from")
 ##-- end expansion keys
 
@@ -54,26 +58,26 @@
         result = {}
         for k,v in kwargs.items():
             key = DootKey.build(v, explicit=True)
             val = key.to_type(spec, state)
             result[k] = val
         return result
 
-class AddStateFn(Action_p, Importer_m):
+class AddStateFn(Action_p):
     """ for each toml kwarg, import its value and set the state[kwarg] = val
       with expansion
     """
 
     @DootKey.dec.kwargs
     def __call__(self, spec, state:dict, kwargs) -> dict|bool|None:
         result = {}
         for kwarg, val in kwargs:
             key = DootKey.build(val, explicit=True)
             val = key.expand(spec, state)
-            ref = DootCodeReference.build(val)
+            ref = CodeReference.build(val)
             result[kwarg] = ref.try_import()
 
         return result
 
 class PushState(Action_p):
     """
       state[update_] += [state[x] for x in spec.args]
```

### Comparing `doot-0.7.2/doot/actions/templater.py` & `doot-0.8.0/doot/actions/templater.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/actions/util.py` & `doot-0.8.0/doot/actions/util.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/cmds/__tests/test_list_cmd.py` & `doot-0.8.0/doot/cmds/__tests/test_list_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 #!/usr/bin/env python3
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
+import contextlib
+import datetime
+import enum
+import functools as ftz
+import io
+import itertools as itz
 import logging as logmod
+import pathlib as pl
+import sys
 import unittest
 import warnings
-import pathlib as pl
-from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
-                    Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
-                    TypeVar, cast)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from unittest import mock
-##-- end imports
-logging = logmod.root
+from uuid import UUID, uuid1
+
+# ##-- end stdlib imports
 
+# ##-- 3rd party imports
 import pytest
-import functools as ftz
-import sys
-import io
-import contextlib
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
+
+# ##-- end 1st party imports
+
 doot._test_setup()
+
+# ##-- 1st party imports
 import doot.errors
 from doot._abstract import Command_i
-from doot.structs import DootTaskSpec
 from doot.cmds.list_cmd import ListCmd
+from doot.structs import TaskSpec
+
+# ##-- end 1st party imports
+
+logging = logmod.root
 
 class TestListCmd:
 
     def test_initial(self):
         obj = ListCmd()
         assert(isinstance(obj, Command_i))
 
@@ -61,15 +82,14 @@
         doot.args.cmd.arg.all      = True
         obj    = ListCmd()
         obj({}, {"reporter": [mocker.stub("Reporter Stub")]})
 
         message_set = {x.message for x in caplog.records}
         assert("No Tasks Defined" in message_set)
 
-
     def test_call_all_not_empty(self, caplog, mocker):
         mocker.patch("doot.args")
         del doot.args.cmd.args.keys
         doot.args.cmd.args.__iter__.return_value = iter([("pattern", ""), ("all", True)])
         doot.args.cmd.args.pattern = ""
         doot.args.cmd.args.all     = True
 
@@ -78,54 +98,79 @@
         mock_class1.__module__ = "builtins"
         mock_class1.__name__   = "type"
         mock_class2 = mocker.MagicMock(type)
         mock_class2.__module__ = "builtins"
         mock_class2.__name__   = "other.type"
         plugin_mock = {"reporter": [mocker.stub("Reporter Stub")]}
         job_mock = {
-            "simple" : DootTaskSpec.build({"group": "blah", "name": "simple", "ctor": mock_class1}),
-            "other"  : DootTaskSpec.build({"group": "bloo", "name": "other", "ctor": mock_class2})
+            "simple" : TaskSpec.build({"group": "blah", "name": "simple"}), # "ctor": mock_class1}),
+            "other"  : TaskSpec.build({"group": "bloo", "name": "other"}),  # "ctor": mock_class2})
             }
         obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("defined task generators by group:" in message_set)
         assert(any(x.startswith("simple :: ") for x in message_set) )
         assert(any(x.startswith("other  :: ") for x in message_set) )
 
+    def test_list_even_with_ctor_failure(self, caplog, mocker):
+        mocker.patch("doot.args")
+        del doot.args.cmd.args.keys
+        doot.args.cmd.args.__iter__.return_value = iter([("pattern", ""), ("all", True)])
+        doot.args.cmd.args.pattern = ""
+        doot.args.cmd.args.all     = True
+
+        obj = ListCmd()
+        mock_class1 = mocker.MagicMock(type)
+        mock_class1.__module__ = "builtins"
+        mock_class1.__name__   = "type"
+        mock_class2 = mocker.MagicMock(type)
+        mock_class2.__module__ = "builtins"
+        mock_class2.__name__   = "other.type"
+        plugin_mock = {"reporter": [mocker.stub("Reporter Stub")]}
+        job_mock = {
+            "simple" : TaskSpec.build({"group": "blah", "name": "simple", "ctor": mock_class1}),
+            "other"  : TaskSpec.build({"group": "bloo", "name": "other", "ctor": mock_class2})
+            }
+        obj(job_mock, plugin_mock)
+        message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
+
+        assert("defined task generators by group:" in message_set)
+        assert(any(x.startswith("simple :: ") for x in message_set) )
+        assert(any(x.startswith("ctor import failed") for x in message_set) )
+
     def test_call_target_not_empty(self, caplog, mocker):
         mocker.patch("doot.args")
         del doot.args.cmd.args.keys
         doot.args.cmd.args.__iter__.return_value = iter([("pattern", "simple"), ("all", False)])
         doot.args.cmd.args.pattern = "simple"
         doot.args.cmd.args.all     = False
         obj = ListCmd()
         plugin_mock  = {"reporter": [mocker.stub("Reporter Stub")]}
         job_mock = {
-                       "simple" : DootTaskSpec.build({"group": "blah", "name": "simple"}),
-                       "other"  : DootTaskSpec.build({"group": "bloo", "name": "other"}),
+                       "simple" : TaskSpec.build({"group": "blah", "name": "simple"}),
+                       "other"  : TaskSpec.build({"group": "bloo", "name": "other"}),
             }
         result = obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("tasks for pattern: simple" in message_set)
         assert( any(x.startswith("blah::simple :: doot.task.base_task:doottask") for x in message_set) )
 
-
     def test_call_partial_target_not_empty(self, caplog, mocker):
         mocker.patch("doot.args")
         del doot.args.cmd.args.keys
         doot.args.cmd.args.__iter__.return_value = iter([("pattern", "simp"), ("all", False)])
         doot.args.cmd.args.pattern = "simp"
         doot.args.cmd.args.all     = False
         obj = ListCmd()
         plugin_mock = {"reporter": [mocker.stub("Reporter Stub")]}
-        job_mock = { "blah::simple" : DootTaskSpec.build({"group": "blah", "name": "simple"}),
-                        "bloo::other": DootTaskSpec.build({"group": "bloo", "name": "other"}),
-                        "bloo::diffSimple": DootTaskSpec.build({"group": "bloo", "name": "diffSimple"}),
+        job_mock = { "blah::simple" : TaskSpec.build({"group": "blah", "name": "simple"}),
+                        "bloo::other": TaskSpec.build({"group": "bloo", "name": "other"}),
+                        "bloo::diffSimple": TaskSpec.build({"group": "bloo", "name": "diffSimple"}),
                        }
         result = obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("tasks for pattern: simp" in message_set)
         assert( any(x.startswith("blah::simple     :: doot.task.base_task:doottask") for x in message_set) )
         assert( any(x.startswith("bloo::diffsimple :: doot.task.base_task:doottask") for x in message_set) )
```

### Comparing `doot-0.7.2/doot/cmds/base_cmd.py` & `doot-0.8.0/doot/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/cmds/clean_cmd.py` & `doot-0.8.0/doot/cmds/clean_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/cmds/graph_cmd.py` & `doot-0.8.0/doot/cmds/graph_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from collections import defaultdict
 import sh
 
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.cmds.base_cmd import BaseCommand
-from doot.structs import DootParamSpec
+from doot.structs import ParamSpec
 from doot.utils.plugin_selector import plugin_selector
 import networkx as nx
 import matplotlib.pyplot as plt
 
 printer                  = logmod.getLogger("doot._printer")
 
 INDENT : Final[str]      = " "*8
@@ -51,15 +51,15 @@
 
 @doot.check_protocol
 class GraphCmd(BaseCommand):
     _name      = "graph"
     _help      = ["Create a graph representation of the task network"]
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
+    def param_specs(self) -> list[ParamSpec]:
         return super().param_specs + [
             self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
             self.build_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
             self.build_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
             self.build_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
             self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
             self.build_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
```

### Comparing `doot-0.7.2/doot/cmds/help_cmd.py` & `doot-0.8.0/doot/cmds/help_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,19 +29,24 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 import doot
 from doot.cmds.base_cmd import BaseCommand
-from doot.structs import DootParamSpec, DootTaskSpec, DootCodeReference
+from doot.structs import ParamSpec, TaskSpec, CodeReference
 from collections import defaultdict
 
 NON_DEFAULT_KEY : Final[str] = doot.constants.misc.NON_DEFAULT_KEY
 
+LINE_SEP        : Final[str] = "------------------------------"
+GROUP_INDENT    : Final[str] = "----"
+ITEM_INDENT     : Final[str] = "-"
+
+
 class HelpCmd(BaseCommand):
     _name      = "help"
     _help      = ["Print info about the specified cmd or task",
                   "Can also be triggered by passing --help to any command or task"
                   ]
 
     @property
@@ -59,25 +64,25 @@
             case {"target": ""|None} if not bool(doot.args.tasks):
                 pass
             case {"target": ""|None}:
                 task_targets +=  [tasks[x] for x in doot.args.tasks.keys()]
                 cmd_targets  +=  [x for x in plugins.command if x.name == doot.args.cmd.args.target]
             case {"target": target}:
                 # Print help of just the specified target(s)
-                task_targets +=  [y for x,y in tasks.items() if target in x ]
+                task_targets +=  [y for x,y in tasks.items() if x in target]
                 cmd_targets  +=  [x for x in plugins.command if x.name == doot.args.cmd.args.target]
             case {"help": True}:
                 printer.info(self.help)
                 return
 
         logging.debug("Matched %s commands, %s tasks", len(cmd_targets), len(task_targets))
         if len(cmd_targets) == 1:
             cmd_class = cmd_targets[0].load()()
             printer.info(cmd_class.help)
-            if bool(doot.args.cmd[NON_DEFAULT_KEY]):
+            if bool(doot.args.cmd.args[NON_DEFAULT_KEY]):
                 self._print_current_param_assignments(cmd_class.param_specs, doot.args.cmd.args)
 
         elif bool(task_targets):
             for i, spec in enumerate(task_targets):
                 self.print_task_spec(i, spec)
 
         else:
@@ -86,74 +91,72 @@
             printer.info("Available Command Targets: ")
             for x in sorted(plugins.command, key=lambda x: x.name):
                 printer.info("-- %s", x.name)
 
         printer.info("\n------------------------------")
         printer.info("Call a command by doing 'doot [cmd] [args]'. Eg: doot list --help")
 
-    def print_task_spec(self, count, spec:DootTaskSpec):
-        task_name = spec.name
+    def print_task_spec(self, count, spec:TaskSpec):
+        task_name = str(spec.name)
         match spec.ctor:
             case None:
                 ctor = None
-            case DootCodeReference():
+            case CodeReference():
                 ctor = spec.ctor.try_import()
             case _:
                 ctor = spec.ctor
 
-        lines     = []
-        lines.append("")
-        lines.append("------------------------------")
-        lines.append(f"{count:4}: Task: {task_name}")
-        lines.append("------------------------------")
-        lines.append(f"ver    : {spec.version}")
-        lines.append(f"Group  : {spec.name.group}")
-        lines.append(f"Source : {spec.source}")
-
-        if ctor is not None:
-            lines.append(ctor.class_help())
+        printer.info("")
+        printer.info(LINE_SEP)
+        printer.info(f"{count:4}: Task: {task_name}")
+        printer.info(LINE_SEP)
+        printer.info("ver     : %s", spec.version)
+        printer.info("Group   : %s", spec.name.group)
+        sources = "; ".join([str(x) for x in spec.sources])
+        printer.info("Sources : %s", sources)
 
         match spec.doc:
             case None:
                 pass
             case str():
-                lines.append("")
-                lines.append(f"--   {spec.doc}")
+                printer.info("")
+                printer.info(spec.doc)
+                printer.info("")
             case list() as xs:
-                lines.append("")
-                lines.append("--  " + "\n--  ".join(xs))
+                printer.info("")
+                printer.info("\n".join(xs))
+                printer.info("")
+
+        if ctor is not None:
+            printer.info("%s Ctor Class:", GROUP_INDENT)
+            printer.info(ctor.class_help())
+            printer.info(GROUP_INDENT)
 
-        printer.info("\n".join(lines))
 
         if bool(spec.extra):
             printer.info("")
-            printer.info("Toml Parameters:")
+            printer.info("%s Toml Parameters:", GROUP_INDENT)
             for kwarg,val in spec.extra:
-                printer.info("-- %-20s : %s", kwarg, val)
+                printer.info("%s %-20s : %s", ITEM_INDENT, kwarg, val)
 
         if bool(spec.actions):
             printer.info("")
-            printer.info("Task Actions: ")
+            printer.info("-- Task Actions: ")
             for action in spec.actions:
-                printer.info("-- %-20s : Args=%-20s Kwargs=%s", action.do, action.args, dict(action.kwargs) )
+                printer.info("%s %-20s : Args=%-20s Kwargs=%s", ITEM_INDENT, action.do, action.args, dict(action.kwargs) )
 
-        cli_has_params = str(task_name) in doot.args.tasks
-        cli_has_non_default = bool(doot.args.tasks[str(task_name)][NON_DEFAULT_KEY])
+        cli_has_params      = task_name in doot.args.tasks
+        cli_has_non_default = bool(doot.args.tasks[task_name][NON_DEFAULT_KEY])
 
         if cli_has_params and cli_has_non_default and ctor is not None:
             self._print_current_param_assignments(ctor.param_specs, doot.args.tasks[task_name])
 
-    def _print_current_param_assignments(self, specs:list[DootParamSpec], args:TomlGuard):
-        if not bool(specs):
-            return
-
+    def _print_current_param_assignments(self, specs:list[ParamSpec], args:TomlGuard):
         printer.info("")
-        printer.info("Current Param Assignments:")
-        results = []
+        printer.info("%s Current Param Assignments:", GROUP_INDENT)
+
+        assignments = sorted([x for x in specs if not x.invisible], key=ParamSpec.key_func)
         max_param_len = 5 + ftz.reduce(max, map(len, map(lambda x: x.name, specs)), 0)
-        fmt_str = f"%-{max_param_len}s %s : %s"
-        for spec in sorted(specs, key=DootParamSpec.key_func):
-            if spec.invisible:
-                continue
-            value = args._table().get(spec.name, spec.default)
-            is_default = "   " if value == spec.default else "(*)"
-            printer.info(fmt_str, spec.name, is_default, value)
+        fmt_str = f"%s %-{max_param_len}s : %s "
+        for key in args[NON_DEFAULT_KEY]:
+            value = args[key]
+            printer.info(fmt_str, ITEM_INDENT, key, value)
```

### Comparing `doot-0.7.2/doot/cmds/list_cmd.py` & `doot-0.8.0/doot/cmds/list_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 
 #!/usr/bin/env python3
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-import types
+# ##-- stdlib imports
 import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
+import types
+from collections import defaultdict
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
 
-##-- end imports
+# ##-- end stdlib imports
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- 3rd party imports
+from tomlguard import TomlGuard
 
-printer = logmod.getLogger("doot._printer")
+# ##-- end 3rd party imports
 
-from collections import defaultdict
-from tomlguard import TomlGuard
+# ##-- 1st party imports
 import doot
 import doot.errors
-from doot.enums import TaskFlags
 from doot.cmds.base_cmd import BaseCommand
-from doot.structs import DootParamSpec
+from doot.enums import TaskFlags
+from doot.structs import ParamSpec
+
+# ##-- end 1st party imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
+help_l  = printer.getChild("help")
+cmd_l   = printer.getChild("cmd")
+##-- end logging
 
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
 class ListCmd(BaseCommand):
     _name      = "list"
     _help      = ["A simple command to list all loaded task heads."]
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
+    def param_specs(self) -> list[ParamSpec]:
         return super().param_specs + [
             self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
             self.build_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
             self.build_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
             self.build_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
             self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
             self.build_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
@@ -68,15 +78,15 @@
         if (doot.args.cmd.args.pattern == ""     # type: ignore
             and not bool(doot.args.tasks)        # type: ignore
             and not doot.args.cmd.args.by_source # type: ignore
             and not doot.args.cmd.args.all):     # type: ignore
             raise doot.errors.DootCommandError("ListCmd Needs a Matcher, or all")
 
         if not bool(tasks):
-            printer.info("No Tasks Defined", extra={"colour": "red"})
+            help_l.info("No Tasks Defined", extra={"colour": "red"})
             return
 
         match dict(doot.args.cmd.args): # type: ignore
             case {"locations": True}:
                 self._print_locations()
             case {"by-source": True}:
                 self._print_all_by_source(tasks)
@@ -92,92 +102,101 @@
                 raise doot.errors.DootCommandError("Bad args passed in", doot.args.cmd.args)
 
     def _print_matches(self, tasks):
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"%-{max_key}s :: %-25s <%s>"
         pattern = doot.args.cmd.args.pattern.lower()
         matches = {x for x in tasks.keys() if pattern in x.lower()}
-        printer.info("Tasks for Pattern: %s", pattern)
+        cmd_l.info("Tasks for Pattern: %s", pattern)
         for key in matches:
             spec = tasks[key]
-            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.flags and not doot.args.cmd.args.internal:
+                continue
+            if TaskFlags.DISABLED in spec.flags:
                 continue
 
-            printer.info(fmt_str,
+            cmd_l.info(fmt_str,
                          spec.name,
                          spec.ctor,
-                         spec.source)
+                         spec.sources)
 
     def _print_group_matches(self, tasks):
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"    %-{max_key}s :: %-25s <%s>"
         pattern  = doot.args.cmd.args.pattern.lower()
         groups  = defaultdict(list)
         for name, spec in tasks.items():
             if pattern not in name:
                 continue
-            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.flags and not doot.args.cmd.args.internal:
+                continue
+            if TaskFlags.DISABLED in spec.flags:
                 continue
 
             groups[spec.name.group].append((spec.name.task,
-                                                  spec.ctor.__module__,
-                                                  spec.ctor.__name__,
-                                                  spec.source))
+                                            spec.ctor.__module__,
+                                            spec.ctor.__name__,
+                                            spec.sources))
 
-        printer.info("Tasks for Matching Groups: %s", pattern, extra={"colour":"cyan"})
+        cmd_l.info("Tasks for Matching Groups: %s", pattern, extra={"colour":"cyan"})
         for group, tasks in groups.items():
-            printer.info("*   %s::", group)
+            cmd_l.info("*   %s::", group)
             for task in tasks:
                 printer.info(fmt_str, *task)
 
     def _print_all_by_group(self, tasks):
-        printer.info("Defined Task Generators by Group:", extra={"colour":"cyan"})
+        cmd_l.info("Defined Task Generators by Group:", extra={"colour":"cyan"})
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"{INDENT}%-{max_key}s :: %-60s :: <Source: %s>"
         groups  = defaultdict(list)
         for spec in tasks.values():
-            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.flags and not doot.args.cmd.args.internal:
+                continue
+            if TaskFlags.DISABLED in spec.flags:
                 continue
 
+
             groups[spec.name.group].append((spec.name.task,
-                                                  (spec.doc[0] if bool(spec.doc) else "")[:60],
-                                                  spec.source))
+                                            (spec.doc[0] if bool(spec.doc) else "")[:60],
+                                            spec.sources))
 
         for group, tasks in groups.items():
-            printer.info("*   %s::", group, extra={"colour":"magenta"})
+            cmd_l.info("*   %s::", group, extra={"colour":"magenta"})
             for task in tasks:
                 printer.info(fmt_str, *task)
 
-        printer.info("")
-        printer.info("Full Task Name: {group}::{task}", extra={"colour":"cyan"})
+        cmd_l.info("")
+        cmd_l.info("Full Task Name: {group}::{task}", extra={"colour":"cyan"})
 
     def _print_all_by_source(self, tasks):
-        printer.info("Defined Task Generators by Source File:", extra={"colour":"cyan"})
+        cmd_l.info("Defined Task Generators by Source File:", extra={"colour":"cyan"})
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"{INDENT}%-{max_key}s :: %s.%-25s"
         sources = defaultdict(list)
         for key, spec in tasks.items():
-            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.flags and not doot.args.cmd.args.internal:
+                continue
+            if TaskFlags.DISABLED in spec.flags:
                 continue
 
-            sources[spec.source].append((spec.name.task,
+            sources[spec.sources[0]].append((spec.name.task,
                                          spec.ctor.__module__,
                                          spec.ctor.__name__,
                                         ))
 
         for source, tasks in sources.items():
-            printer.info(":: %s ::", source, extra={"colour":"red"})
+            cmd_l.info(":: %s ::", source, extra={"colour":"red"})
             for task in tasks:
                 printer.info(fmt_str, *task)
 
     def _print_just_groups(self, tasks):
-        printer.info("Defined Task Groups:", extra={"colour":"cyan"})
+        cmd_l.info("Defined Task Groups:", extra={"colour":"cyan"})
 
         group_set = set(spec.name.group for spec in tasks.values())
         for group in group_set:
             printer.info("- %s", group)
 
     def _print_locations(self):
-        printer.info("Defined Locations: ")
+        cmd_l.info("Defined Locations: ")
 
         for x in sorted(doot.locs):
             printer.info("-- %-25s : %s", x, doot.locs.get(x))
```

### Comparing `doot-0.7.2/doot/cmds/locs_cmd.py` & `doot-0.8.0/doot/cmds/locs_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.cmds.base_cmd import BaseCommand
-from doot.structs import DootParamSpec
+from doot.structs import ParamSpec
 
 
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
 class LocsCmd(BaseCommand):
     _name      = "locs"
     _help      = ["A simple command to list all config defined locations."]
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
+    def param_specs(self) -> list[ParamSpec]:
         return super().param_specs + [
             self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
             self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
             self.build_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
```

### Comparing `doot-0.7.2/doot/cmds/plugins_cmd.py` & `doot-0.8.0/doot/cmds/plugins_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.cmds.base_cmd import BaseCommand
-from doot.structs import DootParamSpec
+from doot.structs import ParamSpec
 
 
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
 class PluginsCmd(BaseCommand):
     _name      = "plugins"
     _help      = ["A simple command to list all loaded plugins."]
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
+    def param_specs(self) -> list[ParamSpec]:
         return super().param_specs + [
             self.build_param(name="all",                  default=True,                   desc="List all loaded tasks, by group"),
             self.build_param(name="groups",    type=bool, default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
             self.build_param(name="pattern",   type=str,  default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
@@ -76,15 +76,15 @@
         matches = {x for x in plugins.keys() if pattern in x.lower()}
         printer.info("Plugins for Pattern: %s", pattern)
         for key in matches:
             spec = plugins[key]
             printer.info(fmt_str,
                          spec.name,
                          spec.ctor,
-                         spec.source)
+                         spec.sources)
 
     def _print_group_matches(self, plugins):
         max_key = len(max(plugins.keys(), key=len))
         fmt_str = f"{INDENT}%-{max_key}s :: %-25s"
         pattern  = re.compile(doot.args.cmd.args.pattern.lower())
         groups  = defaultdict(list)
         for group_name, specs in plugins.items():
```

### Comparing `doot-0.7.2/doot/cmds/run_cmd.py` & `doot-0.8.0/doot/cmds/run_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 #!/usr/bin/env python3
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
-# import datetime
-# import enum
+# ##-- stdlib imports
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
-
-##-- end imports
+from collections import defaultdict
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end stdlib imports
 
-from collections import defaultdict
+# ##-- 3rd party imports
 from tomlguard import TomlGuard
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
+from doot._abstract import TaskRunner_i
 from doot.cmds.base_cmd import BaseCommand
-from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i
-from doot.utils.plugin_selector import plugin_selector
+from doot.structs import CodeReference
 from doot.task.check_locs import CheckLocsTask
-from doot.structs import DootCodeReference
+from doot.utils.plugin_selector import plugin_selector
+
+# ##-- end 1st party imports
 
-printer                  = logmod.getLogger("doot._printer")
+##-- logging
+logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
+cmd_l   = printer.getChild("cmd")
+##-- end logging
 
 tracker_target           = doot.config.on_fail("default", str).commands.run.tracker()
 runner_target            = doot.config.on_fail("default", str).commands.run.runner()
 reporter_target          = doot.config.on_fail("default", str).commands.run.reporter()
 report_line_targets      = doot.config.on_fail([]).commands.run.report_line(wrapper=list)
 interrupt_handler        = doot.config.on_fail("doot.utils.signal_handler:SignalHandler", bool|str).commands.run.interrupt()
 
@@ -57,51 +62,61 @@
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
             self.build_param(name="step", default=False),
             self.build_param(name="interrupt", default=False),
             self.build_param(name="dry-run", default=False),
+            self.build_param(name="confirm", default=False),
             self.build_param(name="target", type=list[str], default=[], positional=True),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         # Note the final parens to construct:
         available_reporters    = plugins.on_fail([], list).report_line()
         report_lines           = [plugin_selector(available_reporters, target=x)() for x in report_line_targets]
         reporter               = plugin_selector(plugins.on_fail([], list).reporter(), target=reporter_target)(report_lines)
         tracker                = plugin_selector(plugins.on_fail([], list).tracker(), target=tracker_target)()
         runner                 = plugin_selector(plugins.on_fail([], list).runner(), target=runner_target)(tracker=tracker, reporter=reporter)
-        printer.info("- Building Task Dependency Network")
+        cmd_l.info("Registering Task Specs: %s", len(tasks))
         for task in tasks.values():
-            tracker.add_task(task)
-        tracker.add_task(CheckLocsTask())
-
-        printer.info("- Task Dependency Network Built")
+            tracker.register_spec(task)
 
+        cmd_l.info("Queuing Initial Tasks")
         for target in doot.args.on_fail([], list).cmd.args.target():
             if target not in tracker:
-                printer.warn("- %s specified as run target, but it doesn't exist")
+                cmd_l.warn("%s specified as run target, but it doesn't exist", target)
             else:
-                tracker.queue_task(target)
+                tracker.queue_entry(target, from_user=True)
 
         for target in doot.args.on_fail({}).tasks().keys():
-            if target not in tracker:
-                printer.warn(- "%s specified as run target, but it doesn't exist")
-            else:
-                tracker.queue_task(target)
+            try:
+                tracker.queue_entry(target, from_user=True)
+            except doot.errors.DootTaskTrackingError as err:
+                cmd_l.warn("Failed to Queue Target: %s", target)
+                logging.debug(err)
 
-        tracker.queue_task(CheckLocsTask.task_name)
+        tracker.queue_entry(CheckLocsTask(), from_user=True)
 
         match interrupt_handler:
             case _ if not doot.args.cmd.args.interrupt:
                 interrupt = None
             case None:
                 interrupt = None
             case bool():
                 interrupt = interrupt_handler
             case str():
-                interrupt = DootCodeReference.build(interrupt_handler).try_import()
+                interrupt = CodeReference.build(interrupt_handler).try_import()
 
-        printer.info("- %s Tasks Queued: %s", len(tracker.active_set), " ".join(tracker.active_set))
+        cmd_l.info("%s Tasks Queued: %s", len(tracker.active_set), " ".join(str(x) for x in tracker.active_set))
         with runner:
+            if doot.args.on_fail(False).cmd.args.confirm():
+                plan = tracker.generate_plan()
+                for i,(depth,node,desc) in enumerate(plan):
+                    cmd_l.info("Step %-4s: %s",i, node)
+                match input("Confirm Execution Plan (Y/*): "):
+                    case "Y":
+                        pass
+                    case _:
+                        cmd_l.info("Cancelling")
+                        return
             runner(handler=interrupt)
```

### Comparing `doot-0.7.2/doot/cmds/step_cmd.py` & `doot-0.8.0/doot/cmds/step_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 from doot.cmds.base_cmd import BaseCommand
-from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i
 from doot.utils.plugin_selector import plugin_selector
 from doot.task.check_locs import CheckLocsTask
 
 printer                  = logmod.getLogger("doot._printer")
 
 runner_target            = doot.config.on_fail("step", str).commands.step.runner()
 tracker_target           = doot.config.on_fail("default", str).commands.step.tracker()
```

### Comparing `doot-0.7.2/doot/cmds/stub_cmd.py` & `doot-0.8.0/doot/cmds/stub_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import importlib
 from importlib.resources import files
 import doot
 import doot.enums
 import doot.errors
 from doot.cmds.base_cmd import BaseCommand
 from doot._abstract import PluginLoader_p, Task_i
-from doot.structs import TaskStub, DootTaskName, DootCodeReference
+from doot.structs import TaskStub, TaskName, CodeReference
 from doot.task.base_job import DootJob
 from doot.task.base_task import DootTask
 from doot._structs.key import HELP_HINT
 from doot.utils.decorators import KEY_ANNOTS
 
 ##-- data
 data_path = files(doot.constants.paths.TEMPLATE_PATH).joinpath(doot.constants.paths.TOML_TEMPLATE)
@@ -56,46 +56,44 @@
     """
     _name      = "stub"
     _help      = ["Create a new stub task either to stdout, or path"]
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
-            self.build_param("file-target", type=str,     default=""),
-            self.build_param("Config",                    default=False,           desc="Stub a doot.toml",                  prefix="-"),
-            self.build_param("Actions",                   default=False,           desc="Help Stub Actions",                 prefix="-"),
-            self.build_param("cli",                       default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
-            self.build_param("printer",                   default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
-
-            self.build_param("Flags",                     default=False,           desc="Help Stub Task Flags",              prefix="-"),
-
-            self.build_param("name",        type=str,     default=None,            desc="The Name of the new task",                          positional=True),
-            self.build_param("ctor",        type=str,     default="task",          desc="The short type name of the task generator",         positional=True),
-            self.build_param("suppress-header",           default=True, invisible=True)
+            self.build_param(name="file-target", type=str,     default=""),
+            self.build_param(name="Config",                    default=False,           desc="Stub a doot.toml",                  prefix="-"),
+            self.build_param(name="Actions",                   default=False,           desc="Help Stub Actions",                 prefix="-"),
+            self.build_param(name="cli",                       default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
+            self.build_param(name="printer",                   default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
+
+            self.build_param(name="Flags",                     default=False,           desc="Help Stub Task Flags",              prefix="-"),
+
+            self.build_param(name="name",        type=str,     default=None,            desc="The Name of the new task",                          positional=True),
+            self.build_param(name="ctor",        type=str,     default="task",          desc="The short type name of the task generator",         positional=True),
+            self.build_param(name="suppress-header",           default=True, invisible=True)
             ]
 
     def _import_task_class(self, ctor_name):
         try:
-            code_ref = DootCodeReference.build(ctor_name)
+            code_ref = CodeReference.build(ctor_name)
             return code_ref.try_import()
         except ImportError as err:
             raise doot.errors.DootTaskLoadError(ctor_name)
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         match dict(doot.args.cmd.args):
             case {"Config": True}:
                 self._stub_doot_toml()
             case {"Actions": True}:
                 self._stub_actions(plugins)
             case {"cli": True}:
                 self._stub_cli_arg()
             case {"Flags": True}:
                 self._list_flags()
-            case {"printer": True}:
-                self._stub_printer_settings()
             case _:
                 self._stub_task_toml(tasks, plugins)
 
     def _stub_doot_toml(self):
         logging.info("Building Doot Toml Stub")
         doot_toml = pl.Path("doot.toml")
         data_text = data_path.read_text()
@@ -110,22 +108,25 @@
         printer.info("doot.toml stub")
 
     def _stub_task_toml(self, tasks, plugins):
         """
         This creates a toml stub using default values, as best it can
         """
         logging.info("Building Task Toml Stub")
-        task_iden                   : DootCodeReference       = DootCodeReference.from_alias(doot.args.on_fail("task").cmd.args.ctor(), "task", plugins)
+        task_iden                   : CodeReference       = CodeReference.from_alias(doot.args.on_fail("task").cmd.args.ctor(), "task", plugins)
 
         if (name:=doot.args.on_fail((None,)).cmd.args.name()) is None:
             raise doot.errors.DootCommandError("No Name Provided for Stub")
 
         # Create stub toml, with some basic information
         stub                          = TaskStub(ctor=task_iden)
-        stub['name'].default          = DootTaskName.build(name)
+        try:
+            stub['name'].default          = TaskName.build(name)
+        except ValueError:
+            raise doot.errors.DootError("Provide a valid TaskName")
 
         # add ctor specific fields,
         # such as for dir_walker: roots [], exts [], recursive bool, subtask "", head_task ""
         # works *towards* the task_type, not away, so more specific elements are added over the top of more general elements
         try:
             task_mro = task_iden.try_import().mro()
         except TypeError as err:
@@ -203,15 +204,15 @@
         if bool(matched):
             printer.info("{ do=\"%s\", args=[] } # plus any kwargs a specific action uses", matched[0].name)
         else:
             printer.info("{ do=\"action name/import path\", args=[], inState=[], outState=[] } # plus any kwargs a specific action uses")
 
         printer.info("")
         printer.info("- For Custom Python Actions, implement the following in the .tasks directory")
-        printer.info("def custom_action(spec:DootActionSpec, task_state:dict) -> None|bool|dict:...")
+        printer.info("def custom_action(spec:ActionSpec, task_state:dict) -> None|bool|dict:...")
 
     def _stub_cli_arg(self):
         printer.info("# - CLI Arg Form. Add to task spec: cli=[]")
         printer.info("")
         stub = []
         stub.append('name="')
         stub.append(doot.args.on_fail("default").cmd.args.name())
@@ -220,14 +221,12 @@
         stub.append('prefix="-", ')
         stub.append('default="", ')
         stub.append('desc="", ')
         stub.append('positional=false ')
 
         printer.info("{ %s }", "".join(stub))
 
-    def _stub_printer_settings(self):
-        printer.info("print_levels = { %s }", ", ".join(f'{x}="INFO"' for x in PRINT_LOCATIONS))
 
     def _list_flags(self):
         printer.info("Task Flags: ")
         for x in sorted(doot.enums.TaskFlags, key=lambda x: x.name):
             printer.info("-- %s", x.name)
```

### Comparing `doot-0.7.2/doot/control/__tests/test_locations.py` & `doot-0.8.0/doot/control/__tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/control/__tests/test_overlord.py` & `doot-0.8.0/doot/control/__tests/test_overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/control/__tests/test_tracker.py` & `doot-0.8.0/doot/control/__tests/obsolete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 #!/usr/bin/env python3
 """
 
+
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
+# import abc
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
-import unittest
-import warnings
 import pathlib as pl
-from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
-                    Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
-                    TypeVar, cast)
-##-- end imports
-logging = logmod.root
-
-import pytest
-import doot
-doot._test_setup()
-
-import doot.errors
-import doot.structs
-from doot.control.tracker import DootTracker
-from doot._abstract import Task_i
-from doot.utils import mock_gen
+import re
+import time
+import types
+import weakref
+# from copy import deepcopy
+# from dataclasses import InitVar, dataclass, field
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
+                    Iterable, Iterator, Mapping, Match, MutableMapping,
+                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
+
+##-- end builtin imports
+
+##-- lib imports
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+##-- end logging
 
 @pytest.mark.parametrize("ctor", [DootTracker])
 class TestTrackerBasic:
 
     def test_initial(self, ctor):
         tracker = ctor()
         assert(tracker is not None)
@@ -71,15 +84,15 @@
                                            "subtask"   : [[], [pl.Path("blah.other")]],
                                            "subtask2"  : [[], [pl.Path("test.file")]],
 
                                           }):
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+        assert(isinstance(next_task, doot.structs.TaskArtifact))
 
     @pytest.mark.xfail
     def test_task_artifact_exists(self, ctor, mocker):
         """
           check that if artifacts exist, tasks that generate them aren't queued
         """
         mocker.patch.object(pl.Path, "exists", return_value=True)
@@ -88,29 +101,29 @@
                                            "subtask"   : [[], [pl.Path("blah.other")]],
                                            "subtask2"  : [[], [pl.Path("test.file")]],
 
                                           }):
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+        assert(isinstance(next_task, doot.structs.TaskArtifact))
 
     @pytest.mark.skip
     def test_task_artifact_doesnt_exists(self, ctor, mocker):
         mocker.patch.object(pl.Path, "exists", return_value=False)
         tracker = ctor()
         for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
                                            "subtask"   : [[], [pl.Path("blah.other")]],
                                            "subtask2"  : [[], [pl.Path("test.file")]],
 
                                           }):
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+        assert(isinstance(next_task, doot.structs.TaskArtifact))
 
     @pytest.mark.xfail
     def test_task_artifact_partial_exists(self, ctor, mocker):
 
         def temp_exists(self):
             return not "*" in self.stem
 
@@ -120,26 +133,26 @@
                                            "subtask"   : [[], [pl.Path("blah.other")]],
                                            "subtask2"  : [[], [pl.Path("test.file")]],
 
                                           }):
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+        assert(isinstance(next_task, doot.structs.TaskArtifact))
 
 @pytest.mark.parametrize("ctor", [DootTracker])
 class TestTrackerInsertion:
 
     def test_add_task(self, ctor, mocker):
         mock_task = mock_gen.mock_task("task1")
         tracker = ctor()
         tracker.add_task(mock_task)
 
         assert("default::task1" in tracker.tasks)
-        assert(tracker.task_graph.nodes['default::task1']['state'] == tracker.state_e.DEFINED)
+        assert(tracker.task_graph.nodes['default::task1']['state'] == TaskStatus_e.DEFINED)
 
     def test_duplicate_add_fail(self, ctor, mocker):
         """ dont add a duplicately named task, or its dependencies """
         task1 = mock_gen.mock_task("task1")
         task2 = mock_gen.mock_task("task1")
 
         tracker = ctor()
@@ -175,37 +188,37 @@
         mock_task = mock_gen.mock_task("test_task")
         mock_task.spec.depends_on.append("example")
         mock_task.spec.depends_on.append("blah")
 
         tracker = ctor()
         tracker.add_task(mock_task)
 
-        assert(tracker.task_graph.nodes['example']['state'] == tracker.state_e.DECLARED)
-        assert(tracker.task_graph.nodes['blah']['state'] == tracker.state_e.DECLARED)
+        assert(tracker.task_graph.nodes['example']['state'] == TaskStatus_e.DECLARED)
+        assert(tracker.task_graph.nodes['blah']['state'] == TaskStatus_e.DECLARED)
         assert("example" in tracker.task_graph)
         assert("blah" in tracker.task_graph)
 
     @pytest.mark.skip
     def test_task_post_registration(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
-        mock_task.required_for.append(doot.structs.DootTaskName.build("example"))
-        mock_task.required_for.append(doot.structs.DootTaskName.build("blah"))
+        mock_task.required_for.append(doot.structs.TaskName.build("example"))
+        mock_task.required_for.append(doot.structs.TaskName.build("blah"))
 
         tracker = ctor()
         tracker.add_task(mock_task)
-        assert(tracker.task_graph.nodes['default::example']['state'] == tracker.state_e.DECLARED)
-        assert(tracker.task_graph.nodes['default::blah']['state'] == tracker.state_e.DECLARED)
+        assert(tracker.task_graph.nodes['default::example']['state'] == TaskStatus_e.DECLARED)
+        assert(tracker.task_graph.nodes['default::blah']['state'] == TaskStatus_e.DECLARED)
         assert("default::example" in tracker.task_graph)
         assert("default::blah" in tracker.task_graph)
 
     @pytest.mark.skip
     def test_declared_set(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
-        mock_task.depends_on   += map(doot.structs.DootTaskName.build, ["subtask", "sub2"])
-        mock_task.required_for += map(doot.structs.DootTaskName.build, ["example", "blah"])
+        mock_task.depends_on   += map(doot.structs.TaskName.build, ["subtask", "sub2"])
+        mock_task.required_for += map(doot.structs.TaskName.build, ["example", "blah"])
 
         tracker = ctor()
         tracker.add_task(mock_task)
         declared = tracker.declared_set()
         assert(declared == {"__root", "default::test_task", "default::subtask","default::sub2", "default::example", "default::blah"})
 
     def test_defined_set(self, ctor, mocker):
@@ -251,23 +264,23 @@
 
         tracker  = ctor()
         for task in tasks:
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
         assert(next_task.name == "default::subsub")
-        tracker.update_state(next_task, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task, TaskStatus_e.SUCCESS)
 
         next_task_2 = tracker.next_for()
         assert(next_task_2.name in {"default::subtask", "default::subtask2"})
-        tracker.update_state(next_task_2, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task_2, TaskStatus_e.SUCCESS)
 
         next_task_3 = tracker.next_for()
         assert(next_task_3.name in {"default::subtask", "default::subtask2"} - {next_task_2.name})
-        tracker.update_state(next_task_3, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task_3, TaskStatus_e.SUCCESS)
 
         next_task_4 = tracker.next_for()
         assert(next_task_4.name in "default::task1")
 
     def test_task_iter(self, ctor, mocker):
         tasks = mock_gen.task_network({
             "task1"   : [["default::subtask", "default::subtask2", "default::subtask3"], []],
@@ -284,50 +297,50 @@
             tracker.add_task(task)
 
         result_tasks = []
         tracker.queue_task("default::task1")
         for x in tracker:
             if x:
                 result_tasks.append(x.name)
-                tracker.update_state(x.name, tracker.state_e.SUCCESS)
+                tracker.update_status(x.name, TaskStatus_e.SUCCESS)
 
         assert(len(result_tasks) == 5)
 
     def test_task_iter_state_changed(self, ctor, mocker):
         tracker  = ctor()
         for task in mock_gen.task_network({"task1"   : [["default::subtask", "default::subtask2", "default::subtask3"], []],
                                            "subtask" : [["default::subsub"], []],
                                            "subtask2": [["default::subsub"], []],
                                            "subtask3": [["default::subsub"], []],
                                            "subsub"  : [[], []]
                                           }):
             tracker.add_task(task)
 
-        tracker.update_state("default::subtask2", tracker.state_e.SUCCESS)
+        tracker.update_status("default::subtask2", TaskStatus_e.SUCCESS)
         tasks = []
         tracker.queue_task("default::task1")
         for x in tracker:
             if x:
                 tasks.append(x.name)
-                tracker.update_state(x.name, tracker.state_e.SUCCESS)
+                tracker.update_status(x.name, TaskStatus_e.SUCCESS)
 
         assert("default::subtask2" not in tasks)
         assert(len(tasks) == 4)
 
     @pytest.mark.xfail
     def test_task_failure(self, ctor, mocker, caplog):
         tracker = ctor()
         for task in mock_gen.task_network({"task1"   : [["default::subtask"], []],
                                            "subtask" : [["default::subsub"], []],
                                           }):
             tracker.add_task(task)
 
         result = tracker.next_for("default::task1")
         assert(result.name == "default::subtask")
-        tracker.update_state(result, tracker.state_e.SUCCESS)
+        tracker.update_status(result, TaskStatus_e.SUCCESS)
         assert(tracker.next_for().name == "default::task1")
         assert("Tried to Schedule a Declared but Undefined Task: subsub" in caplog.messages)
 
     def test_post_task_order(self, ctor, mocker):
         tracker = ctor()
         for task in mock_gen.task_network({"task1"     : [["default::subtask", "default::subtask2"], []],
                                            "subtask"   : [["default::subsub"], ["default::sidesuper"]],
@@ -336,23 +349,23 @@
                                            "sidesuper" : [[], []],
 
                                           }):
             tracker.add_task(task)
 
         next_task = tracker.next_for("default::task1")
         assert(next_task.name == "default::subtask2")
-        tracker.update_state(next_task, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task, TaskStatus_e.SUCCESS)
 
         next_task_2 = tracker.next_for()
         assert(next_task_2.name == "default::subsub")
-        tracker.update_state(next_task_2, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task_2, TaskStatus_e.SUCCESS)
 
         next_task_3 = tracker.next_for()
         assert(next_task_3.name == "default::subtask")
-        tracker.update_state(next_task_3, tracker.state_e.SUCCESS)
+        tracker.update_status(next_task_3, TaskStatus_e.SUCCESS)
 
         next_task_4 = tracker.next_for()
         assert(next_task_4.name == "default::task1" )
 
 class TestTrackerPersistence:
 
     @pytest.mark.skip("TODO")
```

### Comparing `doot-0.7.2/doot/control/base_runner.py` & `doot-0.8.0/doot/control/base_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,142 @@
 #!/usr/bin/env python3
 """
 
 See EOF for license/metadata/notes as applicable
 """
 
-##-- builtin imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
 # import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
+from collections import defaultdict
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 
-##-- end builtin imports
+# ##-- end stdlib imports
 
-##-- lib imports
+# ##-- 3rd party imports
 import more_itertools as mitz
-##-- end lib imports
 
-##-- logging
-logging = logmod.getLogger(__name__)
-printer = logmod.getLogger("doot._printer")
-##-- end logging
+# ##-- end 3rd party imports
 
-from collections import defaultdict
+# ##-- 1st party imports
 import doot
 import doot.errors
-from doot.enums import ReportEnum, ActionResponseEnum as ActRE, TaskStateEnum
-from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i, ReportLine_i, Action_p, Reporter_i
-from doot.structs import DootTaskArtifact, DootActionSpec
-from doot.utils.signal_handler import SignalHandler
-from doot.structs import DootTaskSpec, DootActionSpec
+from doot._abstract import (Action_p, FailPolicy_p, Job_i, Reporter_p, Task_i,
+                            TaskRunner_i, TaskTracker_i)
+from doot.enums import ActionResponseEnum as ActRE
+from doot.enums import ReportEnum, TaskStatus_e
+from doot.structs import ActionSpec, TaskArtifact, TaskSpec
 from doot.utils.log_context import DootLogContext
+from doot.utils.signal_handler import SignalHandler
+
+# ##-- end 1st party imports
+
+##-- logging
+logging    = logmod.getLogger(__name__)
+printer    = logmod.getLogger("doot._printer")
+setup_l    = printer.getChild("setup")
+taskloop_l = printer.getChild("task_loop")
+report_l   = printer.getChild("report")
+success_l  = printer.getChild("success")
+fail_l     = printer.getChild("fail")
+sleep_l    = printer.getChild("sleep")
+artifact_l = printer.getChild("artifact")
+##-- end logging
 
 dry_run                                      = doot.args.on_fail(False).cmd.args.dry_run()
 head_level           : Final[str]            = doot.constants.printer.DEFAULT_HEAD_LEVEL
 build_level          : Final[str]            = doot.constants.printer.DEFAULT_BUILD_LEVEL
 action_level         : Final[str]            = doot.constants.printer.DEFAULT_ACTION_LEVEL
 sleep_level          : Final[str]            = doot.constants.printer.DEFAULT_SLEEP_LEVEL
 execute_level        : Final[str]            = doot.constants.printer.DEFAULT_EXECUTE_LEVEL
 enter_level          : Final[str]            = doot.constants.printer.DEFAULT_ENTER_LEVEL
 max_steps            : Final[str]            = doot.config.on_fail(100_000).settings.tasks.max_steps()
-fail_prefix          : Final[str]            = doot.constants.printer.FAILURE_PREFIX
+fail_prefix          : Final[str]            = doot.constants.printer.fail_prefix
+loop_entry_msg       : Final[str]            = doot.constants.printer.loop_entry
+loop_exit_msg        : Final[str]            = doot.constants.printer.loop_exit
 
 default_SLEEP_LENGTH : Fina[int|float]       = doot.config.on_fail(0.2, int|float).settings.tasks.sleep.task()
 logctx               : Final[DootLogContext] = DootLogContext(printer)
 
 class BaseRunner(TaskRunner_i):
     """ An incomplete implementation for runners to extend """
 
-    def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_i, policy=None):
+    def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_p):
         self.tracker                                          = tracker
         self.reporter                                         = reporter
-        self.policy                                           = policy
         self.step                                             = 0
         self._signal_failure : None|doot.errors.DootError     = None
-        self._enter_msg                                       = "---------- Task Loop Starting ----------"
-        self._exit_msg                                        = "---------- Task Loop Finished ----------"
+        self._enter_msg                                       = loop_entry_msg
+        self._exit_msg                                        = loop_exit_msg
 
     def __enter__(self) -> Any:
-        printer.info("- Validating Task Network, building remaining abstract tasks: %s", self.tracker.late_count)
-        self.tracker.validate()
-        printer.info(self._enter_msg, extra={"colour" : "green"})
+        setup_l.info("Building Task Network...")
+        self.tracker.build_network()
+        setup_l.info("Task Network Built. %s Nodes, %s Edges, %s Edges from Root.",
+                     len(self.tracker.network.nodes), len(self.tracker.network.edges), len(self.tracker.network.pred[self.tracker._root_node]))
+        setup_l.info("Validating Task Network...")
+        self.tracker.validate_network()
+        setup_l.info("Validation Complete")
+        taskloop_l.info(self._enter_msg, extra={"colour" : "green"})
         return
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
         # TODO handle exc_types?
         printer.setLevel("INFO")
-        printer.info("")
-        printer.info(self._exit_msg, extra={"colour":"green"})
+        taskloop_l.info("")
+        taskloop_l.info(self._exit_msg, extra={"colour":"green"})
         self._finish()
         return
 
     def _finish(self):
         """finish running tasks, summarizing results using the reporter
           separate from __exit__ to allow it to be overridden
         """
-        logging.info("Task Running Completed")
+        report_l.info("Task Running Completed")
         if self.step >= max_steps:
-            printer.info("Runner Hit the Step Limit: %s", max_steps)
+            report_l.info("Runner Hit the Step Limit: %s", max_steps)
 
-        printer.info("Final Summary: ")
-        printer.info(str(self.reporter), extra={"colour":"magenta"})
+        report_l.info("Final Summary: ")
+        report_l.info(str(self.reporter), extra={"colour":"magenta"})
         match self._signal_failure:
             case None:
                 return
             case doot.errors.DootError():
                 raise self._signal_failure
 
-    def _handle_task_success(self, task:None|Task_i|DootTaskArtifact):
+    def _handle_task_success(self, task:None|Task_i|TaskArtifact):
         """ The basic success handler. just informs the tracker of the success """
-        if task:
-            self.tracker.update_state(task, self.tracker.state_e.SUCCESS)
+        success_l.debug("(Task): %s", task)
+        match task:
+            case None:
+                pass
+            case _:
+                self.tracker.set_status(task, TaskStatus_e.SUCCESS)
         return task
 
-    def _handle_failure(self, task:None|Task_i, failure:Error) -> None:
+    def _handle_failure(self, task:Task_i, failure:Error) -> None:
         """ The basic failure handler.
           Triggers a breakpoint on DootTaskInterrupt,
           otherwise informs the tracker of the failure.
 
           Halts any failed or errored tasks, which propagates to any successors
           Fails any DootErrors, TrackingErrors, and non-doot errors
 
@@ -121,45 +144,44 @@
         """
         match failure:
             case doot.errors.DootTaskInterrupt():
                 breakpoint()
                 pass
             case doot.errors.DootTaskFailed() as err:
                 self._signal_failure = err
-                printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(err.task.name, self.tracker.state_e.HALTED)
+                fail_l.warning("%s %s", fail_prefix, err)
+                self.tracker.set_status(err.task, TaskStatus_e.HALTED)
             case doot.errors.DootTaskError() as err:
                 self._signal_failure = err
-                printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(err.task.name, self.tracker.state_e.HALTED)
+                fail_l.warning("%s %s", fail_prefix, err)
+                self.tracker.set_status(err.task, TaskStatus_e.FAILED)
             case doot.errors.DootError() as err:
                 self._signal_failure = err
-                printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(task, self.tracker.state_e.FAILED)
+                fail_l.warning("%s %s", fail_prefix, err)
+                self.tracker.set_status(task, TaskStatus_e.FAILED)
             case doot.errors.DootTaskTrackingError() as err:
                 self._signal_failure = err
-                printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(task, self.tracker.state_e.FAILED)
+                fail_l.warning("%s %s", fail_prefix, err)
+                self.tracker.set_status(task, TaskStatus_e.FAILED)
             case _:
                 self._signal_failure = doot.errors.DootError("Unknown Failure")
-                printer.exception("%s Unknown failure occurred: %s", fail_prefix, failure)
-                self.tracker.update_state(task, self.tracker.state_e.FAILED)
+                fail_l.exception("%s Unknown failure occurred: %s", fail_prefix, failure)
+                self.tracker.set_status(task, TaskStatus_e.FAILED)
 
     def _sleep(self, task):
         """
           The runner's sleep method, which spaces out tasks
         """
         match task:
             case None:
                 return
-            case DootTaskArtifact():
+            case TaskArtifact():
                 return
 
-        with logctx(task.spec.print_levels.on_fail(sleep_level).sleep()) as p:
-            sleep_len = task.spec.extra.on_fail(default_SLEEP_LENGTH, int|float).sleep()
-            p.info("[Sleeping (%s)...]", sleep_len, extra={"colour":"white"})
-            time.sleep(sleep_len)
+        sleep_len = task.spec.extra.on_fail(default_SLEEP_LENGTH, int|float).sleep()
+        sleep_l.debug("[Sleeping (%s)...]", sleep_len, extra={"colour":"white"})
+        time.sleep(sleep_len)
 
-    def _notify_artifact(self, art:DootTaskArtifact) -> None:
+    def _notify_artifact(self, art:TaskArtifact) -> None:
         """ A No-op for when the tracker gives an artifact """
-        printer.info("---- Artifact: %s", art)
+        artifact_l.info("---- Artifact: %s : %s", art, art.to_path())
         self.reporter.add_trace(art, flags=ReportEnum.ARTIFACT)
```

### Comparing `doot-0.7.2/doot/control/base_tracker.py` & `doot-0.8.0/doot/_structs/task_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,413 +1,472 @@
 #!/usr/bin/env python3
 """
 
 See EOF for license/metadata/notes as applicable
 """
 
-##-- builtin imports
+# Imports:
 from __future__ import annotations
 
-# import abc
+# ##-- stdlib imports
 import datetime
 import enum
 import functools as ftz
+import importlib
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+from dataclasses import _MISSING_TYPE, InitVar, dataclass, field, fields
+from importlib.metadata import EntryPoint
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Literal, Mapping, Match,
+                    MutableMapping, Protocol, Self, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 
-##-- end builtin imports
+# ##-- end stdlib imports
 
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+# ##-- 3rd party imports
+from pydantic import (BaseModel, BeforeValidator, Field, ValidationError,
+                      ValidationInfo, ValidatorFunctionWrapHandler,
+                      WrapValidator, field_validator, model_validator)
+from tomlguard import TomlGuard
+from typing_extensions import Annotated
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
+import doot
+import doot.errors
+from doot._abstract.protocols import SpecStruct_p
+from doot._abstract.task import Task_i
+from doot._structs.action_spec import ActionSpec
+from doot._structs.artifact import TaskArtifact
+from doot._structs.code_ref import CodeReference
+from doot._structs.relation_spec import RelationSpec
+from doot._structs.task_name import TaskName
+from doot.enums import (LocationMeta, RelationMeta, ReportEnum, TaskFlags,
+                        TaskQueueMeta)
+
+# ##-- end 1st party imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
-import networkx as nx
-import boltons.queueutils
-from collections import defaultdict
-import tomlguard
-import doot
-import doot.errors
-from doot.enums import TaskStateEnum, TaskQueueMeta
-from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference, DootActionSpec
-from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i
-from doot.task.base_task import DootTask
-
-class EDGE_E(enum.Enum):
-    """ Enum describing the possible edges of the task tracker's task network """
-    TASK               = enum.auto()
-    ARTIFACT           = enum.auto()
-    TASK_CROSS         = enum.auto() # Task to artifact
-    ARTIFACT_CROSS     = enum.auto() # artifact to task
-
-ROOT             : Final[str]                  = "__root" # Root node of dependency graph
-STATE            : Final[str]                  = "state"  # Node attribute name
-PRIORITY         : Final[str]                  = "priority"
-REACTIVE_ADD     : Final[str]                  = "reactive-add"
-COMPLETE_STATES  : Final[set[TaskStateEnum]]   = {TaskStateEnum.SUCCESS, TaskStateEnum.EXISTS}
-ARTIFACT_EDGES   : Final[set[EDGE_E]]          = [EDGE_E.ARTIFACT, EDGE_E.TASK_CROSS]
-DECLARE_PRIORITY : Final[int]                  = 10
-MIN_PRIORITY     : Final[int]                  = -10
-
-class _InternalTrackerBase(TaskTracker_i):
-    """ Standard implementation of private tracker methods and plumbing """
-
-    state_e            = TaskStateEnum
-    INITIAL_TASK_STATE = TaskStateEnum.DEFINED
-
-    def __init__(self, shadowing:bool=False, *, policy=None):
-        self.policy                                                              = policy
-        self.tasks                   : dict[str, Task_i]                         = {}
-        self.artifacts               : dict[str, DootTaskArtifact]               = {}
-        self.task_graph              : nx.DiGraph                                = nx.DiGraph()
-        self.active_set              : list[str|DootTaskName|DootTaskArtifact]   = set()
-        self.execution_path          : list[str]                                 = []
-        self.shadowing               : bool                                      = shadowing
-        self._root_name              : str                                       = ROOT
-        self._build_late             : list[str]                                 = list()
-        self.task_queue                                                          = boltons.queueutils.HeapPriorityQueue()
-        self._declare_priority                                                   = DECLARE_PRIORITY
-        self._min_priority                                                       = MIN_PRIORITY
-
-        self.task_graph.add_node(ROOT, state=self.state_e.WAIT)
-
-    def __bool__(self):
-        return bool(self.active_set)
-
-    def __len__(self):
-        return len(self.tasks)
-
-    def __iter__(self) -> Generator[Any,Any,Any]:
-        while bool(self):
-            logging.info("Tracker Queue: %s", self.active_set)
-            yield self.next_for()
-
-    def __contains__(self, target:str) -> bool:
-        # TODO handle definite artifacts -> indefinite artifacts
-        return target in self.tasks
-
-    def _prep_task(self, spec:DootTaskSpec|Task_i) -> Task_i:
-        """ Internal utility method to convert task identifier into actual task
-        doesn't modify tracker state
-        """
-        # Build the Task if necessary
+def _prepare_action_group(deps:list[str], handler:ValidatorFunctionWrapHandler, info:ValidationInfo) -> list[RelationSpec|ActionSpec]:
+    """
+      Prepares action groups / dependencies,
+      converting toml specified strings, list, and dicts to Artifacts (ie:files), Task Names, ActionSpecs
+
+      As a wrap handler, it has the context of what field is being processed,
+      this allows it to set the correct RelationMeta type
+
+      # TODO handle callables?
+    """
+    results = []
+    if deps is None:
+        return results
+
+    relation_type = RelationMeta.requirementFor if info.field_name in TaskSpec._dependant_groups else RelationMeta.dependencyOf
+    for x in deps:
+        match x:
+            case ActionSpec() | RelationSpec():
+                results.append(x)
+            case { "do": action  }:
+                results.append(ActionSpec.build(x))
+            case _:
+                results.append(RelationSpec.build(x, relation=relation_type))
+
+    return handler(results)
 
-        match spec:
-            case DootTaskSpec(ctor=str()|DootTaskName() as ctor) if str(ctor) in self.tasks:
-                # specialize a loaded task
-                base_spec           = self.tasks.get(str(ctor)).spec
-                initial_specialized = base_spec.specialize_from(spec)
-                cli_specialized     = self._insert_cli_args_into_spec(initial_specialized)
-                task : Task_i       = cli_specialized.make()
-            case DootTaskSpec(ctor=DootCodeReference() as ctor) if spec.check(ensure=Task_i):
-                # Specialized a custom task class
-                cli_specialized   = self._insert_cli_args_into_spec(spec)
-                task : Task_i     = cli_specialized.make()
-            case DootTaskSpec():
-                cli_specialized   = self._insert_cli_args_into_spec(spec)
-                task : Task_i = DootTask(cli_specialized)
-            case Task_i():
-                task = spec
+ActionGroup = Annotated[list[ActionSpec|RelationSpec], WrapValidator(_prepare_action_group)]
+
+class _SpecUtils_m:
+
+    def instantiate_onto(self, data:None|TaskSpec) -> TaskSpec:
+        """ apply self over the top of data """
+        match data:
+            case None:
+                return self.specialize_from(self)
+            case TaskSpec():
+                return data.specialize_from(self)
             case _:
-                raise doot.errors.DootTaskTrackingError("Unknown task attempted to be added: %s", spec)
+                raise TypeError("Can't instantiate onto something not a task spec", data)
+
+    def instantiate_transformer(self, target:TaskArtifact|tuple[TaskArtifact, TaskArtifact]) -> None|TaskSpec:
+        """ Create an instantiated transformer spec.
+          ie     : ?.txt -> spec -> ?.blah
+          becomes: a.txt -> spec -> a.blah
 
-        # Check it doesn't shadow another task
-        match task.name in self.tasks, task.name in self.task_graph:
-            case True, False:
-                raise doot.errors.DootTaskTrackingError("Task exists in defined tasks, but not the task graph")
-            case True, True if not self.shadowing:
-                raise doot.errors.DootTaskTrackingError("Task with Duplicate Name not added: ", task.name)
-            case True, True:
-                logging.warning("Task Shadowed by Duplicate Name: %s", task.readable_name)
-            case False, True:
-                logging.debug("Defining a declared dependency task: %s", task.readable_name)
-
-        return task
-
-    def _add_artifact(self, artifact:DootTaskArtifact) -> str:
-        """ convert a path to an artifact, and connect it with matching artifacts """
-        match artifact:
-            case _ if str(artifact) in self.artifacts: # artifact already known
+          can be given one artifact, which will be used for matching on pre and post,
+          or a tuple, which specifies an exact transform
+
+          TODO: handle ?/?.txt, */?.txt, blah/*/?.txt, path/blah.?
+        """
+        match target:
+            case TaskArtifact():
+                pre, post = target, target
+            case (TaskArtifact() as pre, TaskArtifact() as post):
                 pass
-            case DootTaskArtifact() if artifact.is_definite: # x/y/y.ext
-                self.artifacts[str(artifact)] = artifact
-                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
-                # connect to matching indefinites
-                for x in filter(lambda x: artifact in x, self.artifacts.values()):
-                    self.task_graph.add_edge(str(artifact), str(x), type=EDGE_E.ARTIFACT)
-            case DootTaskArtifact(): # x/*/*.ext
-                self.artifacts[str(artifact)] = artifact
-                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
-                # connect to definites
-                for x in filter(lambda x: x in artifact, self.artifacts.values()):
-                    self.task_graph.add_edge(str(x), str(artifact), type=EDGE_E.ARTIFACT)
 
-        return str(artifact)
+        instance = self.instantiate_onto(None)
+        match self.transformer_of():
+            case None:
+                raise doot.errors.DootTaskTrackingError("Tried to transformer instantiate a non-transformer", self.name)
+            case (x, y) if pre in x.target or post in y.target:
+                # exact transform
+                # replace x with pre in depends_on
+                instance.depends_on.remove(x)
+                instance.depends_on.append(x.instantiate(pre))
+                # replace y with post in required_for
+                instance.required_for.remove(y)
+                instance.required_for.append(y.instantiate(post))
+            case _:
+                return None
+
+        return instance
 
-    def _build_head(self, spec:DootTaskSpec) -> None|TaskSpec:
+    def make(self, ensure:type=Any) -> Task_i:
+        """ Create actual task instance """
+        task_ctor = self.ctor.try_import(ensure=ensure)
+        return task_ctor(self)
+
+    def job_top(self) -> None|TaskSpec:
         """
-          Build a head task for a job, taking the jobs cleanup actions
+          Generate a top spec for a job, taking the jobs cleanup actions
           and using them as the head's main action.
           Depends on the job, and its reactively queued.
         """
+        if TaskFlags.JOB not in self.flags:
+            return None
+        if (TaskFlags.CONCRETE | TaskFlags.JOB_HEAD) & self.flags:
+            return None
+        if self.name.job_head() == self.name:
+            return None
+
         # build $head$
-        head : DootTaskSpec = DootTaskSpec.build({
-            "name"            : spec.name.task_head(),
-            "source"          : spec.name,
-            "actions"         : spec.cleanup,
-            "print_levels"    : spec.print_levels,
-            "extra"           : spec.extra,
+        head : TaskSpec = TaskSpec.build({
+            "name"            : self.name.job_head(),
+            "sources"         : self.sources[:] + [self.name, None],
+            "actions"         : self.cleanup,
+            "extra"           : self.extra,
             "queue_behaviour" : TaskQueueMeta.reactive,
-            "depends_on"      : [spec.name],
+            "depends_on"      : [self.name] + [x for x in self.cleanup if isinstance(x, RelationSpec)],
+            "flags"           : (self.flags | TaskFlags.JOB_HEAD) & ~TaskFlags.JOB,
             })
+        assert(TaskFlags.JOB not in head.name)
+        assert(TaskFlags.JOB not in head.flags)
         return head
 
-    def _insert_cli_args_into_spec(self, spec:DootTaskSpec) -> DootTaskSpec:
-        """ Takes a task spec, and inserts matching cli args into it if necessary """
-        spec_extra : dict = dict(spec.extra.items() or [])
-
-        for cli in spec.extra.on_fail([]).cli():
-            if cli.name not in spec_extra:
-                spec_extra[cli.name] = cli.default
-
-        if spec.name not in doot.args.on_fail({}).tasks():
-            spec.extra = tomlguard.TomlGuard(spec_extra)
-            return spec
-
-        for key,val in doot.args.tasks[str(spec.name)].items():
-            spec_extra[key] = val
-
-        spec.extra = tomlguard.TomlGuard(spec_extra)
-
-        return spec
-
-    def _insert_dependencies(self, task):
-        """ insert a task's dependencies into the network, connecting them to the task """
-        for pre in task.depends_on:
-            logging.debug("Connecting Dependency: %s -> %s", pre, task.readable_name)
-            match pre:
-                case DootActionSpec():
-                    # Action spec dependencies are tested when running, not as part of the DAG
-                    # TODO use decorations to know about implicit depencies, eg: artifacts
+    def match_with_constraints(self, control:TaskSpec, *, relation:None|RelationSpec=None) -> bool:
+        """ Test this spec to see if it matches a spec,
+          when using a given relation and a given controlling spec to source values from
+
+          if not given a relation, acts as a coherence check between
+          self(a concrete spec) and control(the abstract source spec)
+          """
+        match relation:
+            case None:
+                assert(control.name <= self.name)
+                constraints = control.extra.keys()
+            case RelationSpec(constraints=None):
+                return True
+            case RelationSpec(constraints=constraints):
+                assert(relation.target <= self.name)
+
+        extra         = self.extra
+        control_extra = control.extra
+        for k in constraints:
+            if k not in extra:
+                return False
+            if extra[k] != control_extra[k]:
+                return False
+        else:
+            return True
+
+    def build_relevant_data(self, context:RelationSpec) -> dict:
+        """ Builds a dict of the data a matching spec will need, according
+          to a relations constraints.
+        """
+        if not bool(context.constraints):
+            return {}
+        extra = self.extra
+        return {k:extra[k] for k in context.constraints}
+
+    def transformer_of(self) -> None|tuple[RelationSpec, RelationSpec]:
+        """ If this spec can transform an artifact,
+          return those relations.
+
+          Transformers have file relations of a single solo abstract artifact
+          so: 'file:>a/path/?.txt' -> 'file:>b/path/?.bib'
+          (other relations can exist as well, but to be a transformer there needs to
+          be only 1 in, 1 out solo file relation
+
+          """
+        match self._transform:
+            case False:
+                return None
+            case (x,y):
+                return self._transform
+            case None:
+                pass
+
+        assert(TaskFlags.TRANSFORMER in self.flags)
+
+        pre, post = None, None
+        for x in self.depends_on:
+            match x:
+                case RelationSpec(target=TaskArtifact() as target) if LocationMeta.glob in target:
                     pass
-                case DootTaskArtifact():
-                    pre = self._add_artifact(pre)
-                    self.task_graph.add_edge(pre, task.name, type=EDGE_E.ARTIFACT_CROSS)
-                case DootTaskName() if all([(in_graph:=str(pre) in self.task_graph),(has_args:=bool(pre.args))]):
-                    base_spec                 = self.tasks[str(pre)].spec
-                    name_spec                 = DootTaskSpec.build(pre)
-                    name_spec.ctor            = base_spec.name
-                    name_spec.required_for.append(task.name)
-                    self.add_task(name_spec, no_root_connection=True)
-                case DootTaskName() if in_graph and not has_args:
-                    # just connect if the tracker already knows the task
-                    self.task_graph.add_edge(str(pre), task.name, type=EDGE_E.TASK)
-                case DootTaskName() if has_args:
-                    assert(str(pre) not in self.task_graph.nodes)
-                    name_spec      = DootTaskSpec.build(pre.specialize(info="late"))
-                    name_spec.ctor = pre
-                    name_spec.required_for.append(task.name)
-                    self._build_late.append(name_spec)
-                case str() | DootTaskName():
-                    logging.debug("Adding Dummy Dependency Task: %s -> %s", task.readable_name, pre)
-                    # Otherwise add a dummy task until its defined
-                    self.task_graph.add_node(str(pre), state=self.state_e.DECLARED, priority=self._declare_priority)
-                    self.task_graph.add_edge(str(pre), task.name, type=EDGE_E.TASK)
+                case RelationSpec(target=TaskArtifact() as target) if LocationMeta.abstract in target:
+                    if pre is not None:
+                        self._transform = False
+                        return None
+                    pre = x
                 case _:
-                    raise doot.errors.DootTaskTrackingError("Unknown dependency task attempted to be added: %s", pre)
-
-    def _insert_dependents(self, task):
-        """ insert a task's downstream dependents into the network, connecting them to the task """
-        for post in task.required_for:
-            logging.debug("Connecting Successor: %s -> %s", task.readable_name, post)
-            match post:
-                case DootActionSpec():
+                    pass
 
+        for y in self.required_for:
+            match x:
+                case RelationSpec(target=TaskArtifact() as target) if LocationMeta.glob in target:
                     pass
-                case DootTaskArtifact():
-                    post = self._add_artifact(post)
-                    self.task_graph.add_edge(task.name, post, type=EDGE_E.TASK_CROSS)
-                case DootTaskName() if all([(in_graph:=str(post) in self.task_graph), (has_args:=bool(post.args))]):
-                    base_spec                 = self.tasks[str(post)].spec
-                    name_spec                 = DootTaskSpec.build(post)
-                    name_spec.ctor            = base_spec.name
-                    name_spec.depends_on.append(task.name)
-                    self.add_task(name_spec)
-                case DootTaskName() if in_graph and not has_args:
-                    # just connect if the tracker already knows the task
-                    self.task_graph.add_edge(task.name, str(post), type=EDGE_E.TASK)
-                case DootTaskName() if has_args:
-                    assert(str(post) not in self.task_graph.nodes)
-                    name_spec      = DootTaskSpec.build(post.specialize(info="late"))
-                    name_spec.ctor = post
-                    name_spec.depends_on.append(task.name)
-                    self._build_late.append(name_spec)
-                case str() | DootTaskName():
-                    logging.debug("Adding Dummy Dependent Task: %s -> %s", task.readable_name, post)
-                    # Otherwise add a dummy task until its defined
-                    self.task_graph.add_node(str(post), state=self.state_e.DECLARED, priority=self._declare_priority)
-                    self.task_graph.add_edge(task.name, str(post), type=EDGE_E.TASK)
+                case RelationSpec(target=TaskArtifact() as target) if LocationMeta.abstract in target:
+                    if post is not None:
+                        self._transform = False
+                        return None
+                    post = y
                 case _:
-                    raise doot.errors.DootTaskTrackingError("Unknown successor task attempted to be added: %s", post)
+                    pass
+
+        match pre, post:
+            case None, _:
+                self._transform = False
+                return None
+            case _, None:
+                self._transform = False
+                return None
+            case RelationSpec(), RelationSpec():
+                self._transform = (pre, post)
+                return self._transform
+
+        raise ValueError("This shouldn't be possible")
+
+class TaskSpec(_SpecUtils_m, BaseModel, arbitrary_types_allowed=True, extra="allow"):
+    """ The information needed to describe a generic task.
+    Optional things are shoved into 'extra', so things can use .on_fail on the tomlguard
+
+    the cli parser can understand cli=[{}] specs
+    actions                      : list[ [args] | {do='', args=[], **kwargs} ]
+
+    Notes:
+      sources = [root, ... grandparent, parent]. 'None' indicates halt on climbing source chain
+
+    """
+    name                         : str|TaskName
+    doc                          : list[str]                                                               = []
+    sources                      : list[TaskName|pl.Path|None]                                         = []
+
+    # Action Groups:
+    actions                      : ActionGroup                                                             = []
+    required_for                 : ActionGroup                                                             = []
+    depends_on                   : ActionGroup                                                             = []
+    setup                        : ActionGroup                                                             = []
+    cleanup                      : ActionGroup                                                             = []
+    on_fail                      : ActionGroup                                                             = []
+
+    # Any additional information:
+    version                      : str                                                                     = doot.__version__ # TODO: make dict?
+    priority                     : int                                                                     = 10
+    ctor                         : CodeReference                                                       = Field(default=None, validate_default=True)
+    queue_behaviour              : TaskQueueMeta                                                           = TaskQueueMeta.default
+    flags                        : TaskFlags                                                               = TaskFlags.default
+    _transform                   : None|Literal[False]|tuple[RelationSpec, RelationSpec]                            = None
+    # task specific extras to use in state
+    _default_ctor         : ClassVar[str]       = doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS
+    _allowed_print_locs   : ClassVar[list[str]] = doot.constants.printer.PRINT_LOCATIONS
+    _action_group_wipe    : ClassVar[dict]      = {"required_for": [], "setup": [], "actions": [], "depends_on": []}
+    # Action Groups that are dependant on, rather than are dependencies of, this task:
+    _dependant_groups    : ClassVar[list[str]]  = ["required_for", "on_fail"]
+
+    @staticmethod
+    def build(data:TomlGuard|dict|TaskName|str) -> Self:
+        match data:
+            case TomlGuard() | dict() if "source" in data:
+                raise ValueError("source is deprecated, use 'sources'", data)
+            case TomlGuard() | dict():
+                return TaskSpec.model_validate(data)
+            case TaskName():
+                return TaskSpec(name=data)
+            case str():
+                return TaskSpec(name=TaskName.build(data))
+
+    @model_validator(mode="before")
+    def _convert_toml_keys(cls, data:dict) -> dict:
+        """ converts a-key into a_key, and joins group+name """
+        cleaned = {k.replace("-","_") : v  for k,v in data.items()}
+        if "group" in cleaned and TaskName._separator not in cleaned["name"]:
+            cleaned['name'] = TaskName._separator.join([cleaned['group'], cleaned['name']])
+            del cleaned['group']
+        return cleaned
+
+    @model_validator(mode="after")
+    def _validate_metadata(self):
+        self.flags |= self.name.meta
+        if self.extra.on_fail(False).disabled():
+            self.flags |= TaskFlags.DISABLED
+        try:
+            match self.ctor.try_import():
+                case x if issubclass(x, Task_i):
+                    self.flags |= x._default_flags
+                    self.name.meta |= x._default_flags
+                case x:
+                    pass
+        except ImportError as err:
+            logging.warning("Ctor Import Failed for: %s : %s", self.name, self.ctor)
+            self.flags |= TaskFlags.DISABLED
+            self.ctor = None
+
+        if TaskFlags.TRANSFORMER not in self.flags:
+            self._transform = False
+
+        self.name.meta |= self.flags
+        return self
+
+    @field_validator("name", mode="before")
+    def _validate_name(cls, val):
+        match val:
+            case TaskName():
+                return val
+            case str():
+                name = TaskName.build(val)
+                return name
+            case _:
+                raise TypeError("A TaskSpec Name should be a str or TaskName", val)
+
+    @field_validator("flags", mode="before")
+    def _validate_flags(cls, val):
+        match val:
+            case TaskFlags():
+                return val
+            case str()|list():
+                return TaskFlags.build(val)
+
+    @field_validator("ctor", mode="before")
+    def _validate_ctor(cls, val):
+        match val:
+            case None:
+                default_alias = TaskSpec._default_ctor
+                coderef_str   = doot.aliases.task[default_alias]
+                return CodeReference.build(coderef_str)
+            case EntryPoint():
+                return CodeReference.build(val)
+            case CodeReference():
+                return val
+            case type()|str():
+                return CodeReference.build(val)
+            case _:
+                return CodeReference.build(val)
+
+    @field_validator("queue_behaviour", mode="before")
+    def _validate_queue_behaviour(cls, val):
+        match val:
+            case TaskQueueMeta():
+                return val
+            case str():
+                return TaskQueueMeta.build(val)
+            case _:
+                raise ValueError("Queue Behaviour needs to be a str or a TaskQueueMeta enum", val)
+
+    @field_validator("sources", mode="before")
+    def _validate_sources(cls, val):
+        """ builds the soures list, converting strings to task names,
 
-    def _maybe_implicit_queue(self, task):
-        """ tasks can be activated for running by a number of different conditions
-          this handles that
           """
-        match task.spec.queue_behaviour:
-            case TaskQueueMeta.auto:
-                self.queue_task(task.name)
-            case TaskQueueMeta.reactive:
-                self.task_graph.nodes[task.name][REACTIVE_ADD] = True
-            case TaskQueueMeta.default:
-                # Waits for explicit queue
+        match val:
+            case None:
+                val = []
+            case list():
                 pass
             case _:
-                raise doot.errors.DootTaskTrackingError("Unknown queue behaviour specified: %s", task.spec.queue_behaviour)
+                val = [val]
 
-    def _task_dependencies(self, task) -> tuple[list[str], list[str]]:
-        """ get predecessors of the task,
-          return [list[incomplete], list[all]]
-        """
-        dependencies = list(self.task_graph.pred[task].keys())
-        incomplete   = list(filter(lambda x: self.task_state(x) not in COMPLETE_STATES, dependencies))
-        return incomplete, dependencies
+        result = []
+        for x in val:
+            match x:
+                case "None" | None:
+                    result.append(None)
+                case TaskName() | pl.Path():
+                    result.append(x)
+                case str():
+                    try:
+                        name = TaskName.build(x)
+                        result.append(name)
+                    except (ValueError, ValidationError):
+                        result.append(pl.Path(x))
 
-    def _task_products(self, task) -> tuple[list[str], list[str]]:
-        """
-          Get task 'required-for' files: [list[not-existing], list[total]]
-        """
-        # TODO detect 'write!' actions as implicit products
-        artifacts    = list(map(lambda x: x[0], filter(lambda x: x[1].get('type', None) in ARTIFACT_EDGES, self.task_graph.succ[str(task)].items())))
-        incomplete   = list(filter(lambda x: not bool(self.artifacts[x]), artifacts))
-        return incomplete, artifacts
-
-    def _task_dependents(self, task) -> tuple[list[str], list[str]]:
-        """ TODO get [list[incomplete], list[total]] successors for a task """
-        raise NotImplementedError()
-
-    def _reactive_queue(self, focus:str):
-        """ Queue any known task in the network that auto-reacts to a focus """
-        for adj in self.task_graph.adj[focus]:
-            if self.task_graph.nodes[adj].get(REACTIVE_ADD, False):
-                self.queue_task(adj, silent=True)
-
-    def _reactive_fail_queue(self, focus:str):
-        """ TODO: make reactive failure tasks that can be triggered from
-          a tasks 'on_fail' collection
-          """
-        raise NotImplementedError()
+        return result
 
-class BaseTracker(_InternalTrackerBase):
-    """ The public part of the standard tracker implementation """
+    def __hash__(self):
+        return hash(str(self.name))
 
     @property
-    def late_count(self):
-        """ Get the count of tasks which are to be built after all definnitions are loaded """
-        return len(self._build_late)
+    def params(self) -> dict:
+        return self.model_extra
 
-    def queue_task(self, *tasks:str|DootTaskName|DootTaskArtifact|tuple, silent=False) -> None:
-        """
-          Add tasks to the queue.
-          By default it does *not* complain on trying to re-add already queued tasks,
+    @property
+    def extra(self) -> TomlGuard:
+        return TomlGuard(self.model_extra)
+
+    @property
+    def action_groups(self):
+        # TODO: use introspection on the model to get any fields annotated as an ActionGroup
+        return [self.depends_on, self.setup, self.actions, self.cleanup, self.on_fail]
+
+    def specialize_from(self, data:dict|TaskSpec) -> TaskSpec:
         """
-        logging.debug("Queue Request: %s", tasks)
-        targets = set()
-        for task in tasks:
-            # Retrieve the actual task
-            match task:
-                case str() | DootTaskName() | DootTaskArtifact() if str(task) in self.active_set:
-                    if not silent:
-                        logging.warning("Trying to queue an already active task: %s", task)
-                    continue
-                case str() | DootTaskName() | DootTaskArtifact() if str(task) not in self.task_graph.nodes:
-                    raise doot.errors.DootTaskTrackingError("Attempted To Queue an undefined Task: %s", task)
-                case DootTaskArtifact():
-                    targets.add(task)
-                case str() | DootTaskName():
-                    # Queue successor artifacts instead of the task itself
-                    incomplete, total = self._task_products(task)
-                    if bool(incomplete) or not bool(total):
-                        targets.add(task)
-                    else:
-                        targets.update(total)
-                case _:
-                    raise doot.errors.DootTaskTrackingError("Unrecognized Queue Argument: %s", task)
+          apply data over the top of self.
+          a *single* application, as a spec on it's own has no means to look up other specs,
+          which is the tracker's responsibility.
 
-        logging.debug("Queueing: %s", targets)
-        for task in targets:
-            if str(task) not in self.active_set:
-                self.active_set.add(str(task))
-                self.task_queue.add(str(task), self.task_graph.nodes[str(task)].get(PRIORITY, self._declare_priority))
-
-    def deque_task(self) -> None:
-        """ remove the top task from the queue """
-        focus = self.task_queue.pop()
-        self.task_graph.nodes[focus][PRIORITY] -= 1
-        logging.debug("Task Priority Decrement: %s = %s", focus, self.task_graph.nodes[focus][PRIORITY])
-        self.active_set.remove(focus)
-
-    def clear_queue(self) -> None:
-        """ Remove everything from the task queue """
-        # TODO queue the task's failure/cleanup task
-        self.active_set =  set()
-        self.task_queue = boltons.queueutils.HeapPriorityQueue()
-
-    def validate(self) -> bool:
-        """ Finalise and ensure consistence of the task network.
-        run tests to check the dependency graph is acceptable
+          so source chain: [root..., self, data]
         """
-        logging.debug("Building %s abstract tasks", len(self._build_late))
-        while bool(self._build_late):
-            curr = self._build_late.pop()
-            assert(isinstance(curr, DootTaskSpec))
-            self.add_task(curr)
-
-        logging.debug("Validating Graph")
-        return all([nx.is_directed_acyclic_graph(self.task_graph),
-                    self.declared_set() == self.defined_set()
-                   ])
-
-    def declared_set(self) -> set[str]:
-        """ Get the set of tasks which have been declared, directly or indirectly """
-        return set(self.task_graph.nodes)
-
-    def defined_set(self) -> set[str]:
-        """ get the set of tasks which are explicitly defined """
-        return set(self.tasks.keys())
-
-    def task_state(self, task:str|DootTaskName|DootTaskArtifact|pl.Path) -> self.state_e:
-        """ Get the state of a task """
-        if str(task) in self.task_graph.nodes:
-            return self.task_graph.nodes[str(task)][STATE]
-        else:
-            raise doot.errors.DootTaskTrackingError("Unknown Task state requested: %s", task)
+        match data:
+            case dict():
+                specialized = dict(self)
+                specialized.update(data)
+                return TaskSpec.build(specialized)
+            case TaskSpec() if self is data:
+                # specializing on self, just instantiate a name
+                specialized           = dict(self)
+                specialized['name']   = self.name.instantiate()
+                # Otherwise theres interference:
+                specialized['sources'] = self.sources[:] + [self.name]
+                return TaskSpec.build(specialized)
+            case TaskSpec(sources=[*xs, TaskName() as x] ) if not x <= self.name:
+                raise doot.errors.DootTaskTrackingError("Tried to specialize a task that isn't based on this task", str(data.name), str(self.name), str(data.sources))
+            case TaskSpec(ctor=ctor) if self.ctor != ctor and ctor != TaskSpec._default_ctor:
+                raise doot.errors.DootTaskTrackingError("Unknown ctor for spec", data.ctor)
+            case TaskSpec():
+                specialized = dict(self)
+                specialized.update({k:v for k,v in dict(data).items() if k in data.model_fields_set})
+
+        # Then special updates
+        specialized['name']   = data.name.instantiate()
+        specialized['sources'] = self.sources[:] + [self.name, data.name]
+
+        specialized['actions']      = self.actions      + data.actions
+        specialized["depends_on"]   = self.depends_on   + data.depends_on
+        specialized["required_for"] = self.required_for + data.required_for
+        specialized["cleanup"]      = self.cleanup      + data.cleanup
+        specialized["on_fail"]      = self.on_fail      + data.on_fail
+        specialized["setup"]        = self.setup        + data.setup
+
+        specialized['flags']        = self.flags | data.flags
 
-    def all_states(self) -> dict:
-        """ Get a dict of all tasks, and their current state """
-        nodes = self.task_graph.nodes
-        return {x: y[STATE] for x,y in nodes.items()}
-
-    def write(self, target:pl.Path) -> None:
-        """ TODO Write the dependency graph to a file """
-        raise NotImplementedError()
-
-    def read(self, target:pl.Path) -> None:
-        """ TODO Read the dependency graph from a file """
-        raise NotImplementedError()
+        logging.debug("Specialized Task: %s on top of: %s", data.name.readable, self.name)
+        return TaskSpec.build(specialized)
```

### Comparing `doot-0.7.2/doot/control/locations.py` & `doot-0.8.0/doot/control/locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ##-- end logging
 
 import os
 import re
 import tomlguard
 import doot
 from doot.errors import DootDirAbsent, DootLocationExpansionError, DootLocationError
-from doot.structs import DootTaskArtifact, DootKey, TomlLocation
+from doot.structs import TaskArtifact, DootKey, Location
 from doot._structs.key import DootSimpleKey, DootMultiKey, DootNonKey
 from doot.mixins.path_manip import PathManip_m
 from doot.enums import LocationMeta
 
 KEY_PAT        = doot.constants.patterns.KEY_PATTERN
 MAX_EXPANSIONS = doot.constants.patterns.MAX_KEY_EXPANSIONS
 
@@ -56,15 +56,15 @@
       locs['{temp}/somewhere']
       will expand 'temp' (if it is a registered location)
       """
     locmeta = LocationMeta
 
     def __init__(self, root:Pl.Path):
         self._root    : pl.Path()               = root.expanduser().absolute()
-        self._data    : dict[str, TomlLocation] = dict()
+        self._data    : dict[str, Location]     = dict()
         self._loc_ctx : None|DootLocations      = None
 
     def __repr__(self):
         keys = ", ".join(iter(self))
         return f"<DootLocations : {str(self.root)} : ({keys})>"
 
     def __getattr__(self, key) -> pl.Path:
@@ -73,15 +73,15 @@
           delegates to __getitem__
           eg: locs.temp
           """
         if key == "__self__":
             return None
         return self[DootKey.build(key, strict=True)]
 
-    def __getitem__(self, val:str|DootKey|pl.Path|DootTaskArtifact) -> pl.Path:
+    def __getitem__(self, val:str|DootKey|pl.Path|TaskArtifact) -> pl.Path:
         """
           eg: doot.locs['{data}/somewhere']
           A public utility method to easily convert paths.
           delegates to DootKey's path expansion
 
           Get a location using item access for extending a stored path.
           eg: locs['{temp}/imgs/blah.jpg']
@@ -92,15 +92,15 @@
             case DootSimpleKey() as key:
                 return key.to_path(locs=self)
             case DootMultiKey() as key:
                 return key.to_path(locs=self)
             case _:
                 raise DootLocationExpansionError("Unrecognized location expansion argument", val)
 
-    def __contains__(self, key:str|DootKey|pl.Path|DootTaskArtifact):
+    def __contains__(self, key:str|DootKey|pl.Path|TaskArtifact):
         """ Test whether a key is a registered location """
         return key in self._data
 
     def __iter__(self) -> Generator[str]:
         """ Iterate over the registered location names """
         return iter(self._data.keys())
 
@@ -133,15 +133,15 @@
           More complex expansion is handled in DootKey and subclasses
         """
         assert(isinstance(key,(DootSimpleKey,str))), (str(key), type(key))
         match key:
             case DootNonKey():
                 return pl.Path(key.form)
             case str() | DootSimpleKey() if key in self._data:
-                return self._data[key].base
+                return self._data[key].path
             case _ if on_fail is None:
                 return None
             case _ if on_fail != Any:
                 return self.get(on_fail)
             case DootSimpleKey():
                 return pl.Path(key.form)
             case _:
@@ -192,28 +192,28 @@
             case _:
                 raise doot.errors.DootLocationError("Tried to update locations with unknown type: %s", extra)
 
         raw          = dict(self._data.items())
         base_keys    = set(raw.keys())
         new_keys     = set()
         for k,v in extra.items():
-            match TomlLocation.build(k, v):
+            match Location.build(v, key=k):
                 case _ if k in new_keys and v != raw[k]:
                     raise DootLocationError("Duplicated, non-matching Key", k)
                 case _ if k in base_keys:
                     logging.debug("Skipping Location update of: %s", k)
                     pass
-                case TomlLocation() as l if l.check(LocationMeta.normOnLoad):
-                    raw[l.key] = TomlLocation.build(k, v, base=self.normalize(l.base))
+                case Location() as l if l.check(LocationMeta.normOnLoad):
+                    raw[l.key] = Location.build(v, key=k, target=self.normalize(l.path))
                     new_keys.add(l.key)
-                case TomlLocation() as l:
+                case Location() as l:
                     raw[l.key] = l
                     new_keys.add(l.key)
                 case _:
-                    raise DootLocationError("Couldn't build a TomlLocation for: (%s : %s)", k, v)
+                    raise DootLocationError("Couldn't build a Location for: (%s : %s)", k, v)
 
         logging.debug("Registered New Locations: %s", ", ".join(new_keys))
         self._data = raw
         return self
 
     def ensure(self, *values, task="doot"):
         """ Ensure the values passed in are registered locations,
```

### Comparing `doot-0.7.2/doot/control/overlord.py` & `doot-0.8.0/doot/control/overlord.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
-# import datetime
-# import enum
+# ##-- stdlib imports
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import sys
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+import os
+from importlib.metadata import EntryPoint
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-# from uuid import UUID, uuid1
-# from weakref import ref
+# ##-- end stdlib imports
 
-##-- end imports
+# ##-- 3rd party imports
+import sh
+import tomlguard
 
-##-- logging
-logging = logmod.getLogger(__name__)
-printer = logmod.getLogger("doot._printer")
-##-- end logging
+# ##-- end 3rd party imports
 
-from importlib.metadata import EntryPoint
-
-import sh
-import sys
+# ##-- 1st party imports
 import doot
 import doot.errors
-import tomlguard
-from doot._abstract import (ArgParser_i, Command_i, CommandLoader_p,
-                            Overlord_p, Task_i, Job_i, TaskLoader_p)
-
-from doot.utils.plugin_selector import plugin_selector
+from doot._abstract import (ArgParser_i, Command_i, CommandLoader_p, Job_i,
+                            Overlord_p, Task_i, TaskLoader_p)
 from doot.errors import DootInvalidConfig, DootParseError
 from doot.loaders.cmd_loader import DootCommandLoader
 from doot.loaders.plugin_loader import DootPluginLoader
 from doot.loaders.task_loader import DootTaskLoader
-from doot.parsers.flexible import DootFlexibleParser
 from doot.mixins.param_spec import ParamSpecMaker_m
+from doot.parsers.flexible import DootFlexibleParser
+from doot.utils.plugin_selector import plugin_selector
+
+# ##-- end 1st party imports
 
-plugin_loader_key  : Final = doot.constants.entrypoints.DEFAULT_PLUGIN_LOADER_KEY
-command_loader_key : Final = doot.constants.entrypoints.DEFAULT_COMMAND_LOADER_KEY
-task_loader_key    : Final = doot.constants.entrypoints.DEFAULT_TASK_LOADER_KEY
-announce_exit      : bool  = doot.constants.misc.ANNOUNCE_EXIT
-announce_voice     : str   = doot.constants.misc.ANNOUNCE_VOICE
-
-DEFAULT_CLI_CMD    : Final = doot.constants.misc.DEFAULT_CLI_CMD
-
-preferred_cmd_loader       = doot.config.on_fail("default").settings.general.loaders.command()
-preferred_task_loader      = doot.config.on_fail("default").settings.general.loaders.task()
-preferred_parser           = doot.config.on_fail("default").settings.general.loaders.parser()
+##-- logging
+logging    = logmod.getLogger(__name__)
+printer    = logmod.getLogger("doot._printer")
+header_l   = printer.getChild("header")
+setup_l    = printer.getChild("setup")
+help_l     = printer.getChild("help")
+shutdown_l = printer.getChild("shutdown")
+##-- end logging
+
+env = os.environ
+plugin_loader_key  : Final[str]   = doot.constants.entrypoints.DEFAULT_PLUGIN_LOADER_KEY
+command_loader_key : Final[str]   = doot.constants.entrypoints.DEFAULT_COMMAND_LOADER_KEY
+task_loader_key    : Final[str]   = doot.constants.entrypoints.DEFAULT_TASK_LOADER_KEY
+announce_exit      : Final[bool]  = doot.constants.misc.ANNOUNCE_EXIT
+announce_voice     : Final[str]   = doot.constants.misc.ANNOUNCE_VOICE
+
+DEFAULT_CLI_CMD    : Final[str]   = doot.constants.misc.DEFAULT_CLI_CMD
+HEADER_MSG         : Final[str]   = doot.constants.printer.doot_header
+
+preferred_cmd_loader              = doot.config.on_fail("default").settings.general.loaders.command()
+preferred_task_loader             = doot.config.on_fail("default").settings.general.loaders.task()
+preferred_parser                  = doot.config.on_fail("default").settings.general.loaders.parser()
 
-defaulted_file             = doot.config.on_fail(pl.Path(".doot_defaults.toml"), pl.Path).report.defaulted_file(pl.Path)
+defaulted_file                    = doot.config.on_fail(pl.Path("{logs}.doot_defaults.toml"), pl.Path).report.defaulted_file(pl.Path)
 
 @doot.check_protocol
 class DootOverlord(ParamSpecMaker_m, Overlord_p):
     """
     Main control point for doot.
     prefers passed in loaders, then plugins it finds.
 
@@ -95,18 +103,42 @@
         self._errored     : None|DootError       = None
         self._current_cmd : None|str             = None
 
         self._load_plugins(extra_config)
         self._load_commands(extra_config)
         self._load_tasks(extra_config)
         self._parse_args()
-        logging.debug("Core Overlord Initialisation complete")
+        setup_l.debug("Core Overlord Initialisation complete")
+
+    def __call__(self, cmd=None) -> int:
+
+        if not doot.args.on_fail((None,)).cmd.args.suppress_header():
+            header_l.info(HEADER_MSG, extra={"colour": "green"})
+
+        if doot.args.on_fail(False).head.args.debug():
+            breakpoint()
+            pass
+
+        # perform head args
+        if self._cli_arg_response():
+            return
+
+        # Do the cmd
+        setup_l.debug("Overlord Calling: %s", cmd or doot.args.on_fail("Unknown").cmd.name())
+        try:
+            cmd = self._get_cmd(cmd)
+            cmd(self.tasks, self.plugins)
+        except doot.errors.DootError as err:
+            self._errored = err
+            raise err
+        else:
+            return 0
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
+    def param_specs(self) -> list[ParamSpec]:
         return [
            self.build_param(name="version" , prefix="--"),
            self.build_param(name="help"    , prefix="--"),
            self.build_param(name="verbose" , prefix="--"),
            self.build_param(name="debug",    prefix="--")
         ]
 
@@ -128,16 +160,17 @@
 
     def _load_plugins(self, extra_config:dict|TomlGuard=None):
         """ Use a plugin loader to find all applicable `importlib.EntryPoint`s  """
         try:
             self.plugin_loader    = self.loaders.get(plugin_loader_key, DootPluginLoader())
             self.plugin_loader.setup(extra_config)
             self.plugins : TomlGuard = self.plugin_loader.load()
+            doot._update_aliases(self.plugins)
         except doot.errors.DootPluginError as err:
-            printer.warning("Plugins Not Loaded Due to Error: %s", err)
+            setup_l.warning("Plugins Not Loaded Due to Error: %s", err)
             self.plugins = tomlguard.TomlGuard()
 
     def _load_commands(self, extra_config):
         """ Select Commands from the discovered plugins """
         self.cmd_loader = plugin_selector(self.loaders.get(command_loader_key, None) or self.plugins.on_fail([], list).command_loader(),
                                         target=preferred_cmd_loader,
                                         fallback=DootCommandLoader)()
@@ -147,15 +180,15 @@
         if not isinstance(self.cmd_loader, CommandLoader_p):
             raise TypeError("Attempted to use a non-CommandLoader_p as a CommandLoader: ", self.cmd_loader)
 
         try:
             self.cmd_loader.setup(self.plugins, extra_config)
             self.cmds = self.cmd_loader.load()
         except doot.errors.DootPluginError as err:
-            printer.warning("Commands Not Loaded due to Error: %s", err)
+            setup_l.warning("Commands Not Loaded due to Error: %s", err)
             self.cmds = tomlguard.TomlGuard()
 
     def _load_tasks(self, extra_config):
         """ Load task entry points """
 
         self.task_loader = plugin_selector(self.loaders.get(task_loader_key, None) or self.plugins.on_fail([], list).task_loader(),
                                             target=preferred_task_loader,
@@ -181,28 +214,28 @@
         doot.args = self.parser.parse(args or self.args, doot_specs=self.param_specs, cmds=self.cmds, tasks=self.tasks)
 
     def _cli_arg_response(self) -> bool:
         """ Overlord specific cli arg responses. modify verbosity,
           print version, and help.
         """
         if doot.args.on_fail(False).head.args.verbose() and self.log_config:
-            printer.info("Switching to Verbose Output")
+            setup_l.info("Switching to Verbose Output")
             self.log_config.set_level("NOTSET")
             pass
 
         logging.info("CLI Args: %s", doot.args._table())
         logging.info("Plugins: %s", dict(self.plugins))
         logging.info("Tasks: %s", self.tasks.keys())
 
         if doot.args.on_fail(False).head.args.version():
-            printer.info("\n\n----- Doot Version: %s\n\n", doot.__version__)
+            help_l.info("\n\n----- Doot Version: %s\n\n", doot.__version__)
             return True
 
         if doot.args.on_fail(False).head.args.help():
-            printer.info(self.help)
+            help_l.info(self.help)
 
             return True
 
         return False
 
     def _get_cmd(self, cmd=None):
         if self.current_cmd is not None:
@@ -213,76 +246,41 @@
         self.current_cmd = self.cmds.get(target, None)
         if self.current_cmd is None:
             self._errored = DootParseError("Specified Command Couldn't be Found: %s", target)
             raise self._errored
 
         return self.current_cmd
 
-    def __call__(self, cmd=None) -> int:
-
-        if not doot.args.on_fail((None,)).cmd.args.suppress_header():
-            printer.info("----------------------------------------------", extra={"colour" : "green"})
-            printer.info("-------------------- Doot --------------------", extra={"colour" : "yellow"})
-            printer.info("----------------------------------------------", extra={"colour": "green"})
-
-        if doot.args.on_fail(False).head.args.debug():
-            breakpoint()
-            pass
-
-        # perform head args
-        if self._cli_arg_response():
-            return
+    def _announce_exit(self, message:str):
+        match sys.platform:
+            case _ if "PRE_COMMIT" in env:
+                return
+            case "linux":
+                sh.espeak(message)
+            case "darwin":
+                sh.say("-v", "Moira", "-r", "50", message)
 
-        # Do the cmd
-        logging.info("Overlord Calling: %s", cmd or doot.args.on_fail("Unknown").cmd.name())
-        try:
-            cmd = self._get_cmd(cmd)
-            cmd(self.tasks, self.plugins)
-        except doot.errors.DootError as err:
-            self._errored = err
-            raise err
-        else:
-            return 0
+    def _record_defaulted_config_values(self):
+        defaulted_toml = tomlguard.TomlGuard.report_defaulted()
+        expanded_path = doot.locs[defaulted_file]
+        with open(expanded_path, 'w') as f:
+            f.write("# default values used:\n")
+            f.write("\n".join(defaulted_toml) + "\n\n")
 
     def shutdown(self):
         """ Doot has finished normally, so report on what was done """
         if self.current_cmd is not None and hasattr(self.current_cmd, "shutdown"):
             self.current_cmd.shutdown(self._errored, self.tasks, self.plugins)
 
+        say_on_exit = doot.config.on_fail(False).settings.general.notify.say_on_exit()
+
         match self._errored:
-            case doot.errors.DootError():
-                pass
+            case doot.errors.DootError() if say_on_exit:
+                self._record_defaulted_config_values()
+                self._announce_exit("Doot encountered an error")
+            case None if say_on_exit:
+                shutdown_l.info("Doot Shutting Down Normally")
+                self._record_defaulted_config_values()
+                self._announce_exit("Doot Finished")
             case None:
-                logging.info("Shutting Doot Down Normally")
+                shutdown_l.info("Doot Shutting Down Normally")
                 self._record_defaulted_config_values()
-
-        self._announce_exit()
-
-    def _announce_exit(self):
-        match sys.platform:
-            case "linux":
-                pass
-            case "darwin":
-                if doot.config is not None:
-                    announce_exit        = doot.config.on_fail(announce_exit, bool|str).settings.general.notify.say_on_exit()
-                    announce_voice       = doot.config.on_fail(announce_voice, str).setttings.general.notify.announce_voice()
-
-                match result, announce_exit:
-                    case 0, str() as say_text:
-                        cmd = sh.say("-v", announce_voice, "-r", "50", say_text)
-                    case 0, True:
-                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Has Finished")
-                    case _, True|str():
-                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Encountered a problem")
-                    case _, _:
-                        cmd = None
-                if cmd is not None:
-                    cmd.execute()
-
-    def _record_defaulted_config_values(self):
-
-        defaulted_toml = tomlguard.TomlGuard.report_defaulted()
-        with open(defaulted_file, 'w') as f:
-            f.write("# default values used:\n")
-            f.write("\n".join(defaulted_toml) + "\n\n")
-            # f.write("[.directories]\n")
-            # f.write("\n".join(defaulted_locs))
```

### Comparing `doot-0.7.2/doot/control/step_runner.py` & `doot-0.8.0/doot/control/step_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,22 @@
 ##-- end logging
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 import doot
 import doot.structs as structs
 import doot.errors
-from doot.enums import TaskStateEnum, ReportEnum, TaskFlags
+from doot.enums import TaskStatus_e, ReportEnum, TaskFlags
 import doot._abstract as abstract
 from doot.control.runner import DootRunner
 from doot.utils.signal_handler import SignalHandler
 
-dry_run      = doot.args.on_fail(False).cmd.args.dry_run()
-SLEEP_LENGTH = doot.config.on_fail(0.2, int|float).settings.tasks.sleep.task()
+dry_run                     = doot.args.on_fail(False).cmd.args.dry_run()
+SLEEP_LENGTH                = doot.config.on_fail(0.2, int|float).settings.tasks.sleep.task()
+MAX_LOG_ACTIVE : Final[int] = 100
 
 @doot.check_protocol
 class DootStepRunner(DootRunner):
     """ extends the default runner with step control """
     _conf_prompt  = "::- Command? (? for help): "
     _cmd_prefix   = "_do_"
     _aliases      = { ""  : "continue",
@@ -65,16 +66,16 @@
                      "?"  : "help",
                      "I"  : "print_info",
                      "W"  : "print_warn",
                      "D"  : "print_debug",
                      "s"  : "print_state"
                      }
 
-    def __init__(self:Self, *, tracker:abstract.TaskTracker_i, reporter:abstract.Reporter_i, policy=None):
-        super().__init__(tracker=tracker, reporter=reporter, policy=policy)
+    def __init__(self:Self, *, tracker:abstract.TaskTracker_i, reporter:abstract.Reporter_p):
+        super().__init__(tracker=tracker, reporter=reporter)
         self._conf_types = []
         self._override_level = "INFO"
         self._has_quit = False
 
     def _expand_job(self, job:abstract.Job_i) -> None:
         if self._pause(job):
             super()._expand_job(job)
@@ -104,15 +105,15 @@
         match target:
             case _ if True in self._conf_types:
                 pass
             case abstract.Job_i() if abstract.Job_i not in self._conf_types:
                 return True
             case abstract.Task_i() if abstract.Task_i not in self._conf_types:
                 return True
-            case structs.DootActionSpec() if structs.DootActionSpec not in self._conf_types:
+            case structs.ActionSpec() if structs.ActionSpec not in self._conf_types:
                 return True
 
         printer.info("")
         printer.info( "::- Step %s: %s", (step or self.step), str(target))
         result = None
         while not isinstance(result, bool):
             response = input(self._conf_prompt)
@@ -152,15 +153,18 @@
         printer.info("::-- Pausing on: %s", self._conf_types)
 
         return None
 
     def _do_quit(self, *args):
         printer.info("::- Quitting Doot")
         self.tracker.clear_queue()
-        printer.info("Tracker Queue: %s", self.tracker.active_set)
+        if len(self.tracker.active_set) < MAX_LOG_ACTIVE:
+            printer.info("Tracker Queue: %s", self.tracker.active_set)
+        else:
+            printer.info("Tracker Queue: %s", len(self.tracker_set))
         self._has_quit = True
         return False
 
     def _do_list(self, *args):
         printer.info("::- Listing Trace:")
         for x in self.tracker.execution_path[:-1]:
             printer.info("::-- %s", x)
@@ -180,24 +184,24 @@
         match self._conf_types:
             case [True]:
                 self.set_confirm_type("job")
             case [abstract.Job_i]:
                 self.set_confirm_type("task")
             case [abstract.Task_i]:
                 self.set_confirm_type("action")
-            case [structs.DootActionSpec]:
+            case [structs.ActionSpec]:
                 self.set_confirm_type("all")
                 pass
 
         printer.info("::- Stepping at: %s", self._conf_types)
 
     def _do_up(self, *args):
         printer.info("Up")
         match self._conf_types:
-            case [structs.DootActionSpec]:
+            case [structs.ActionSpec]:
                 self.set_confirm_type("task")
             case [abstract.Task_i]:
                 self.set_confirm_type("job")
             case [abstract.Job_i]:
                 self.set_confirm_type("all")
             case [True]:
                 pass
@@ -206,29 +210,29 @@
 
     def _do_print_info(self, *args):
         self._override_level = "INFO"
         printer.warning("Overring Printer to: %s", self._override_level)
         self._set_print_level(self._override_level)
 
     def _do_print_warn(self, *args):
-        self._override_level = "WARN"
+        self._override_level = "WARNING"
         printer.warning("Overring Printer to: %s", self._override_level)
         self._set_print_level(self._override_level)
 
     def _do_print_debug(self, *args):
         self._override_level = "DEBUG"
         printer.warning("Overring Printer to: %s", self._override_level)
         self._set_print_level(self._override_level)
 
     def _do_print_state(self, *args):
         printer.info("Current State:")
         printer.info("%20s : %s", "CLI Args", dict(doot.args))
         for arg in args:
             match arg:
-                case structs.DootActionSpec():
+                case structs.ActionSpec():
                     printer.info("%20s : %s", "Action", str(arg.do))
                     printer.info("%20s : %s", "Action Spec kwargs", dict(arg.kwargs))
                 case abstract.Task_i():
                     printer.info("%20s : %s", "Task Name", str(arg.name))
                     printer.info("%20s : %s", "Task State", arg.state)
                 case abstract.Job_i():
                     printer.info("%20s : %s", "Job Args", arg.args)
@@ -243,13 +247,13 @@
         """ Sets the runners `breakpoints` """
         match val:
             case "job":
                 self._conf_types = [abstract.Job_i]
             case "task":
                 self._conf_types = [abstract.Task_i]
             case "action":
-                self._conf_types = [structs.DootActionSpec]
+                self._conf_types = [structs.ActionSpec]
             case "all":
                 self._conf_types = [True]
 """
 
 """
```

### Comparing `doot-0.7.2/doot/errors.py` & `doot-0.8.0/doot/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 #!/usr/bin/env python3
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
 import pathlib as pl
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-##-- end imports
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
+
+# ##-- end stdlib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-__all__ = ["DootError", "DootTaskError", "DootTaskLoadError", "DootTaskFailed", "DootTaskTrackingError", "DootTaskInterrupt"
-           "DootParseError", "DootInvalidConfig", "DootLocationError", "DootLocationExpansionError", "DootDirAbsent",
-           "DootPluginError", "DootCommandError", "DootConfigError"]
+__all__ = []
 
 class DootError(Exception):
     """
       The base class for all Doot Errors
       will try to % format the first argument with remaining args in str()
     """
     general_msg = "Non-Specific Doot Error:"
@@ -33,23 +39,23 @@
             return self.args[0] % self.args[1:]
         except TypeError:
             return str(self.args)
 
 class DootTaskError(DootError):
     general_msg = "Doot Task Error:"
 
-    def __init__(self, msg, *args, task=None):
+    def __init__(self, msg, *args, task:None|"Task_i"=None):
         super().__init__(msg, *args)
         self.task = task
 
     @property
     def task_name(self):
         if not self.task:
             return ""
-        return str(self.task.name)
+        return self.task.shortname
 
     @property
     def task_source(self):
         if not self.task:
             return ""
         return self.task.source
```

### Comparing `doot-0.7.2/doot/loaders/__tests/test_cmd_loader.py` & `doot-0.8.0/doot/loaders/__tests/test_cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/loaders/__tests/test_plugin_loader.py` & `doot-0.8.0/doot/loaders/__tests/test_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/loaders/__tests/test_task_loader.py` & `doot-0.8.0/doot/loaders/__tests/test_task_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,18 @@
                     TypeVar, cast)
 ##-- end imports
 
 import pytest
 import importlib.metadata
 import tomlguard
 import doot
+from doot.enums import TaskFlags
 doot._test_setup()
 
-from doot.structs import DootTaskSpec
+from doot.structs import TaskSpec
 from doot._abstract.task import Task_i
 from doot.utils.mock_gen import mock_entry_point, mock_task_ctor
 
 doot.config = tomlguard.TomlGuard({})
 from doot.loaders import task_loader
 logging = logmod.root
 
@@ -54,15 +55,15 @@
         basic = task_loader.DootTaskLoader()
         basic.setup({}, specs)
         result = basic.load()
 
         assert(isinstance(result, tomlguard.TomlGuard))
         assert(len(result) == 1)
         assert("basic::test" in result)
-        assert(isinstance(result['basic::test'], DootTaskSpec))
+        assert(isinstance(result['basic::test'], TaskSpec))
 
     def test_multi_load(self, mocker):
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
 
         specs = {"tasks": { "basic" : []}}
         specs['tasks']['basic'].append({"name"  : "test", "ctor" : "doot.task.base_job:DootJob"})
@@ -110,83 +111,81 @@
 
         specs = {"tasks": { "basic": []}}
         specs['tasks']['basic'].append({"name"  : "test", "ctor" : "doot.task.base_job:DoesntExistJob"})
 
         basic = task_loader.DootTaskLoader()
         basic.setup({}, specs)
 
-        with pytest.raises(doot.errors.DootTaskLoadError):
-            basic.load()
+        result = basic.load()
+        assert(TaskFlags.DISABLED in  result["basic::test"].flags)
 
     def test_bad_task_module(self, mocker):
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
 
         specs = {"tasks": { "basic" : []}}
         specs['tasks']['basic'].append({"name"  : "test", "ctor" : "doot.task.doesnt_exist_module:DoesntExistJob"})
         basic = task_loader.DootTaskLoader()
         basic.setup({}, specs)
 
-        with pytest.raises(doot.errors.DootTaskLoadError):
-            basic.load()
+        result = basic.load()
+        assert(TaskFlags.DISABLED in  result["basic::test"].flags)
 
     @pytest.mark.xfail
     def test_bad_spec(self, mocker):
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
 
         specs = {"tasks": { "basic" : []}}
         specs['tasks']['basic'].append({"name"  : "test"})
         basic = task_loader.DootTaskLoader()
         basic.setup({}, specs)
 
         with pytest.raises(doot.errors.DootTaskLoadError):
             result = basic.load()
 
+    @pytest.mark.xfail
     def test_task_type(self, mocker):
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
         specs = {"tasks": {"basic": []}}
         specs['tasks']['basic'].append({"name": "simple", "ctor": "basic"})
 
         mock_ctor                   = mock_task_ctor()
         mock_ep                     = mock_entry_point(name="basic", value=mock_ctor)
 
-        plugins                     = tomlguard.TomlGuard({"job": [mock_ep]})
+        plugins                     = tomlguard.TomlGuard({"task": [mock_ep]})
         basic                       = task_loader.DootTaskLoader()
         basic.setup(plugins, tomlguard.TomlGuard(specs))
 
         result    = basic.load()
 
         assert(len(result) == 1)
         task_spec = result['basic::simple']
-        assert(str(task_spec.ctor) == "default:basic")
-        assert(task_spec.ctor.value == "basic")
+        assert(task_spec.ctor is not None)
 
-
-
-    def test_task_missing_plugin_in(self, mocker):
+    def test_task_missing_plugin_results_in_disabled(self, mocker):
+        """ a bad ctor alias disables the task """
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
         mocker.patch("importlib.metadata.EntryPoint")
         specs = {"tasks": {"basic": []}}
         specs['tasks']['basic'].append({"name": "simple", "ctor": "bad:not_basic"})
 
         mock_ep      = importlib.metadata.EntryPoint()
         mock_ep.name = "basic"
 
         plugins      = tomlguard.TomlGuard({"job": [mock_ep]})
         basic        = task_loader.DootTaskLoader()
         basic.setup(plugins, tomlguard.TomlGuard(specs))
 
-        with pytest.raises(doot.errors.DootTaskLoadError):
-            basic.load()
+        result = basic.load()
+        assert(TaskFlags.DISABLED in  result["basic::simple"].flags)
 
 
-    @pytest.mark.xfail
     def test_task_bad_type_loaded(self, mocker):
         mocker.patch("doot.loaders.task_loader.task_sources")
         mocker.patch("doot._configs_loaded_from")
         mocker.patch("importlib.metadata.EntryPoint")
         specs = {"tasks": {"basic": []}}
         specs['tasks']['basic'].append({"name": "simple", "ctor": "basic"})
```

### Comparing `doot-0.7.2/doot/loaders/cmd_loader.py` & `doot-0.8.0/doot/loaders/cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/loaders/plugin_loader.py` & `doot-0.8.0/doot/loaders/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/loaders/task_loader.py` & `doot-0.8.0/doot/loaders/task_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ##-- end logging
 
 from collections import ChainMap
 import importlib
 import tomlguard
 import doot
 import doot.errors
-from doot.structs import DootTaskSpec, DootTaskName, DootCodeReference
+from doot.structs import TaskSpec, TaskName, CodeReference
 from doot._abstract import TaskLoader_p, Job_i, Task_i
 
 DEFAULT_TASK_GROUP        = doot.constants.names.DEFAULT_TASK_GROUP
 IMPORT_SEP                = doot.constants.patterns.IMPORT_SEP
 TASK_STRING : Final[str]  = "task_"
 prefix_len  : Final[int]  = len(TASK_STRING)
 
@@ -51,25 +51,29 @@
 allow_overloads           = doot.config.on_fail(False, bool).allow_overloads()
 
 def apply_group_and_source(group, source, x):
     match x:
         case tomlguard.TomlGuard():
             x = dict(x.items())
             x['group']  = x.get('group', group)
-            x['source'] = str(source)
+            if 'sources' not in x:
+                x['sources'] = []
+            x['sources'].append(str(source))
         case dict():
             x['group']  = x.get('group', group)
-            x['source'] = str(source)
+            if 'sources' not in x:
+                x['sources'] = []
+            x['sources'].append(str(source))
     return x
 
 
 @doot.check_protocol
 class DootTaskLoader(TaskLoader_p):
     """
-    load toml defined tasks, and create doot.structs.DootTaskSpecs of them
+    load toml defined tasks, and create doot.structs.TaskSpecs of them
     """
     tasks         : dict[str, tuple(dict, Job_i)] = {}
     cmd_names     : set[str]                         = set()
     task_builders : dict[str,Any]                    = dict()
     extra : TomlGuard
 
     def setup(self, plugins, extra=None) -> Self:
@@ -184,69 +188,65 @@
                 raw_specs += map(ftz.partial(apply_group_and_source, group, path), val)
             logging.info("Loaded Tasks from: %s", path)
             self._load_location_updates(data.on_fail([]).locations(), path)
 
         return raw_specs
 
 
-    def _build_task_specs(self, group_specs:list[dict], command_names) -> list[DootTaskSpec]:
+    def _build_task_specs(self, group_specs:list[dict], command_names) -> list[TaskSpec]:
         """
-        convert raw dicts into DootTaskSpec objects,
+        convert raw dicts into TaskSpec objects,
           checking nothing tries to shadow a command name or other task name
         """
-        task_descriptions : dict[str, DootTaskSpec] = {}
+        task_descriptions : dict[str, TaskSpec] = {}
         dont_allow_overloads = lambda task_name, group_name: not allow_overloads and task_name in task_descriptions and group_name == task_descriptions[task_name][0]['group']
         for spec in group_specs:
             task_alias = "task"
             try:
                 match spec:
-                    case {"name": task_name, "disable" : True}: # Disabled specs
-                        logging.info("Spec is disabled: %s", task_name)
                     # case {"name": task_name} if task_name in command_names:
                     #     raise doot.errors.DootTaskLoadError("Name conflict: %s is already a Command", task_name)
                     case {"name": task_name, "group": group} if dont_allow_overloads(task_name, group): # complain on overload
                         raise doot.errors.DootTaskLoadError("Task Name Overloaded: %s : %s", task_name, group)
                     case {"name": task_name, "ctor": str() as task_alias} if task_alias in self.task_builders: # build named plugin type
                         logging.info("Building Task from short name: %s : %s", task_name, task_alias)
-                        task_iden                   : DootCodeReference       = DootCodeReference.from_alias(task_alias, "task", self.plugins)
+                        task_iden                   : CodeReference       = CodeReference.from_alias(task_alias, "task", self.plugins)
                         spec['ctor'] = task_iden
-                        task_spec = DootTaskSpec.build(spec)
+                        task_spec = TaskSpec.build(spec)
                         if str(task_spec.name) in task_descriptions:
                             logging.warning("Overloading Task: %s : %s", str(task_spec.name), task_alias)
 
-                        task_spec.check(ensure=Task_i)
                         task_descriptions[str(task_spec.name)] = task_spec
                     case {"name": task_name}:
                         logging.info("Building Task: %s", task_name)
-                        task_spec = DootTaskSpec.build(spec)
+                        task_spec = TaskSpec.build(spec)
                         if str(task_spec.name) in task_descriptions:
                             logging.warning("Overloading Task: %s : %s", str(task_spec.name), str(task_spec.ctor))
 
-                        task_spec.check(ensure=Task_i)
                         task_descriptions[str(task_spec.name)] = task_spec
 
                     case _: # Else complain
-                        raise doot.errors.DootTaskLoadError("Task Spec missing, at least, a name and ctor: %s: %s", spec['source'], spec)
+                        raise doot.errors.DootTaskLoadError("Task Spec missing, at least, needs at least a name and ctor: %s: %s", spec, spec['sources'][0] )
             except doot.errors.DootLocationError as err:
-                logging.warning("Task Spec '%s' Load Failure: Missing Location: '%s'. Source File: %s", task_name, str(err), spec['source'])
+                logging.warning("Task Spec '%s' Load Failure: Missing Location: '%s'. Source File: %s", task_name, str(err), spec['sources'][0])
             except ModuleNotFoundError as err:
                 logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Module Name: '%s'. Source File: %s", task_name, task_alias, spec['source']) from err
+                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Module Name: '%s'. Source File: %s", task_name, task_alias, spec['sources'][0]) from err
             except AttributeError as err:
                 logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Class Name: '%s'. Source File: %s", task_name, task_alias, spec['source'], err.args) from err
+                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Class Name: '%s'. Source File: %s", task_name, task_alias, spec['sources'][0], err.args) from err
             except ValueError as err:
                 logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Module/Class Split failed on: '%s'. Source File: %s", task_name, task_alias, spec['source']) from err
+                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: '%s'. Source File: %s. Message:\n %s", task_name, task_alias, spec['sources'][0], str(err)) from err
             except TypeError as err:
                 logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Type constructor: '%s'. Source File: %s", task_name, spec['ctor'], spec['source']) from err
+                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Type constructor: '%s'. Source File: %s", task_name, spec['ctor'], spec['sources'][0]) from err
             except ImportError as err:
                 logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: ctor import check failed. Source File: %s", task_name, spec['source']) from err
+                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: ctor import check failed. Source File: %s", task_name, spec['sources'][0]) from err
 
         return task_descriptions
 
     def _load_location_updates(self, data:list[TomlGuard], source):
         logging.debug("Loading Location Updates: %s", source)
         for group in data:
             try:
```

### Comparing `doot-0.7.2/doot/mixins/enums.py` & `doot-0.8.0/doot/mixins/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,27 @@
                 case str():
                     return cls[val]
                 case cls():
                     return val
         except KeyError:
             logging.warning("Can't Create a flag of (%s):%s. Available: %s", cls, val, list(cls.__members__.keys()))
 
+    @classmethod
+    def get_default(cls) -> Self:
+        return cls.default
+
 class FlagsBuilder_m:
 
     @classmethod
     def build(cls, vals:str|list|dict) -> Self:
+        """ Assemble a flag from names.
+          a str is just the flag,
+          a list treats each name as a true falg
+          a dict is {name=bool}
+          """
         match vals:
             case str():
                 vals = [vals]
             case list():
                 pass
             case dict():
                 vals = [x for x,y in vals.items() if bool(y)]
```

### Comparing `doot-0.7.2/doot/mixins/fail_handler.py` & `doot-0.8.0/doot/mixins/fail_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/mixins/human_numbers.py` & `doot-0.8.0/doot/mixins/human_numbers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/mixins/importer.py` & `doot-0.8.0/doot/mixins/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 #!/usr/bin/env python3
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-import types
+# ##-- stdlib imports
 import abc
 import datetime
 import enum
 import functools as ftz
+import importlib
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
+import types
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
 
-##-- end imports
-
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end stdlib imports
 
-import importlib
+# ##-- 1st party imports
 import doot
 import doot.errors
 from doot._abstract.loader import PluginLoader_p
 
+# ##-- end 1st party imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+##-- end logging
+
 IMPORT_SEP   = doot.constants.patterns.IMPORT_SEP
 ACTION_CTORS = {}
 
 if PluginLoader_p.loaded:
     ACTION_CTORS = {x.name : x for x in PluginLoader_p.loaded.action}
 
 class Importer_m:
@@ -61,15 +66,14 @@
         except ImportError as err:
             raise doot.errors.DootTaskLoadError("Task Import Failed: %s : %s", pathname, err.msg, task=self.spec) from err
         except (AttributeError, KeyError) as err:
             raise doot.errors.DootTaskLoadError("Task Import Failed: Module has missing attribute/key: %s", pathname, task=self.spec) from err
         except ValueError as err:
             raise doot.errors.DootTaskLoadError("Task Import Failed: Can't split %s : %s", pathname, task=self.spec) from err
 
-
     def import_callable(self, pathname:None|str) -> None|callable[Any]:
         """
           given a path in the form `package.sub.sub:function`, import the package, and return the named function.
         """
         if pathname is None:
             return None
```

### Comparing `doot-0.7.2/doot/mixins/param_spec.py` & `doot-0.8.0/doot/mixins/param_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from doot._structs.param_spec import DootParamSpec
+from doot._structs.param_spec import ParamSpec
 
 class ParamSpecMaker_m:
 
     @staticmethod
-    def build_param(*args:Any, **kwargs:Any) -> DootParamSpec:
+    def build_param(**kwargs:Any) -> ParamSpec:
         """ Utility method for easily making paramspecs """
-        return DootParamSpec(*args, **kwargs)
+        return ParamSpec(**kwargs)
```

### Comparing `doot-0.7.2/doot/mixins/path_manip.py` & `doot-0.8.0/doot/mixins/path_manip.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/mixins/zipper.py` & `doot-0.8.0/doot/mixins/zipper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/parsers/__tests/test_flexible.py` & `doot-0.8.0/doot/parsers/__tests/test_flexible.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,374 +1,379 @@
 #!/usr/bin/env python4
 """
 
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
+# ##-- stdlib imports
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
-import warnings
 import pathlib as pl
-from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
-                    Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
-                    TypeVar, cast)
-##-- end imports
-logging = logmod.root
+import warnings
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
+
+# ##-- end stdlib imports
 
+# ##-- 3rd party imports
 import pytest
+from tomlguard import TomlGuard
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
+
+# ##-- end 1st party imports
+
 doot._test_setup()
 
+# ##-- 1st party imports
 import doot.errors
-from doot._abstract import ArgParser_i, Task_i
+from doot._abstract import ArgParser_i, Task_i, Command_i
 from doot.parsers.flexible import DootFlexibleParser
-from doot.structs import DootParamSpec, DootTaskSpec, DootCodeReference
-from doot.utils.mock_gen import mock_parse_cmd, mock_parse_task
+from doot.structs import CodeReference, ParamSpec, TaskSpec
+
+# ##-- end 1st party imports
 
+logging = logmod.root
 
 @pytest.mark.parametrize("ctor", [DootFlexibleParser])
 class TestArgParser:
 
+    @pytest.fixture(scope="function")
+    def cmd_mock(self, mocker):
+        return mocker.MagicMock(spec=Command_i, param_specs=[ParamSpec(name="all")])
+
+    @pytest.fixture(scope="function")
+    def spec_mock(self, mocker):
+        return self.make_spec_mock(mocker)
+
+    def make_spec_mock(self, mocker):
+        task_mock                 = mocker.MagicMock(spec=TaskSpec, ctor=mocker.MagicMock(spec=CodeReference))
+        ctor_mock                 = mocker.Mock()
+        ctor_mock.param_specs     = []
+        task_mock.ctor.try_import = mocker.Mock(return_value=ctor_mock)
+        task_mock.extra           = TomlGuard({"cli": [ParamSpec(name="all")]})
+
+        return task_mock
+
     def test_initial(self, ctor):
         parser = ctor()
         assert(isinstance(parser, ArgParser_i))
 
-    def test_cmd(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd(name="list")
+    def test_cmd(self, ctor, mocker, cmd_mock):
         parser                     = ctor()
 
         result                     = parser.parse(["doot", "list"],
             doot_specs=[], cmds={"list": cmd_mock}, tasks={}
             )
 
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name()  == "list")
 
-    def test_cmd_args(self, ctor, mocker):
-        cmd_mock  = mock_parse_cmd(params=[DootParamSpec(name="all")])
+    def test_cmd_args(self, ctor, mocker, cmd_mock):
         parser    = ctor()
         result    = parser.parse([
             "doot", "list", "-all"
-                               ],
+                                 ],
             doot_specs=[], cmds={"list": cmd_mock}, tasks={}
             )
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name() == "list")
         assert(result.on_fail(False).cmd.args.all() == True)
 
-    def test_cmd_arg_fail(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd(params=[DootParamSpec(name="all")])
-
+    def test_cmd_arg_fail(self, ctor, mocker, cmd_mock):
         parser = ctor()
         with pytest.raises(Exception):
             parser.parse([
                 "doot", "list", "-all", "-bloo"
             ],
             doot_specs=[], cmds={"list": cmd_mock}, tasks={}
         )
 
-    def test_cmd_then_task(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd(params=[DootParamSpec(name="all")])
-        task_mock                  = mock_parse_task(params=[{"name":"all"}])
-
-        parser = ctor()
-        result = parser.parse([
-            "doot", "list", "blah"
+    def test_cmd_then_task(self, ctor, mocker, cmd_mock, spec_mock):
+        cmd_mock    = mocker.MagicMock(spec=Command_i, param_specs=[ParamSpec(name="all")])
+        parser      = ctor()
+        result      = parser.parse([
+            "doot", "list", "agroup::blah"
                                ],
-            doot_specs=[], cmds={"list": cmd_mock}, tasks={"blah": task_mock},
+            doot_specs=[], cmds={"list": cmd_mock}, tasks={"agroup::blah": spec_mock},
             )
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name() == "list")
-        assert("blah" in result.tasks)
-
-    def test_cmd_then_complex_task(self, ctor, mocker):
-        cmd_mock  = mock_parse_cmd(params=[DootParamSpec(name="all")])
-        task_mock = mock_parse_task(params=[{"name":"all"}])
+        assert("agroup::blah" in result.tasks)
 
+    def test_cmd_then_complex_task(self, ctor, mocker, cmd_mock, spec_mock):
         parser    = ctor()
         result    = parser.parse([
             "doot", "list", "blah::bloo.blee"
                                ],
-            doot_specs=[], cmds={"list": cmd_mock}, tasks={"blah::bloo.blee": task_mock},
+            doot_specs=[], cmds={"list": cmd_mock}, tasks={"blah::bloo.blee": spec_mock},
             )
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name() == "list")
         assert( "blah::bloo.blee" in result.tasks)
 
-    def test_task_args(self, ctor, mocker):
+    def test_task_args(self, ctor, mocker, cmd_mock, spec_mock):
         """ check tasks can recieve args """
-        cmd_mock                                    = mock_parse_cmd()
-        task_mock                                   = mock_parse_task(params=[{"name":"all"}])
-
         parser                                      = ctor()
         result                                      = parser.parse([
             "doot", "basic::list", "-all"
                                ],
-            doot_specs=[], cmds={"run": cmd_mock}, tasks={"basic::list": task_mock},
+            doot_specs=[], cmds={"run": cmd_mock}, tasks={"basic::list": spec_mock},
             )
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name() == "run")
         assert(bool(result.on_fail(False).tasks["basic::list"]()))
         assert(result.on_fail(False).tasks["basic::list"].all() == True)
 
-    def test_task_with_name_spaces(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[{"name":"all"}])
-
+    def test_task_with_name_spaces(self, ctor, mocker, cmd_mock, spec_mock):
         parser = ctor()
         result = parser.parse([
-            "doot", "simple task", "-all"
+            "doot", "agroup::simple task", "-all"
                                ],
-            doot_specs=[], cmds={"run": cmd_mock}, tasks={"simple task": task_mock},
+            doot_specs=[], cmds={"run": cmd_mock}, tasks={"agroup::simple task": spec_mock},
             )
         assert(result.on_fail(False).head.name() == "doot")
         assert(result.on_fail(False).cmd.name() == "run")
-        assert(bool(result.on_fail(False).tasks['simple task']()))
-        assert(result.on_fail(False).tasks['simple task'].all() == True)
-
-    def test_task_args_default(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[{"name":"all"}])
+        assert(bool(result.on_fail(False).tasks['agroup::simple task']()))
+        assert(result.on_fail(False).tasks['agroup::simple task'].all() == True)
 
+    def test_task_args_default(self, ctor, mocker, cmd_mock, spec_mock):
         parser = ctor()
         result = parser.parse([
-            "doot", "list", # no "-all"
+            "doot", "agroup::list", # no "-all"
                                ],
-            doot_specs=[], cmds={"run": cmd_mock}, tasks={"list": task_mock},
+            doot_specs=[], cmds={"run": cmd_mock}, tasks={"agroup::list": spec_mock},
             )
         assert(result.on_fail(False).head.name() == "doot")
-        assert(bool(result.on_fail(False).tasks.list()))
-        assert(result.on_fail(False).tasks.list.all() == False)
-
-    def test_tasks_dup_fail(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[{"name":"all"}])
+        assert(bool(result.on_fail(False).tasks['agroup::list']()))
+        assert(result.on_fail(False).tasks['agroup::list'].all() == False)
 
+    def test_tasks_dup_fail(self, ctor, mocker, cmd_mock, spec_mock):
+        cmd_mock, task_mock    = cmd_mock, spec_mock
         parser = ctor()
         with pytest.raises(doot.errors.DootParseError):
             parser.parse([
-                "doot", "list", "-all", "list"
+                "doot", "agroup::list", "-all", "agroup::list"
                          ],
-                doot_specs=[], cmds={"run": cmd_mock}, tasks={"list": task_mock}
+                doot_specs=[], cmds={"run": cmd_mock}, tasks={"agroup::list": task_mock}
             )
 
-    def test_positional_cmd_arg(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd(params=[DootParamSpec("test", type=str, positional=True)])
-        task_mock                  = mock_parse_task(params=[{"name":"key"}])
-
+    def test_positional_cmd_arg(self, ctor, mocker, cmd_mock, spec_mock):
+        cmd_mock.param_specs.append(ParamSpec(name="test", type=str, positional=True))
+        spec_mock.extra.cli.append(ParamSpec(name="key"))
         parser = ctor()
         result = parser.parse([
             "doot", "example", "blah"
                         ],
-            doot_specs=[], cmds={"example": cmd_mock}, tasks={"other": task_mock},
+            doot_specs=[], cmds={"example": cmd_mock}, tasks={"other": spec_mock},
             )
         assert(result.cmd.name == "example")
         assert(result.cmd.args.test == "blah")
 
-    def test_positional_cmd_arg_seq(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd(params=[
-            DootParamSpec(name="first", type=str, positional=True),
-            DootParamSpec(name="second", type=str, positional=True)
-            ])
-        task_mock                  = mock_parse_task(params=[{"name":"key"}])
+    def test_positional_cmd_arg_seq(self, ctor, mocker, cmd_mock, spec_mock):
+        cmd_mock.param_specs.append(ParamSpec(name="first", type=str, positional=True))
+        cmd_mock.param_specs.append(ParamSpec(name="second", type=str, positional=True))
 
         parser = ctor()
         result = parser.parse([
             "doot", "example", "blah", "bloo"
                         ],
             doot_specs=[], cmds={"example": cmd_mock}, tasks={}
             )
         assert(result.cmd.args.first == "blah")
         assert(result.cmd.args.second == "bloo")
 
-    def test_positional_task_arg(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[{"name":"test", "type":str, "positional":True, "default":""}])
+    def test_positional_task_arg(self, ctor, mocker, cmd_mock, spec_mock):
+        spec_mock.extra.cli.append(ParamSpec.build({"name":"test", "type":str, "positional":True, "default":""}))
 
         parser = ctor()
         result = parser.parse([
-            "doot", "example", "blah"
+            "doot", "agroup::example", "blah"
                         ],
-            doot_specs=[], cmds={"run": cmd_mock}, tasks={"example": task_mock},
+            doot_specs=[], cmds={"run": cmd_mock}, tasks={"agroup::example": spec_mock},
             )
-        assert("example" in result.tasks)
-        assert(result.tasks.example.test == "blah")
+        assert("agroup::example" in result.tasks)
+        assert(result.tasks['agroup::example'].test == "blah")
 
-    def test_positional_taskarg_seq(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[
-            {"name":"first", "type":str, "positional":True},
-            {"name":"second", "type":str, "positional":True}
-            ])
+    def test_positional_taskarg_seq(self, ctor, mocker, cmd_mock, spec_mock):
+        spec_mock.extra.cli.append(ParamSpec.build({"name":"first", "type":str, "positional":True}))
+        spec_mock.extra.cli.append(ParamSpec.build({"name":"second", "type":str, "positional":True}))
 
         parser = ctor()
         result = parser.parse([
-            "doot", "example", "blah", "bloo"
+            "doot", "agroup::example", "blah", "bloo"
                         ],
-            doot_specs=[], cmds={"run": cmd_mock}, tasks={"example": task_mock},
+            doot_specs=[], cmds={"run": cmd_mock}, tasks={"agroup::example": spec_mock},
             )
-        assert(result.tasks.example.first == "blah")
-        assert(result.tasks.example.second == "bloo")
+        assert(result.tasks['agroup::example'].first == "blah")
+        assert(result.tasks['agroup::example'].second == "bloo")
 
     def test_simple_head_arg(self, ctor, mocker):
-        param = DootParamSpec("key", bool)
+        param = ParamSpec(name="key", type=bool)
         parser   = ctor()
         result   = parser.parse(["doot", "-key"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is True)
 
 
     def test_simple_short_arg(self, ctor, mocker):
-        param = DootParamSpec("key", bool)
+        param = ParamSpec(name="key", type=bool)
         parser   = ctor()
         result   = parser.parse(["doot", "-k"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is True)
 
     def test_simple_invert(self, ctor, mocker):
-        param = DootParamSpec("key", bool)
+        param = ParamSpec(name="key", type=bool)
         parser   = ctor()
         result   = parser.parse(["doot", "-no-key"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is False)
 
     def test_simple_multi(self, ctor, mocker):
-        param    = DootParamSpec("key", bool)
-        param2   = DootParamSpec("other", bool)
+        param    = ParamSpec(name="key", type=bool)
+        param2   = ParamSpec(name="other", type=bool)
         parser   = ctor()
         result   = parser.parse(["doot", "-no-key", "-other"],
             doot_specs=[param, param2], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is False)
         assert(result.head.args.other is True)
 
     def test_simple_default(self, ctor, mocker):
-        param    = DootParamSpec("key", bool)
+        param    = ParamSpec(name="key", type=bool)
         parser   = ctor()
         result   = parser.parse(["doot"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is False)
 
     def test_simple_assign(self, ctor, mocker):
-        param    = DootParamSpec("key", str, prefix="--")
+        param    = ParamSpec(name="key", type=str, prefix="--")
         parser   = ctor()
         result   = parser.parse(["doot", "--key=blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
 
     def test_assign_fail_with_wrong_prefix(self, ctor, mocker):
-        param    = DootParamSpec("key", str, prefix="-")
+        param    = ParamSpec(name="key", type=str, prefix="-")
         parser   = ctor()
 
         with pytest.raises(doot.errors.DootParseError):
             parser.parse(["doot", "--key=blah"],
                 doot_specs=[param], cmds={}, tasks={}
                 )
 
 
 
     def test_simple_follow_assign(self, ctor, mocker):
-        param    = DootParamSpec("key", str)
+        param    = ParamSpec(name="key", type=str)
         parser   = ctor()
         result   = parser.parse(["doot", "-key", "blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
 
     def test_simple_prefix_change(self, ctor, mocker):
-        param    = DootParamSpec("key", str, prefix="--")
+        param    = ParamSpec(name="key", type=str, prefix="--")
         parser   = ctor()
         result   = parser.parse(["doot", "--key", "blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
 
     def test_simple_separator_change(self, ctor, mocker):
-        param    = DootParamSpec("key", str, separator="%%", prefix="--")
+        param    = ParamSpec(name="key", type=str, separator="%%", prefix="--")
         parser   = ctor()
         result   = parser.parse(["doot", "--key%%blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
-    def test_simple_cmd(self, ctor, mocker):
-        cmd_mock = mock_parse_cmd(params=[DootParamSpec(name="key")])
+    def test_simple_cmd(self, ctor, mocker, cmd_mock):
+        cmd_mock.param_specs.append(ParamSpec(name="key"))
         parser   = ctor()
         result   = parser.parse(["doot", "list"],
             doot_specs=[], cmds={"list" : cmd_mock}, tasks={}
             )
 
         assert(result.cmd.name == "list")
         assert(result.cmd.args.key is False)
 
-    def test_simple_cmd_arg(self, ctor, mocker):
-        cmd_mock            = mocker.MagicMock()
-        type(cmd_mock).param_specs = mocker.PropertyMock(return_value=[
-            DootParamSpec(name="key")
-            ])
-        param = DootParamSpec("key", bool)
+    def test_simple_cmd_arg(self, ctor, mocker, cmd_mock):
+        cmd_mock.param_specs.append(ParamSpec(name="key"))
         parser   = ctor()
         result   = parser.parse(["doot", "list", '-key'],
             doot_specs=[], cmds={"list" : cmd_mock}, tasks={}
             )
 
         assert(result.cmd.name == "list")
         assert(result.cmd.args.key is True)
 
-    def test_cmd_default(self, ctor, mocker):
-        cmd_mock                   = mock_parse_cmd()
-        task_mock                  = mock_parse_task(params=[{"name":"key"}])
+    def test_cmd_default(self, ctor, mocker, cmd_mock, spec_mock):
+        spec_mock.extra.cli.append(ParamSpec.build({"name":"key"}))
 
         parser   = ctor()
-        result   = parser.parse(["doot" , "val"],
-            doot_specs=[], cmds={"run": cmd_mock }, tasks={"val": task_mock}
+        result   = parser.parse(["doot" , "agroup::val"],
+            doot_specs=[], cmds={"run": cmd_mock }, tasks={"agroup::val": spec_mock}
             )
 
         assert(result.cmd.name == "run")
 
 
-    def test_simple_task(self, ctor, mocker):
-        cmd_mock             = mock_parse_cmd()
-        task_mock            = mock_parse_task(params=[{"name":"key"}])
+    def test_simple_task(self, ctor, mocker, cmd_mock, spec_mock):
+        spec_mock.extra.cli.append(ParamSpec.build({"name":"key"}))
 
         parser               = ctor()
-        result               = parser.parse(["doot", "list", '-key'],
-            doot_specs=[], cmds={"run": cmd_mock }, tasks={"list" : task_mock}
+        result               = parser.parse(["doot", "agroup::list", '-key'],
+            doot_specs=[], cmds={"run": cmd_mock }, tasks={"agroup::list" : spec_mock}
             )
 
         assert(result.cmd.name == "run")
-        assert("list" in result.tasks)
-        assert(result.tasks.list.key is True)
+        assert("agroup::list" in result.tasks)
+        assert(result.tasks['agroup::list'].key is True)
+
 
+    def test_simple_task_sequence(self, ctor, mocker, cmd_mock):
+        spec_1 = self.make_spec_mock(mocker)
+        spec_2 = self.make_spec_mock(mocker)
 
-    def test_simple_task_sequence(self, ctor, mocker):
-        cmd_mock   = mock_parse_cmd()
-        task_mock  = mock_parse_task(params=[{"name":"key", "type":bool}])
-        task_mock2 = mock_parse_task(params=[{"name":"other", "type":bool}])
+        spec_1.extra.cli.append(ParamSpec.build({"name":"key", "type":bool}))
+        spec_2.extra.cli.append(ParamSpec.build({"name":"other", "type":bool}))
 
         parser     = ctor()
-        result     = parser.parse(["doot", "list", "-key", "blah", "-other"],
-            doot_specs=[], cmds={"run": cmd_mock }, tasks={"list" : task_mock, "blah": task_mock2}
+        result     = parser.parse(["doot", "agroup::list", "-key", "agroup::blah", "-other"],
+            doot_specs=[], cmds={"run": cmd_mock }, tasks={"agroup::list" : spec_1, "agroup::blah": spec_2}
             )
 
         assert(result.cmd.name == "run")
-        assert("list" in result.tasks)
-        assert(result.tasks.list.key is True)
-        assert("blah" in result.tasks)
-        assert(result.tasks.blah.other is True)
+        assert("agroup::list" in result.tasks)
+        assert(result.tasks['agroup::list'].key is True)
+        assert("agroup::blah" in result.tasks)
+        assert(result.tasks['agroup::blah'].other is True)
```

### Comparing `doot-0.7.2/doot/parsers/flexible.py` & `doot-0.8.0/doot/parsers/flexible.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-##-- imports
+#!/usr/bin/env python3
+"""
+
+"""
+# Imports:
 from __future__ import annotations
 
-# import abc
-# import datetime
+# ##-- stdlib imports
+import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
+from collections import ChainMap
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
-
-##-- end imports
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end stdlib imports
 
+# ##-- 3rd party imports
 from tomlguard import TomlGuard
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
 import doot.errors
 from doot._abstract import ArgParser_i
-from doot.structs import DootParamSpec, DootTaskSpec
-from collections import ChainMap
+from doot.structs import ParamSpec, TaskSpec, TaskName
+
+# ##-- end 1st party imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+##-- end logging
 
 SEP : Final[str]          = "--"
 PARAM_ASSIGN_PREFIX       = doot.constants.patterns.PARAM_ASSIGN_PREFIX
 NON_DEFAULT_KEY           = doot.constants.misc.NON_DEFAULT_KEY
 
-default_task : Final[str] = doot.config.on_fail((None,)).general.settings.default_task()
+default_task : Final[str] = doot.config.on_fail((None,)).general.settings.default_task(wrapper=TaskName.build)
+
 default_cmd  : Final[str] = doot.config.on_fail("run", str).general.settings.default_cmd()
 
 class DootFlexibleParser(ArgParser_i):
     """
     convert argv to tomlguard by:
     parsing each arg as toml,
 
@@ -56,71 +68,69 @@
         EXTRA = enum.auto()
 
     def __init__(self):
         self.PS               = DootFlexibleParser._ParseState
         self.head_arg_specs   = None
         self.registered_cmds  = None
         self.registered_tasks = None
-        self.default_help     = DootParamSpec(name="help", default=False, prefix="--")
+        self.default_help     = ParamSpec(name="help", default=False, prefix="--")
 
         ## -- results
         self.head_call                          = None
         self.head_args                          = None
         self.cmd_name                           = None
         self.cmd_args                           = {}
-        self.non_default_cmd_args               = []
         self.tasks_args                         = []
         self.extras                             = {}
         self.force_help                         = False
 
         ## -- loop state
         self.focus                             = self.PS.HEAD
 
     def _build_defaults_dict(self, param_specs:list) -> dict:
         return { x.name : x.default for x in param_specs }
 
-    def parse(self, args:list, *, doot_specs:list[DootParamSpec], cmds:TomlGuard, tasks:TomlGuard) -> None|TomlGuard:
+    def parse(self, args:list, *, doot_specs:list[ParamSpec], cmds:TomlGuard, tasks:TomlGuard) -> None|TomlGuard:
         """
           Parses the list of arguments against available registered parameter specs, cmds, and tasks.
         """
         logging.debug("Parsing args: %s", args)
-        self.head_call                  = args[0]
-        self.head_args                  = self._build_defaults_dict(doot_specs)
-        self.head_arg_specs             = doot_specs
-        self.registered_cmds            = cmds
-        self.registered_tasks           = tasks
-        self.focus                      = self.PS.HEAD
+        self.head_call                                                    = args[0]
+        self.head_args                                                    = self._build_defaults_dict(doot_specs)
+        self.head_arg_specs                                               = doot_specs
+        self.registered_cmds  : dict[str, Command_i]                      = cmds
+        self.registered_tasks : dict[TaskName, TaskSpec]          = tasks
+        self.focus                                                        = self.PS.HEAD
 
-        remaining                      = args[1:]
+        remaining                                                         = args[1:]
         while bool(remaining):
             match self.focus:
                 case self.PS.HEAD:
                     remaining = self.process_head(remaining)
                     self.focus = self.PS.CMD
                 case self.PS.CMD:
                     remaining = self.process_cmd(remaining)
                     self.focus = self.PS.TASK
                 case self.PS.TASK:
                     remaining = self.process_task(remaining)
                     self.focus = self.PS.EXTRA
                 case self.PS.EXTRA:
                     remaining = self.process_extra(remaining)
 
-
         if self.cmd_args.get('help', False) is True:
             self.cmd_args['target']      = self.cmd_name
             self.cmd_name                = "help"
         elif any(x[1].get('help', False) is True for x in self.tasks_args if (target:=x[0])):
             self.cmd_args['target'] = target
             self.cmd_name = "help"
 
         # TODO ensure duplicated tasks have different args
         data = {
             "head"   : {"name": self.head_call, "args": self.head_args },
-            "cmd"    : {"name" : self.cmd_name, "args" : self.cmd_args, NON_DEFAULT_KEY: self.non_default_cmd_args },
+            "cmd"    : {"name" : self.cmd_name, "args" : self.cmd_args },
             "tasks"  : { name : args for name,args in self.tasks_args  },
             "extras" : self.extras
             }
         return TomlGuard(data)
 
     def process_head(self, args) -> list[str]:
         """ consume arguments for doot actual """
@@ -142,19 +152,19 @@
         logging.debug("Cmd Parsing: %s", args)
         head                     = args[0]
         cmd                      = self.registered_cmds.get(head, None)
         self.cmd_name            = head
         if cmd is None:
             cmd                      = self.registered_cmds[default_cmd]
             self.cmd_name            = default_cmd
-            current_specs            = list(sorted(cmd.param_specs, key=DootParamSpec.key_func))
+            current_specs            = list(sorted(cmd.param_specs, key=ParamSpec.key_func))
             self.cmd_args            = self._build_defaults_dict(current_specs)
             return args
 
-        current_specs            = list(sorted(cmd.param_specs, key=DootParamSpec.key_func))
+        current_specs            = list(sorted(cmd.param_specs, key=ParamSpec.key_func))
         self.cmd_args            = self._build_defaults_dict(current_specs)
 
         args.pop(0)
         while bool(args) and args[0] not in self.registered_tasks:
             if args[0] == SEP: # hit SEP, the forced separator
                 # eg: doot list a b c -- something else
                 args.pop(0)
@@ -162,83 +172,83 @@
             match [x for x in current_specs if x == args[0]]:
                 case []:
                     raise doot.errors.DootParseError("Unrecognized cmd arg", head, args[0])
                 case [x]:
                     x.maybe_consume(args, self.cmd_args)
                 case [*xs] if all(y.positional for y in xs):
                     self._consume_next_positional(args, self.cmd_args, xs)
-                case [*xs] if len(y for y in xs if not y.positional):
+                case [*xs] if len(list(y for y in xs if not y.positional)):
                     raise doot.errors.DootParseError("Multiple possible cmd args", head, args[0])
 
-        self.non_default_cmd_args = self._calc_non_default(self._build_defaults_dict(current_specs), self.cmd_args)
+        self.cmd_args[NON_DEFAULT_KEY] = self._calc_non_default(self._build_defaults_dict(current_specs), self.cmd_args)
         return args
 
     def process_task(self, args) -> list[str]:
         """ consume arguments for tasks """
         logging.debug("Task Parsing: %s", args)
         if args[0] not in self.registered_tasks:
+            if default_task is None:
+                return args
             task                     = self.registered_tasks[default_task]
-            assert(isinstance(task, DootTaskSpec))
+            assert(isinstance(task, TaskSpec))
             task_name                 = default_task
-            spec_params               = [DootParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
+            spec_params               = [ParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
             ctor_params               = task.ctor.try_import().param_specs
-            current_specs             = list(sorted(spec_params + ctor_params, key=DootParamSpec.key_func))
+            current_specs             = list(sorted(spec_params + ctor_params, key=ParamSpec.key_func))
             task_args                 = self._build_defaults_dict(current_specs)
             task_args[NON_DEFAULT_KEY] = []
             self.tasks_args.append((task_name, task_args))
             return args
 
-
         while bool(args) and args[0] in self.registered_tasks:
             task_name                 = args.pop(0)
             task                      = self.registered_tasks[task_name]
-            assert(isinstance(task, DootTaskSpec))
-            spec_params               = [DootParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
+            assert(isinstance(task, TaskSpec))
+            spec_params               = [ParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
             ctor_params               = task.ctor.try_import().param_specs
-            current_specs             = list(sorted(spec_params + ctor_params, key=DootParamSpec.key_func))
+            current_specs             = list(sorted(spec_params + ctor_params, key=ParamSpec.key_func))
             task_args                 = self._build_defaults_dict(current_specs)
+
             default_args              = task_args.copy()
             logging.debug("Parsing Task args for: %s: Available: %s", task_name, task_args.keys())
 
             while bool(args) and args[0] not in self.registered_tasks:
                 if args[0] == SEP:
                     args.pop(0)
                     break
 
                 match [x for x in current_specs if x == args[0]]:
                     case [] if args[0].startswith(PARAM_ASSIGN_PREFIX):
                         # No matches, its a free cli arg.
                         try:
-                            key, *values     = args[0].split("=")
-                            task_args[key.removeprefix("--")] = values
+                            key, value = args[0].split("=")
+                            task_args[key.removeprefix("--")] = value
                             args.pop(0)
                         except ValueError:
                             raise doot.errors.DootParseError("Arg failed to split into key=value", args[0])
                     case [x] if not x.positional:
                         x.maybe_consume(args, task_args)
                     case [*xs] if all(y.positional for y in xs):
                         self._consume_next_positional(args, task_args, xs)
                     case [*xs]:
                         raise doot.errors.DootParseError("Multiple possible task args", task_name, args[0])
 
-
             if task_name in [x[0] for x in self.tasks_args]:
                 raise doot.errors.DootParseError("a single task was specified twice")
 
             task_args[NON_DEFAULT_KEY] = self._calc_non_default(default_args, task_args)
             logging.debug("Resulting Arg Assignments for %s : %s", task_name, task_args)
             self.tasks_args.append((task_name, task_args))
 
         return args
 
     def process_extra(self, args) -> None:
         logging.debug("Extra Parsing: %s", args)
         return None
 
-
     def _consume_next_positional(self, args, arg_dict, params:list):
         """
           try each positional param until success
         """
         for param in params:
             try:
                 if 1 <= param.maybe_consume(args, arg_dict):
```

### Comparing `doot-0.7.2/doot/reporters/__tests/test_stack_manager.py` & `doot-0.8.0/doot/reporters/__tests/test_stack_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
                     TypeVar, cast)
 import warnings
 
 import pytest
 import doot
 doot._test_setup()
 
-from doot._abstract import Reporter_i
+from doot._abstract import Reporter_p
 from doot.reporters.stack_manager import DootReportManagerStack
-from doot.structs import DootTraceRecord
+from doot.structs import TraceRecord
 from doot.enums import ReportEnum
 
 logging = logmod.root
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
@@ -34,32 +34,32 @@
 
 ##-- end pytest reminder
 
 class TestReportStackManager:
 
     def test_initial(self):
         manager = DootReportManagerStack()
-        assert(isinstance(manager, Reporter_i))
+        assert(isinstance(manager, Reporter_p))
 
 
     def test_add_basic_trace(self):
         manager = DootReportManagerStack()
         assert(not bool(manager._full_trace))
         manager.add_trace("test")
         assert(bool(manager._full_trace))
-        assert(isinstance(manager._full_trace[0], DootTraceRecord))
+        assert(isinstance(manager._full_trace[0], TraceRecord))
 
     def test_multi_add(self):
         manager = DootReportManagerStack()
         assert(not bool(manager._full_trace))
         manager.add_trace("test")
         manager.add_trace("test")
         manager.add_trace("test")
         assert(len(manager._full_trace) == 3)
-        assert(all(isinstance(x, DootTraceRecord) for x in manager._full_trace))
+        assert(all(isinstance(x, TraceRecord) for x in manager._full_trace))
 
 
     def test_str(self):
         manager = DootReportManagerStack()
         manager.add_trace("test")
         manager.add_trace("test")
         manager.add_trace("test")
```

### Comparing `doot-0.7.2/doot/reporters/__tests/test_summary_manager.py` & `doot-0.8.0/doot/reporters/__tests/test_summary_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import pytest
 
 import doot
 doot._test_setup()
 
 from doot.reporters.summary_manager import DootReportManagerSummary
 from doot.enums import ReportEnum
-from doot.structs import DootTraceRecord
-from doot._abstract import Reporter_i, ReportLine_i
+from doot.structs import TraceRecord
+from doot._abstract import Reporter_p
 
 logging = logmod.root
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
@@ -35,31 +35,31 @@
 
 ##-- end pytest reminder
 
 class TestSummaryReporter:
 
     def test_initial(self):
         manager = DootReportManagerSummary()
-        assert(isinstance(manager, Reporter_i))
+        assert(isinstance(manager, Reporter_p))
 
     def test_add_basic_trace(self):
         manager = DootReportManagerSummary()
         assert(not bool(manager._full_trace))
         manager.add_trace("test")
         assert(bool(manager._full_trace))
-        assert(isinstance(manager._full_trace[0], DootTraceRecord))
+        assert(isinstance(manager._full_trace[0], TraceRecord))
 
     def test_multi_add(self):
         manager = DootReportManagerSummary()
         assert(not bool(manager._full_trace))
         manager.add_trace("test")
         manager.add_trace("test")
         manager.add_trace("test")
         assert(len(manager._full_trace) == 3)
-        assert(all(isinstance(x, DootTraceRecord) for x in manager._full_trace))
+        assert(all(isinstance(x, TraceRecord) for x in manager._full_trace))
 
     @pytest.mark.skip("TODO")
     def test_str(self):
         manager = DootReportManagerSummary()
         manager.add_trace("test", flags=ReportEnum.SUCCEED | ReportEnum.TASK)
         manager.add_trace("test", flags=ReportEnum.FAIL    | ReportEnum.JOB)
         manager.add_trace("test", flags=ReportEnum.SUCCEED | ReportEnum.ACTION)
```

### Comparing `doot-0.7.2/doot/reporters/basic_reporters.py` & `doot-0.8.0/doot/reporters/basic_reporters.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,20 +32,21 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from doot.structs import DootTraceRecord
-from doot._abstract import Reporter_i
+from doot.structs import TraceRecord
+from doot.reporters.base_reporter import BaseReporter
+from doot._abstract import Reporter_p
 
-class DootAlwaysReport(Reporter_i):
+class DootAlwaysReport(BaseReporter):
 
     def __call__(self, trace):
         return str(trace)
 
-class TimeReporter(Reporter_i):
+class TimeReporter(BaseReporter):
 
     def __call__(self, trace):
         time = trace.time.strftime("%H:%M")
         return "{:10} : {}".format(time, str(trace))
```

### Comparing `doot-0.7.2/doot/reporters/stack_manager.py` & `doot-0.8.0/doot/reporters/stack_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,25 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from doot._abstract import Reporter_i, ReportLine_i
-from doot.structs import DootTraceRecord
+from doot._abstract import Reporter_p, ReportLine_p
+from doot.structs import TraceRecord
+from doot.reporters.base_reporter import BaseReporter
 
-class DootReportManagerStack(Reporter_i):
+class DootReportManagerStack(BaseReporter):
     """
     A Stack of Reporters to try using.
     The First one that returns a DootTrace is used.
     """
 
-    def __init__(self, reporters:list[ReportLine_i]=None):
+    def __init__(self, reporters:list[ReportLine_p]=None):
         super().__init__(reporters)
 
     def __str__(self):
         result = []
         for trace in self._full_trace:
             for reporter in self._reporters:
                 match reporter(trace):
```

### Comparing `doot-0.7.2/doot/reporters/summary_manager.py` & `doot-0.8.0/doot/reporters/summary_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,20 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from doot._abstract import Reporter_i, ReportLine_i
-from doot.structs import DootTraceRecord
+from doot._abstract import Reporter_p
+from doot.structs import TraceRecord
 from doot.enums import ReportEnum
+from doot.reporters.base_reporter import BaseReporter
 
-class DootReportManagerSummary(Reporter_i):
+class DootReportManagerSummary(BaseReporter):
     """
     Groups job,task,action success and failures, returns information on them
 
     """
 
     def __init__(self, reporters:list=None):
         super().__init__(reporters)
```

### Comparing `doot-0.7.2/doot/structs.py` & `doot-0.8.0/doot/structs.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,17 @@
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
-from doot._structs.param_spec import DootParamSpec
-from doot._structs.sname import DootStructuredName
-from doot._structs.task_name import DootTaskName
-from doot._structs.code_ref import DootCodeReference
-from doot._structs.action_spec import DootActionSpec
-from doot._structs.task_spec import DootTaskSpec
-from doot._structs.artifact import DootTaskArtifact
-from doot._structs.stub import TaskStub, TaskStubPart
-from doot._structs.trace import DootTraceRecord
+from doot._structs.action_spec import ActionSpec
+from doot._structs.artifact import TaskArtifact
+from doot._structs.code_ref import CodeReference
 from doot._structs.key import DootKey
-from doot._structs.toml_loc import TomlLocation
+from doot._structs.location import Location
+from doot._structs.param_spec import ParamSpec
+from doot._structs.stub import TaskStub, TaskStubPart
+from doot._structs.task_name import TaskName
+from doot._structs.task_spec import TaskSpec
+from doot._structs.trace import TraceRecord
```

### Comparing `doot-0.7.2/doot/task/__tests/test_base_job.py` & `doot-0.8.0/doot/task/__tests/test_base_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 import pytest
 
 logging = logmod.root
 
 import doot
 doot._test_setup()
 from doot.enums import TaskFlags
-from doot.structs import DootTaskSpec, TaskStub
+from doot.structs import TaskSpec, TaskStub
 from doot.task.base_job import DootJob
 import doot._abstract
 
 class TestBaseJob:
 
     def test_initial(self):
-        job = DootJob(DootTaskSpec.build({"name": "basic::example", "flags": ["JOB"]}))
+        job = DootJob(TaskSpec.build({"name": "basic::example", "flags": ["JOB"]}))
         assert(isinstance(job, doot._abstract.Task_i))
         assert(TaskFlags.JOB in job.spec.flags)
 
     def test_paramspecs(self):
-        job = DootJob(DootTaskSpec.build({"name": "basic::example"}))
+        job = DootJob(TaskSpec.build({"name": "basic::example"}))
         param_specs = job.param_specs
         assert(isinstance(param_specs, list))
         assert(len(param_specs) == 3)
 
     def test_spec(self):
         ##-- setup
-        job1 = DootJob(DootTaskSpec.build({"name" :"basic::example"}))
-        job2 = DootJob(DootTaskSpec.build({"name" :"other.group::blah"}))
+        job1 = DootJob(TaskSpec.build({"name" :"basic::example"}))
+        job2 = DootJob(TaskSpec.build({"name" :"other.group::blah"}))
         ##-- end setup
         assert(str(job1.name) == "basic::example")
         assert(str(job2.name) == "\"other.group\"::blah")
         assert(job1 != job2)
         assert(job1 == job1)
 
     def test_class_stub(self):
```

### Comparing `doot-0.7.2/doot/task/__tests/test_base_task.py` & `doot-0.8.0/doot/task/__tests/test_base_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import pytest
 logging = logmod.root
 
 import tomlguard
 import doot
 doot._test_setup()
-from doot.structs import DootTaskSpec, TaskStub
+from doot.structs import TaskSpec, TaskStub
 from doot.task.base_task import DootTask
 import doot._abstract
 
 ##-- reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
@@ -35,66 +35,66 @@
 ##-- end reminder
 
 basic_action = lambda x: ftz.partial(lambda val, state: logging.info("Got: %s : %s", val, state), x)
 
 class TestBaseTask:
 
     def test_initial(self):
-        task = DootTask(DootTaskSpec(name="basic::example"), job=None)
+        task = DootTask(TaskSpec(name="basic::example"), job=None)
         assert(isinstance(task, doot._abstract.Task_i))
 
 
     def test_lambda_action(self):
-        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action}), job=None)
+        task         = DootTask(TaskSpec.build({"name":"basic::example", "action_ctor":basic_action}), job=None)
         assert(isinstance(task, doot._abstract.Task_i))
 
 
     def test_expand_lambda_action(self):
-        task                = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task                = DootTask(TaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions             = list(task.actions)
         assert(len(actions) == 1)
 
 
     def test_run_lambda_action(self, caplog):
         caplog.set_level("DEBUG", logger="doot._printer")
-        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task         = DootTask(TaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions      = list(task.actions)
         result       = actions[0]({"example": "state"})
         assert(result == {"count": 1})
         assert("Base Action Called: 0" in caplog.messages)
         assert("blah" in caplog.messages)
 
 
     def test_expand_action_str(self, caplog):
         caplog.set_level("DEBUG", logger="doot._printer")
-        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor": "test_base_task:basic_action", "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task         = DootTask(TaskSpec.build({"name":"basic::example", "action_ctor": "test_base_task:basic_action", "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions      = list(task.actions)
         result       = actions[0]({"example": "state"})
         assert(result == {"count" : 1})
         assert("Base Action Called: 0" in caplog.messages)
 
     def test_toml_class_stub(self):
         """ build the simplest stub from the class itself """
         stub_obj = TaskStub(ctor=DootTask)
         stub     = DootTask.stub_class(stub_obj)
         assert(str(stub['name'].default) == doot.constants.names.DEFAULT_STUB_TASK_NAME)
 
     def test_toml_instance_stub(self):
         """ build the next simplest stub from an instance of the task """
         stub_obj = TaskStub(ctor=DootTask)
-        task     = DootTask(DootTaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
+        task     = DootTask(TaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
         stub     = task.stub_instance(stub_obj)
         assert(str(stub['name'].default) == "basic::example")
         as_str = stub.to_toml()
 
     def test_toml_instance_stub_rebuild(self):
         """ take a stub and turn it into a task spec  """
         stub_obj         = TaskStub(ctor=DootTask)
-        task             = DootTask(DootTaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
+        task             = DootTask(TaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
         stub             = task.stub_instance(stub_obj)
         as_str           = stub.to_toml()
         loaded           = tomlguard.read(as_str)
-        as_dict          = dict(loaded.tasks.basic[0])
+        as_dict          = dict(loaded)
         as_dict['group'] = "basic"
-        new_spec         = DootTaskSpec.build(as_dict)
-        assert(isinstance(new_spec, DootTaskSpec))
+        new_spec         = TaskSpec.build(as_dict)
+        assert(isinstance(new_spec, TaskSpec))
         assert(str(new_spec.name) == str(task.spec.name))
```

### Comparing `doot-0.7.2/doot/task/base_job.py` & `doot-0.8.0/doot/task/base_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 #!/usr/bin/env python3
 """
 Utility classes for building tasks with a bit of structure
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-# import abc
-# import datetime
-# import enum
+# ##-- stdlib imports
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
-# from uuid import UUID, uuid1
-# from weakref import ref
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
+from uuid import UUID, uuid1
 
-##-- end imports
-
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- end stdlib imports
 
+# ##-- 3rd party imports
 from tomlguard import TomlGuard
+
+# ##-- end 3rd party imports
+
+# ##-- 1st party imports
 import doot
 import doot.errors
-from doot.enums import TaskFlags
-from doot.structs import DootTaskSpec, TaskStub, TaskStubPart, DootTaskName, DootCodeReference, DootStructuredName
 from doot._abstract import Job_i, Task_i
+from doot.enums import TaskFlags
 from doot.errors import DootDirAbsent
+from doot.structs import CodeReference, TaskName, TaskSpec
 from doot.task.base_task import DootTask
 
+# ##-- end 1st party imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+##-- end logging
+
 SUBTASKED_HEAD = doot.constants.patterns.SUBTASKED_HEAD
 
 @doot.check_protocol
 class DootJob(Job_i, DootTask):
     """ Util Class for building single tasks
       wraps with setup and teardown tasks,
       manages cleaning,
       and holds state
 
     """
     _help = ["A Basic Task Constructor"]
     _default_flags = TaskFlags.JOB
 
-    def __init__(self, spec:DootTaskSpec):
+    def __init__(self, spec:TaskSpec):
         assert(spec is not None), "Spec is empty"
         super(DootJob, self).__init__(spec)
 
-    def default_task(self, name:str|DootTaskName|None, extra:None|dict|TomlGuard) -> DootTaskSpec:
+    def default_task(self, name:str|TaskName|None, extra:None|dict|TomlGuard) -> TaskSpec:
         task_name = None
         match name:
             case None:
-                task_name = self.fullname.subtask(SUBTASKED_HEAD)
+                task_name = self.name.subtask(SUBTASKED_HEAD)
             case str():
-                task_name = self.fullname.subtask(name)
-            case DootTaskName():
+                task_name = self.name.subtask(name)
+            case TaskName():
                 task_name = name
             case _:
-                raise doot.errors.DootTaskError("Bad value used to make a subtask in %s : %s", self.name, name)
+                raise doot.errors.DootTaskError("Bad value used to make a subtask in %s : %s", self.shortname, name)
 
         assert(task_name is not None)
-        return DootTaskSpec(name=task_name, extra=TomlGuard(extra))
+        return TaskSpec(name=task_name, extra=TomlGuard(extra))
 
     def is_stale(self, task:Task_i):
         return False
 
     def specialize_task(self, task):
         return task
 
@@ -87,15 +92,15 @@
         stub['head_task'].set(type="taskname", default="", prefix="# ", priority=100)
         stub['queue_behaviour'].default = "default"
         stub['queue_behaviour'].comment = "default | auto | reactive"
         return stub
 
     def stub_instance(self, stub) -> TaskStub:
         stub                      = self.__class__.stub_class(stub)
-        stub['name'].default      = self.fullname
+        stub['name'].default      = self.shortname
         if bool(self.doc):
             stub['doc'].default   = [f"\"{x}\"" for x in self.doc]
         return stub
 
     @classmethod
     def class_help(cls) -> str:
         """ Job *class* help. """
```

### Comparing `doot-0.7.2/doot/task/base_task.py` & `doot-0.8.0/doot/task/base_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 #!/usr/bin/env python3
 """
 """
-##-- imports
+# Imports:
 from __future__ import annotations
 
-import types
+# ##-- stdlib imports
 import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
+import types
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
 
-##-- end imports
+# ##-- end stdlib imports
 
-##-- logging
-logging = logmod.getLogger(__name__)
-##-- end logging
+# ##-- 3rd party imports
+import tomlguard
 
-printer = logmod.getLogger("doot._printer")
+# ##-- end 3rd party imports
 
+# ##-- 1st party imports
 import doot
 import doot.errors
-import tomlguard
-from doot._abstract import Task_i, Job_i, Action_p, PluginLoader_p
-from doot.enums import TaskFlags, TaskStateEnum, TaskQueueMeta
-from doot.structs import TaskStub, TaskStubPart, DootActionSpec, DootCodeReference, DootTaskName, DootTaskArtifact
+from doot._abstract import Action_p, Job_i, PluginLoader_p, Task_i
 from doot.actions.base_action import DootBaseAction
-from doot.errors import DootTaskLoadError, DootTaskError
-
+from doot.enums import TaskFlags, TaskQueueMeta, TaskStatus_e
+from doot.errors import DootTaskError, DootTaskLoadError
 from doot.mixins.param_spec import ParamSpecMaker_m
-from doot.mixins.importer import Importer_m
+from doot.structs import (ActionSpec, CodeReference, TaskArtifact,
+                          TaskName)
+from doot._structs.relation_spec import RelationSpec
+
+# ##-- end 1st party imports
+
+##-- logging
+logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
+##-- end logging
 
-TASK_ALISES     = doot.aliases.task
-PRINT_LOCATIONS = doot.constants.printer.PRINT_LOCATIONS
+TASK_ALISES                    = doot.aliases.task
+PRINT_LOCATIONS                = doot.constants.printer.PRINT_LOCATIONS
 STATE_TASK_NAME_K : Final[str] = doot.constants.patterns.STATE_TASK_NAME_K
 
 class _TaskProperties_m(ParamSpecMaker_m):
 
     @classmethod
     @property
-    def param_specs(cls) -> list[DootParamSpec]:
+    def param_specs(cls) -> list[ParamSpec]:
         """  make class parameter specs  """
         return [
             cls.build_param(name="help", default=False, invisible=True, prefix="--"),
             cls.build_param(name="debug", default=False, invisible=True, prefix="--"),
             cls.build_param(name="verbose", default=0, type=int, invisible=True, prefix="--")
            ]
 
     @property
-    def readable_name(self) -> str:
-        return str(self.spec.name.readable)
-
-    @property
     def actions(self):
         """lazy creation of action instances,
           `prepare_actions` has already ensured all ctors can be found
         """
         yield from iter(self.spec.actions)
 
     @property
-    def name(self) -> str:
-        return str(self.spec.name)
+    def shortname(self) -> str:
+        return str(self.spec.name.readable)
 
     @property
-    def fullname(self) -> DootTaskName:
+    def name(self) -> TaskName:
         return self.spec.name
 
     @property
     def short_doc(self) -> str:
         """ Generate Job Class 1 line help string """
         try:
             split_doc = [x for x in self.__class__.__doc__.split("\n") if bool(x)]
@@ -88,93 +92,68 @@
             return ":: "
 
     @property
     def doc(self) -> list[str]:
         return self.spec.doc or self._help
 
     @property
-    def depends_on(self) -> abc.Generator[str|DootTaskName]:
-        for x in self.spec.depends_on:
-            yield x
+    def is_stale(self):
+        return False
 
-    @property
-    def required_for(self) -> abc.Generator[str|DootTaskName]:
-        for x in self.spec.required_for:
-            yield x
+@doot.check_protocol
+class DootTask(_TaskProperties_m, Task_i):
+    """
+      The simplest task, which can import action classes.
+      eg:
+      actions = [ {do = "doot.actions.shell_action:DootShellAction", args = ["echo", "this is a test"] } ]
 
-    def add_execution_record(self, arg):
-        """ Record some execution record information for display or debugging """
-        self._records.append(arg)
+      Actions are imported upon task creation.
+    """
+    action_ctor                                   = DootBaseAction
+    _default_flags                                = TaskFlags.TASK
+    _help                                         = ["The Simplest Task"]
+    COMPLETE_STATES  : Final[set[TaskStatus_e]]   = {TaskStatus_e.SUCCESS, TaskStatus_e.EXISTS}
+    INITIAL_STATE    : Final[TaskStatus_e]        = TaskStatus_e.INIT
 
-    def log(self, msg, level=logmod.DEBUG, prefix=None) -> None:
-        """
-        utility method to log a message, useful as tasks are running
-        """
-        prefix : str       = prefix or ""
-        lines  : list[str] = []
-        match msg:
-            case str():
-                lines.append(msg)
-            case types.LambdaType():
-                lines.append(msg())
-            case [types.LambdaType()]:
-                lines += msg[0]()
-            case list():
-                lines += msg
+    def __init__(self, spec, *, job=None, action_ctor=None, **kwargs):
+        self.spec        : SpecStruct_p        = spec
+        self.priority    : int                 = self.spec.priority
+        self.status      : TaskStatus_e        = DootTask.INITIAL_STATE
+        self.flags       : TaskFlags           = TaskFlags.TASK
+        self.state       : dict                = dict(spec.extra)
+        self.action_ctor : callable            = action_ctor
+        self._records    : list[Any]           = []
 
-        for line in lines:
-            logging.log(level, prefix + str(line))
+        self.state[STATE_TASK_NAME_K]          = self.spec.name
+        self.state['_action_step']             = 0
 
-    @property
-    def is_stale(self):
-        return False
+        self.prepare_actions()
+
+    def __repr__(self):
+        return f"<Task: {self.shortname}>"
+
+    def __bool__(self):
+        return self.status in DootTask.COMPLETE_STATES
 
     def __hash__(self):
         return hash(self.name)
 
-    def __lt__(self, other:Task_i) -> bool:
-        """ Task A < Task B iff A ∈ B.run_after   """
-        return (other.name in self.spec.after_artifacts
-                or other.name in self.spec.depends_on)
+    def __lt__(self, other:TaskName|Task_i) -> bool:
+        """ Task A < Task B if A ∈ B.run_after or B ∈ A.runs_before  """
+        return any(other.name in x.target for x in self.spec.depends_on)
 
     def __eq__(self, other):
         match other:
-            case str():
+            case str() | TaskName():
                 return self.name == other
             case Task_i():
                 return self.name == other.name
             case _:
                 return False
 
-@doot.check_protocol
-class DootTask(_TaskProperties_m, Importer_m, Task_i):
-    """
-      The simplest task, which can import action classes.
-      eg:
-      actions = [ {do = "doot.actions.shell_action:DootShellAction", args = ["echo", "this is a test"] } ]
-    """
-    action_ctor    = DootBaseAction
-    _default_flags = TaskFlags.TASK
-    _help          = ["The Simplest Task"]
-
-    def __init__(self, spec, *, job=None, action_ctor=None, **kwargs):
-        self.spec       : SpecStruct_p        = spec
-        self.status     : TaskStateEnum       = TaskStateEnum.WAIT
-        self.flags      : TaskFlags           = TaskFlags.JOB
-        self._records   : list[Any]           = []
-        self.state                            = dict(spec.extra)
-        self.job                              = job
-        self.state[STATE_TASK_NAME_K]         = self.spec.name
-        self.state['_action_step']            = 0
-        self.action_ctor                      = action_ctor
-        self.prepare_actions()
-
-    def __repr__(self):
-        return f"<Task: {self.name}>"
-
     @classmethod
     def class_help(cls):
         """ Task *class* help. """
         help_lines = [f"Task   : {cls.__qualname__} v{cls._version}", ""]
         mro = " -> ".join(x.__name__ for x in cls.mro())
         help_lines.append(f"Task MRO: {mro}")
         help_lines.append("")
@@ -190,44 +169,76 @@
         else:
             stub.ctor                   = cls
 
         # Come first
         stub['required_for'].priority   = -90
         stub['depends_on'].priority     = -100
 
-        stub['print_levels'].type       = f"Dict: {PRINT_LOCATIONS}"
-        stub['print_levels'].default    = {"head":"INFO","build":"INFO","sleep":"INFO","action":"INFO", "execute":"INFO"}
-
         stub['priority'].default        = 10
         stub['queue_behaviour'].default = "default"
         stub['queue_behaviour'].comment = " | ".join({x.name for x in TaskQueueMeta})
         stub['flags'].comment = " | ".join({x.name for x in TaskFlags})
         return stub
 
     def stub_instance(self, stub) -> TaskStub:
         """ extend the class toml stub with details from this instance """
-        stub['name'].default      = self.fullname
+        stub['name'].default      = self.shortname
         if bool(self.doc):
             stub['doc'].default   = self.doc[:]
         stub['flags'].default     = self.spec.flags
 
         return stub
 
     def prepare_actions(self):
         """ if the task/action spec requires particular action ctors, load them.
           if the action spec doesn't have a ctor, use the task's action_ctor
         """
-        logging.info("Preparing Actions: %s", self.name)
+        logging.debug("Preparing Actions: %s", self.shortname)
+        failed = []
         for group in self.spec.action_groups:
             for action_spec in group:
                 match action_spec:
-                    case DootTaskName() | DootTaskArtifact():
+                    case RelationSpec():
                         pass
-                    case DootActionSpec() if action_spec.fun is not None:
+                    case ActionSpec() if action_spec.fun is not None:
                         pass
-                    case DootActionSpec() if action_spec.do is not None:
-                        action_ref = self.import_callable(action_spec.do)
-                        action_spec.set_function(action_ref)
-                    case DootActionSpec():
+                    case ActionSpec() if action_spec.do is not None:
+                        try:
+                            action_ctor = action_spec.do.try_import()
+                            action_spec.set_function(action_ctor)
+                        except ImportError as err:
+                            failed.append(err)
+                    case ActionSpec():
                         action_spec.set_function(self.action_ctor)
                     case _:
-                        raise doot.errors.DootTaskError("Unknown element in action group: ", action_spec, self.spec.name)
+                        failed.append(doot.errors.DootTaskError("Unknown element in action group: ", action_spec, self.shortname))
+
+        match failed:
+            case []:
+                pass
+            case [x]:
+                raise x
+            case [*xs]:
+                raise ImportError("Multiple Action Spec import failures", xs)
+
+    def add_execution_record(self, arg):
+        """ Record some execution record information for display or debugging """
+        self._records.append(arg)
+
+    def log(self, msg, level=logmod.DEBUG, prefix=None) -> None:
+        """
+        utility method to log a message, useful as tasks are running
+        """
+        prefix : str       = prefix or ""
+        lines  : list[str] = []
+        match msg:
+            case str():
+                lines.append(msg)
+            case types.LambdaType():
+                lines.append(msg())
+            case [types.LambdaType()]:
+                lines += msg[0]()
+            case list():
+                lines += msg
+
+        for line in lines:
+            logging.log(level, prefix + str(line))
```

### Comparing `doot-0.7.2/doot/task/specialised_jobs.py` & `doot-0.8.0/doot/_abstract/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,48 @@
 #!/usr/bin/env python3
 """
 
 """
 ##-- imports
 from __future__ import annotations
 
-# import abc
-# import datetime
-# import enum
+import types
+import abc
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
-import types
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from copy import deepcopy
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
+from uuid import UUID, uuid1
+from weakref import ref
 
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import doot
-from doot.task.base_job import DootJob
-
-
-@doot.check_protocol
-class GroupJob(DootJob):
-    """ A Group of task specs, none of which require params """
-
-    def __init__(self, spec:DootTaskSpec):
-        super().__init__(spec)
-        self.name       = name.replace(" ", "_")
-        self.tasks      = list(args)
-        self.as_creator = as_creator
+from abc import abstractmethod
+from tomlguard import TomlGuard
+from jgdv.structs.regex import RegexEqual
 
-    def __str__(self):
-        return f"group:{self.name}({len(self)})"
+from doot._abstract.protocols import ParamStruct_p
 
-    def __len__(self):
-        return len(self.tasks)
-
-    def __iadd__(self, other):
-        self.tasks.append(other)
-        return self
-
-    def to_dict(self):
-        # this can add jobs to the namespace,
-        # but doesn't help for dicts
-        return {f"doot_{self.name}_{id(x)}": x for x in self.tasks}
-
-    def add_tasks(self, *other):
-        for x in other:
-            self.tasks.append(other)
-
-@doot.check_protocol
-class WatchJob(DootJob):
+class ArgParser_i:
     """
-    Job that watches for conditions, *then*
-    generates tasks.
-    eg: a file watcher
+    A Single standard process point for turning the list of passed in args,
+    into a dict, into a tomlguard,
+    along the way it determines the cmds and tasks that have been chosne
     """
-    pass
+
+    @abstractmethod
+    def parse(self, args:list[str], doot_arg_specs:list[ParamStruct_p], cmds:TomlGuard, tasks:TomlGuard) -> TomlGuard:
+        pass
```

### Comparing `doot-0.7.2/doot/utils/__tests/test_action_decorators.py` & `doot-0.8.0/doot/utils/__tests/test_action_decorators.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/action_decorators.py` & `doot-0.8.0/doot/utils/action_decorators.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/chain_get.py` & `doot-0.8.0/doot/utils/chain_get.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/check_protocol.py` & `doot-0.8.0/doot/utils/check_protocol.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/decorators.py` & `doot-0.8.0/doot/utils/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import abc
 import builtins
 from typing import Type
 import decorator
 import doot
 import doot.errors
 from doot.enums import LocationMeta
-from doot._abstract.structs import SpecStruct_p
+from doot._abstract.protocols import SpecStruct_p
 
 DOOT_ANNOTATIONS : Final[str]                = "__DOOT_ANNOTATIONS__"
 KEYS_HANDLED   : Final[str]                = "_doot_keys_handler"
 ORIG_ARGS      : Final[str]                = "_doot_orig_args"
 KEY_ANNOTS     : Final[str]                = "_doot_keys"
 FUNC_WRAPPED   : Final[str]                = "__wrapped__"
 PARAM_PREFIX   : Final[str] = "_"
```

### Comparing `doot-0.7.2/doot/utils/log_colour.py` & `doot-0.8.0/doot/utils/log_colour.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/log_context.py` & `doot-0.8.0/doot/utils/log_context.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/mock_gen.py` & `doot-0.8.0/doot/utils/mock_gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,109 +51,101 @@
     built = []
     for name, [pre, post] in tasks.items():
         current = mock_task_spec(name, pre=pre, post=post)
         built.append(current)
 
     return built
 
-
-
 def mock_task(name, spec=None, actions:int=1, **kwargs):
     task_m = MagicMock(spec=Task_i,
                        name=name,
                        state={},
                        **kwargs)
     task_m.spec = spec or mock_task_spec(name=name, action_count=actions)
-    _add_prop(task_m, "name", structs.DootTaskName.build(name))
+    _add_prop(task_m, "name", structs.TaskName.build(name))
     _add_prop(task_m, "actions", task_m.spec.actions)
     return task_m
 
 def mock_job(name, pre=None, post=None, spec=None, **kwargs):
     task_m = MagicMock(spec=Job_i,
                        name=name,
                        state={},
                        **kwargs)
     _add_prop(task_m, "name", name)
     task_m.spec = spec or mock_task_spec(name=name)
     return task_m
 
-def mock_task_spec(name="mockSpec", pre=None, post=None, action_count=1, extra=None,  **kwargs):
+def mock_task_spec(name="agroup::mockSpec", pre=None, post=None, action_count=1, extra=None,  **kwargs):
     extra = extra or {}
     if "sleep" not in extra:
         extra['sleep'] = 0.1
-    spec_m = MagicMock(structs.DootTaskSpec(name=name),
+    spec_m = MagicMock(structs.TaskSpec(name=name),
                        actions=mock_action_specs(num=action_count),
                        extra=tomlguard.TomlGuard(extra),
                        priority=10,
                        queue_behaviour=TaskQueueMeta.default,
                        depends_on=pre or [],
                        required_for=post or [],
                        setup=[],
                        cleanup=[],
-                       print_levels=tomlguard.TomlGuard({}),
                        )
-    spec_m.name = structs.DootTaskName.build(name)
+    spec_m.name = structs.TaskName.build(name)
     return spec_m
 
 def mock_action_specs(num=1) -> list:
     results = []
     for x in range(num):
-        action_spec_m = MagicMock(spec=structs.DootActionSpec(),
+        action_spec_m = MagicMock(spec=structs.ActionSpec(),
                                   args=[],
                                   kwargs=tomlguard.TomlGuard())
         type(action_spec_m).__call__ = MagicMock(return_value=None)
         results.append(action_spec_m)
 
     return results
 
-def mock_parse_cmd(name="cmd", params=None):
-    """ Build a mock command with cli params """
-    cmd_mock = MagicMock(spec=Command_i, name=name)
-    _add_prop(cmd_mock, "name", name)
-    _add_prop(cmd_mock, "param_specs", [mock_param_spec("help", False, type=bool)] + (params or []))
-    return cmd_mock
-
-def mock_parse_task(params=None, ctor_params=None):
-    """ Build a mock Task Spec, with spec defined cli params, and ctor defined cli params  """
-    task_ctor_mock       = mock_task_ctor(params=ctor_params)
-    task_ctor_ref_mock   = mock_code_ref(returns=task_ctor_mock)
-    task_mock            = mock_task_spec(extra={"cli": params})
-    task_mock.ctor       = task_ctor_ref_mock
-    return task_mock
 
 def mock_entry_point(name="basic", value=None):
     m = MagicMock(spec=EntryPoint)
     _add_prop(m, "name", name)
-    _add_prop(m, "value", name)
-    m.load.return_value = value
+    _add_prop(m, "value", value)
+    m.load = MagicMock(return_value=value)
     return m
 
 def mock_task_ctor(name="APretendClass", module="pretend", params=None):
-    mock_ctor = MagicMock(spec=Task_i)
-    _add_prop(mock_ctor, "name", name)
-    _add_prop(mock_ctor, "param_specs", params or [])
+    class MockedSubClass(Task_i):
+        def __new__(cls, *args, **kwargs):
+            m = mock.Mock(spec=cls)
+            _add_prop(mock_ctor, "name", name)
+            _add_prop(mock_ctor, "param_specs", params or [])
+            return m
+
+        @classmethod
+        @property
+        def param_specs(cls):
+            return params or []
+
+    mock_ctor = MockedSubClass
     mock_ctor.__module__ = module
     mock_ctor.__name__   = name
     return mock_ctor
 
 def mock_code_ref(returns=None):
-    code_ref_m  = MagicMock(spec=structs.DootCodeReference())
-    code_ref_m.try_import.return_value  = returns
+    code_ref_m  = MagicMock(spec=structs.CodeReference())
+    code_ref_m.try_import = MagicMock(return_value=returns)
     return code_ref_m
 
 def mock_param_spec(name, val, type=Any):
-    m = MagicMock(spec=structs.DootParamSpec(name, type), default=val, positional=False, prefix="-")
+    m = MagicMock(spec=structs.ParamSpec(name=name, type=type), default=val, positional=False, prefix="-")
 
     return m
 
-
 def mock_tracker(tasks):
     tracker_m        = MagicMock(spec=TaskTracker_i)
     local_tasks      = tasks[:]
+
     def simple_pop():
         if bool(local_tasks):
             return local_tasks.pop()
         return None
 
     tracker_m.next_for = simple_pop
-    tracker_m.__bool__ = lambda x: bool(local_tasks)
     return tracker_m
```

### Comparing `doot-0.7.2/doot/utils/plugin_selector.py` & `doot-0.8.0/doot/utils/plugin_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,25 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from importlib.metadata import EntryPoint
-from doot.structs import DootCodeReference
+from doot.structs import CodeReference
 import doot.errors
 
 def plugin_selector(plugins:TomlGuard, *, target="default", fallback=None) -> type:
     """ Selects and loads plugins from a tomlguard, based on a target,
     with an available fallback constructor """
     logging.debug("Selecting plugin for target: %s", target)
 
     if target != "default":
         try:
-            name = DootCodeReference.build(target)
+            name = CodeReference.build(target)
             return name.try_import()
         except ImportError as err:
             # raise doot.errors.DootInvalidConfig("Import Failed: %s : %s", target, err.msg) from err
             pass
         except (AttributeError, KeyError) as err:
             # raise doot.errors.DootInvalidConfig("Import Failed: Module has missing attritbue/key: %s", target) from err
             pass
```

### Comparing `doot-0.7.2/doot/utils/retrievers.py` & `doot-0.8.0/doot/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/signal_handler.py` & `doot-0.8.0/doot/utils/signal_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot/utils/testing_fixtures.py` & `doot-0.8.0/doot/utils/url_expand.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 #!/usr/bin/env python3
 """
-Pytest testing fixtures
-"""
 
-##-- builtin imports
+"""
+##-- imports
 from __future__ import annotations
 
-# import abc
+import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from copy import deepcopy
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+                    cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
+from weakref import ref
 
-##-- end builtin imports
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import pytest
-import os
-import doot
-
-@pytest.fixture
-def wrap_tmp(tmp_path):
-    """ create a new temp directory, and change cwd to it,
-      returning to original cwd after the test
-      """
-    logging.debug("Moving to temp dir")
-    orig     = pl.Path().cwd()
-    new_base = tmp_path / "test_root"
-    new_base.mkdir()
-    with doot.locs(new_base):
-        yield new_base
-    logging.debug("Returning to original dir")
-
-
-@pytest.fixture
-def wrap_locs():
-    logging.debug("Activating temp locs")
-    with doot.locs() as temp:
-        yield temp
+from time import sleep
+import requests
+
+
+def expander(current):
+    # header = {'user-agent': args.agent}
+    try:
+        response = requests.head(current, allow_redirects=True, timeout=2, headers=header)
+        if response.ok:
+            expanded[current] = response.url
+        else:
+            expanded[current] = response.status_code
+
+        return "{} |%| {}".format(current, args.separator, expanded[current])
+    except Exception as err:
+        cmd    = 'say -v Moira -r 50 "Error"'
+        system(cmd)
+        expanded[current] = f"400.1 : {str(err)}"
+        logging.info("Error: %s", str(err))
```

### Comparing `doot-0.7.2/doot/utils/trace_helper.py` & `doot-0.8.0/doot/utils/trace_helper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.2/doot.egg-info/PKG-INFO` & `doot-0.8.0/doot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.2
+Version: 0.8.0
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -57,25 +57,27 @@
 Requires-Dist: stackprinter>=0.2.10
 Requires-Dist: matplotlib
 Requires-Dist: sty
 Requires-Dist: boltons
 Requires-Dist: more_itertools
 Requires-Dist: decorator-validation>=3.0.0
 Requires-Dist: decorator>=5.0.0
-Requires-Dist: jgdv
+Requires-Dist: pydantic
+Requires-Dist: jgdv>=0.1.3
 Provides-Extra: test
 Requires-Dist: pytest<5.0.0; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
+<!-- <!--  README.md -*- mode: GFM -*-
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.2  
+Version : 0.8.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
@@ -97,23 +99,23 @@
 
 eg:
 ``` toml
 # -*- mode:conf-toml; -*-
 [settings.general]
 notify                   = { say-on-exit = false }
 loaders                  = { commands="default", task="default", parser="default"}
-location_check           = { make_missing = true, print_levels={action="WARN", execute="WARN" } }
+location_check           = { make_missing = true }
 
 [settings.tasks]
 sources = [".tasks"] # Files or directories where task specs can be loaded from, expanded according to [[locations]] keys
 code    = []         # Directories where task specific code can be imported from, expanded according to [[locations]] keys
 sleep   = { task=0.2, subtask=1, batch=1 }
 
 [logging]
-stream  = { level="WARN",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
+stream  = { level="WARNING",  allow=["doot"], format="{levelname:<8} : {message}", colour=true }
 file    = { level="DEBUG", allow=["doot"], format="{levelname:<8} : {message:<20} :|: (module:{module} line:{lineno} fn:{funcName})" }
 printer = { level="INFO", colour=true}
 
 [plugins]
 # Allows for defining shorthands
 command        = { other-run = "doot.cmds.run_cmd:RunCmd", tasks = "doot.cmds.list_cmd:ListCmd" }
 report-line    = {}
@@ -137,16 +139,16 @@
 
 ``` toml
 [[tasks.mygroup]] # mygroup is the group this task is part of
 name                 = "mytask" # combined together, this means this specific task is `mygroup::mytask`
 version              = "0.1"    # <str>
 ctor                 = "task"   # <type> the python class this task uses. See the plugins listed in 'doot plugins'
 doc                  = ["Text to help understand what this task does"] # <list[str]>
-required_for         = []                   # <list[DootTaskArtifact]> see below
-depends_on           = []                   # <list[DootTaskArtifact]> see below
+required_for         = []                   # <list[TaskArtifact]> see below
+depends_on           = []                   # <list[TaskArtifact]> see below
 actions              = []                   # <list[Any]> See below
 ```
 
 You can see what tasks are available by calling `doot list`.
 You can get help on a specific task by calling `doot {task} --help` or `doot help {task}`.
 You can run a task by calling `doot {task}` or `doot run {task}`.
 eg: `doot mygroup::mytask`
@@ -166,15 +168,15 @@
 - Action write! : doot.actions.io:WriteAction
 -- Declared kwargs for action: ['from_', 'to']
 
 -- Toml Form:
 { do="write!", args=[] }
 
 - For Custom Python Actions, implement the following in the .tasks director
-def custom_action(spec:DootActionSpec, task_state:dict) -> None|bool|dict:...
+def custom_action(spec:ActionSpec, task_state:dict) -> None|bool|dict:...
 ```
 
 When specifying values in toml you can use direct keys, or indirect keys.
 For example, the action:
 ``` toml
 { do="log", msg="This is a test", level="INFO" }
 ```
```

### Comparing `doot-0.7.2/doot.egg-info/SOURCES.txt` & `doot-0.8.0/doot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,54 +10,59 @@
 doot.egg-info/SOURCES.txt
 doot.egg-info/dependency_links.txt
 doot.egg-info/entry_points.txt
 doot.egg-info/requires.txt
 doot.egg-info/top_level.txt
 doot/__data/aliases.toml
 doot/__data/constants.toml
-doot/__templates/basic_toml
+doot/__templates/basic_config_toml
 doot/__templates/stub_task_py
 doot/__templates/tasks_toml
 doot/__tests/test_basic.py
 doot/__tests/test_inits.py
 doot/_abstract/__init__.py
 doot/_abstract/cmd.py
 doot/_abstract/control.py
 doot/_abstract/dbm.py
 doot/_abstract/loader.py
 doot/_abstract/overlord.py
 doot/_abstract/parser.py
 doot/_abstract/policy.py
+doot/_abstract/protocols.py
 doot/_abstract/reporter.py
-doot/_abstract/structs.py
 doot/_abstract/task.py
 doot/_structs/__init__.py
 doot/_structs/action_spec.py
 doot/_structs/artifact.py
 doot/_structs/code_ref.py
 doot/_structs/key.py
+doot/_structs/location.py
+doot/_structs/log.doot
+doot/_structs/logger_spec.py
 doot/_structs/param_spec.py
-doot/_structs/sname.py
+doot/_structs/relation_spec.py
 doot/_structs/structured_name.py
 doot/_structs/stub.py
 doot/_structs/task_name.py
 doot/_structs/task_spec.py
-doot/_structs/toml_loc.py
 doot/_structs/trace.py
 doot/_structs/__tests/test_action_spec.py
 doot/_structs/__tests/test_artifact.py
 doot/_structs/__tests/test_code_ref.py
 doot/_structs/__tests/test_formatter.py
 doot/_structs/__tests/test_key.py
 doot/_structs/__tests/test_key_decorators.py
 doot/_structs/__tests/test_key_multi.py
 doot/_structs/__tests/test_key_path_expansion.py
 doot/_structs/__tests/test_key_string_expansion.py
 doot/_structs/__tests/test_key_type_expansion.py
+doot/_structs/__tests/test_location.py
 doot/_structs/__tests/test_param_spec.py
+doot/_structs/__tests/test_relation_spec.py
+doot/_structs/__tests/test_structured_name.py
 doot/_structs/__tests/test_stub.py
 doot/_structs/__tests/test_task_name.py
 doot/_structs/__tests/test_task_spec.py
 doot/actions/__init__.py
 doot/actions/base_action.py
 doot/actions/compression.py
 doot/actions/control_flow.py
@@ -95,18 +100,21 @@
 doot/cmds/step_cmd.py
 doot/cmds/stub_cmd.py
 doot/cmds/__tests/test_list_cmd.py
 doot/control/__init__.py
 doot/control/base_runner.py
 doot/control/base_tracker.py
 doot/control/locations.py
+doot/control/log.doot
 doot/control/overlord.py
 doot/control/runner.py
 doot/control/step_runner.py
 doot/control/tracker.py
+doot/control/__tests/obsolete.py
+doot/control/__tests/test_base_tracker.py
 doot/control/__tests/test_locations.py
 doot/control/__tests/test_overlord.py
 doot/control/__tests/test_runner.py
 doot/control/__tests/test_tracker.py
 doot/loaders/__init__.py
 doot/loaders/cmd_loader.py
 doot/loaders/plugin_loader.py
@@ -122,22 +130,24 @@
 doot/mixins/param_spec.py
 doot/mixins/path_manip.py
 doot/mixins/zipper.py
 doot/parsers/__init__.py
 doot/parsers/flexible.py
 doot/parsers/__tests/test_flexible.py
 doot/reporters/__init__.py
+doot/reporters/base_reporter.py
 doot/reporters/basic_reporters.py
 doot/reporters/stack_manager.py
 doot/reporters/summary_manager.py
 doot/reporters/__tests/test_stack_manager.py
 doot/reporters/__tests/test_summary_manager.py
 doot/task/__init__.py
 doot/task/base_job.py
 doot/task/base_task.py
+doot/task/base_transformer.py
 doot/task/check_locs.py
 doot/task/specialised_jobs.py
 doot/task/__tests/test_base_job.py
 doot/task/__tests/test_base_task.py
 doot/task/__tests/test_check_locs.py
 doot/utils/__init__.py
 doot/utils/action_decorators.py
```

