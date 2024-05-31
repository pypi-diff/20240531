# Comparing `tmp/cli_command_parser-2024.5.19.tar.gz` & `tmp/cli_command_parser-2024.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2024.5.19.tar", last modified: Sun May 19 16:15:16 2024, max compression
+gzip compressed data, was "cli_command_parser-2024.5.31.tar", last modified: Fri May 31 10:47:01 2024, max compression
```

## Comparing `cli_command_parser-2024.5.19.tar` & `cli_command_parser-2024.5.31.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.467397 cli_command_parser-2024.5.19/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.19/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.19/MANIFEST.in
--rw-rw-rw-   0        0        0     6002 2024-05-19 16:15:16.467397 cli_command_parser-2024.5.19/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.19/entry_points.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.395397 cli_command_parser-2024.5.19/lib/
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.425398 cli_command_parser-2024.5.19/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1172 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2024-05-19 16:15:02.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0     2876 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19242 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    17578 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5113 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    21162 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    19894 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.447397 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12662 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0     2047 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/cli.py
--rw-rw-rw-   0        0        0    24268 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     8941 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    12652 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    15347 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6781 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8297 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.452396 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     9786 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    21375 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9358 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     7927 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.459397 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6695 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     9525 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     7864 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0     7625 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/patterns.py
--rw-rw-rw-   0        0        0    23981 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     7589 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    17645 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     8144 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.465397 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    17323 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/actions.py
--rw-rw-rw-   0        0        0    26713 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    17287 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    11206 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     8230 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    25503 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11277 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    16870 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    12374 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     2117 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     5858 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:16.466396 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     6002 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-19 16:15:16.000000 cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1991 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/pyproject.toml
--rw-rw-rw-   0        0        0     4483 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/readme.rst
--rw-rw-rw-   0        0        0      116 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.19/requirements-dev.txt
--rw-rw-rw-   0        0        0     1500 2024-05-19 16:15:16.472397 cli_command_parser-2024.5.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.239330 cli_command_parser-2024.5.31/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.31/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     6002 2024-05-31 10:47:01.239330 cli_command_parser-2024.5.31/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.31/entry_points.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.049329 cli_command_parser-2024.5.31/lib/
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.134330 cli_command_parser-2024.5.31/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1172 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2024-05-31 10:46:51.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2876 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19242 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    17578 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5113 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    21162 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    19894 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.174331 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12662 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0     2047 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/cli.py
+-rw-rw-rw-   0        0        0    24268 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     8941 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12652 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15347 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6781 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8297 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.190328 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9786 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    21375 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9358 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     7927 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.206331 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6695 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     9836 2024-05-31 10:46:41.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     7864 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7625 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    23981 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     7589 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    17645 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.237328 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    17323 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    26713 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    17287 2024-05-19 16:14:44.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    11206 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8230 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25503 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11277 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16870 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12374 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     2117 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5858 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:47:01.238329 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     6002 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-31 10:47:01.000000 cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1991 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/pyproject.toml
+-rw-rw-rw-   0        0        0     4483 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/readme.rst
+-rw-rw-rw-   0        0        0      116 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.31/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1500 2024-05-31 10:47:01.243328 cli_command_parser-2024.5.31/setup.cfg
```

### Comparing `cli_command_parser-2024.5.19/LICENSE` & `cli_command_parser-2024.5.31/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/PKG-INFO` & `cli_command_parser-2024.5.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2024.5.19
+Version: 2024.5.31
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
```

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/__init__.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/annotations.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/command_parameters.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/commands.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/commands.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/compat.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/compat.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/config.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/config.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/context.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/context.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/cli.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/command_builder.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/conversion/visitor.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/core.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/core.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/documentation.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/commands.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/params.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,19 @@
     pass_file: bool = InputParam(False)
 
     def __init__(self, converter: Converter, *, pass_file: Bool = False, **kwargs):
         super().__init__(**kwargs)
         self.converter = converter
         self.pass_file = pass_file
 
+    def __repr__(self) -> str:
+        non_defaults = ', '.join(f'{k}={v!r}' for k, v in self.__dict__.items() if k != 'converter')
+        # `converter` must be excluded to prevent infinite recursion when an instance method is stored in that attr
+        return f'<{self.__class__.__name__}({non_defaults})>'
+
     def _prep_file_wrapper(self, path: _Path) -> FileWrapper:
         return FileWrapper(path, self.mode, self.encoding, self.errors, self.converter, self.pass_file, self.parents)
 
 
 class Json(Serialized):
     """
     :param kwargs: Additional keyword arguments to pass to :class:`.File`
```

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/numeric.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/patterns.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/patterns.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/time.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/metadata.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/metadata.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/nargs.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/nargs.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/actions.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/actions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/choice_map.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/option_strings.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/options.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parameters/positionals.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parse_tree.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/parser.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/testing.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/testing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/typing.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/typing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser/utils.py` & `cli_command_parser-2024.5.31/lib/cli_command_parser/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2024.5.19
+Version: 2024.5.31
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
```

### Comparing `cli_command_parser-2024.5.19/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2024.5.31/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/pyproject.toml` & `cli_command_parser-2024.5.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/readme.rst` & `cli_command_parser-2024.5.31/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.5.19/setup.cfg` & `cli_command_parser-2024.5.31/setup.cfg`

 * *Files identical despite different names*

