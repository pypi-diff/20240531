# Comparing `tmp/experimaestro-1.5.6.tar.gz` & `tmp/experimaestro-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimaestro-1.5.6.tar", max compression
+gzip compressed data, was "experimaestro-1.5.7.tar", max compression
```

## Comparing `experimaestro-1.5.6.tar` & `experimaestro-1.5.7.tar`

### file list

```diff
@@ -1,146 +1,148 @@
--rw-r--r--   0        0        0    35149 2024-05-10 08:06:03.132675 experimaestro-1.5.6/LICENSE
--rw-r--r--   0        0        0     4047 2024-05-10 08:06:03.132675 experimaestro-1.5.6/README.md
--rw-r--r--   0        0        0     3540 2024-05-10 08:06:31.884682 experimaestro-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     1501 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/__init__.py
--rw-r--r--   0        0        0    13528 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/__main__.py
--rw-r--r--   0        0        0     8450 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/annotations.py
--rw-r--r--   0        0        0      696 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/checkers.py
--rw-r--r--   0        0        0     1377 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/click.py
--rw-r--r--   0        0        0     9463 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/commandline.py
--rw-r--r--   0        0        0      171 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/compat.py
--rw-r--r--   0        0        0     5461 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/connectors/__init__.py
--rw-r--r--   0        0        0     5816 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/connectors/local.py
--rw-r--r--   0        0        0     8290 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/connectors/ssh.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/core/__init__.py
--rw-r--r--   0        0        0     5620 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/core/arguments.py
--rw-r--r--   0        0        0     2638 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/core/context.py
--rw-r--r--   0        0        0    63989 2024-05-10 08:06:03.140674 experimaestro-1.5.6/src/experimaestro/core/objects.py
--rw-r--r--   0        0        0     7131 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/core/objects.pyi
--rw-r--r--   0        0        0     3836 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/core/serialization.py
--rw-r--r--   0        0        0     1197 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/core/serializers.py
--rw-r--r--   0        0        0    20176 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/core/types.py
--rw-r--r--   0        0        0      495 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/core/utils.py
--rw-r--r--   0        0        0       44 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/exceptions.py
--rw-r--r--   0        0        0      159 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/experiments/__init__.py
--rw-r--r--   0        0        0     7916 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/experiments/cli.py
--rw-r--r--   0        0        0     1150 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/experiments/configuration.py
--rw-r--r--   0        0        0     5794 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/filter.py
--rw-r--r--   0        0        0     1230 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/generators.py
--rw-r--r--   0        0        0     2956 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/huggingface.py
--rw-r--r--   0        0        0     1490 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/ipc.py
--rw-r--r--   0        0        0      294 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launcherfinder/__init__.py
--rw-r--r--   0        0        0     1020 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launcherfinder/base.py
--rw-r--r--   0        0        0     2279 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launcherfinder/parser.py
--rw-r--r--   0        0        0     8925 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launcherfinder/registry.py
--rw-r--r--   0        0        0     6448 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launcherfinder/specs.py
--rw-r--r--   0        0        0     2525 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/__init__.py
--rw-r--r--   0        0        0     1967 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/direct.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/oar.py
--rw-r--r--   0        0        0       41 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/slurm/__init__.py
--rw-r--r--   0        0        0    14135 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/slurm/base.py
--rw-r--r--   0        0        0      818 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/slurm/cli.py
--rw-r--r--   0        0        0    19357 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/launchers/slurm/configuration.py
--rw-r--r--   0        0        0     1477 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/locking.py
--rw-r--r--   0        0        0       34 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mkdocs/__init__.py
--rw-r--r--   0        0        0      263 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mkdocs/annotations.py
--rw-r--r--   0        0        0    16716 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mkdocs/base.py
--rw-r--r--   0        0        0     1481 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mkdocs/metaloader.py
--rw-r--r--   0        0        0       66 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mkdocs/style.css
--rw-r--r--   0        0        0      285 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/mypy.py
--rw-r--r--   0        0        0     8710 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/notifications.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/py.typed
--rw-r--r--   0        0        0     3605 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/rpyc.py
--rw-r--r--   0        0        0     5294 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/run.py
--rw-r--r--   0        0        0       20 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scheduler/__init__.py
--rw-r--r--   0        0        0    32120 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scheduler/base.py
--rw-r--r--   0        0        0     1994 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scheduler/dependencies.py
--rw-r--r--   0        0        0     2189 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scheduler/services.py
--rw-r--r--   0        0        0     2280 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scheduler/workspace.py
--rw-r--r--   0        0        0     4533 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/scriptbuilder.py
--rw-r--r--   0        0        0    10854 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/server/__init__.py
--rw-r--r--   0        0        0   189684 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf
--rw-r--r--   0        0        0   128352 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
--rw-r--r--   0        0        0   135984 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
--rw-r--r--   0        0        0   156236 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
--rw-r--r--   0        0        0   339600 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
--rw-r--r--   0        0        0   164912 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
--rw-r--r--   0        0        0   215704 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
--rw-r--r--   0        0        0    63348 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/50701fbb8177c2dde530.ttf
--rw-r--r--   0        0        0   206260 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/5d681e2edae8c60630db.woff
--rw-r--r--   0        0        0   155276 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
--rw-r--r--   0        0        0   109808 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/878f31251d960bd6266f.woff2
--rw-r--r--   0        0        0    24488 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2
--rw-r--r--   0        0        0   150020 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2
--rw-r--r--   0        0        0   173620 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
--rw-r--r--   0        0        0   394668 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf
--rw-r--r--   0        0        0   182028 2024-05-10 08:06:30.868682 experimaestro-1.5.6/src/experimaestro/server/data/f882956fd323fd322f31.woff
--rw-r--r--   0        0        0     3870 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/favicon.ico
--rw-r--r--   0        0        0   418843 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/index.css
--rw-r--r--   0        0        0   576970 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/index.css.map
--rw-r--r--   0        0        0      706 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/index.html
--rw-r--r--   0        0        0  3734128 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/index.js
--rw-r--r--   0        0        0  3904832 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/index.js.map
--rw-r--r--   0        0        0      511 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/login.html
--rw-r--r--   0        0        0      318 2024-05-10 08:06:30.900681 experimaestro-1.5.6/src/experimaestro/server/data/manifest.json
--rw-r--r--   0        0        0     2181 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/settings.py
--rw-r--r--   0        0        0     9560 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/sphinx/__init__.py
--rw-r--r--   0        0        0      294 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/sphinx/static/experimaestro.css
--rw-r--r--   0        0        0      499 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/taskglobals.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/__init__.py
--rw-r--r--   0        0        0      695 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/conftest.py
--rw-r--r--   0        0        0       21 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/connectors/bin/executable.py
--rw-r--r--   0        0        0     1204 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/connectors/test_local.py
--rw-r--r--   0        0        0      702 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/connectors/utils.py
--rw-r--r--   0        0        0      414 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/definitions_types.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/__init__.py
--rwxr-xr-x   0        0        0      639 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/bin/sacct
--rwxr-xr-x   0        0        0     1177 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/bin/sbatch
--rw-r--r--   0        0        0      477 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/bin/test.py
--rw-r--r--   0        0        0     2468 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/common.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/config_slurm/__init__.py
--rw-r--r--   0        0        0     2497 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
--rw-r--r--   0        0        0      717 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/test_local.py
--rw-r--r--   0        0        0     2534 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/launchers/test_slurm.py
--rw-r--r--   0        0        0     4016 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/restart.py
--rw-r--r--   0        0        0      295 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/restart_main.py
--rw-r--r--   0        0        0      407 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/scripts/notifyandwait.py
--rw-r--r--   0        0        0      120 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/scripts/waitforfile.py
--rw-r--r--   0        0        0      477 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/task_tokens.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/tasks/all.py
--rw-r--r--   0        0        0      153 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/tasks/foreign.py
--rw-r--r--   0        0        0      403 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_checkers.py
--rw-r--r--   0        0        0     2005 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_dependencies.py
--rw-r--r--   0        0        0     2967 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_findlauncher.py
--rw-r--r--   0        0        0      780 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_forward.py
--rw-r--r--   0        0        0    13397 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_identifier.py
--rw-r--r--   0        0        0     1540 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_instance.py
--rw-r--r--   0        0        0     2037 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_objects.py
--rw-r--r--   0        0        0      781 2024-05-10 08:06:03.144674 experimaestro-1.5.6/src/experimaestro/tests/test_outputs.py
--rw-r--r--   0        0        0     6405 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_param.py
--rw-r--r--   0        0        0     7580 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_progress.py
--rw-r--r--   0        0        0     2338 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_serializers.py
--rw-r--r--   0        0        0     3081 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_snippets.py
--rw-r--r--   0        0        0      979 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_ssh.py
--rw-r--r--   0        0        0     1975 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_tags.py
--rw-r--r--   0        0        0     9429 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_tasks.py
--rw-r--r--   0        0        0     7826 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_tokens.py
--rw-r--r--   0        0        0     1257 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_types.py
--rw-r--r--   0        0        0     4339 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/test_validation.py
--rw-r--r--   0        0        0     1701 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/token_reschedule.py
--rw-r--r--   0        0        0     3805 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tests/utils.py
--rw-r--r--   0        0        0    14681 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tokens.py
--rw-r--r--   0        0        0        0 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tools/__init__.py
--rw-r--r--   0        0        0     3436 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tools/diff.py
--rw-r--r--   0        0        0     9184 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tools/documentation.py
--rw-r--r--   0        0        0     3516 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/tools/jobs.py
--rw-r--r--   0        0        0     3334 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/typingutils.py
--rw-r--r--   0        0        0     2434 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/__init__.py
--rw-r--r--   0        0        0      601 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/asyncio.py
--rw-r--r--   0        0        0     2394 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/jobs.py
--rw-r--r--   0        0        0     2183 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/jupyter.py
--rw-r--r--   0        0        0     1006 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/resources.py
--rw-r--r--   0        0        0      793 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/settings.py
--rw-r--r--   0        0        0     6766 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/utils/yaml.py
--rw-r--r--   0        0        0      638 2024-05-10 08:06:03.148675 experimaestro-1.5.6/src/experimaestro/xpmutils.py
--rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 experimaestro-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-31 15:24:58.194144 experimaestro-1.5.7/LICENSE
+-rw-r--r--   0        0        0     4047 2024-05-31 15:24:58.194144 experimaestro-1.5.7/README.md
+-rw-r--r--   0        0        0     3540 2024-05-31 15:25:28.250863 experimaestro-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1501 2024-05-31 15:24:58.202144 experimaestro-1.5.7/src/experimaestro/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-31 15:24:58.202144 experimaestro-1.5.7/src/experimaestro/__main__.py
+-rw-r--r--   0        0        0     8450 2024-05-31 15:24:58.202144 experimaestro-1.5.7/src/experimaestro/annotations.py
+-rw-r--r--   0        0        0      696 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/checkers.py
+-rw-r--r--   0        0        0     9610 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/cli/__init__.py
+-rw-r--r--   0        0        0     5790 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/cli/filter.py
+-rw-r--r--   0        0        0     7319 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/cli/jobs.py
+-rw-r--r--   0        0        0     1377 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/click.py
+-rw-r--r--   0        0        0     9463 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/commandline.py
+-rw-r--r--   0        0        0      171 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/compat.py
+-rw-r--r--   0        0        0     5461 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/connectors/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/connectors/local.py
+-rw-r--r--   0        0        0     8290 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/connectors/ssh.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/__init__.py
+-rw-r--r--   0        0        0     5620 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/arguments.py
+-rw-r--r--   0        0        0     2638 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/context.py
+-rw-r--r--   0        0        0    64142 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/objects.py
+-rw-r--r--   0        0        0     7131 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/objects.pyi
+-rw-r--r--   0        0        0     3836 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/serialization.py
+-rw-r--r--   0        0        0     1197 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/serializers.py
+-rw-r--r--   0        0        0    20176 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/types.py
+-rw-r--r--   0        0        0      495 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/core/utils.py
+-rw-r--r--   0        0        0       44 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/exceptions.py
+-rw-r--r--   0        0        0      159 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/experiments/__init__.py
+-rw-r--r--   0        0        0     7254 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/experiments/cli.py
+-rw-r--r--   0        0        0     1150 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/experiments/configuration.py
+-rw-r--r--   0        0        0     1230 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/generators.py
+-rw-r--r--   0        0        0     2956 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/huggingface.py
+-rw-r--r--   0        0        0     1490 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/ipc.py
+-rw-r--r--   0        0        0      294 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launcherfinder/__init__.py
+-rw-r--r--   0        0        0     1020 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launcherfinder/base.py
+-rw-r--r--   0        0        0     2279 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launcherfinder/parser.py
+-rw-r--r--   0        0        0     8925 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launcherfinder/registry.py
+-rw-r--r--   0        0        0     6448 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launcherfinder/specs.py
+-rw-r--r--   0        0        0     2525 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/__init__.py
+-rw-r--r--   0        0        0     1967 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/direct.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/oar.py
+-rw-r--r--   0        0        0       41 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/slurm/__init__.py
+-rw-r--r--   0        0        0    14185 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/slurm/base.py
+-rw-r--r--   0        0        0      818 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/slurm/cli.py
+-rw-r--r--   0        0        0    19357 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/launchers/slurm/configuration.py
+-rw-r--r--   0        0        0     1477 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/locking.py
+-rw-r--r--   0        0        0       34 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mkdocs/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mkdocs/annotations.py
+-rw-r--r--   0        0        0    16716 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mkdocs/base.py
+-rw-r--r--   0        0        0     1481 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mkdocs/metaloader.py
+-rw-r--r--   0        0        0       66 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mkdocs/style.css
+-rw-r--r--   0        0        0      285 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/mypy.py
+-rw-r--r--   0        0        0     9257 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/notifications.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/py.typed
+-rw-r--r--   0        0        0     3605 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/rpyc.py
+-rw-r--r--   0        0        0     5222 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/run.py
+-rw-r--r--   0        0        0       20 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scheduler/__init__.py
+-rw-r--r--   0        0        0    31941 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scheduler/base.py
+-rw-r--r--   0        0        0     1994 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scheduler/dependencies.py
+-rw-r--r--   0        0        0     2189 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scheduler/services.py
+-rw-r--r--   0        0        0     2280 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scheduler/workspace.py
+-rw-r--r--   0        0        0     4533 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/scriptbuilder.py
+-rw-r--r--   0        0        0    10854 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/server/__init__.py
+-rw-r--r--   0        0        0   189684 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf
+-rw-r--r--   0        0        0   128352 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
+-rw-r--r--   0        0        0   135984 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
+-rw-r--r--   0        0        0   156236 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
+-rw-r--r--   0        0        0   339600 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
+-rw-r--r--   0        0        0   164912 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
+-rw-r--r--   0        0        0   215704 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
+-rw-r--r--   0        0        0    63348 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/50701fbb8177c2dde530.ttf
+-rw-r--r--   0        0        0   206260 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/5d681e2edae8c60630db.woff
+-rw-r--r--   0        0        0   155276 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
+-rw-r--r--   0        0        0   109808 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/878f31251d960bd6266f.woff2
+-rw-r--r--   0        0        0    24488 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2
+-rw-r--r--   0        0        0   150020 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2
+-rw-r--r--   0        0        0   173620 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
+-rw-r--r--   0        0        0   394668 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf
+-rw-r--r--   0        0        0   182028 2024-05-31 15:25:27.150838 experimaestro-1.5.7/src/experimaestro/server/data/f882956fd323fd322f31.woff
+-rw-r--r--   0        0        0     3870 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/favicon.ico
+-rw-r--r--   0        0        0   418843 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/index.css
+-rw-r--r--   0        0        0   576970 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/index.css.map
+-rw-r--r--   0        0        0      706 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/index.html
+-rw-r--r--   0        0        0  3734128 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/index.js
+-rw-r--r--   0        0        0  3904832 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/index.js.map
+-rw-r--r--   0        0        0      511 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/login.html
+-rw-r--r--   0        0        0      318 2024-05-31 15:25:27.186838 experimaestro-1.5.7/src/experimaestro/server/data/manifest.json
+-rw-r--r--   0        0        0     3145 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/settings.py
+-rw-r--r--   0        0        0     9560 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/sphinx/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/sphinx/static/experimaestro.css
+-rw-r--r--   0        0        0      499 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/taskglobals.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/conftest.py
+-rw-r--r--   0        0        0       21 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/connectors/bin/executable.py
+-rw-r--r--   0        0        0     1204 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/connectors/test_local.py
+-rw-r--r--   0        0        0      702 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/connectors/utils.py
+-rw-r--r--   0        0        0      414 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/definitions_types.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/launchers/__init__.py
+-rwxr-xr-x   0        0        0      639 2024-05-31 15:24:58.206144 experimaestro-1.5.7/src/experimaestro/tests/launchers/bin/sacct
+-rwxr-xr-x   0        0        0     1177 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/bin/sbatch
+-rw-r--r--   0        0        0      477 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/bin/test.py
+-rw-r--r--   0        0        0     2468 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/common.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/config_slurm/__init__.py
+-rw-r--r--   0        0        0     2497 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
+-rw-r--r--   0        0        0      717 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/test_local.py
+-rw-r--r--   0        0        0     2534 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/launchers/test_slurm.py
+-rw-r--r--   0        0        0     4016 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/restart.py
+-rw-r--r--   0        0        0      295 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/restart_main.py
+-rw-r--r--   0        0        0      407 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/scripts/notifyandwait.py
+-rw-r--r--   0        0        0      120 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/scripts/waitforfile.py
+-rw-r--r--   0        0        0      477 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/task_tokens.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/tasks/all.py
+-rw-r--r--   0        0        0      153 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/tasks/foreign.py
+-rw-r--r--   0        0        0      403 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_checkers.py
+-rw-r--r--   0        0        0     2005 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2967 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_findlauncher.py
+-rw-r--r--   0        0        0      780 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_forward.py
+-rw-r--r--   0        0        0    13397 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_identifier.py
+-rw-r--r--   0        0        0     1540 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_instance.py
+-rw-r--r--   0        0        0     2037 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_objects.py
+-rw-r--r--   0        0        0      781 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_outputs.py
+-rw-r--r--   0        0        0     6405 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_param.py
+-rw-r--r--   0        0        0     7580 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_progress.py
+-rw-r--r--   0        0        0     2338 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_serializers.py
+-rw-r--r--   0        0        0     3081 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_snippets.py
+-rw-r--r--   0        0        0      979 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_ssh.py
+-rw-r--r--   0        0        0     2921 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_tags.py
+-rw-r--r--   0        0        0     9429 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_tasks.py
+-rw-r--r--   0        0        0     7826 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_tokens.py
+-rw-r--r--   0        0        0     1257 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_types.py
+-rw-r--r--   0        0        0     4339 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/test_validation.py
+-rw-r--r--   0        0        0     1701 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/token_reschedule.py
+-rw-r--r--   0        0        0     3805 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tests/utils.py
+-rw-r--r--   0        0        0    14681 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tools/__init__.py
+-rw-r--r--   0        0        0     3436 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tools/diff.py
+-rw-r--r--   0        0        0     9184 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tools/documentation.py
+-rw-r--r--   0        0        0     3516 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/tools/jobs.py
+-rw-r--r--   0        0        0     3334 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/typingutils.py
+-rw-r--r--   0        0        0     2434 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/asyncio.py
+-rw-r--r--   0        0        0     2394 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/jobs.py
+-rw-r--r--   0        0        0     2183 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/jupyter.py
+-rw-r--r--   0        0        0     1006 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/resources.py
+-rw-r--r--   0        0        0      793 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/settings.py
+-rw-r--r--   0        0        0     6766 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/utils/yaml.py
+-rw-r--r--   0        0        0      638 2024-05-31 15:24:58.210144 experimaestro-1.5.7/src/experimaestro/xpmutils.py
+-rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 experimaestro-1.5.7/PKG-INFO
```

### Comparing `experimaestro-1.5.6/LICENSE` & `experimaestro-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/README.md` & `experimaestro-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/pyproject.toml` & `experimaestro-1.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "src/experimaestro/server/data/*",
     "src/experimaestro/sphinx/static/experimaestro.css",
     "src/experimaestro/mkdocs/style.css"
 ]
-version = "1.5.6"
+version = "1.5.7"
 repository = "https://github.com/experimaestro/experimaestro-python"
 documentation = "https://experimaestro-python.readthedocs.io/"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
@@ -119,11 +119,11 @@
 
 [tool.mypy]
 python_version = "3.9"
 warn_unused_ignores = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.5.6"
+version = "1.5.7"
 changelog_start_rev = "0.15.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
```

### Comparing `experimaestro-1.5.6/src/experimaestro/__init__.py` & `experimaestro-1.5.7/src/experimaestro/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/__main__.py` & `experimaestro-1.5.7/src/experimaestro/cli/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # flake8: noqa: T201
 import sys
-from types import ModuleType
 from typing import Set, Optional
 import pkg_resources
 from itertools import chain
 from shutil import rmtree
 import click
 import logging
 from functools import cached_property, update_wrapper
 from pathlib import Path
 import subprocess
-from termcolor import colored, cprint
+from termcolor import cprint
 
 import experimaestro
 from experimaestro.experiments.cli import experiments_cli
 import experimaestro.launcherfinder.registry as launcher_registry
+from experimaestro.settings import find_workspace
 
 # --- Command line main options
 logging.basicConfig(level=logging.INFO)
 
 
 def pass_cfg(f):
     """Pass configuration information"""
@@ -171,129 +171,14 @@
         elif isinstance(value, dict):
             for key, dict_value in value.items():
                 check(f"{path}.{key}", dict_value, new_value[key], done)
 
     check(".", job, new_job, set())
 
 
-@click.argument("path", type=Path, callback=check_xp_path)
-@click.option("--experiment", default=None, help="Restrict to this experiment")
-@click.option("--tags", is_flag=True, help="Show tags")
-@click.option("--ready", is_flag=True, help="Include tasks which are not yet scheduled")
-@click.option("--filter", default="", help="Filter expression")
-@click.option(
-    "--force",
-    is_flag=True,
-    help="Force operation even if experiment has not been completed yet",
-)
-@click.option("--kill", is_flag=True, help="Kill filtered tasks (when/before running)")
-@click.option("--clean", is_flag=True, help="Remove finished tasks directories")
-@cli.command()
-def jobs(
-    path: Path,
-    experiment: str,
-    filter: str,
-    tags: bool,
-    ready: bool,
-    kill: bool,
-    clean: bool,
-    force: bool,
-):
-    """Job control: list, kill and clean
-
-    The job filter is a boolean expression where tags (alphanumeric)
-    and special job information (@state for job state, @name for job full
-    name) can be compared to a given value (using '~' for regex matching,
-    '=', 'not in', or 'in')
-
-    For instance,
-
-    model = "bm25" and mode in ["a", b"] and @state = "RUNNING"
-
-    selects jobs where the tag model is "bm25", the tag mode is either
-    "a" or "b", and the state is running.
-
-    """
-    for p in (path / "xp").glob("*"):
-        if experiment and p.name != experiment:
-            continue
-
-        from .filter import createFilter, JobInformation
-        from experimaestro.scheduler import JobState
-
-        _filter = createFilter(filter) if filter else lambda x: True
-
-        print(f"* Experiment {p.name}")
-        if (p / "jobs.bak").is_dir():
-            cprint("  Experiment has not finished yet", "red")
-            if not force and (kill or clean):
-                cprint("  Preventing kill/clean (use --force if you want to)", "yellow")
-                kill = False
-                clean = False
-        print()
-
-        for job in p.glob("jobs/*/*"):
-            info = None
-            p = job.resolve()
-            if p.is_dir():
-                *_, scriptname = p.parent.name.rsplit(".", 1)
-
-                info = JobInformation(p, scriptname)
-                if filter:
-                    if not _filter(info):
-                        continue
-
-                if info.state is None:
-                    print(
-                        colored(f"NODIR   {job.parent.name}/{job.name}", "red"), end=""
-                    )
-                elif info.state.running():
-                    if kill:
-                        process = info.getprocess()
-                        print("KILLING", process)
-                        process.kill()
-                    print(
-                        colored(
-                            f"{info.state.name:8}{job.parent.name}/{job.name}", "yellow"
-                        ),
-                        end="",
-                    )
-                elif info.state == JobState.DONE:
-                    print(
-                        colored(f"DONE    {job.parent.name}/{job.name}", "green"),
-                        end="",
-                    )
-                elif info.state == JobState.ERROR:
-                    print(
-                        colored(f"FAIL    {job.parent.name}/{job.name}", "red"), end=""
-                    )
-                else:
-                    print(
-                        colored(
-                            f"{info.state.name:8}{job.parent.name}/{job.name}", "red"
-                        ),
-                        end="",
-                    )
-
-            else:
-                if not ready:
-                    continue
-                print(colored(f"READY {job.parent.name}/{job.name}", "yellow"), end="")
-
-            if tags:
-                print(f""" {" ".join(f"{k}={v}" for k, v in info.tags.items())}""")
-            else:
-                print()
-
-            if clean and info.state and info.state.finished():
-                cprint("Cleaning...", "red")
-                rmtree(p)
-        print()
-
-
 @click.option("--show-all", is_flag=True, help="Show even not orphans")
 @click.option(
     "--ignore-old", is_flag=True, help="Ignore old jobs for unfinished experiments"
 )
 @click.option("--clean", is_flag=True, help="Prune the orphan folders")
 @click.option("--size", is_flag=True, help="Show size of each folder")
 @click.argument("path", type=Path, callback=check_xp_path)
@@ -403,30 +288,25 @@
 
 cli.add_command(Launchers("launchers", help="Launcher specific commands"))
 cli.add_command(Launchers("connectors", help="Connector specific commands"))
 cli.add_command(Launchers("tokens", help="Token specific commands"))
 
 
 @cli.group()
-@click.argument("workdir", type=Path, callback=check_xp_path)
+@click.option("--workdir", type=Path, default=None)
+@click.option("--workspace", type=str, default=None)
 @click.pass_context
-def experiments(ctx, workdir):
+def experiments(ctx, workdir, workspace):
     """Manage experiments"""
-    ctx.obj = workdir
+    ws = find_workspace(workdir=workdir, workspace=workspace)
+    path = check_xp_path(None, None, ws.path)
+    ctx.obj = path
 
 
 @experiments.command()
 @pass_cfg
 def list(workdir: Path):
     for p in (workdir / "xp").iterdir():
         if (p / "jobs.bak").exists():
             cprint(f"[unfinished] {p.name}", "yellow")
         else:
             cprint(p.name, "cyan")
-
-
-def main():
-    cli(obj=None)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `experimaestro-1.5.6/src/experimaestro/annotations.py` & `experimaestro-1.5.7/src/experimaestro/annotations.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/checkers.py` & `experimaestro-1.5.7/src/experimaestro/checkers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/click.py` & `experimaestro-1.5.7/src/experimaestro/click.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/commandline.py` & `experimaestro-1.5.7/src/experimaestro/commandline.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/connectors/__init__.py` & `experimaestro-1.5.7/src/experimaestro/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/connectors/local.py` & `experimaestro-1.5.7/src/experimaestro/connectors/local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/connectors/ssh.py` & `experimaestro-1.5.7/src/experimaestro/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/arguments.py` & `experimaestro-1.5.7/src/experimaestro/core/arguments.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/context.py` & `experimaestro-1.5.7/src/experimaestro/core/context.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/objects.py` & `experimaestro-1.5.7/src/experimaestro/core/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -912,22 +912,22 @@
         if self.job:
             raise Exception("task %s was already submitted" % self)
         if not self.xpmtype.task:
             raise ValueError("%s is not a task" % self.xpmtype)
 
         # --- Submit the job
 
+        # Sets the init tasks
+        self.init_tasks = init_tasks
+
         # Creates a new job
         self.job = self.xpmtype.task(
             self.pyobject, launcher=launcher, workspace=workspace, run_mode=run_mode
         )
 
-        # Sets the init tasks
-        self.init_tasks = init_tasks
-
         # Validate the object
         job_context = JobContext(self.job)
         self.validate_and_seal(job_context)
 
         # --- Workspace
 
         workspace = workspace or (
@@ -975,14 +975,17 @@
             if self.job.workspace is not None:
                 if self.job.donepath.is_file():
                     color = "light_green"
                     cprint(f"[done] {s}", color, file=sys.stderr)
                 elif self.job.failedpath.is_file():
                     color = "light_red"
                     cprint(f"[failed] {s}", color, file=sys.stderr)
+                elif self.job.pidpath.is_file():
+                    color = "blue"
+                    cprint(f"[running] {s}", color, file=sys.stderr)
                 else:
                     color = "light_blue"
                     cprint(f"[not run] {s}", color, file=sys.stderr)
 
                 if launcher:
                     cprint(f"   [Launcher] {launcher}", color, file=sys.stderr)
```

### Comparing `experimaestro-1.5.6/src/experimaestro/core/objects.pyi` & `experimaestro-1.5.7/src/experimaestro/core/objects.pyi`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/serialization.py` & `experimaestro-1.5.7/src/experimaestro/core/serialization.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/serializers.py` & `experimaestro-1.5.7/src/experimaestro/core/serializers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/core/types.py` & `experimaestro-1.5.7/src/experimaestro/core/types.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/experiments/cli.py` & `experimaestro-1.5.7/src/experimaestro/experiments/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import click
 import omegaconf
 import yaml
 from experimaestro import LauncherRegistry, RunMode, experiment
 from experimaestro.experiments.configuration import ConfigurationBase
 from experimaestro.exceptions import HandledException
-from experimaestro.settings import get_workspace
+from experimaestro.settings import find_workspace
 from omegaconf import OmegaConf, SCMode
 from termcolor import cprint
 
 
 class ExperimentHelper:
     """Helper for experiments"""
 
@@ -227,35 +227,16 @@
 
     # Move to an object container
     configuration = OmegaConf.to_container(
         configuration, structured_config_mode=SCMode.INSTANTIATE
     )
 
     # Define the workspace
-    workdir = Path(workdir) if workdir else None
-
-    if workspace:
-        ws_env = get_workspace(workspace)
-        if ws_env is None:
-            raise RuntimeError("No workspace named %s", workspace)
-
-        logging.info("Using workspace %s", ws_env.id)
-        if workdir:
-            # Overrides working directory
-            logging.info(" override working directory: %s", workdir)
-            ws_env.path = workdir
-        else:
-            workdir = ws_env.path
-    elif workdir:
-        logging.info("Using workdir %s", workdir)
-        ws_env = workdir
-    else:
-        ws_env = get_workspace()
-        assert ws_env is not None, "No workdir or workspace defined, and no default"
-        logging.info("Using default workspace %s", ws_env.id)
+    ws_env = find_workspace(workdir=workdir, workspace=workspace)
+    workdir = ws_env.path
 
     logging.info("Using working directory %s", str(workdir.resolve()))
 
     # --- Runs the experiment
     with experiment(
         ws_env, configuration.id, host=host, port=port, run_mode=run_mode
     ) as xp:
```

### Comparing `experimaestro-1.5.6/src/experimaestro/experiments/configuration.py` & `experimaestro-1.5.7/src/experimaestro/experiments/configuration.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/filter.py` & `experimaestro-1.5.7/src/experimaestro/cli/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
     @cached_property
     def tags(self) -> List[str]:
         return self.params["tags"]
 
     @cached_property
     def state(self) -> Optional[JobState]:
-        if (self.path / f"{self.scriptname}.pid").is_file():
-            return JobState.RUNNING
-        elif (self.path / f"{self.scriptname}.done").is_file():
+        if (self.path / f"{self.scriptname}.done").is_file():
             return JobState.DONE
-        elif (self.path / f"{self.scriptname}.failed").is_file():
+        if (self.path / f"{self.scriptname}.failed").is_file():
             return JobState.ERROR
+        if (self.path / f"{self.scriptname}.pid").is_file():
+            return JobState.RUNNING
         else:
             return None
 
     def getprocess(self):
         from experimaestro.connectors import Process
         from experimaestro.connectors.local import LocalConnector
```

### Comparing `experimaestro-1.5.6/src/experimaestro/generators.py` & `experimaestro-1.5.7/src/experimaestro/generators.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/huggingface.py` & `experimaestro-1.5.7/src/experimaestro/huggingface.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/ipc.py` & `experimaestro-1.5.7/src/experimaestro/ipc.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launcherfinder/base.py` & `experimaestro-1.5.7/src/experimaestro/launcherfinder/base.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launcherfinder/parser.py` & `experimaestro-1.5.7/src/experimaestro/launcherfinder/parser.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launcherfinder/registry.py` & `experimaestro-1.5.7/src/experimaestro/launcherfinder/registry.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launcherfinder/specs.py` & `experimaestro-1.5.7/src/experimaestro/launcherfinder/specs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launchers/__init__.py` & `experimaestro-1.5.7/src/experimaestro/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launchers/direct.py` & `experimaestro-1.5.7/src/experimaestro/launchers/direct.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launchers/slurm/base.py` & `experimaestro-1.5.7/src/experimaestro/launchers/slurm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,17 @@
         builder.command.extend(self.launcher.options.args())
 
         addstream(builder.command, "-e", self.stderr)
         addstream(builder.command, "-o", self.stdout)
         addstream(builder.command, "-i", self.stdin)
 
         builder.command.extend(self.command)
-        logger.info("slurm sbatch command: %s", builder.command)
+        logger.info(
+            "slurm sbatch command: %s", " ".join(f'"{s}"' for s in builder.command)
+        )
         handler = OutputCaptureHandler()
         builder.stdout = Redirect.pipe(handler)
         builder.stderr = Redirect.inherit()
         p = builder.start()
         if p.wait() != 0:
             logger.error("Error while running sbatch command")
             raise RuntimeError("Error while submitting job")
```

### Comparing `experimaestro-1.5.6/src/experimaestro/launchers/slurm/cli.py` & `experimaestro-1.5.7/src/experimaestro/launchers/slurm/cli.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/launchers/slurm/configuration.py` & `experimaestro-1.5.7/src/experimaestro/launchers/slurm/configuration.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/locking.py` & `experimaestro-1.5.7/src/experimaestro/locking.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/mkdocs/base.py` & `experimaestro-1.5.7/src/experimaestro/mkdocs/base.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/mkdocs/metaloader.py` & `experimaestro-1.5.7/src/experimaestro/mkdocs/metaloader.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/notifications.py` & `experimaestro-1.5.7/src/experimaestro/notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,20 @@
             result["desc"] = self.desc
         return result
 
     def __repr__(self) -> str:
         return f"[{self.level}] {self.desc} {int(self.progress*1000)/10}%"
 
 
+class ListenerInformation:
+    def __init__(self, url: str):
+        self.url = url
+        self.error_count = 0
+
+
 class Reporter(threading.Thread):
     NOTIFICATION_FOLDER = ".notifications"
 
     console: bool
     """Whether to output to the console if no notification server is up"""
 
     def __init__(self, path: Path):
@@ -55,15 +61,15 @@
 
         Arguments:
             path: The path where notification URLs will be put (one file per URL)
         """
         super().__init__(daemon=True)
         self.path = path / Reporter.NOTIFICATION_FOLDER
         self.path.mkdir(exist_ok=True)
-        self.urls: Dict[str, str] = {}
+        self.urls: Dict[str, ListenerInformation] = {}
 
         # Last check of notification URLs
         self.lastcheck = 0
 
         self.levels = [LevelInformation(0, None, -1)]
 
         self.stopping = False
@@ -76,36 +82,43 @@
 
     def stop(self):
         self.stopping = True
         with self.cv:
             self.cv.notifyAll()
 
     @staticmethod
-    def isfatal_httperror(e: Exception) -> bool:
+    def isfatal_httperror(e: Exception, info: ListenerInformation) -> bool:
         """Returns True if this HTTP error indicates that the server won't recover"""
         if isinstance(e, HTTPError):
             if e.code >= 400 and e.code < 500:
                 return True
         elif isinstance(e, URLError):
             if isinstance(e.reason, ConnectionRefusedError):
                 return True
             if isinstance(e.reason, socket.gaierror) and e.reason.errno == -2:
                 return True
+            if isinstance(e.reason, TimeoutError):
+                info.error_count += 1
+
+            # Too many errors
+            if info.error_count > 3:
+                logger.info("Too many errors with %s", info.error_count)
+                return True
 
         return False
 
     def modified(self):
         return any(level.modified(self) for level in self.levels)
 
     def check_urls(self):
         mtime = os.path.getmtime(self.path)
         if mtime > self.lastcheck:
             for f in self.path.iterdir():
-                self.urls[f.name] = f.read_text().strip()
-                logger.info("Added new notification URL: %s", self.urls[f.name])
+                self.urls[f.name] = ListenerInformation(f.read_text().strip())
+                logger.info("Added new notification URL: %s", self.urls[f.name].url)
                 f.unlink()
 
             self.lastcheck = os.path.getmtime(self.path)
 
     def run(self):
         logger.info("Running notification thread")
 
@@ -124,15 +137,17 @@
             if self.urls:
                 # OK, let's go
                 for level in self.levels:
                     if level.modified(self):
                         params = level.report()
 
                         # Go over all URLs
-                        for key, baseurl in self.urls.items():
+                        for key, info in self.urls.items():
+                            baseurl = info.url
+
                             url = "{}/progress?{}".format(
                                 baseurl, urllib.parse.urlencode(params)
                             )
                             logger.debug("Reporting progress %s", params)
                             try:
                                 with urlopen(url) as _:
                                     logger.debug(
@@ -143,15 +158,15 @@
                             except Exception as e:
                                 logger.warning(
                                     "Progress: %s [error while notifying %s]: %s",
                                     level,
                                     url,
                                     e,
                                 )
-                                if Reporter.isfatal_httperror(e):
+                                if Reporter.isfatal_httperror(e, info):
                                     toremove.append(key)
 
                 # Removes unvalid URLs
                 for key in toremove:
                     logger.info("Removing notification URL %s", self.urls[key])
                     del self.urls[key]
             elif self.console:
@@ -161,15 +176,16 @@
                         logger.info("Progress: %s", level)
 
     def eoj(self):
         with self.cv:
             self.check_urls()
             if self.urls:
                 # Go over all URLs
-                for key, baseurl in self.urls.items():
+                for key, info in self.urls.items():
+                    baseurl = info.url
                     url = "{}?status=eoj".format(baseurl)
                     try:
                         with urlopen(url) as _:
                             logger.debug(
                                 "EOJ botification sent for %s",
                                 baseurl,
                             )
@@ -239,15 +255,15 @@
         self.is_tty = hasattr(_file, "isatty") or _file.isatty()
 
         super().__init__(iterable, disable=False, file=file, *args, **kwargs)
         progress(0.0, level=self.pos, desc=kwargs.get("desc", None), console=False)
 
     def update(self, n=1):
         result = super().update(n)
-        if self.total is not None:
+        if self.total is not None and self.total > 0:
             progress(self.n / self.total, level=self.pos, console=False)
         return result
 
     def refresh(self, nolock=False, lock_args=None):
         if self.is_tty:
             super().refresh(nolock=nolock, lock_args=lock_args)
```

### Comparing `experimaestro-1.5.6/src/experimaestro/rpyc.py` & `experimaestro-1.5.7/src/experimaestro/rpyc.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/run.py` & `experimaestro-1.5.7/src/experimaestro/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,11 +151,10 @@
 
         except SystemExit as e:
             if e.code == 0:
                 # Normal exit, just create the ".done" file
                 self.donepath.touch()
 
                 # ... and finish the exit process
-                logger.info("This is the end (TODO: remove this line)")
                 raise
             else:
                 self.handle_error(e.code, None)
```

### Comparing `experimaestro-1.5.6/src/experimaestro/scheduler/base.py` & `experimaestro-1.5.7/src/experimaestro/scheduler/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,19 +799,14 @@
         self.server = (
             Server(self.scheduler, settings.server)
             if (settings.server.port is not None and settings.server.port >= 0)
             and self.workspace.run_mode == RunMode.NORMAL
             else None
         )
 
-        # Copy environment variable from main (but do not
-        # override)
-        for key, value in settings.env.items():
-            self.setenv(key, value, override=False)
-
         if os.environ.get("XPM_ENABLEFAULTHANDLER", "0") == "1":
             import faulthandler
 
             logger.info("Enabling fault handler")
             faulthandler.enable(all_threads=True)
 
     def submit(self, job: Job):
```

### Comparing `experimaestro-1.5.6/src/experimaestro/scheduler/dependencies.py` & `experimaestro-1.5.7/src/experimaestro/scheduler/dependencies.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/scheduler/services.py` & `experimaestro-1.5.7/src/experimaestro/scheduler/services.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/scheduler/workspace.py` & `experimaestro-1.5.7/src/experimaestro/scheduler/workspace.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/scriptbuilder.py` & `experimaestro-1.5.7/src/experimaestro/scriptbuilder.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/__init__.py` & `experimaestro-1.5.7/src/experimaestro/server/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf` & `experimaestro-1.5.7/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/0c35d18bf06992036b69.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/0c35d18bf06992036b69.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/3a4004a46a653d4b2166.woff` & `experimaestro-1.5.7/src/experimaestro/server/data/3a4004a46a653d4b2166.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/3baa5b8f3469222b822d.woff` & `experimaestro-1.5.7/src/experimaestro/server/data/3baa5b8f3469222b822d.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/4d73cb90e394b34b7670.woff` & `experimaestro-1.5.7/src/experimaestro/server/data/4d73cb90e394b34b7670.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/50701fbb8177c2dde530.ttf` & `experimaestro-1.5.7/src/experimaestro/server/data/50701fbb8177c2dde530.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/5d681e2edae8c60630db.woff` & `experimaestro-1.5.7/src/experimaestro/server/data/5d681e2edae8c60630db.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/878f31251d960bd6266f.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/878f31251d960bd6266f.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/c380809fd3677d7d6903.woff2` & `experimaestro-1.5.7/src/experimaestro/server/data/c380809fd3677d7d6903.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf` & `experimaestro-1.5.7/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/f882956fd323fd322f31.woff` & `experimaestro-1.5.7/src/experimaestro/server/data/f882956fd323fd322f31.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/favicon.ico` & `experimaestro-1.5.7/src/experimaestro/server/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/index.css` & `experimaestro-1.5.7/src/experimaestro/server/data/index.css`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/index.css.map` & `experimaestro-1.5.7/src/experimaestro/server/data/index.css.map`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/index.html` & `experimaestro-1.5.7/src/experimaestro/server/data/index.html`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/index.js` & `experimaestro-1.5.7/src/experimaestro/server/data/index.js`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/server/data/index.js.map` & `experimaestro-1.5.7/src/experimaestro/server/data/index.js.map`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/sphinx/__init__.py` & `experimaestro-1.5.7/src/experimaestro/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/conftest.py` & `experimaestro-1.5.7/src/experimaestro/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/connectors/test_local.py` & `experimaestro-1.5.7/src/experimaestro/tests/connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/connectors/utils.py` & `experimaestro-1.5.7/src/experimaestro/tests/connectors/utils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/bin/sacct` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/bin/sacct`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/bin/sbatch` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/bin/sbatch`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/common.py` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/common.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/config_slurm/launchers.yaml` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/config_slurm/launchers.yaml`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/test_local.py` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/test_local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/launchers/test_slurm.py` & `experimaestro-1.5.7/src/experimaestro/tests/launchers/test_slurm.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/restart.py` & `experimaestro-1.5.7/src/experimaestro/tests/restart.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/tasks/all.py` & `experimaestro-1.5.7/src/experimaestro/tests/tasks/all.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_dependencies.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_findlauncher.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_findlauncher.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_forward.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_forward.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_identifier.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_instance.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_objects.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_outputs.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_outputs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_param.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_progress.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_serializers.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_snippets.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_ssh.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_tags.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict
 from pathlib import Path
 from experimaestro import (
     tag,
+    LightweightTask,
     config,
     argument,
     Config,
     Task,
     Param,
 )
 from experimaestro.scheduler.workspace import RunMode
@@ -65,14 +66,48 @@
     task.submit(run_mode=RunMode.DRY_RUN)
     assert output.tags() == {"hello": "world"}
 
     evaluate = Evaluate(task=task).submit(run_mode=RunMode.DRY_RUN)
     assert evaluate.__xpm__.tags() == {"hello": "world"}
 
 
+def test_tags_init_tasks():
+    """Test tags within init tasks"""
+
+    class MyTask(Task):
+        pass
+
+    class InitTask(LightweightTask):
+        pass
+
+    class MyConfig(Config):
+        pass
+
+    class TaskWithOutput(Task):
+        x: Param[MyConfig]
+
+        def task_outputs(self, dep) -> MyConfig:
+            return dep(MyConfig())
+
+    init_task = InitTask().tag("hello", "world")
+    task = MyTask()
+    result = task.submit(run_mode=RunMode.DRY_RUN, init_tasks=[init_task])
+    assert result.tags() == {"hello": "world"}
+
+    other_task = TaskWithOutput(x=MyConfig().tag("hello", "world"))
+    assert other_task.tags() == {"hello": "world"}
+
+    result = other_task.submit(run_mode=RunMode.DRY_RUN)
+    assert isinstance(result, MyConfig)
+    assert result.tags() == {"hello": "world"}
+
+    result = MyTask().submit(run_mode=RunMode.DRY_RUN, init_tasks=[result])
+    assert result.tags() == {"hello": "world"}
+
+
 class TaskDirectoryContext(DirectoryContext):
     def __init__(self, task, path):
         super().__init__(path)
         self._task = task
 
     @property
     def task(self):
```

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_tasks.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_tokens.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_types.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/test_validation.py` & `experimaestro-1.5.7/src/experimaestro/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/token_reschedule.py` & `experimaestro-1.5.7/src/experimaestro/tests/token_reschedule.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tests/utils.py` & `experimaestro-1.5.7/src/experimaestro/tests/utils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tokens.py` & `experimaestro-1.5.7/src/experimaestro/tokens.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tools/diff.py` & `experimaestro-1.5.7/src/experimaestro/tools/diff.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tools/documentation.py` & `experimaestro-1.5.7/src/experimaestro/tools/documentation.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/tools/jobs.py` & `experimaestro-1.5.7/src/experimaestro/tools/jobs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/typingutils.py` & `experimaestro-1.5.7/src/experimaestro/typingutils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/__init__.py` & `experimaestro-1.5.7/src/experimaestro/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/asyncio.py` & `experimaestro-1.5.7/src/experimaestro/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/jobs.py` & `experimaestro-1.5.7/src/experimaestro/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/jupyter.py` & `experimaestro-1.5.7/src/experimaestro/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/resources.py` & `experimaestro-1.5.7/src/experimaestro/utils/resources.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/settings.py` & `experimaestro-1.5.7/src/experimaestro/utils/settings.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/utils/yaml.py` & `experimaestro-1.5.7/src/experimaestro/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/src/experimaestro/xpmutils.py` & `experimaestro-1.5.7/src/experimaestro/xpmutils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.6/PKG-INFO` & `experimaestro-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimaestro
-Version: 1.5.6
+Version: 1.5.7
 Summary: "Experimaestro is a computer science experiment manager"
 Home-page: https://github.com/experimaestro/experimaestro-python
 License: GPL-3
 Keywords: experiment manager
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 Requires-Python: >=3.8,<4.0
```

