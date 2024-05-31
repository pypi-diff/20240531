# Comparing `tmp/codeflash-0.6.4.tar.gz` & `tmp/codeflash-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.6.4.tar", max compression
+gzip compressed data, was "codeflash-0.6.5.tar", max compression
```

## Comparing `codeflash-0.6.4.tar` & `codeflash-0.6.5.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.4/README.md
--rw-r--r--   0        0        0     4405 2024-05-30 02:49:44.753622 codeflash-0.6.4/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.4/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.4/codeflash/api/__init__.py
--rw-r--r--   0        0        0     8936 2024-05-23 20:37:01.092407 codeflash-0.6.4/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4833 2024-05-29 02:22:36.999360 codeflash-0.6.4/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.4/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     8062 2024-05-29 02:22:36.999766 codeflash-0.6.4/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0      305 2024-05-29 02:22:37.000004 codeflash-0.6.4/codeflash/cli_cmds/cli_common.py
--rw-r--r--   0        0        0    22576 2024-05-29 02:22:37.000347 codeflash-0.6.4/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      475 2024-05-29 02:22:37.000790 codeflash-0.6.4/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1835 2024-05-29 02:22:37.000925 codeflash-0.6.4/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.4/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     9586 2024-05-30 02:48:32.417243 codeflash-0.6.4/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8556 2024-05-23 20:36:49.437532 codeflash-0.6.4/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2956 2024-05-23 20:36:49.437828 codeflash-0.6.4/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.4/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.4/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3908 2024-04-26 00:11:25.877810 codeflash-0.6.4/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2979 2024-05-23 20:36:49.438085 codeflash-0.6.4/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     2056 2024-05-23 20:36:49.438180 codeflash-0.6.4/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3143 2024-05-29 02:22:37.001222 codeflash-0.6.4/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0     1083 2024-05-29 02:22:37.001407 codeflash-0.6.4/codeflash/code_utils/github_utils.py
--rw-r--r--   0        0        0    24003 2024-05-23 20:36:49.438744 codeflash-0.6.4/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.4/codeflash/code_utils/main_calls_bubblesort.py
--rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.4/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0        0 2024-05-23 20:36:49.438788 codeflash-0.6.4/codeflash/code_utils/sqlalchemy_experiment.py
--rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.4/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1898 2024-05-23 20:36:49.439035 codeflash-0.6.4/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.4/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    18481 2024-05-23 20:36:49.439328 codeflash-0.6.4/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    20032 2024-05-23 20:36:49.439635 codeflash-0.6.4/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1291 2024-05-23 20:36:49.439889 codeflash-0.6.4/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.4/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-05-29 01:00:54.268195 codeflash-0.6.4/codeflash/main.py
--rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.4/codeflash/models/ExperimentMetadata.py
--rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.4/codeflash/models/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.4/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    12006 2024-05-23 20:36:49.440092 codeflash-0.6.4/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    54363 2024-05-23 20:36:49.440453 codeflash-0.6.4/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.4/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-23 20:36:49.440782 codeflash-0.6.4/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1992 2024-05-23 20:36:49.441057 codeflash-0.6.4/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.4/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.4/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 03:48:11.207884 codeflash-0.6.4/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0    20467 2024-05-23 20:36:49.441169 codeflash-0.6.4/codeflash/tracer.py
--rw-r--r--   0        0        0        1 2024-05-23 20:36:49.441293 codeflash-0.6.4/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     2644 2024-05-23 20:36:49.441383 codeflash-0.6.4/codeflash/tracing/profile_stats.py
--rw-r--r--   0        0        0     5942 2024-05-23 20:36:49.441614 codeflash-0.6.4/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.4/codeflash/tracing/tracing_utils.py
--rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.4/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.4/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.4/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1241 2024-05-23 20:36:49.441868 codeflash-0.6.4/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14621 2024-05-23 20:36:49.442151 codeflash-0.6.4/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6830 2024-05-23 20:36:49.442405 codeflash-0.6.4/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1759 2024-05-23 20:36:49.442652 codeflash-0.6.4/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.4/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4189 2024-05-23 20:36:49.442883 codeflash-0.6.4/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-05-30 02:49:52.922329 codeflash-0.6.4/codeflash/version.py
--rw-r--r--   0        0        0     2963 2024-05-30 02:49:52.917532 codeflash-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.5/README.md
+-rw-r--r--   0        0        0     4405 2024-05-31 21:03:43.421623 codeflash-0.6.5/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.5/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.5/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     8936 2024-05-31 21:03:09.269838 codeflash-0.6.5/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4833 2024-05-30 23:15:57.599950 codeflash-0.6.5/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.5/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8042 2024-05-31 20:15:40.283230 codeflash-0.6.5/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0      305 2024-05-30 23:15:57.600218 codeflash-0.6.5/codeflash/cli_cmds/cli_common.py
+-rw-r--r--   0        0        0    22606 2024-05-31 20:15:40.283425 codeflash-0.6.5/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      475 2024-05-30 23:15:57.600580 codeflash-0.6.5/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1835 2024-05-30 23:15:57.600684 codeflash-0.6.5/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.5/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9586 2024-05-30 23:15:57.600858 codeflash-0.6.5/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-30 23:15:57.601031 codeflash-0.6.5/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-30 23:15:57.601170 codeflash-0.6.5/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.5/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.5/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3464 2024-05-31 20:15:40.283606 codeflash-0.6.5/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2979 2024-05-30 23:15:57.601358 codeflash-0.6.5/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-30 23:15:57.601485 codeflash-0.6.5/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3143 2024-05-30 23:15:57.601623 codeflash-0.6.5/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0     1083 2024-05-30 23:15:57.601723 codeflash-0.6.5/codeflash/code_utils/github_utils.py
+-rw-r--r--   0        0        0    24003 2024-05-30 23:15:57.601895 codeflash-0.6.5/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.5/codeflash/code_utils/main_calls_bubblesort.py
+-rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.5/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:15:57.601953 codeflash-0.6.5/codeflash/code_utils/sqlalchemy_experiment.py
+-rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.5/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-30 23:15:57.602091 codeflash-0.6.5/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.5/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18481 2024-05-30 23:15:57.602285 codeflash-0.6.5/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20032 2024-05-30 23:15:57.602480 codeflash-0.6.5/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1291 2024-05-30 23:15:57.602653 codeflash-0.6.5/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.5/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-05-29 01:00:54.268195 codeflash-0.6.5/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.5/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.5/codeflash/models/__init__.py
+-rw-r--r--   0        0        0     1218 2024-05-31 20:15:40.283706 codeflash-0.6.5/codeflash/models/models.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.5/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    12006 2024-05-30 23:15:57.602810 codeflash-0.6.5/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    52972 2024-05-31 21:03:09.270371 codeflash-0.6.5/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.5/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-30 23:15:57.603224 codeflash-0.6.5/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1667 2024-05-31 20:15:40.284056 codeflash-0.6.5/codeflash/result/critic.py
+-rw-r--r--   0        0        0     1992 2024-05-30 23:15:57.603526 codeflash-0.6.5/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.5/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.5/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-05-31 21:03:09.270524 codeflash-0.6.5/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-30 23:15:57.603649 codeflash-0.6.5/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-30 23:15:57.603926 codeflash-0.6.5/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-30 23:15:57.604036 codeflash-0.6.5/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-30 23:15:57.604189 codeflash-0.6.5/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.5/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.5/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.5/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.5/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1241 2024-05-30 23:15:57.604500 codeflash-0.6.5/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14621 2024-05-30 23:15:57.604745 codeflash-0.6.5/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6830 2024-05-30 23:15:57.604952 codeflash-0.6.5/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1759 2024-05-30 23:15:57.605103 codeflash-0.6.5/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.5/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4189 2024-05-31 21:03:09.270676 codeflash-0.6.5/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-05-31 21:04:03.043254 codeflash-0.6.5/codeflash/version.py
+-rw-r--r--   0        0        0     2963 2024-05-31 21:04:03.042230 codeflash-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.5/PKG-INFO
```

### Comparing `codeflash-0.6.4/codeflash/LICENSE` & `codeflash-0.6.5/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/api/aiservice.py` & `codeflash-0.6.5/codeflash/api/aiservice.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/api/cfapi.py` & `codeflash-0.6.5/codeflash/api/cfapi.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/cli_cmds/cli.py` & `codeflash-0.6.5/codeflash/cli_cmds/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 )
 from codeflash.code_utils.github_utils import get_github_secrets_page_url, require_github_app_or_exit
 from codeflash.version import __version__ as version
 
 
 def parse_args() -> Namespace:
     parser = ArgumentParser()
-    parser.add_argument("command", nargs="*", help="The command to run (e.g., 'init' or 'init actions')")
+    subparsers = parser.add_subparsers(dest='command', help='Sub-commands')
+
+    init_parser = subparsers.add_parser('init', help='Initialize Codeflash for a Python project.')
+    init_parser.set_defaults(func=init_codeflash)
+
+    init_actions_parser = subparsers.add_parser('init-actions', help='Initialize GitHub Actions workflow')
+    init_actions_parser.set_defaults(func=install_github_actions)
     parser.add_argument("--file", help="Try to optimize only this file")
     parser.add_argument(
         "--function",
         help="Try to optimize only this function within the given file path",
     )
     parser.add_argument(
         "--all",
@@ -73,34 +79,25 @@
     parser.add_argument("-v", "--verbose", action="store_true", help="Print verbose debug logs")
     parser.add_argument("--version", action="store_true", help="Print the version of codeflash")
     args: Namespace = parser.parse_args()
     return process_cmd_args(args)
 
 
 def process_cmd_args(args: Namespace) -> Namespace:
-    is_init: bool = "command" in args and args.command and args.command[0] == "init"
+    is_init: bool = args.command.startswith("init") if args.command else False
     if args.verbose:
         logging_config.set_level(logging.DEBUG, echo_setting=not is_init)
     else:
         logging_config.set_level(logging.INFO, echo_setting=not is_init)
     if args.version:
         logging.info(f"Codeflash version {version}")
         sys.exit()
-
-    if is_init:
-        if args.command == ["init"]:
-            init_codeflash()
-            sys.exit()
-        if args.command == ["init", "actions"]:
-            install_github_actions()
-            sys.exit()
-        else:
-            logging.error(f"Command `{' '.join(args.command)}` not recognized")
-            sys.exit(1)
-
+    if args.command:
+        args.func()
+        sys.exit(1)
     if args.function and not args.file:
         logging.error("If you specify a --function, you must specify the --file it is in")
         sys.exit(1)
     if args.file:
         if not os.path.exists(args.file):
             logging.error(f"File {args.file} does not exist")
             exit(1)
@@ -117,15 +114,14 @@
         logging.exception(e.args[0])
         sys.exit(1)
     supported_keys = [
         "module_root",
         "tests_root",
         "test_framework",
         "ignore_paths",
-        "minimum_performance_gain",
         "pytest_cmd",
         "formatter_cmd",
         "disable_telemetry",
         "imports_sort_cmd",
     ]
     for key in supported_keys:
         if key in pyproject_config:
```

### Comparing `codeflash-0.6.4/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.5/codeflash/cli_cmds/cmd_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ast
-import logging
 import os
 import re
 import subprocess
 import sys
 import time
 from typing import Optional
 
@@ -121,15 +120,15 @@
     ]
     valid_subdirs = [
         d
         for d in next(os.walk("."))[1]
         if not d.startswith(".") and not d.startswith("__") and d not in ignore_subdirs
     ]
 
-    valid_module_subdirs = [dir for dir in valid_subdirs if dir != "tests"]
+    valid_module_subdirs = [d for d in valid_subdirs if d != "tests"]
 
     curdir_option = "current directory (" + curdir + ")"
     module_subdir_options = valid_module_subdirs + [curdir_option]
 
     module_root_answer = inquirer.list_input(
         message="Which Python module do you want me to optimize going forward? (Usually the top-most directory with all of your Python source code)",
         choices=module_subdir_options,
@@ -137,15 +136,17 @@
     )
     module_root = "." if module_root_answer == curdir_option else module_root_answer
     ph("cli-project-root-provided")
 
     # Discover test directory
     default_tests_subdir = "tests"
     create_for_me_option = f"okay, create a tests{os.pathsep} directory for me!"
-    test_subdir_options = valid_subdirs if len(valid_subdirs) > 0 else [create_for_me_option]
+    test_subdir_options = valid_subdirs
+    if "tests" not in valid_subdirs:
+        test_subdir_options.append(create_for_me_option)
     custom_dir_option = "enter a custom directory..."
     test_subdir_options.append(custom_dir_option)
     tests_root_answer = inquirer.list_input(
         message="Where are your tests located? "
         f"(If you don't have any tests yet, I can create an empty tests{os.pathsep} directory for you)",
         choices=test_subdir_options,
         default=(
@@ -345,23 +346,19 @@
             {"confirm_creation": confirm_creation_yes},
         )
         if not confirm_creation_yes:
             click.echo("⏩️ Exiting workflow creation.")
             ph("cli-github-workflow-skipped")
             apologize_and_exit()
         os.makedirs(workflows_path, exist_ok=True)
-        from importlib.resources import read_text
-
+        from importlib.resources import files
         py_version = sys.version_info
         python_version_string = f" {py_version.major}.{py_version.minor}"
-
-        optimize_yml_content = read_text(
-            "codeflash.cli_cmds.workflows",
-            "codeflash-optimize.yaml",
-        )
+        optimize_yml_content = files("codeflash").joinpath(
+            "cli_cmds", "workflows", "codeflash-optimize.yaml").read_text(encoding='utf-8')
         optimize_yml_content = optimize_yml_content.replace(
             " {{ python_version }}",
             python_version_string,
         )
         with open(optimize_yaml_path, "w", encoding="utf8") as optimize_yml_file:
             optimize_yml_file.write(optimize_yml_content)
         click.echo(f"✅ Created {optimize_yaml_path}{LF}")
```

### Comparing `codeflash-0.6.4/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.5/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/code_extractor.py` & `codeflash-0.6.5/codeflash/code_utils/code_extractor.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.5/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/code_utils.py` & `codeflash-0.6.5/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/config_parser.py` & `codeflash-0.6.5/codeflash/code_utils/config_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 
 import tomlkit
 
-from codeflash.code_utils.config_consts import MIN_IMPROVEMENT_THRESHOLD
-
 
 def find_pyproject_toml(config_file=None):
     # Find the pyproject.toml file on the root of the project
 
     if config_file is not None:
         if not config_file.lower().endswith(".toml"):
             raise ValueError(
@@ -53,32 +51,23 @@
             f"Please run 'codeflash init' to create the config file.",
         )
     assert isinstance(config, dict)
 
     # default values:
     path_keys = ["module-root", "tests-root"]
     path_list_keys = ["ignore-paths"]
-    # TODO: minimum-peformance-gain should become a more dynamic auto-detection in the future
-    float_keys = {
-        "minimum-performance-gain": MIN_IMPROVEMENT_THRESHOLD,
-    }  # the value is the default value
     str_keys = {
         "pytest-cmd": "pytest",
         "formatter-cmd": "black",
         "imports-sort-cmd": "isort",
     }
     bool_keys = {
         "disable-telemetry": False,
     }
 
-    for key in float_keys:
-        if key in config:
-            config[key] = float(config[key])
-        else:
-            config[key] = float_keys[key]
     for key in str_keys:
         if key in config:
             config[key] = str(config[key])
         else:
             config[key] = str_keys[key]
     for key in bool_keys:
         if key in config:
```

### Comparing `codeflash-0.6.4/codeflash/code_utils/env_utils.py` & `codeflash-0.6.5/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/formatter.py` & `codeflash-0.6.5/codeflash/code_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/git_utils.py` & `codeflash-0.6.5/codeflash/code_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/github_utils.py` & `codeflash-0.6.5/codeflash/code_utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.5/codeflash/code_utils/instrument_existing_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.5/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.5/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/code_utils/time_utils.py` & `codeflash-0.6.5/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.5/codeflash/discovery/discover_unit_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.6.5/codeflash/discovery/functions_to_optimize.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/github/PrComment.py` & `codeflash-0.6.5/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/main.py` & `codeflash-0.6.5/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/optimization/function_context.py` & `codeflash-0.6.5/codeflash/optimization/function_context.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/optimization/optimizer.py` & `codeflash-0.6.5/codeflash/optimization/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import logging
 import os
 import pathlib
 import sys
 import uuid
 from argparse import Namespace
 from collections import defaultdict
-from typing import Optional
 
 import isort
 import libcst as cst
-from pydantic import BaseModel
 from returns.pipeline import is_successful
 from returns.result import Failure, Result, Success
 
 from codeflash.api.aiservice import (
     AiServiceClient,
     LocalAiServiceClient,
     OptimizedCandidate,
@@ -48,68 +46,40 @@
 )
 from codeflash.discovery.functions_to_optimize import (
     FunctionParent,
     FunctionToOptimize,
     get_functions_to_optimize,
 )
 from codeflash.models.ExperimentMetadata import ExperimentMetadata
+from codeflash.models.models import (
+    BestOptimization,
+    CodeOptimizationContext,
+    GeneratedTests,
+    OptimizationSet,
+    OptimizedCandidateResult,
+    OriginalCodeBaseline,
+)
 from codeflash.optimization.function_context import (
     Source,
     get_constrained_function_context_and_helper_functions,
 )
 from codeflash.result.create_pr import check_create_pr, existing_tests_source_for
+from codeflash.result.critic import speedup_critic
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
 from codeflash.telemetry.posthog import ph
 from codeflash.telemetry.sentry import init_sentry
 from codeflash.verification.equivalence import compare_test_results
 from codeflash.verification.parse_test_output import parse_test_results
 from codeflash.verification.test_results import TestResults, TestType
 from codeflash.verification.test_runner import run_tests
 from codeflash.verification.verification_utils import TestConfig, get_test_file_path
 from codeflash.verification.verifier import generate_tests
 
 
-class OptimizationSet(BaseModel):
-    control: list[OptimizedCandidate]
-    experiment: Optional[list[OptimizedCandidate]]
-
-
-class OptimizedCandidateResult(BaseModel):
-    times_run: int
-    best_test_runtime: int
-    best_test_results: TestResults
-
-
-class OriginalCodeBaseline(BaseModel):
-    generated_test_results: TestResults
-    existing_test_results: TestResults
-    overall_test_results: Optional[TestResults]
-    runtime: int
-
-
-class GeneratedTests(BaseModel):
-    generated_original_test_source: str
-    instrumented_test_source: str
-
-
-class BestOptimization(BaseModel):
-    candidate: OptimizedCandidate
-    helper_functions: list[tuple[Source, str, str]]
-    runtime: int
-    winning_test_results: TestResults
-
-
-class CodeOptimizationContext(BaseModel):
-    code_to_optimize_with_helpers: str
-    contextual_dunder_methods: set[tuple[str, str]]
-    helper_functions: list[tuple[Source, str, str]]
-    preexisting_functions: list[str]
-
-
 class Optimizer:
     def __init__(self, args: Namespace) -> None:
         self.args = args
         init_sentry(not args.disable_telemetry)
         posthog.initialize_posthog(not args.disable_telemetry)
 
         self.test_cfg = TestConfig(
@@ -497,40 +467,29 @@
                 candidate_result: OptimizedCandidateResult = run_results.unwrap()
                 best_test_runtime = candidate_result.best_test_runtime
                 optimized_runtimes[candidate.optimization_id] = best_test_runtime
                 is_correct[candidate.optimization_id] = True
                 speedup_ratios[candidate.optimization_id] = (
                     original_code_baseline.runtime - best_test_runtime
                 ) / best_test_runtime
-
                 logging.info(
                     f"Candidate runtime measured over {candidate_result.times_run} run{'s' if candidate_result.times_run > 1 else ''}: "
                     f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
                     f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime):.3f}",
                 )
-                if (
-                    ((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)
-                    > self.args.minimum_performance_gain
-                ) and best_test_runtime < best_runtime_until_now:
-                    logging.info(
-                        "This candidate is better than the previous best candidate.",
-                    )
 
-                    logging.info(
-                        f"Original runtime: {humanize_runtime(original_code_baseline.runtime)} Best test runtime: "
-                        f"{humanize_runtime(best_test_runtime)}, ratio = "
-                        f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)}",
-                    )
+                if speedup_critic(candidate_result, original_code_baseline.runtime, best_runtime_until_now):
                     best_optimization = BestOptimization(
                         candidate=candidate,
                         helper_functions=code_context.helper_functions,
                         runtime=best_test_runtime,
                         winning_test_results=candidate_result.best_test_results,
                     )
                     best_runtime_until_now = best_test_runtime
+
             self.write_code_and_helpers(
                 original_code,
                 original_helper_code,
                 function_to_optimize.file_path,
                 helper_functions_by_module_abspath,
             )
             logging.info("----------------")
```

### Comparing `codeflash-0.6.4/codeflash/result/create_pr.py` & `codeflash-0.6.5/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/result/explanation.py` & `codeflash-0.6.5/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/telemetry/posthog.py` & `codeflash-0.6.5/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/telemetry/sentry.py` & `codeflash-0.6.5/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/tracer.py` & `codeflash-0.6.5/codeflash/tracer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/tracing/profile_stats.py` & `codeflash-0.6.5/codeflash/tracing/profile_stats.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/tracing/replay_test.py` & `codeflash-0.6.5/codeflash/tracing/replay_test.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/update_license_version.py` & `codeflash-0.6.5/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/comparator.py` & `codeflash-0.6.5/codeflash/verification/comparator.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/equivalence.py` & `codeflash-0.6.5/codeflash/verification/equivalence.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/parse_test_output.py` & `codeflash-0.6.5/codeflash/verification/parse_test_output.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/test_results.py` & `codeflash-0.6.5/codeflash/verification/test_results.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/test_runner.py` & `codeflash-0.6.5/codeflash/verification/test_runner.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/verification_utils.py` & `codeflash-0.6.5/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/codeflash/verification/verifier.py` & `codeflash-0.6.5/codeflash/verification/verifier.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.4/pyproject.toml` & `codeflash-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.6.4" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.5" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
```

### Comparing `codeflash-0.6.4/PKG-INFO` & `codeflash-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.6.4
+Version: 0.6.5
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
```

