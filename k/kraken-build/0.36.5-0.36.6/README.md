# Comparing `tmp/kraken_build-0.36.5.tar.gz` & `tmp/kraken_build-0.36.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_build-0.36.5.tar", max compression
+gzip compressed data, was "kraken_build-0.36.6.tar", max compression
```

## Comparing `kraken_build-0.36.5.tar` & `kraken_build-0.36.6.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0      998 2024-04-11 17:13:39.290367 kraken_build-0.36.5/LICENSE
--rw-r--r--   0        0        0     2943 2024-04-11 18:13:27.437407 kraken_build-0.36.5/README.md
--rw-r--r--   0        0        0     2422 2024-04-11 19:39:33.065166 kraken_build-0.36.5/pyproject.toml
--rw-r--r--   0        0        0      918 2024-04-11 17:13:39.290864 kraken_build-0.36.5/src/kraken/build/__init__.py
--rw-r--r--   0        0        0     1162 2024-04-11 17:13:39.291009 kraken_build-0.36.5/src/kraken/build/tests/test_import.py
--rw-r--r--   0        0        0      858 2024-04-11 17:13:39.291155 kraken_build-0.36.5/src/kraken/build/utils/import_helper.py
--rw-r--r--   0        0        0     2120 2024-04-11 19:39:33.065366 kraken_build-0.36.5/src/kraken/common/__init__.py
--rw-r--r--   0        0        0      471 2024-04-11 17:13:39.291411 kraken_build-0.36.5/src/kraken/common/_argparse.py
--rw-r--r--   0        0        0     1944 2024-04-11 18:13:27.438198 kraken_build-0.36.5/src/kraken/common/_asciitable.py
--rw-r--r--   0        0        0      121 2024-04-11 17:13:39.291598 kraken_build-0.36.5/src/kraken/common/_auth.py
--rw-r--r--   0        0        0     5226 2024-04-11 18:13:27.438496 kraken_build-0.36.5/src/kraken/common/_buildscript.py
--rw-r--r--   0        0        0      666 2024-04-11 17:13:39.291855 kraken_build-0.36.5/src/kraken/common/_buildscript_test.py
--rw-r--r--   0        0        0      609 2024-04-11 17:13:39.291954 kraken_build-0.36.5/src/kraken/common/_date.py
--rw-r--r--   0        0        0      690 2024-04-11 17:13:39.292039 kraken_build-0.36.5/src/kraken/common/_date_test.py
--rw-r--r--   0        0        0     1410 2024-04-11 17:13:39.292128 kraken_build-0.36.5/src/kraken/common/_environment.py
--rw-r--r--   0        0        0     3088 2024-04-11 18:13:27.438669 kraken_build-0.36.5/src/kraken/common/_fs.py
--rw-r--r--   0        0        0      709 2024-04-11 17:13:39.292310 kraken_build-0.36.5/src/kraken/common/_generic.py
--rw-r--r--   0        0        0     1083 2024-04-11 17:13:39.292406 kraken_build-0.36.5/src/kraken/common/_importlib.py
--rw-r--r--   0        0        0     1605 2024-04-11 17:13:39.292508 kraken_build-0.36.5/src/kraken/common/_option_sets.py
--rw-r--r--   0        0        0     9392 2024-04-11 18:13:27.438927 kraken_build-0.36.5/src/kraken/common/_requirements.py
--rw-r--r--   0        0        0     1037 2024-04-11 17:13:39.292777 kraken_build-0.36.5/src/kraken/common/_requirements_test.py
--rw-r--r--   0        0        0     8177 2024-04-11 18:13:27.439229 kraken_build-0.36.5/src/kraken/common/_runner.py
--rw-r--r--   0        0        0     2920 2024-04-11 18:13:27.439395 kraken_build-0.36.5/src/kraken/common/_runner_test.py
--rw-r--r--   0        0        0      494 2024-04-11 17:13:39.293140 kraken_build-0.36.5/src/kraken/common/_terminal.py
--rw-r--r--   0        0        0     1267 2024-04-11 17:13:39.293235 kraken_build-0.36.5/src/kraken/common/_text.py
--rw-r--r--   0        0        0      197 2024-04-11 17:13:39.293316 kraken_build-0.36.5/src/kraken/common/_text_test.py
--rw-r--r--   0        0        0     1201 2024-04-11 17:13:39.293404 kraken_build-0.36.5/src/kraken/common/_tomlconfig.py
--rw-r--r--   0        0        0      811 2024-04-11 17:13:39.293492 kraken_build-0.36.5/src/kraken/common/_tomlconfig_test.py
--rw-r--r--   0        0        0      898 2024-04-11 17:13:39.293575 kraken_build-0.36.5/src/kraken/common/exceptions.py
--rw-r--r--   0        0        0     8963 2024-04-11 17:13:39.293717 kraken_build-0.36.5/src/kraken/common/findpython.py
--rw-r--r--   0        0        0     2218 2024-04-11 17:13:39.293859 kraken_build-0.36.5/src/kraken/common/http/__init__.py
--rw-r--r--   0        0        0     3449 2024-04-11 17:13:39.293954 kraken_build-0.36.5/src/kraken/common/http/lint_ban_bare_requests.py
--rw-r--r--   0        0        0      824 2024-04-11 17:13:39.294041 kraken_build-0.36.5/src/kraken/common/path.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.294074 kraken_build-0.36.5/src/kraken/common/py.typed
--rw-r--r--   0        0        0      326 2024-04-11 17:13:39.294230 kraken_build-0.36.5/src/kraken/common/pyenv/__init__.py
--rw-r--r--   0        0        0     4960 2024-04-11 17:13:39.294672 kraken_build-0.36.5/src/kraken/common/pyenv/_distributions.py
--rw-r--r--   0        0        0     1996 2024-04-11 17:13:39.294781 kraken_build-0.36.5/src/kraken/common/pyenv/_virtualenv.py
--rw-r--r--   0        0        0      266 2024-04-11 17:13:39.294869 kraken_build-0.36.5/src/kraken/common/strings.py
--rw-r--r--   0        0        0     8695 2024-04-11 17:13:39.295014 kraken_build-0.36.5/src/kraken/common/supplier.py
--rw-r--r--   0        0        0      869 2024-04-11 19:39:33.065497 kraken_build-0.36.5/src/kraken/core/__init__.py
--rw-r--r--   0        0        0      468 2024-04-11 17:13:39.295292 kraken_build-0.36.5/src/kraken/core/address/__init__.py
--rw-r--r--   0        0        0    21824 2024-04-11 17:13:39.295415 kraken_build-0.36.5/src/kraken/core/address/_address.py
--rw-r--r--   0        0        0    14459 2024-04-11 17:13:39.295627 kraken_build-0.36.5/src/kraken/core/address/_address_resolver.py
--rw-r--r--   0        0        0     6070 2024-04-11 17:13:39.295923 kraken_build-0.36.5/src/kraken/core/address/_address_resolver_test.py
--rw-r--r--   0        0        0     6658 2024-04-11 17:13:39.296105 kraken_build-0.36.5/src/kraken/core/address/_address_test.py
--rw-r--r--   0        0        0      525 2024-04-11 17:13:39.296194 kraken_build-0.36.5/src/kraken/core/address/_addressable.py
--rw-r--r--   0        0        0      263 2024-04-11 17:13:39.296326 kraken_build-0.36.5/src/kraken/core/base/__init__.py
--rw-r--r--   0        0        0     2201 2024-04-11 17:13:39.296417 kraken_build-0.36.5/src/kraken/core/base/currentable.py
--rw-r--r--   0        0        0     1141 2024-04-11 17:13:39.296508 kraken_build-0.36.5/src/kraken/core/base/metadata.py
--rw-r--r--   0        0        0     2396 2024-04-11 17:13:39.296645 kraken_build-0.36.5/src/kraken/core/cli/executor.py
--rw-r--r--   0        0        0      325 2024-04-11 17:13:39.296732 kraken_build-0.36.5/src/kraken/core/cli/executor_test.py
--rw-r--r--   0        0        0    27380 2024-04-11 17:13:39.296887 kraken_build-0.36.5/src/kraken/core/cli/main.py
--rw-r--r--   0        0        0     7401 2024-04-11 17:13:39.297101 kraken_build-0.36.5/src/kraken/core/cli/option_sets.py
--rw-r--r--   0        0        0     2000 2024-04-11 17:13:39.297200 kraken_build-0.36.5/src/kraken/core/cli/serialize.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.297236 kraken_build-0.36.5/src/kraken/core/py.typed
--rw-r--r--   0        0        0      132 2024-04-11 17:13:39.297388 kraken_build-0.36.5/src/kraken/core/system/__init__.py
--rw-r--r--   0        0        0    17516 2024-04-11 18:13:27.439800 kraken_build-0.36.5/src/kraken/core/system/context.py
--rw-r--r--   0        0        0     4367 2024-04-11 17:13:39.297911 kraken_build-0.36.5/src/kraken/core/system/context_test.py
--rw-r--r--   0        0        0     1366 2024-04-11 18:13:27.440417 kraken_build-0.36.5/src/kraken/core/system/errors.py
--rw-r--r--   0        0        0     2759 2024-04-11 17:13:39.298143 kraken_build-0.36.5/src/kraken/core/system/executor/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-11 17:13:39.298234 kraken_build-0.36.5/src/kraken/core/system/executor/colored.py
--rw-r--r--   0        0        0     8511 2024-04-11 17:13:39.298375 kraken_build-0.36.5/src/kraken/core/system/executor/default.py
--rw-r--r--   0        0        0     9377 2024-04-11 18:13:27.440716 kraken_build-0.36.5/src/kraken/core/system/executor/default_test.py
--rw-r--r--   0        0        0     1554 2024-04-11 17:13:39.298600 kraken_build-0.36.5/src/kraken/core/system/executor/utils.py
--rw-r--r--   0        0        0    24343 2024-04-11 17:13:39.298771 kraken_build-0.36.5/src/kraken/core/system/graph.py
--rw-r--r--   0        0        0    15570 2024-04-11 17:13:39.299324 kraken_build-0.36.5/src/kraken/core/system/graph_test.py
--rw-r--r--   0        0        0      947 2024-04-11 17:13:39.299412 kraken_build-0.36.5/src/kraken/core/system/kraken_object.py
--rw-r--r--   0        0        0    16455 2024-04-11 18:13:27.440934 kraken_build-0.36.5/src/kraken/core/system/project.py
--rw-r--r--   0        0        0     2893 2024-04-11 18:13:27.441140 kraken_build-0.36.5/src/kraken/core/system/project_test.py
--rw-r--r--   0        0        0    18566 2024-04-11 17:13:39.299789 kraken_build-0.36.5/src/kraken/core/system/property.py
--rw-r--r--   0        0        0     7588 2024-04-11 17:13:39.300117 kraken_build-0.36.5/src/kraken/core/system/property_test.py
--rw-r--r--   0        0        0    28698 2024-04-11 18:13:27.441376 kraken_build-0.36.5/src/kraken/core/system/task.py
--rw-r--r--   0        0        0      776 2024-04-11 17:13:39.300732 kraken_build-0.36.5/src/kraken/core/system/task_supplier.py
--rw-r--r--   0        0        0     1458 2024-04-11 17:13:39.300820 kraken_build-0.36.5/src/kraken/core/system/task_test.py
--rw-r--r--   0        0        0     1200 2024-04-11 17:13:39.300969 kraken_build-0.36.5/src/kraken/core/testing/__init__.py
--rw-r--r--   0        0        0       23 2024-04-11 19:39:33.065646 kraken_build-0.36.5/src/kraken/std/__init__.py
--rw-r--r--   0        0        0     1950 2024-04-11 18:13:27.442173 kraken_build-0.36.5/src/kraken/std/buffrs/__init__.py
--rw-r--r--   0        0        0     1921 2024-04-11 17:13:39.301351 kraken_build-0.36.5/src/kraken/std/buffrs/manifest.py
--rw-r--r--   0        0        0     2338 2024-04-11 18:13:27.442334 kraken_build-0.36.5/src/kraken/std/buffrs/tasks.py
--rw-r--r--   0        0        0    18824 2024-04-11 18:13:27.442552 kraken_build-0.36.5/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2461 2024-04-11 17:13:39.302059 kraken_build-0.36.5/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     9339 2024-04-11 18:13:27.443555 kraken_build-0.36.5/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.302308 kraken_build-0.36.5/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0      867 2024-04-11 17:13:39.302425 kraken_build-0.36.5/src/kraken/std/cargo/tasks/_cargo_sqlx.py
--rw-r--r--   0        0        0     4931 2024-04-11 18:13:27.443851 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     7126 2024-04-11 18:13:27.444135 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     2177 2024-04-11 17:13:39.302875 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0     1330 2024-04-11 17:13:39.302966 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0     1004 2024-04-11 17:13:39.303057 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0     3527 2024-04-11 17:13:39.303157 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     1180 2024-04-11 17:13:39.303250 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_generate_deb.py
--rw-r--r--   0        0        0     1503 2024-04-11 17:13:39.303339 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_login.py
--rw-r--r--   0        0        0     4642 2024-04-11 17:13:39.303617 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0      368 2024-04-11 17:13:39.303702 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_database_create.py
--rw-r--r--   0        0        0      360 2024-04-11 17:13:39.303798 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_database_drop.py
--rw-r--r--   0        0        0      583 2024-04-11 17:13:39.303887 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
--rw-r--r--   0        0        0      927 2024-04-11 17:13:39.303977 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
--rw-r--r--   0        0        0     3144 2024-04-11 18:13:27.444320 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      462 2024-04-11 17:13:39.304158 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      387 2024-04-11 17:13:39.304245 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      761 2024-04-11 17:13:39.304332 kraken_build-0.36.5/src/kraken/std/cargo/tasks/rustup_target_add_task.py
--rw-r--r--   0        0        0      720 2024-04-11 17:13:39.304419 kraken_build-0.36.5/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.304507 kraken_build-0.36.5/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      872 2024-04-11 17:13:39.304617 kraken_build-0.36.5/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10250 2024-04-11 17:13:39.304775 kraken_build-0.36.5/src/kraken/std/dist.py
--rw-r--r--   0        0        0     1574 2024-04-11 17:13:39.304924 kraken_build-0.36.5/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0      399 2024-04-11 17:13:39.305024 kraken_build-0.36.5/src/kraken/std/docker/_test.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305059 kraken_build-0.36.5/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305170 kraken_build-0.36.5/src/kraken/std/docker/tasks/__init__.py
--rw-r--r--   0        0        0     2915 2024-04-11 17:13:39.305281 kraken_build-0.36.5/src/kraken/std/docker/tasks/base_build_task.py
--rw-r--r--   0        0        0     4013 2024-04-11 18:13:27.444511 kraken_build-0.36.5/src/kraken/std/docker/tasks/buildx_build_task.py
--rw-r--r--   0        0        0     3685 2024-04-11 17:13:39.305489 kraken_build-0.36.5/src/kraken/std/docker/tasks/docker_build_task.py
--rw-r--r--   0        0        0     8509 2024-04-11 18:13:27.444994 kraken_build-0.36.5/src/kraken/std/docker/tasks/kaniko_build_task.py
--rw-r--r--   0        0        0     1461 2024-04-11 17:13:39.305732 kraken_build-0.36.5/src/kraken/std/docker/tasks/manifest_tool_push_task.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305819 kraken_build-0.36.5/src/kraken/std/docker/util/__init__.py
--rw-r--r--   0        0        0     1426 2024-04-11 17:13:39.305931 kraken_build-0.36.5/src/kraken/std/docker/util/dockerapi.py
--rw-r--r--   0        0        0     2273 2024-04-11 17:13:39.306023 kraken_build-0.36.5/src/kraken/std/docker/util/dockerfile.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.306107 kraken_build-0.36.5/src/kraken/std/docs/__init__.py
--rw-r--r--   0        0        0        5 2024-04-11 17:13:39.306257 kraken_build-0.36.5/src/kraken/std/docs/tasks/__init__.py
--rw-r--r--   0        0        0     2214 2024-04-11 18:13:27.445215 kraken_build-0.36.5/src/kraken/std/docs/tasks/mkdocs.py
--rw-r--r--   0        0        0     2414 2024-04-11 17:13:39.306433 kraken_build-0.36.5/src/kraken/std/docs/tasks/novella.py
--rw-r--r--   0        0        0     1574 2024-04-11 17:13:39.306568 kraken_build-0.36.5/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1119 2024-04-11 17:13:39.306655 kraken_build-0.36.5/src/kraken/std/git/config.py
--rw-r--r--   0        0        0       61 2024-04-11 17:13:39.306784 kraken_build-0.36.5/src/kraken/std/git/gitignore/__init__.py
--rw-r--r--   0        0        0     6157 2024-04-11 17:13:39.306990 kraken_build-0.36.5/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz
--rw-r--r--   0        0        0     2739 2024-04-11 17:13:39.307086 kraken_build-0.36.5/src/kraken/std/git/gitignore/generated.py
--rw-r--r--   0        0        0     1849 2024-04-11 17:13:39.307171 kraken_build-0.36.5/src/kraken/std/git/gitignore/generated_test.py
--rw-r--r--   0        0        0     3309 2024-04-11 17:13:39.307268 kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io.py
--rw-r--r--   0        0        0      687 2024-04-11 17:13:39.307361 kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io_test.py
--rw-r--r--   0        0        0     4369 2024-04-11 17:13:39.307524 kraken_build-0.36.5/src/kraken/std/git/gitignore/parser.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.307558 kraken_build-0.36.5/src/kraken/std/git/gitignore_test.py
--rw-r--r--   0        0        0      134 2024-04-11 17:13:39.307707 kraken_build-0.36.5/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0     3011 2024-04-11 17:13:39.307802 kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task.py
--rw-r--r--   0        0        0     2690 2024-04-11 17:13:39.307892 kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task_test.py
--rw-r--r--   0        0        0     3667 2024-04-11 18:13:27.445402 kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task.py
--rw-r--r--   0        0        0     2349 2024-04-11 17:13:39.308075 kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task_test.py
--rw-r--r--   0        0        0     3164 2024-04-11 17:13:39.308185 kraken_build-0.36.5/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6354 2024-04-11 17:13:39.308407 kraken_build-0.36.5/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2328 2024-04-11 17:13:39.308498 kraken_build-0.36.5/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0     3292 2024-04-11 18:13:27.445591 kraken_build-0.36.5/src/kraken/std/mitm/__init__.py
--rw-r--r--   0        0        0      861 2024-04-11 17:13:39.308739 kraken_build-0.36.5/src/kraken/std/mitm/mitm_addon.py
--rw-r--r--   0        0        0     1347 2024-04-11 17:13:39.308871 kraken_build-0.36.5/src/kraken/std/protobuf/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.308905 kraken_build-0.36.5/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1754 2024-04-11 17:13:39.309069 kraken_build-0.36.5/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     6778 2024-04-11 18:13:27.445891 kraken_build-0.36.5/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-11 18:13:27.446074 kraken_build-0.36.5/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0    10349 2024-04-11 18:13:27.446339 kraken_build-0.36.5/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     9785 2024-04-11 18:13:27.446647 kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm.py
--rw-r--r--   0        0        0     2105 2024-04-11 17:13:39.309833 kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm_test.py
--rw-r--r--   0        0        0    10853 2024-04-11 18:13:27.446887 kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     3094 2024-04-11 17:13:39.310049 kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry_test.py
--rw-r--r--   0        0        0     5177 2024-04-11 18:13:27.447198 kraken_build-0.36.5/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     6251 2024-04-11 18:13:27.447487 kraken_build-0.36.5/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     8712 2024-04-11 18:13:27.447748 kraken_build-0.36.5/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2024-04-11 17:13:39.310643 kraken_build-0.36.5/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-11 17:13:39.310759 kraken_build-0.36.5/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     3352 2024-04-11 17:13:39.310853 kraken_build-0.36.5/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     2002 2024-04-11 18:13:27.447939 kraken_build-0.36.5/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     2207 2024-04-11 18:13:27.448118 kraken_build-0.36.5/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2580 2024-04-11 17:13:39.311161 kraken_build-0.36.5/src/kraken/std/python/tasks/info_task.py
--rw-r--r--   0        0        0     3298 2024-04-11 17:13:39.311250 kraken_build-0.36.5/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     3003 2024-04-11 17:13:39.311344 kraken_build-0.36.5/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      970 2024-04-11 17:13:39.311447 kraken_build-0.36.5/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     2491 2024-04-11 17:13:39.311535 kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_stubtest_task.py
--rw-r--r--   0        0        0     4522 2024-04-11 17:13:39.311734 kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     8000 2024-04-11 18:13:27.448441 kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_task.py
--rw-r--r--   0        0        0     1682 2024-04-11 17:13:39.312262 kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_test.py
--rw-r--r--   0        0        0     3447 2024-04-11 17:13:39.312404 kraken_build-0.36.5/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2750 2024-04-11 18:13:27.448586 kraken_build-0.36.5/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     2041 2024-04-11 17:13:39.312616 kraken_build-0.36.5/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     3887 2024-04-11 17:13:39.312730 kraken_build-0.36.5/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     5451 2024-04-11 18:13:27.448873 kraken_build-0.36.5/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1689 2024-04-11 17:13:39.313043 kraken_build-0.36.5/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1619 2024-04-11 17:13:39.313145 kraken_build-0.36.5/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1144 2024-04-11 17:13:39.313244 kraken_build-0.36.5/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4115 2024-04-11 17:13:39.313564 kraken_build-0.36.5/src/kraken/std/sccache.py
--rw-r--r--   0        0        0     3841 2024-04-11 18:13:27.448980 kraken_build-0.36.5/src/kraken/std/shellcheck.py
--rw-r--r--   0        0        0      232 2024-04-11 17:13:39.313831 kraken_build-0.36.5/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     2198 2024-04-11 17:13:39.313935 kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task.py
--rw-r--r--   0        0        0      910 2024-04-11 17:13:39.314041 kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task_test.py
--rw-r--r--   0        0        0     2838 2024-04-11 17:13:39.314147 kraken_build-0.36.5/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     9660 2024-04-11 18:13:27.449242 kraken_build-0.36.5/src/kraken/std/util/daemon_controller.py
--rw-r--r--   0        0        0     1167 2024-04-11 18:13:27.449335 kraken_build-0.36.5/src/kraken/std/util/http.py
--rw-r--r--   0        0        0     3417 2024-04-11 17:13:39.314517 kraken_build-0.36.5/src/kraken/std/util/render_file_task.py
--rw-r--r--   0        0        0      625 2024-04-11 18:13:27.449424 kraken_build-0.36.5/src/kraken/std/util/url.py
--rw-r--r--   0        0        0     7175 2024-04-11 17:13:39.314833 kraken_build-0.36.5/src/kraken/std/util/validate_readme.py
--rw-r--r--   0        0        0     3173 2024-04-11 17:13:39.314950 kraken_build-0.36.5/src/kraken/std/util/validate_readme_test.py
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 kraken_build-0.36.5/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-11-08 11:28:21.661737 kraken_build-0.36.6/LICENSE
+-rw-r--r--   0        0        0     2922 2024-05-31 08:48:10.113818 kraken_build-0.36.6/README.md
+-rw-r--r--   0        0        0     2422 2024-05-31 11:48:46.789072 kraken_build-0.36.6/pyproject.toml
+-rw-r--r--   0        0        0      918 2024-05-31 10:30:29.998503 kraken_build-0.36.6/src/kraken/build/__init__.py
+-rw-r--r--   0        0        0     1162 2024-05-31 10:30:30.000237 kraken_build-0.36.6/src/kraken/build/tests/test_import.py
+-rw-r--r--   0        0        0      858 2024-05-31 10:30:30.002148 kraken_build-0.36.6/src/kraken/build/utils/import_helper.py
+-rw-r--r--   0        0        0     2120 2024-05-31 11:48:46.789451 kraken_build-0.36.6/src/kraken/common/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-31 10:30:30.008357 kraken_build-0.36.6/src/kraken/common/_argparse.py
+-rw-r--r--   0        0        0     1944 2024-05-31 10:30:30.001594 kraken_build-0.36.6/src/kraken/common/_asciitable.py
+-rw-r--r--   0        0        0      121 2024-05-31 10:30:30.003638 kraken_build-0.36.6/src/kraken/common/_auth.py
+-rw-r--r--   0        0        0     5226 2024-05-31 10:30:30.007985 kraken_build-0.36.6/src/kraken/common/_buildscript.py
+-rw-r--r--   0        0        0      666 2024-05-31 10:30:30.012200 kraken_build-0.36.6/src/kraken/common/_buildscript_test.py
+-rw-r--r--   0        0        0      609 2024-05-31 10:30:30.016620 kraken_build-0.36.6/src/kraken/common/_date.py
+-rw-r--r--   0        0        0      690 2024-05-31 10:30:30.017342 kraken_build-0.36.6/src/kraken/common/_date_test.py
+-rw-r--r--   0        0        0     1410 2024-05-31 10:30:29.998380 kraken_build-0.36.6/src/kraken/common/_environment.py
+-rw-r--r--   0        0        0     3088 2024-05-31 10:30:29.999980 kraken_build-0.36.6/src/kraken/common/_fs.py
+-rw-r--r--   0        0        0      709 2024-05-31 10:30:30.001638 kraken_build-0.36.6/src/kraken/common/_generic.py
+-rw-r--r--   0        0        0     1083 2024-05-31 10:30:30.006066 kraken_build-0.36.6/src/kraken/common/_importlib.py
+-rw-r--r--   0        0        0     1605 2024-05-31 10:30:30.008423 kraken_build-0.36.6/src/kraken/common/_option_sets.py
+-rw-r--r--   0        0        0     9392 2024-05-31 10:30:30.014561 kraken_build-0.36.6/src/kraken/common/_requirements.py
+-rw-r--r--   0        0        0     1037 2024-05-31 10:30:30.016802 kraken_build-0.36.6/src/kraken/common/_requirements_test.py
+-rw-r--r--   0        0        0     8177 2024-05-31 10:30:30.018423 kraken_build-0.36.6/src/kraken/common/_runner.py
+-rw-r--r--   0        0        0     2920 2024-05-31 10:30:30.020571 kraken_build-0.36.6/src/kraken/common/_runner_test.py
+-rw-r--r--   0        0        0      494 2024-05-31 10:30:30.020111 kraken_build-0.36.6/src/kraken/common/_terminal.py
+-rw-r--r--   0        0        0     1267 2024-05-31 10:30:30.020871 kraken_build-0.36.6/src/kraken/common/_text.py
+-rw-r--r--   0        0        0      197 2024-05-31 10:30:30.022964 kraken_build-0.36.6/src/kraken/common/_text_test.py
+-rw-r--r--   0        0        0     1201 2024-05-31 10:30:29.998380 kraken_build-0.36.6/src/kraken/common/_tomlconfig.py
+-rw-r--r--   0        0        0      811 2024-05-31 10:30:29.999076 kraken_build-0.36.6/src/kraken/common/_tomlconfig_test.py
+-rw-r--r--   0        0        0      898 2024-05-31 10:30:29.999981 kraken_build-0.36.6/src/kraken/common/exceptions.py
+-rw-r--r--   0        0        0     8963 2024-05-31 10:30:29.998900 kraken_build-0.36.6/src/kraken/common/findpython.py
+-rw-r--r--   0        0        0     2218 2024-05-31 10:30:30.000894 kraken_build-0.36.6/src/kraken/common/http/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-31 10:30:30.001542 kraken_build-0.36.6/src/kraken/common/http/lint_ban_bare_requests.py
+-rw-r--r--   0        0        0      824 2024-05-31 10:30:29.999971 kraken_build-0.36.6/src/kraken/common/path.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:30.001425 kraken_build-0.36.6/src/kraken/common/py.typed
+-rw-r--r--   0        0        0      326 2024-05-31 10:30:30.003585 kraken_build-0.36.6/src/kraken/common/pyenv/__init__.py
+-rw-r--r--   0        0        0     4960 2024-05-31 10:30:30.008428 kraken_build-0.36.6/src/kraken/common/pyenv/_distributions.py
+-rw-r--r--   0        0        0     1996 2024-05-31 10:30:30.012170 kraken_build-0.36.6/src/kraken/common/pyenv/_virtualenv.py
+-rw-r--r--   0        0        0      266 2024-05-31 10:30:30.014514 kraken_build-0.36.6/src/kraken/common/strings.py
+-rw-r--r--   0        0        0     8695 2024-05-31 10:30:29.999168 kraken_build-0.36.6/src/kraken/common/supplier.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:48:46.789883 kraken_build-0.36.6/src/kraken/core/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-31 10:30:17.546233 kraken_build-0.36.6/src/kraken/core/address/__init__.py
+-rw-r--r--   0        0        0    21824 2024-05-31 10:30:17.549293 kraken_build-0.36.6/src/kraken/core/address/_address.py
+-rw-r--r--   0        0        0    14459 2024-05-31 10:30:17.549842 kraken_build-0.36.6/src/kraken/core/address/_address_resolver.py
+-rw-r--r--   0        0        0     6070 2024-05-31 10:30:17.550310 kraken_build-0.36.6/src/kraken/core/address/_address_resolver_test.py
+-rw-r--r--   0        0        0     6658 2024-05-31 10:30:17.550878 kraken_build-0.36.6/src/kraken/core/address/_address_test.py
+-rw-r--r--   0        0        0      525 2024-05-31 10:30:17.551183 kraken_build-0.36.6/src/kraken/core/address/_addressable.py
+-rw-r--r--   0        0        0      263 2024-05-31 10:30:17.552118 kraken_build-0.36.6/src/kraken/core/base/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-31 10:30:17.553703 kraken_build-0.36.6/src/kraken/core/base/currentable.py
+-rw-r--r--   0        0        0     1141 2024-05-31 10:30:17.553897 kraken_build-0.36.6/src/kraken/core/base/metadata.py
+-rw-r--r--   0        0        0     2396 2024-05-31 10:30:17.554422 kraken_build-0.36.6/src/kraken/core/cli/executor.py
+-rw-r--r--   0        0        0      325 2024-05-31 10:30:17.554599 kraken_build-0.36.6/src/kraken/core/cli/executor_test.py
+-rw-r--r--   0        0        0    27380 2024-05-31 10:30:17.556886 kraken_build-0.36.6/src/kraken/core/cli/main.py
+-rw-r--r--   0        0        0     7401 2024-05-31 10:30:17.557524 kraken_build-0.36.6/src/kraken/core/cli/option_sets.py
+-rw-r--r--   0        0        0     2000 2024-05-31 10:30:17.557965 kraken_build-0.36.6/src/kraken/core/cli/serialize.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.558298 kraken_build-0.36.6/src/kraken/core/py.typed
+-rw-r--r--   0        0        0      132 2024-05-31 10:30:17.558905 kraken_build-0.36.6/src/kraken/core/system/__init__.py
+-rw-r--r--   0        0        0    17516 2024-05-31 10:30:17.559262 kraken_build-0.36.6/src/kraken/core/system/context.py
+-rw-r--r--   0        0        0     4367 2024-05-31 10:30:17.559941 kraken_build-0.36.6/src/kraken/core/system/context_test.py
+-rw-r--r--   0        0        0     1366 2024-05-31 10:30:17.563100 kraken_build-0.36.6/src/kraken/core/system/errors.py
+-rw-r--r--   0        0        0     2759 2024-05-31 10:30:17.566880 kraken_build-0.36.6/src/kraken/core/system/executor/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-31 10:30:17.567583 kraken_build-0.36.6/src/kraken/core/system/executor/colored.py
+-rw-r--r--   0        0        0     8511 2024-05-31 10:30:17.572717 kraken_build-0.36.6/src/kraken/core/system/executor/default.py
+-rw-r--r--   0        0        0     9377 2024-05-31 10:30:17.578143 kraken_build-0.36.6/src/kraken/core/system/executor/default_test.py
+-rw-r--r--   0        0        0     1554 2024-05-31 10:30:17.581141 kraken_build-0.36.6/src/kraken/core/system/executor/utils.py
+-rw-r--r--   0        0        0    24343 2024-05-31 10:30:17.595345 kraken_build-0.36.6/src/kraken/core/system/graph.py
+-rw-r--r--   0        0        0    15570 2024-05-31 10:30:17.600616 kraken_build-0.36.6/src/kraken/core/system/graph_test.py
+-rw-r--r--   0        0        0      947 2024-05-31 10:30:17.601287 kraken_build-0.36.6/src/kraken/core/system/kraken_object.py
+-rw-r--r--   0        0        0    16455 2024-05-31 10:30:17.601552 kraken_build-0.36.6/src/kraken/core/system/project.py
+-rw-r--r--   0        0        0     2893 2024-05-31 10:30:17.601991 kraken_build-0.36.6/src/kraken/core/system/project_test.py
+-rw-r--r--   0        0        0    18566 2024-05-31 10:30:17.602320 kraken_build-0.36.6/src/kraken/core/system/property.py
+-rw-r--r--   0        0        0     7588 2024-05-31 10:30:17.602751 kraken_build-0.36.6/src/kraken/core/system/property_test.py
+-rw-r--r--   0        0        0    28698 2024-05-31 10:30:17.603915 kraken_build-0.36.6/src/kraken/core/system/task.py
+-rw-r--r--   0        0        0      776 2024-05-31 10:30:17.604196 kraken_build-0.36.6/src/kraken/core/system/task_supplier.py
+-rw-r--r--   0        0        0     1458 2024-05-31 10:30:17.604801 kraken_build-0.36.6/src/kraken/core/system/task_test.py
+-rw-r--r--   0        0        0     1200 2024-05-31 10:30:17.605057 kraken_build-0.36.6/src/kraken/core/testing/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-31 11:48:46.789989 kraken_build-0.36.6/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0     1950 2024-05-31 10:30:17.611315 kraken_build-0.36.6/src/kraken/std/buffrs/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-31 10:30:17.611948 kraken_build-0.36.6/src/kraken/std/buffrs/manifest.py
+-rw-r--r--   0        0        0     2338 2024-05-31 10:30:17.612328 kraken_build-0.36.6/src/kraken/std/buffrs/tasks.py
+-rw-r--r--   0        0        0    18824 2024-05-31 10:30:17.613283 kraken_build-0.36.6/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-31 10:30:17.613741 kraken_build-0.36.6/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     9339 2024-05-31 10:30:17.613998 kraken_build-0.36.6/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.614310 kraken_build-0.36.6/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0      867 2024-05-31 10:30:17.615110 kraken_build-0.36.6/src/kraken/std/cargo/tasks/_cargo_sqlx.py
+-rw-r--r--   0        0        0     4931 2024-05-31 10:30:17.618034 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     7126 2024-05-31 10:30:17.618786 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     2177 2024-05-31 10:30:17.619088 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0     1330 2024-05-31 10:30:17.621279 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0     1004 2024-05-31 10:30:17.621502 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0     3527 2024-05-31 10:30:17.621600 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     1180 2024-05-31 10:30:17.621692 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_generate_deb.py
+-rw-r--r--   0        0        0     1503 2024-05-31 10:30:17.621940 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_login.py
+-rw-r--r--   0        0        0     4642 2024-05-31 10:30:17.622037 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0      368 2024-05-31 10:30:17.622142 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_database_create.py
+-rw-r--r--   0        0        0      360 2024-05-31 10:30:17.622223 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_database_drop.py
+-rw-r--r--   0        0        0      583 2024-05-31 10:30:17.622314 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
+-rw-r--r--   0        0        0      927 2024-05-31 10:30:17.622417 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
+-rw-r--r--   0        0        0     3144 2024-05-31 10:30:17.626182 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      462 2024-05-31 10:30:17.626632 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      387 2024-05-31 10:30:17.627105 kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      761 2024-05-31 10:30:17.629435 kraken_build-0.36.6/src/kraken/std/cargo/tasks/rustup_target_add_task.py
+-rw-r--r--   0        0        0      720 2024-05-31 10:30:17.630706 kraken_build-0.36.6/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.630992 kraken_build-0.36.6/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-31 10:30:17.631310 kraken_build-0.36.6/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10250 2024-05-31 10:30:17.632115 kraken_build-0.36.6/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     1574 2024-05-31 10:30:17.632594 kraken_build-0.36.6/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-31 10:30:17.633055 kraken_build-0.36.6/src/kraken/std/docker/_test.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.633612 kraken_build-0.36.6/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.633926 kraken_build-0.36.6/src/kraken/std/docker/tasks/__init__.py
+-rw-r--r--   0        0        0     2915 2024-05-31 10:30:17.634162 kraken_build-0.36.6/src/kraken/std/docker/tasks/base_build_task.py
+-rw-r--r--   0        0        0     4013 2024-05-31 10:30:17.634386 kraken_build-0.36.6/src/kraken/std/docker/tasks/buildx_build_task.py
+-rw-r--r--   0        0        0     3685 2024-05-31 10:30:17.634600 kraken_build-0.36.6/src/kraken/std/docker/tasks/docker_build_task.py
+-rw-r--r--   0        0        0     8509 2024-05-31 10:30:17.637287 kraken_build-0.36.6/src/kraken/std/docker/tasks/kaniko_build_task.py
+-rw-r--r--   0        0        0     1461 2024-05-31 10:30:17.637482 kraken_build-0.36.6/src/kraken/std/docker/tasks/manifest_tool_push_task.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.637711 kraken_build-0.36.6/src/kraken/std/docker/util/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-31 10:30:17.637874 kraken_build-0.36.6/src/kraken/std/docker/util/dockerapi.py
+-rw-r--r--   0        0        0     2273 2024-05-31 10:30:17.638044 kraken_build-0.36.6/src/kraken/std/docker/util/dockerfile.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.638280 kraken_build-0.36.6/src/kraken/std/docs/__init__.py
+-rw-r--r--   0        0        0        5 2024-05-31 10:30:17.641270 kraken_build-0.36.6/src/kraken/std/docs/tasks/__init__.py
+-rw-r--r--   0        0        0     2214 2024-05-31 10:30:17.642374 kraken_build-0.36.6/src/kraken/std/docs/tasks/mkdocs.py
+-rw-r--r--   0        0        0     2414 2024-05-31 10:30:17.645139 kraken_build-0.36.6/src/kraken/std/docs/tasks/novella.py
+-rw-r--r--   0        0        0     1574 2024-05-31 10:30:17.647269 kraken_build-0.36.6/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1119 2024-05-31 10:30:17.647824 kraken_build-0.36.6/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0       61 2024-05-31 10:30:17.648025 kraken_build-0.36.6/src/kraken/std/git/gitignore/__init__.py
+-rw-r--r--   0        0        0     6157 2024-05-31 10:30:17.648273 kraken_build-0.36.6/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz
+-rw-r--r--   0        0        0     2739 2024-05-31 10:30:17.648491 kraken_build-0.36.6/src/kraken/std/git/gitignore/generated.py
+-rw-r--r--   0        0        0     1849 2024-05-31 10:30:17.648642 kraken_build-0.36.6/src/kraken/std/git/gitignore/generated_test.py
+-rw-r--r--   0        0        0     3309 2024-05-31 10:30:17.649173 kraken_build-0.36.6/src/kraken/std/git/gitignore/gitignore_io.py
+-rw-r--r--   0        0        0      687 2024-05-31 10:30:17.649304 kraken_build-0.36.6/src/kraken/std/git/gitignore/gitignore_io_test.py
+-rw-r--r--   0        0        0     4369 2024-05-31 10:30:17.649423 kraken_build-0.36.6/src/kraken/std/git/gitignore/parser.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.649486 kraken_build-0.36.6/src/kraken/std/git/gitignore_test.py
+-rw-r--r--   0        0        0      134 2024-05-31 10:30:17.649677 kraken_build-0.36.6/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0     3011 2024-05-31 10:30:17.649790 kraken_build-0.36.6/src/kraken/std/git/tasks/check_file_task.py
+-rw-r--r--   0        0        0     2690 2024-05-31 10:30:17.650038 kraken_build-0.36.6/src/kraken/std/git/tasks/check_file_task_test.py
+-rw-r--r--   0        0        0     3667 2024-05-31 10:30:17.650152 kraken_build-0.36.6/src/kraken/std/git/tasks/sync_task.py
+-rw-r--r--   0        0        0     2349 2024-05-31 10:30:17.650250 kraken_build-0.36.6/src/kraken/std/git/tasks/sync_task_test.py
+-rw-r--r--   0        0        0     3164 2024-05-31 10:30:17.650359 kraken_build-0.36.6/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6354 2024-05-31 10:30:17.651123 kraken_build-0.36.6/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2328 2024-05-31 10:30:17.651495 kraken_build-0.36.6/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     3292 2024-05-31 10:30:17.652653 kraken_build-0.36.6/src/kraken/std/mitm/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-31 10:30:17.652825 kraken_build-0.36.6/src/kraken/std/mitm/mitm_addon.py
+-rw-r--r--   0        0        0     1347 2024-05-31 10:30:17.653963 kraken_build-0.36.6/src/kraken/std/protobuf/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.654072 kraken_build-0.36.6/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1754 2024-05-31 10:30:17.654356 kraken_build-0.36.6/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     6778 2024-05-31 10:30:17.654639 kraken_build-0.36.6/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1439 2024-05-31 10:30:17.657076 kraken_build-0.36.6/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0    10349 2024-05-31 10:30:17.657572 kraken_build-0.36.6/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     9785 2024-05-31 10:30:17.661982 kraken_build-0.36.6/src/kraken/std/python/buildsystem/pdm.py
+-rw-r--r--   0        0        0     2105 2024-05-31 10:30:17.664035 kraken_build-0.36.6/src/kraken/std/python/buildsystem/pdm_test.py
+-rw-r--r--   0        0        0    10853 2024-05-31 10:30:17.668202 kraken_build-0.36.6/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     3094 2024-05-31 10:30:17.668348 kraken_build-0.36.6/src/kraken/std/python/buildsystem/poetry_test.py
+-rw-r--r--   0        0        0     5177 2024-05-31 10:30:17.670025 kraken_build-0.36.6/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     6251 2024-05-31 10:30:17.670159 kraken_build-0.36.6/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     8712 2024-05-31 10:30:17.671206 kraken_build-0.36.6/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:30:17.671368 kraken_build-0.36.6/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3705 2024-05-31 10:30:17.671654 kraken_build-0.36.6/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     3352 2024-05-31 10:30:17.676148 kraken_build-0.36.6/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     2002 2024-05-31 10:30:17.676293 kraken_build-0.36.6/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     2207 2024-05-31 10:30:17.676946 kraken_build-0.36.6/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2580 2024-05-31 10:30:17.677060 kraken_build-0.36.6/src/kraken/std/python/tasks/info_task.py
+-rw-r--r--   0        0        0     3298 2024-05-31 10:30:17.677167 kraken_build-0.36.6/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     3003 2024-05-31 10:30:17.677759 kraken_build-0.36.6/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      970 2024-05-31 10:30:17.677887 kraken_build-0.36.6/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     2491 2024-05-31 10:30:17.678424 kraken_build-0.36.6/src/kraken/std/python/tasks/mypy_stubtest_task.py
+-rw-r--r--   0        0        0     4522 2024-05-31 10:30:17.680097 kraken_build-0.36.6/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     8000 2024-05-31 10:30:17.680715 kraken_build-0.36.6/src/kraken/std/python/tasks/pex_build_task.py
+-rw-r--r--   0        0        0     1682 2024-05-31 10:30:17.681383 kraken_build-0.36.6/src/kraken/std/python/tasks/pex_build_test.py
+-rw-r--r--   0        0        0     3447 2024-05-31 10:30:17.686625 kraken_build-0.36.6/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2750 2024-05-31 10:30:17.687778 kraken_build-0.36.6/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     2041 2024-05-31 10:30:17.690084 kraken_build-0.36.6/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     3887 2024-05-31 10:30:17.690743 kraken_build-0.36.6/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     5451 2024-05-31 10:30:17.691313 kraken_build-0.36.6/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1689 2024-05-31 10:30:17.691429 kraken_build-0.36.6/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1619 2024-05-31 10:30:17.691523 kraken_build-0.36.6/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1144 2024-05-31 10:30:17.691609 kraken_build-0.36.6/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4115 2024-05-31 10:30:17.691709 kraken_build-0.36.6/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0     3841 2024-05-31 10:30:17.692190 kraken_build-0.36.6/src/kraken/std/shellcheck.py
+-rw-r--r--   0        0        0      232 2024-05-31 10:30:17.692311 kraken_build-0.36.6/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     2198 2024-05-31 10:30:17.692422 kraken_build-0.36.6/src/kraken/std/util/check_file_contents_task.py
+-rw-r--r--   0        0        0      910 2024-05-31 10:30:17.694173 kraken_build-0.36.6/src/kraken/std/util/check_file_contents_task_test.py
+-rw-r--r--   0        0        0     2838 2024-05-31 10:30:17.694332 kraken_build-0.36.6/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     9660 2024-05-31 10:30:17.710086 kraken_build-0.36.6/src/kraken/std/util/daemon_controller.py
+-rw-r--r--   0        0        0     1167 2024-05-31 08:48:10.168381 kraken_build-0.36.6/src/kraken/std/util/http.py
+-rw-r--r--   0        0        0     3674 2024-05-31 10:30:17.715891 kraken_build-0.36.6/src/kraken/std/util/render_file_task.py
+-rw-r--r--   0        0        0      625 2024-05-31 08:48:10.170144 kraken_build-0.36.6/src/kraken/std/util/url.py
+-rw-r--r--   0        0        0     7175 2024-05-31 10:30:17.716880 kraken_build-0.36.6/src/kraken/std/util/validate_readme.py
+-rw-r--r--   0        0        0     3173 2024-05-31 10:30:17.716992 kraken_build-0.36.6/src/kraken/std/util/validate_readme_test.py
+-rw-r--r--   0        0        0     4439 1970-01-01 00:00:00.000000 kraken_build-0.36.6/PKG-INFO
```

### Comparing `kraken_build-0.36.5/LICENSE` & `kraken_build-0.36.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/README.md` & `kraken_build-0.36.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
----
-title: Home
----
-
 # The Kraken build system
 
 ![kraken-logo](https://i.imgur.com/Lqjy2zi.png)
 
 [![Python](https://github.com/kraken-build/kraken/actions/workflows/python.yaml/badge.svg)](https://github.com/kraken-build/kraken/actions/workflows/python.yaml)
 [![PyPI version](https://badge.fury.io/py/kraken-build.svg)](https://badge.fury.io/py/kraken-build)
 [![Documentation](https://img.shields.io/badge/Documentation-blue?style=flat&logo=gitbook&logoColor=white)](https://kraken-build.github.io/kraken/)
```

### Comparing `kraken_build-0.36.5/pyproject.toml` & `kraken_build-0.36.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 packages = [
   {include = "kraken/build", from = "src"},
   {include = "kraken/common", from = "src"},
   {include = "kraken/core", from = "src"},
   {include = "kraken/std", from = "src"},
 ]
 readme = "README.md"
-version = "0.36.5"
+version = "0.36.6"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kraken-build/kraken-build/issues"
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
```

### Comparing `kraken_build-0.36.5/src/kraken/build/__init__.py` & `kraken_build-0.36.6/src/kraken/build/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/build/tests/test_import.py` & `kraken_build-0.36.6/src/kraken/build/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/build/utils/import_helper.py` & `kraken_build-0.36.6/src/kraken/build/utils/import_helper.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/__init__.py` & `kraken_build-0.36.6/src/kraken/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.36.5"
+__version__ = "0.36.6"
 
 from . import path
 from ._argparse import propagate_argparse_formatter_to_subparser
 from ._asciitable import AsciiTable
 from ._auth import CredentialsWithHost
 from ._buildscript import BuildscriptMetadata, BuildscriptMetadataException, buildscript
 from ._date import datetime_to_iso8601, iso8601_to_datetime
```

### Comparing `kraken_build-0.36.5/src/kraken/common/_asciitable.py` & `kraken_build-0.36.6/src/kraken/common/_asciitable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_buildscript.py` & `kraken_build-0.36.6/src/kraken/common/_buildscript.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_buildscript_test.py` & `kraken_build-0.36.6/src/kraken/common/_buildscript_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_date.py` & `kraken_build-0.36.6/src/kraken/common/_date.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_date_test.py` & `kraken_build-0.36.6/src/kraken/common/_date_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_environment.py` & `kraken_build-0.36.6/src/kraken/common/_environment.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_fs.py` & `kraken_build-0.36.6/src/kraken/common/_fs.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_generic.py` & `kraken_build-0.36.6/src/kraken/common/_generic.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_importlib.py` & `kraken_build-0.36.6/src/kraken/common/_importlib.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_option_sets.py` & `kraken_build-0.36.6/src/kraken/common/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_requirements.py` & `kraken_build-0.36.6/src/kraken/common/_requirements.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_requirements_test.py` & `kraken_build-0.36.6/src/kraken/common/_requirements_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_runner.py` & `kraken_build-0.36.6/src/kraken/common/_runner.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_runner_test.py` & `kraken_build-0.36.6/src/kraken/common/_runner_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_text.py` & `kraken_build-0.36.6/src/kraken/common/_text.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_tomlconfig.py` & `kraken_build-0.36.6/src/kraken/common/_tomlconfig.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/_tomlconfig_test.py` & `kraken_build-0.36.6/src/kraken/common/_tomlconfig_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/exceptions.py` & `kraken_build-0.36.6/src/kraken/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/findpython.py` & `kraken_build-0.36.6/src/kraken/common/findpython.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/http/__init__.py` & `kraken_build-0.36.6/src/kraken/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/http/lint_ban_bare_requests.py` & `kraken_build-0.36.6/src/kraken/common/http/lint_ban_bare_requests.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/path.py` & `kraken_build-0.36.6/src/kraken/common/path.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/pyenv/_distributions.py` & `kraken_build-0.36.6/src/kraken/common/pyenv/_distributions.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/pyenv/_virtualenv.py` & `kraken_build-0.36.6/src/kraken/common/pyenv/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/common/supplier.py` & `kraken_build-0.36.6/src/kraken/common/supplier.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/__init__.py` & `kraken_build-0.36.6/src/kraken/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.36.5"
+__version__ = "0.36.6"
 
 from kraken.core.address import Address
 from kraken.core.system.context import Context, ContextEvent
 from kraken.core.system.errors import BuildError, ProjectLoaderError
 from kraken.core.system.executor import Graph
 from kraken.core.system.graph import TaskGraph
 from kraken.core.system.project import Project
```

### Comparing `kraken_build-0.36.5/src/kraken/core/address/_address.py` & `kraken_build-0.36.6/src/kraken/core/address/_address.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/address/_address_resolver.py` & `kraken_build-0.36.6/src/kraken/core/address/_address_resolver.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/address/_address_resolver_test.py` & `kraken_build-0.36.6/src/kraken/core/address/_address_resolver_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/address/_address_test.py` & `kraken_build-0.36.6/src/kraken/core/address/_address_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/address/_addressable.py` & `kraken_build-0.36.6/src/kraken/core/address/_addressable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/base/currentable.py` & `kraken_build-0.36.6/src/kraken/core/base/currentable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/base/metadata.py` & `kraken_build-0.36.6/src/kraken/core/base/metadata.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/cli/executor.py` & `kraken_build-0.36.6/src/kraken/core/cli/executor.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/cli/main.py` & `kraken_build-0.36.6/src/kraken/core/cli/main.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/cli/option_sets.py` & `kraken_build-0.36.6/src/kraken/core/cli/option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/cli/serialize.py` & `kraken_build-0.36.6/src/kraken/core/cli/serialize.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/context.py` & `kraken_build-0.36.6/src/kraken/core/system/context.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/context_test.py` & `kraken_build-0.36.6/src/kraken/core/system/context_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/errors.py` & `kraken_build-0.36.6/src/kraken/core/system/errors.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/executor/__init__.py` & `kraken_build-0.36.6/src/kraken/core/system/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/executor/colored.py` & `kraken_build-0.36.6/src/kraken/core/system/executor/colored.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/executor/default.py` & `kraken_build-0.36.6/src/kraken/core/system/executor/default.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/executor/default_test.py` & `kraken_build-0.36.6/src/kraken/core/system/executor/default_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/executor/utils.py` & `kraken_build-0.36.6/src/kraken/core/system/executor/utils.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/graph.py` & `kraken_build-0.36.6/src/kraken/core/system/graph.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/graph_test.py` & `kraken_build-0.36.6/src/kraken/core/system/graph_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/kraken_object.py` & `kraken_build-0.36.6/src/kraken/core/system/kraken_object.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/project.py` & `kraken_build-0.36.6/src/kraken/core/system/project.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/project_test.py` & `kraken_build-0.36.6/src/kraken/core/system/project_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/property.py` & `kraken_build-0.36.6/src/kraken/core/system/property.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/property_test.py` & `kraken_build-0.36.6/src/kraken/core/system/property_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/task.py` & `kraken_build-0.36.6/src/kraken/core/system/task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/task_supplier.py` & `kraken_build-0.36.6/src/kraken/core/system/task_supplier.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/system/task_test.py` & `kraken_build-0.36.6/src/kraken/core/system/task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/core/testing/__init__.py` & `kraken_build-0.36.6/src/kraken/core/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/buffrs/__init__.py` & `kraken_build-0.36.6/src/kraken/std/buffrs/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/buffrs/manifest.py` & `kraken_build-0.36.6/src/kraken/std/buffrs/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/buffrs/tasks.py` & `kraken_build-0.36.6/src/kraken/std/buffrs/tasks.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/__init__.py` & `kraken_build-0.36.6/src/kraken/std/cargo/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/config.py` & `kraken_build-0.36.6/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/manifest.py` & `kraken_build-0.36.6/src/kraken/std/cargo/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/_cargo_sqlx.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/_cargo_sqlx.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_generate_deb.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_generate_deb.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_login.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_login.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/tasks/rustup_target_add_task.py` & `kraken_build-0.36.6/src/kraken/std/cargo/tasks/rustup_target_add_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/cargo/version.py` & `kraken_build-0.36.6/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/descriptors/resource.py` & `kraken_build-0.36.6/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/dist.py` & `kraken_build-0.36.6/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/__init__.py` & `kraken_build-0.36.6/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/tasks/base_build_task.py` & `kraken_build-0.36.6/src/kraken/std/docker/tasks/base_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/tasks/buildx_build_task.py` & `kraken_build-0.36.6/src/kraken/std/docker/tasks/buildx_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/tasks/docker_build_task.py` & `kraken_build-0.36.6/src/kraken/std/docker/tasks/docker_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/tasks/kaniko_build_task.py` & `kraken_build-0.36.6/src/kraken/std/docker/tasks/kaniko_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/tasks/manifest_tool_push_task.py` & `kraken_build-0.36.6/src/kraken/std/docker/tasks/manifest_tool_push_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/util/dockerapi.py` & `kraken_build-0.36.6/src/kraken/std/docker/util/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docker/util/dockerfile.py` & `kraken_build-0.36.6/src/kraken/std/docker/util/dockerfile.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docs/tasks/mkdocs.py` & `kraken_build-0.36.6/src/kraken/std/docs/tasks/mkdocs.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/docs/tasks/novella.py` & `kraken_build-0.36.6/src/kraken/std/docs/tasks/novella.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/__init__.py` & `kraken_build-0.36.6/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/config.py` & `kraken_build-0.36.6/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/generated.py` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/generated.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/generated_test.py` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/generated_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io.py` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/gitignore_io.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io_test.py` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/gitignore_io_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/gitignore/parser.py` & `kraken_build-0.36.6/src/kraken/std/git/gitignore/parser.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task.py` & `kraken_build-0.36.6/src/kraken/std/git/tasks/check_file_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task_test.py` & `kraken_build-0.36.6/src/kraken/std/git/tasks/check_file_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task.py` & `kraken_build-0.36.6/src/kraken/std/git/tasks/sync_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task_test.py` & `kraken_build-0.36.6/src/kraken/std/git/tasks/sync_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/git/version.py` & `kraken_build-0.36.6/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/helm/__init__.py` & `kraken_build-0.36.6/src/kraken/std/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/helm/helmapi.py` & `kraken_build-0.36.6/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/mitm/__init__.py` & `kraken_build-0.36.6/src/kraken/std/mitm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/mitm/mitm_addon.py` & `kraken_build-0.36.6/src/kraken/std/mitm/mitm_addon.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/protobuf/__init__.py` & `kraken_build-0.36.6/src/kraken/std/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/__init__.py` & `kraken_build-0.36.6/src/kraken/std/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/__init__.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/helpers.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/helpers.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/maturin.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/pdm.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm_test.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/pdm_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/poetry.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry_test.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/poetry_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/buildsystem/slap.py` & `kraken_build-0.36.6/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/pyproject.py` & `kraken_build-0.36.6/src/kraken/std/python/pyproject.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/settings.py` & `kraken_build-0.36.6/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/base_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/black_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/build_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/flake8_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/info_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/info_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/install_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/isort_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/login_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_stubtest_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/mypy_stubtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pex_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_test.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pex_build_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/publish_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pycln_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pylint_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pytest_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_build-0.36.6/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/python/version.py` & `kraken_build-0.36.6/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/sccache.py` & `kraken_build-0.36.6/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/shellcheck.py` & `kraken_build-0.36.6/src/kraken/std/shellcheck.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task.py` & `kraken_build-0.36.6/src/kraken/std/util/check_file_contents_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task_test.py` & `kraken_build-0.36.6/src/kraken/std/util/check_file_contents_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/copyright_task.py` & `kraken_build-0.36.6/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/daemon_controller.py` & `kraken_build-0.36.6/src/kraken/std/util/daemon_controller.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/http.py` & `kraken_build-0.36.6/src/kraken/std/util/http.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/render_file_task.py` & `kraken_build-0.36.6/src/kraken/std/util/render_file_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     """
 
     description = 'Create or update "%(file)s".'
 
     file: Property[Path]
     content: Property[str | bytes]
     encoding: Property[str] = Property.default(DEFAULT_ENCODING)
+    overwrite: Property[bool] = Property.default(True)
 
     def create_check(
         self,
         name: str = "{name}.check",
         task_class: type[CheckFileContentsTask] | None = None,
         description: str | None = None,
         group: str | None = "check",
@@ -45,14 +46,16 @@
         task.depends_on(self, mode="order-only")
         return task
 
     # Task
 
     def prepare(self) -> TaskStatus:
         file = self.file.get()
+        if not self.overwrite.get() and file.exists():
+            return TaskStatus.skipped(f"{file} already exists")
         if file.is_file() and file.read_bytes() == as_bytes(self.content.get(), self.encoding.get()):
             return TaskStatus.up_to_date(f'"{try_relative_to(file)}" is up to date')
         return TaskStatus.pending()
 
     def execute(self) -> TaskStatus:
         file = self.file.get()
         file.parent.mkdir(exist_ok=True, parents=True)
@@ -72,20 +75,22 @@
     project: Project | None = None,
     task_class: type[RenderFileTask] | None = None,
     check_task_class: type[CheckFileContentsTask] | None = None,
     *,
     file: str | Path | Supplier[Path],
     content: str | Supplier[str],
     encoding: str | Supplier[str] = DEFAULT_ENCODING,
+    overwrite: bool | Supplier[bool] = True,
 ) -> tuple[RenderFileTask, CheckFileContentsTask | None]:
     project = project or Project.current()
     render_task = project.task(name, task_class or RenderFileTask, description=description, group=group)
     render_task.file = Path(file) if isinstance(file, str) else file
     render_task.content = content
     render_task.encoding = encoding
+    render_task.overwrite = overwrite
 
     if create_check:
         check_task = render_task.create_check(
             check_name.replace("{name}", name), check_task_class, description=check_description, group=check_group
         )
     else:
         check_task = None
```

### Comparing `kraken_build-0.36.5/src/kraken/std/util/url.py` & `kraken_build-0.36.6/src/kraken/std/util/url.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/validate_readme.py` & `kraken_build-0.36.6/src/kraken/std/util/validate_readme.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/src/kraken/std/util/validate_readme_test.py` & `kraken_build-0.36.6/src/kraken/std/util/validate_readme_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.5/PKG-INFO` & `kraken_build-0.36.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-build
-Version: 0.36.5
+Version: 0.36.6
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,18 +31,14 @@
 Requires-Dist: typing-extensions (>=4.6.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
 Project-URL: Homepage, https://kraken-build.github.io/kraken-build/
 Project-URL: Repository, https://github.com/kraken-build/kraken-build/
 Description-Content-Type: text/markdown
 
----
-title: Home
----
-
 # The Kraken build system
 
 ![kraken-logo](https://i.imgur.com/Lqjy2zi.png)
 
 [![Python](https://github.com/kraken-build/kraken/actions/workflows/python.yaml/badge.svg)](https://github.com/kraken-build/kraken/actions/workflows/python.yaml)
 [![PyPI version](https://badge.fury.io/py/kraken-build.svg)](https://badge.fury.io/py/kraken-build)
 [![Documentation](https://img.shields.io/badge/Documentation-blue?style=flat&logo=gitbook&logoColor=white)](https://kraken-build.github.io/kraken/)
```

