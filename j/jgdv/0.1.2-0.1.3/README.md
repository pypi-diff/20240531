# Comparing `tmp/jgdv-0.1.2.tar.gz` & `tmp/jgdv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgdv-0.1.2.tar", last modified: Tue Apr 16 14:08:05 2024, max compression
+gzip compressed data, was "jgdv-0.1.3.tar", last modified: Fri May 31 20:25:56 2024, max compression
```

## Comparing `jgdv-0.1.2.tar` & `jgdv-0.1.3.tar`

### file list

```diff
@@ -1,364 +1,64 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.673665 jgdv-0.1.2/
--rw-r-xr--   0 john      (1000) john      (1000)     1425 2024-03-04 06:28:16.000000 jgdv-0.1.2/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     2770 2024-04-16 14:08:05.673665 jgdv-0.1.2/PKG-INFO
--rw-r-xr--   0 john      (1000) john      (1000)       99 2024-03-05 14:03:48.000000 jgdv-0.1.2/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.633665 jgdv-0.1.2/jgdv/
--rw-rw-r--   0 john      (1000) john      (1000)      134 2024-04-16 14:07:14.000000 jgdv-0.1.2/jgdv/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.633665 jgdv-0.1.2/jgdv/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/__tests/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/_interfaces/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/_interfaces/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1154 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/_interfaces/accessors.py
--rw-rw-r--   0 john      (1000) john      (1000)     1603 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/_interfaces/decorator.py
--rw-rw-r--   0 john      (1000) john      (1000)     1013 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/_interfaces/factory.py
--rw-rw-r--   0 john      (1000) john      (1000)     1611 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/_interfaces/loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     1004 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/_interfaces/policy.py
--rw-rw-r--   0 john      (1000) john      (1000)     2485 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/_interfaces/singletons.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/_types/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/_types/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.629665 jgdv-0.1.2/jgdv/apis/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/apis/clingo/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/clingo/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/apis/clingo/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/clingo/__tests/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4845 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/clingo/__tests/test_clingo_solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     3317 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/clingo/ast.py
--rw-rw-r--   0 john      (1000) john      (1000)     5648 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/clingo_solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     1521 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/compiler.py
--rw-rw-r--   0 john      (1000) john      (1000)     8264 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/parser.py
--rw-rw-r--   0 john      (1000) john      (1000)     1579 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/reporter.py
--rw-rw-r--   0 john      (1000) john      (1000)     1976 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     4795 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/trace.py
--rw-rw-r--   0 john      (1000) john      (1000)     7513 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/clingo/validate.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/apis/mastodon/
--rw-rw-r--   0 john      (1000) john      (1000)      448 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/mastodon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     7368 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/mastodon/actions.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/mastodon/error.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/apis/selenium/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/selenium/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/apis/selenium/selenium.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/apis/sphinx/
--rw-rw-r--   0 john      (1000) john      (1000)     1540 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/apis/sphinx/directive.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/cli/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/cli/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/cli/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)    13496 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/__tests/test_flexible.py
--rw-rw-r--   0 john      (1000) john      (1000)    11350 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/arg_parser.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.637665 jgdv-0.1.2/jgdv/cli/repl/
--rw-rw-r--   0 john      (1000) john      (1000)      207 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.641665 jgdv-0.1.2/jgdv/cli/repl/commands/
--rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/cli/repl/commands/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5368 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/break_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     1304 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/commands_info.py
--rw-rw-r--   0 john      (1000) john      (1000)     2878 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/control.py
--rw-rw-r--   0 john      (1000) john      (1000)      827 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/exit_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     3029 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/force_parser_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     1984 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/init_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     4393 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/log_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2570 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/memory_cmds.py
--rw-rw-r--   0 john      (1000) john      (1000)     4401 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/print_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     6044 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/report_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)      986 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/tutorial_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2774 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/commands/util.py
--rw-rw-r--   0 john      (1000) john      (1000)     6042 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/repl_commander.py
--rw-rw-r--   0 john      (1000) john      (1000)     3959 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/repl/repl_dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/cli/repl/repl_state.py
--rw-rw-r--   0 john      (1000) john      (1000)     6745 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/shell.py
--rw-rw-r--   0 john      (1000) john      (1000)     2979 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/cli/speak.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.641665 jgdv-0.1.2/jgdv/debugging/
--rw-rw-r--   0 john      (1000) john      (1000)       54 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/debugging/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4923 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/debugging/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     1871 2024-04-15 21:52:45.000000 jgdv-0.1.2/jgdv/debugging/frame_helper.py
--rw-rw-r--   0 john      (1000) john      (1000)     1861 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/debugging/human.py
--rw-rw-r--   0 john      (1000) john      (1000)     5609 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/debugging/malloc.py
--rw-rw-r--   0 john      (1000) john      (1000)     2092 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/debugging/running_debugger.py
--rw-rw-r--   0 john      (1000) john      (1000)     3758 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/debugging/timing.py
--rw-rw-r--   0 john      (1000) john      (1000)     1738 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/debugging/trace_helper.py
--rw-rw-r--   0 john      (1000) john      (1000)     1954 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/debugging/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.641665 jgdv-0.1.2/jgdv/decorators/
--rw-rw-r--   0 john      (1000) john      (1000)     3752 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     1838 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/breakpoint.py
--rw-rw-r--   0 john      (1000) john      (1000)     1180 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/decorators/check_protocol.py
--rw-rw-r--   0 john      (1000) john      (1000)     1844 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/destruction.py
--rw-rw-r--   0 john      (1000) john      (1000)      694 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     1170 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/logging.py
--rw-rw-r--   0 john      (1000) john      (1000)     2926 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/decorators/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.641665 jgdv-0.1.2/jgdv/dsl/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/dsl/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/dsl/consts.py
--rw-rw-r--   0 john      (1000) john      (1000)     1150 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/dsl/ctors.py
--rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/dsl/funcs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1519 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/dsl/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/enums/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/enums/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1272 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/enums/location_meta.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/enums/loop_control.py
--rw-rw-r--   0 john      (1000) john      (1000)     1137 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/enums/task_response.py
--rw-rw-r--   0 john      (1000) john      (1000)     1565 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/enums/task_state.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/error/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/error/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      997 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/error/repl.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/binary/
--rw-rw-r--   0 john      (1000) john      (1000)    13689 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/binary/infinity.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/bookmarks/
--rw-rw-r--   0 john      (1000) john      (1000)     2772 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/bookmarks/bookmark.py
--rw-rw-r--   0 john      (1000) john      (1000)     2829 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/bookmarks/collection.py
--rw-rw-r--   0 john      (1000) john      (1000)     3490 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/bookmarks/netscape.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/epub/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/epub/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      907 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/epub/epub.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/gif/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/gif/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2249 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/gif/gif_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)     1821 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/gif/make_gif.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/graph/
--rw-rw-r--   0 john      (1000) john      (1000)     2046 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/graph/pickles.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/jinja/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/jinja/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3743 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     1654 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/mem_map.py
--rw-rw-r--   0 john      (1000) john      (1000)     1723 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/metadata.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/org/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/org/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      668 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/org/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     2603 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/org/drawer.py
--rw-rw-r--   0 john      (1000) john      (1000)     1918 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/org/file.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/pdf/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/pdf/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4343 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/pdf/pdf.py
--rw-rw-r--   0 john      (1000) john      (1000)     1056 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/sha256.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.645665 jgdv-0.1.2/jgdv/files/tags/
--rw-rw-r--   0 john      (1000) john      (1000)     3361 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/tags/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     3657 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tags/graph.py
--rw-rw-r--   0 john      (1000) john      (1000)     3233 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tags/index.py
--rw-rw-r--   0 john      (1000) john      (1000)     3051 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tags/substitutions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3507 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tar.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.649665 jgdv-0.1.2/jgdv/files/tex/
--rw-rw-r--   0 john      (1000) john      (1000)      112 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/tex/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2628 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/tex/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      984 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tex/bib.py
--rw-rw-r--   0 john      (1000) john      (1000)     1356 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tex/envs.py
--rw-rw-r--   0 john      (1000) john      (1000)     7114 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tex/gantt.py
--rw-rw-r--   0 john      (1000) john      (1000)     7439 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tex/pdf.py
--rw-rw-r--   0 john      (1000) john      (1000)     1075 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/tex/statements.py
--rw-rw-r--   0 john      (1000) john      (1000)     1157 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/tex/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.649665 jgdv-0.1.2/jgdv/files/timeline/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/timeline/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1479 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/timeline/entry.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/timeline/reader.py
--rw-rw-r--   0 john      (1000) john      (1000)     3991 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/timeline/timeline.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/timeline/writer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.649665 jgdv-0.1.2/jgdv/files/twitter/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.649665 jgdv-0.1.2/jgdv/files/twitter/__test/
--rw-rw-r--   0 john      (1000) john      (1000)     2125 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/__test/component_example.json
--rw-rw-r--   0 john      (1000) john      (1000)      979 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/__test/test_file_processing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4210 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/__test/tweet_example.json
--rw-rw-r--   0 john      (1000) john      (1000)     3341 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/__test/user_example.json
--rw-rw-r--   0 john      (1000) john      (1000)      854 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     6516 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/twitter/mixin_passes.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.649665 jgdv-0.1.2/jgdv/files/twitter/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1576 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/structs/thread.py
--rw-rw-r--   0 john      (1000) john      (1000)     1744 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/structs/todo_list.py
--rw-rw-r--   0 john      (1000) john      (1000)     1877 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/structs/tweet.py
--rw-rw-r--   0 john      (1000) john      (1000)     5131 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/tweet_graph.py
--rw-rw-r--   0 john      (1000) john      (1000)     3202 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/files/twitter/writers/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/writers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4125 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/writers/json_component.py
--rw-rw-r--   0 john      (1000) john      (1000)     3496 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/writers/lazy_json_component.py
--rw-rw-r--   0 john      (1000) john      (1000)     5601 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/twitter/writers/thread.py
--rw-rw-r--   0 john      (1000) john      (1000)     6958 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/files/twitter/writers/tweet.py
--rw-rw-r--   0 john      (1000) john      (1000)     1601 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/writers/users_table.py
--rw-rw-r--   0 john      (1000) john      (1000)     1134 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/twitter/writers/util.py
--rw-rw-r--   0 john      (1000) john      (1000)     1487 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/files/zip.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/dcel/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1068 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/constants.py
--rw-rw-r--   0 john      (1000) john      (1000)      918 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/dcel.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/dcel/io/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/io/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3368 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/io/drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     6611 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/io/export.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/dcel/mod/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/mod/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8161 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/mod/adding.py
--rw-rw-r--   0 john      (1000) john      (1000)     8846 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/mod/processing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4322 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/mod/subtracting.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/dcel/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1363 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/draw_settings.py
--rw-rw-r--   0 john      (1000) john      (1000)     1072 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/drawable.py
--rw-rw-r--   0 john      (1000) john      (1000)    26133 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/face.py
--rw-rw-r--   0 john      (1000) john      (1000)    36447 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/halfedge.py
--rw-rw-r--   0 john      (1000) john      (1000)     6413 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/line.py
--rw-rw-r--   0 john      (1000) john      (1000)     5372 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/state.py
--rw-rw-r--   0 john      (1000) john      (1000)    11203 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/dcel/structs/vertex.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.653665 jgdv-0.1.2/jgdv/geom/intersection/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/intersection/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/intersection/result.py
--rw-rw-r--   0 john      (1000) john      (1000)     1965 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/intersection/state.py
--rw-rw-r--   0 john      (1000) john      (1000)    13125 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/intersection/sweep.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/geom/math/
--rw-rw-r--   0 john      (1000) john      (1000)     4782 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/bbox.py
--rw-rw-r--   0 john      (1000) john      (1000)     4083 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/circles.py
--rw-rw-r--   0 john      (1000) john      (1000)     4760 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/direction.py
--rw-rw-r--   0 john      (1000) john      (1000)     3573 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/distance.py
--rw-rw-r--   0 john      (1000) john      (1000)     4664 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/heightmap.py
--rw-rw-r--   0 john      (1000) john      (1000)     8233 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/lines.py
--rw-rw-r--   0 john      (1000) john      (1000)     4585 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/math/movement.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/geom/voronoi/
--rw-rw-r--   0 john      (1000) john      (1000)     2993 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/beachline.py
--rw-rw-r--   0 john      (1000) john      (1000)     1232 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/breakpoint.py
--rw-rw-r--   0 john      (1000) john      (1000)     4072 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/data.py
--rw-rw-r--   0 john      (1000) john      (1000)     9358 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/geom/voronoi/drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     3019 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/events.py
--rw-rw-r--   0 john      (1000) john      (1000)     2484 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/graph.py
--rw-rw-r--   0 john      (1000) john      (1000)    12980 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/line_sweep.py
--rw-rw-r--   0 john      (1000) john      (1000)    21188 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/geom/voronoi/process.py
--rw-rw-r--   0 john      (1000) john      (1000)    21184 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/geom/voronoi/voronoi.py
--rw-rw-r--   0 john      (1000) john      (1000)     9358 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/geom/voronoi/voronoi_drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     1118 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/geom/voronoi/voronoi_io.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/handlers/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/handlers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2740 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/handlers/handler.py
--rw-rw-r--   0 john      (1000) john      (1000)    16665 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/handlers/handler_system.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/importing/
--rw-rw-r--   0 john      (1000) john      (1000)     1808 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/importing/inspect.py
--rw-rw-r--   0 john      (1000) john      (1000)     5986 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/importing/plugin_loader.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/keys/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9347 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     9418 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/decorator.py
--rw-rw-r--   0 john      (1000) john      (1000)     3958 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/formatter.py
--rw-rw-r--   0 john      (1000) john      (1000)     2573 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/multikey.py
--rw-rw-r--   0 john      (1000) john      (1000)     3252 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/path_keys.py
--rw-rw-r--   0 john      (1000) john      (1000)     8046 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/keys/simple.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.657665 jgdv-0.1.2/jgdv/location/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/location/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8220 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/location/locations.py
--rw-rw-r--   0 john      (1000) john      (1000)     2397 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/location/toml_loc.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.661665 jgdv-0.1.2/jgdv/logging/
--rw-rw-r--   0 john      (1000) john      (1000)       87 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/logging/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4525 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/logging/log_colour.py
--rw-rw-r--   0 john      (1000) john      (1000)     5737 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/logging/log_config.py
--rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/logging/log_context.py
--rw-rw-r--   0 john      (1000) john      (1000)     3809 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/logging/stdout_capture.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.661665 jgdv-0.1.2/jgdv/math/
--rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2992 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/colour.py
--rw-rw-r--   0 john      (1000) john      (1000)     5165 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/comparison.py
--rw-rw-r--   0 john      (1000) john      (1000)     5037 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/easings.py
--rw-rw-r--   0 john      (1000) john      (1000)     1670 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/matrices.py
--rw-rw-r--   0 john      (1000) john      (1000)     8413 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/parabola.py
--rw-rw-r--   0 john      (1000) john      (1000)     2947 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/quadratic.py
--rw-rw-r--   0 john      (1000) john      (1000)     1310 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/quantize.py
--rw-rw-r--   0 john      (1000) john      (1000)     1159 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/rand.py
--rw-rw-r--   0 john      (1000) john      (1000)     1412 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/sorting.py
--rw-rw-r--   0 john      (1000) john      (1000)    26889 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/umath.py
--rw-rw-r--   0 john      (1000) john      (1000)     2900 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/math/utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.661665 jgdv-0.1.2/jgdv/mixins/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/mixins/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2117 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/mixins/enums.py
--rw-rw-r--   0 john      (1000) john      (1000)     1184 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/mixins/param_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     7354 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/mixins/path_manip.py
--rw-rw-r--   0 john      (1000) john      (1000)     8951 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/mixins/zipper.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.661665 jgdv-0.1.2/jgdv/setup/
--rw-rw-r--   0 john      (1000) john      (1000)     2080 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/asyncio_client.py
--rw-rw-r--   0 john      (1000) john      (1000)     2557 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/asyncio_server.py
--rw-rw-r--   0 john      (1000) john      (1000)      969 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/gtk.py
--rw-rw-r--   0 john      (1000) john      (1000)     3470 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/setup/hooks.py
--rw-rw-r--   0 john      (1000) john      (1000)     1189 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/importing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4226 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/setup/main.py
--rw-rw-r--   0 john      (1000) john      (1000)     1087 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/pyparsing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4571 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/setup/setup.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/setup/tkinter.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/spiders/
--rw-rw-r--   0 john      (1000) john      (1000)     2238 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/spiders/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/spiders/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     7020 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/__tests/test_runner.py
--rw-rw-r--   0 john      (1000) john      (1000)    11494 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/__tests/test_tracker.py
--rw-rw-r--   0 john      (1000) john      (1000)     1558 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/actions.py
--rw-rw-r--   0 john      (1000) john      (1000)     5438 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/spiders/caching.py
--rw-rw-r--   0 john      (1000) john      (1000)     2645 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/spiders/crawler.py
--rw-rw-r--   0 john      (1000) john      (1000)     4602 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/spiders/middleware.py
--rw-rw-r--   0 john      (1000) john      (1000)     2638 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)     4830 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/spiders/pipeline.py
--rw-rw-r--   0 john      (1000) john      (1000)    11326 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/runner.py
--rw-rw-r--   0 john      (1000) john      (1000)     1854 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/spiders.py
--rw-rw-r--   0 john      (1000) john      (1000)     8343 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/spiders/tracker.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/structs/
--rw-rw-r--   0 john      (1000) john      (1000)     4820 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/artifact.py
--rw-rw-r--   0 john      (1000) john      (1000)     6726 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/code_ref.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/structs/heap/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/heap/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1520 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/heap/element.py
--rw-rw-r--   0 john      (1000) john      (1000)     1643 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/heap/heap.py
--rw-rw-r--   0 john      (1000) john      (1000)     3911 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/name.py
--rw-rw-r--   0 john      (1000) john      (1000)    11727 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/param_spec.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/structs/proxy/
--rw-rw-r--   0 john      (1000) john      (1000)     6094 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/proxy/base.py
--rw-rw-r--   0 john      (1000) john      (1000)    12758 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/proxy/iter_proxy.py
--rw-rw-r--   0 john      (1000) john      (1000)     6312 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/proxy/proxy.py
--rw-rw-r--   0 john      (1000) john      (1000)     3265 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/proxy/proxy_mixin.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/structs/rbtree/
--rw-rw-r--   0 john      (1000) john      (1000)      378 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.665665 jgdv-0.1.2/jgdv/structs/rbtree/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/__tests/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3733 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/rbtree/__tests/test_rbtree.py
--rw-rw-r--   0 john      (1000) john      (1000)     7495 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/rbtree/__tests/test_rbtree_node.py
--rw-rw-r--   0 john      (1000) john      (1000)     3262 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/comparison_functions.py
--rw-rw-r--   0 john      (1000) john      (1000)     1708 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/node.py
--rw-rw-r--   0 john      (1000) john      (1000)     7171 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/operations.py
--rw-rw-r--   0 john      (1000) john      (1000)     1735 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/rb_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     8673 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/rbtree.py
--rw-rw-r--   0 john      (1000) john      (1000)     5268 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rbtree/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1259 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/regex.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/rete/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rete/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rete/alpha.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rete/beta.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/rete/rete.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/time/
--rw-rw-r--   0 john      (1000) john      (1000)      173 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/time/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)    12753 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/time/__tests/test_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1675 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     5217 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/pattern_constructor.py
--rw-rw-r--   0 john      (1000) john      (1000)      889 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/pattern_iterator.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/time/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1566 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/arc.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/event.py
--rw-rw-r--   0 john      (1000) john      (1000)     5558 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/pattern.py
--rw-rw-r--   0 john      (1000) john      (1000)      968 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/structs/var.py
--rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/time/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1835 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/trace.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/tree/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/tree/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11147 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/tree/binary_tree.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/structs/trie/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/trie/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3069 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/structs/trie/leaf.py
--rw-rw-r--   0 john      (1000) john      (1000)     6186 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/trie/semantics.py
--rw-rw-r--   0 john      (1000) john      (1000)     3407 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/structs/trie/trie.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/testing/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/testing/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1748 2024-04-16 13:57:51.000000 jgdv-0.1.2/jgdv/testing/testing_fixtures.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv/utils/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/utils/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1107 2024-04-15 14:39:20.000000 jgdv-0.1.2/jgdv/utils/slice.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 14:08:05.669665 jgdv-0.1.2/jgdv.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     2770 2024-04-16 14:08:05.000000 jgdv-0.1.2/jgdv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     8341 2024-04-16 14:08:05.000000 jgdv-0.1.2/jgdv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-16 14:08:05.000000 jgdv-0.1.2/jgdv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)      144 2024-04-16 14:08:05.000000 jgdv-0.1.2/jgdv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        5 2024-04-16 14:08:05.000000 jgdv-0.1.2/jgdv.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     3920 2024-04-16 14:07:14.000000 jgdv-0.1.2/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-16 14:08:05.673665 jgdv-0.1.2/setup.cfg
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.562135 jgdv-0.1.3/
+-rw-r-xr--   0 john      (1000) john      (1000)     1425 2024-03-04 06:28:16.000000 jgdv-0.1.3/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2794 2024-05-31 20:25:56.562135 jgdv-0.1.3/PKG-INFO
+-rw-r-xr--   0 john      (1000) john      (1000)       99 2024-03-05 14:03:48.000000 jgdv-0.1.3/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.550135 jgdv-0.1.3/jgdv/
+-rw-rw-r--   0 john      (1000) john      (1000)      105 2024-05-31 20:25:02.000000 jgdv-0.1.3/jgdv/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/_abstract/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/_abstract/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      894 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/_abstract/factory.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6705 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/_abstract/protocols.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1334 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/_types.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/debugging/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/debugging/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1859 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/debugging/human.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/decorators/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/decorators/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3531 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/decorators/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1180 2024-04-15 14:39:20.000000 jgdv-0.1.3/jgdv/decorators/check_protocol.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6989 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/decorators/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/enums/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.3/jgdv/enums/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1270 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/enums/location_meta.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1423 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/enums/loop_control.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1207 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/enums/task_response.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1512 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/enums/task_state.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2117 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/enums/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/files/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.554135 jgdv-0.1.3/jgdv/files/bookmarks/
+-rw-rw-r--   0 john      (1000) john      (1000)       83 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/files/bookmarks/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3218 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/files/bookmarks/bookmark.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2928 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/files/bookmarks/collection.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/files/tags/
+-rw-rw-r--   0 john      (1000) john      (1000)       80 2024-05-20 20:01:39.000000 jgdv-0.1.3/jgdv/files/tags/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/files/tags/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1354 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/tags/__tests/example.index
+-rw-rw-r--   0 john      (1000) john      (1000)      453 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/tags/__tests/test.sub
+-rw-rw-r--   0 john      (1000) john      (1000)      325 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/tags/__tests/test.tags
+-rw-rw-r--   0 john      (1000) john      (1000)     3904 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/tags/__tests/test_base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3553 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/files/tags/__tests/test_substitutions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4044 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/files/tags/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3769 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/files/tags/substitutions.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/logging/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/logging/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/logging/context.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1514 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/logging/filter.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/structs/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/structs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1255 2024-05-31 20:23:22.000000 jgdv-0.1.3/jgdv/structs/regex.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/testing/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/testing/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1356 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/testing/tempdir.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv/util/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/util/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1599 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/util/chain_get.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1099 2024-04-19 18:55:03.000000 jgdv-0.1.3/jgdv/util/slice.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-31 20:25:56.558135 jgdv-0.1.3/jgdv.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2794 2024-05-31 20:25:56.000000 jgdv-0.1.3/jgdv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1224 2024-05-31 20:25:56.000000 jgdv-0.1.3/jgdv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-05-31 20:25:56.000000 jgdv-0.1.3/jgdv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      153 2024-05-31 20:25:56.000000 jgdv-0.1.3/jgdv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        5 2024-05-31 20:25:56.000000 jgdv-0.1.3/jgdv.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     3947 2024-05-31 20:25:02.000000 jgdv-0.1.3/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-05-31 20:25:56.562135 jgdv-0.1.3/setup.cfg
```

### Comparing `jgdv-0.1.2/LICENSE` & `jgdv-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.2/PKG-INFO` & `jgdv-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgdv
-Version: 0.1.2
+Version: 0.1.3
 Author-email: John Grey <jgrey.n.plus.one+dejavu@gmail.com>
 License: * ACAB License
         
         © 2024-03-04 John Grey
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -52,14 +52,15 @@
 Requires-Dist: selenium
 Requires-Dist: numpy
 Requires-Dist: scrapy
 Requires-Dist: pyparsing
 Requires-Dist: construct
 Requires-Dist: networkx
 Requires-Dist: pygobject
+Requires-Dist: pydantic
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: doot; extra == "dev"
 Requires-Dist: pipreqs; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>7.0.0; extra == "test"
```

### Comparing `jgdv-0.1.2/jgdv/_interfaces/accessors.py` & `jgdv-0.1.3/jgdv/_abstract/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
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
@@ -32,17 +32,7 @@
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-
-def __set_name__(self, owner, name):
-    self.public_name = name
-    self.private_name = "_" + name
-
-def __get__(self, obj, objtype=None):
-    return getattr(obj, self.private_name)
-
-def __set__(self, obj, value):
-    setattr(obj, self.private_name, value)
```

### Comparing `jgdv-0.1.2/jgdv/_interfaces/decorator.py` & `jgdv-0.1.3/jgdv/testing/tempdir.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,40 +26,32 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class JGDVDecorator_i:
-    """ Base Class for decorators that annotate callables """
-
-    def __init__(self, funcOrCls:Callable):
-        ftz.update_wrapper(self, funcOrCls)
-        self._func = func
-
-    def __call__(self, *args, **kwargs):
-        return self._func(*args, **kwargs)
-
-class JGDVDelayDecorator_i:
-    """ Base Class for decorators that take arguments, then later annotate callables
-
-    https://stackoverflow.com/questions/9416947
+import pytest
+import os
+import tempfile
+
+@pytest.fixture
+def wrap_tmp(tmp_path):
+    """ create a new temp directory, and change cwd to it,
+      returning to original cwd after the test
       """
-
-    def __init__(self):
-        self._func = None
-
-    def __call__(self, func):
-        self._func = func
-        ftz.update_wrapper(self._wrapper, self._func)
-        return self._wrapper
-
-    def _wrapper(self, *args, **kwargs):
-        return
+    logging.debug("Moving to temp dir")
+    orig     = pl.Path().cwd()
+    new_base = tmp_path / "test_root"
+    new_base.mkdir()
+    os.chdir(new_base)
+    yield new_base
+    logging.debug("Returning to original dir")
+    os.chdir(orig)
```

### Comparing `jgdv-0.1.2/jgdv/_interfaces/factory.py` & `jgdv-0.1.3/jgdv/_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 #!/usr/bin/env python3
 """
-
+Types that help add clarity
 
 See EOF for license/metadata/notes as applicable
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
 import time
 import types
 import weakref
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generator,
+                    Generic, Iterable, Iterator, Mapping, Match, NewType,
+                    MutableMapping, Protocol, Sequence, Tuple, TypeAlias,
+                    TypeGuard, TypeVar, cast, final, overload, Optional,
+                    runtime_checkable)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class Factory_p(abc.ABC):
+# TODO when in py3.12 use 'type' kw
+
+T                       = TypeVar("T")
+
+Stack                   = NewType("Stack", list[T])
+Queue                   = NewType("Queue", list[T])
+Vector                  = NewType("Vector", list[float])
+
+Identifier              = NewType("Identifier", str)
+
+Depth                   = NewType("Depth", int)
+Seconds                 = NewType("Seconds", int)
 
-    @classmethod
-    @abc.abstractmethod
-    def build(cls, *args, **kwargs):
-        pass
+Maybe         TypeAlias = Optional
```

### Comparing `jgdv-0.1.2/jgdv/apis/mastodon/actions.py` & `jgdv-0.1.3/jgdv/decorators/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,199 @@
-#!/usr/bin/env python3
 """
-
-
-See EOF for license/metadata/notes as applicable
+Utility decorators
 """
-
-##-- builtin imports
+#pylint: disable=invalid-sequence-index
+##-- imports
 from __future__ import annotations
 
-# import abc
-import datetime
-import enum
-import functools as ftz
-import itertools as itz
 import logging as logmod
-import pathlib as pl
-import re
-import time
-import types
-import weakref
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
-                    Iterable, Iterator, Mapping, Match, MutableMapping,
-                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
-from uuid import UUID, uuid1
-
-##-- end builtin imports
-
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+from enum import Enum
+from functools import wraps
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Dict, Generic,
+                    Iterable, Iterator, List, Mapping, Match, MutableMapping,
+                    Optional, ParamSpec, Sequence, Set, Tuple, TypeAlias,
+                    TypeVar, Union, cast)
+
+##-- end imports
 
 ##-- logging
-logging = logmod.getLogger(__name__)
+logging                                      = logmod.getLogger(__name__)
 ##-- end logging
 
-printer = logmod.getLogger("doot._printer")
+import inspect
 
-import mastodon
-import tomlguard
-from jgdv.apis.mastodon import errors as djerror
-from jgdv.key import JGDVKey
-
-TOOT_SIZE            : Final[int]                   = doot.config.on_fail(250, int).mastodon.toot_size()
-TOOT_IMAGE_SIZE      : Final[str]                   = doot.config.on_fail(8_000_000, int).mastodon.image_size()
-RESOLUTION_BLACKLIST : Final[list]                  = doot.locs.image_blacklist
-RESOLUTION_RE        : Final[re.Pattern]            = re.compile(r".*?([0-9]+x[0-9]+)")
-TOOT_IMAGE_TYPES     : Final[list[str]]             = [".jpg", ".png", ".gif"]
-
-##-- expansion keys
-INSTANCE_KEY           : Final[DootKey]                        = DootKey.make("mastodon")
-TEXT_KEY               : Final[DootKey]                        = DootKey.make("toot_text")
-IMAGE_KEY              : Final[DootKey]                        = DootKey.make("toot_image")
-IMAGE_DESC             : Final[DootKey]                        = DootKey.make("toot_desc")
-UPDATE                 : Final[DootKey]                        = DootKey.make("update_")
-FROM_KEY               : Final[DootKey]                        = DootKey.make("from")
-SECRETS                : Final[DootKey]                        = DootKey.make("mastodon_secrets")
-##-- end expansion keys
-
-
-class MastodonSetup:
-    """ Default Mastodon Setup, using secrets from doot.locs.mastodon_secrets
-      loads the secrets as a tomlguard, and accesses mastodon.access_token and mastodon.url
-      ensures thers an "image_temp" location
-    """
-    instance = None
-    _toml_kwargs = [INSTANCE_KEY, FROM_KEY]
-
-    def __call__(self, spec, task_state) -> dict|bool|None:
-        data_key = INSTANCE_KEY.redirect(spec)
-
-        if MastodonSetup.instance is None:
-            printer.info("---------- Initialising Mastodon", extra={"colour": "green"})
-            secrets_path = FROM_KEY.to_path(spec, task_state, chain=SECRETS)
-            secrets = tomlguard.load(secrets_path)
-            MastodonSetup.instance = mastodon.Mastodon(
-                access_token = secrets.mastodon.access_token,
-                api_base_url = secrets.mastodon.url
-            )
-            doot.locs.ensure("image_temp", task=task_state['_task_name'])
-        else:
-            printer.debug("Reusing Instance")
-
-        return { data_key : MastodonSetup.instance }
-
-
-
-class MastodonPost:
-    """ Default Mastodon Poster  """
-    _toml_kwargs = [INSTANCE_KEY, FROM_KEY, IMAGE_KEY, IMAGE_DESC, TEXT_KEY]
-
-    def __call__(self, spec, task_state):
-        instance           = INSTANCE_KEY.to_type(spec, task_state, type_=Mastodon.Mastodon)
-        text               = FROM_KEY.redirect(spec, chain=TEXT_KEY).expand(spec, task_state)
-        image_path         = IMAGE_KEY.to_path(spec, task_state)
-        image_desc         = IMAGE_DESC.expand(spec, task_state)
-
-        try:
-            if image_path.exists():
-                return self._post_image(instance, text, image_path, image_desc)
-            else:
-                return self._post_text(instance, text)
-        except mastodon.MastodonAPIError as err:
-            general, errcode, form, detail = err.args
-            resolution                     = RESOLUTION_RE.match(detail) if detail else None
-            if resolution and resolution in self.resolution_blacklist:
-                pass
-            elif errcode == 422 and form == "Unprocessable Entity" and resolution:
-                with open(RESOLUTION_BLACKLIST, 'a') as f:
-                    f.write("\n" + resolution[1])
+JGDV_ANNOTATIONS : Final[str]                = "__JGDV_ANNOTATIONS__"
+KEYS_HANDLED     : Final[str]                = "_jgdv_keys_handler"
+ORIG_ARGS        : Final[str]                = "_jgdv_orig_args"
+KEY_ANNOTS       : Final[str]                = "_jgdv_keys"
+FUNC_WRAPPED     : Final[str]                = "__wrapped__"
+PARAM_PREFIX     : Final[str]                = "_"
+PARAM_SUFFIX     : Final[str]                = "_ex"
+
+class DecorationUtils:
+
+    _annot = JGDV_ANNOTATIONS
+
+    @staticmethod
+    def _unwrap(fn:callable) -> callable:
+        # if not hasattr(fn, FUNC_WRAPPED):
+        #     return fn
+
+        # return getattr(fn, FUNC_WRAPPED)
+        return inspect.unwrap(fn)
+
+    @staticmethod
+    def verify_signature(fn, head:list, tail:list=None) -> bool:
+        match fn:
+            case inspect.Signature():
+                sig = fn
+            case _:
+                sig = inspect.signature(fn, follow_wrapped=False)
+
+        params      = list(sig.parameters)
+        tail        = tail or []
+        for x,y in zip(params, head):
+            if x != y:
+                logging.debug("Mismatch in signature head: %s != %s", x, y)
+                return False
+
+        for x,y in zip(params[::-1], tail[::-1]):
+            key_str = str(y)
+            if x.startswith(PARAM_PREFIX) or x.endswith(PARAM_SUFFIX):
+                continue
+            if keyword.iskeyword(key_str):
+                logging.debug("Key is a keyword, the function sig needs to use _{} or {}_ex: %s : %s", x, y)
+                return False
+            if not key_str.isidentifier():
+                logging.debug("Key is not an identifier, the function sig needs to use _{} or {}_ex: %s : %s", x,y)
+                return False
+
+            if x != y:
+                logging.debug("Mismatch in signature tail: %s != %s", x, y)
+                return False
 
-            printer.error("Mastodon Resolution Failure: %s", repr(err))
-            return False
-        except Exception as err:
-            printer.error("Mastodon Post Failed: %s", repr(err))
-            return False
+        return True
 
-    def _post_text(self, instance, text):
-        printer.info("Posting Text Toot: %s", text)
-        if len(text) >= TOOT_SIZE:
-            printer.warning("Resulting Toot too long for mastodon: %s\n%s", len(text), text)
+    def verify_action_signature(fn:Signature|callable, args:list) -> bool:
+        match fn:
+            case inspect.Signature():
+                sig = fn
+            case _:
+                sig = inspect.signature(fn, follow_wrapped=False)
+
+        match sig.parameters.get("self", None):
+            case None:
+                head_sig = ["spec", "state"]
+            case _:
+                head_sig = ["self", "spec", "state"]
+
+        return DecorationUtils.verify_signature(sig, head_sig, args)
+
+    @staticmethod
+    def manipulate_signature(fn, args) -> callable:
+        pass
+
+    @staticmethod
+    def has_annotations(fn, *keys) -> bool:
+        if not hasattr(fn, JGDV_ANNOTATIONS):
             return False
 
-        result = instance.status_post(text)
-        return True
+        annots = getattr(fn, JGDV_ANNOTATIONS)
+        return all(key in annots for key in keys)
 
-    def _post_image(self, instance, text, image_path, image_desc):
-        printer.info("Posting Image Toot")
+    @staticmethod
+    def annotate(fn:callable, annots:dict|set) -> callable:
+        match annots:
+            case dict():
+                fn.__dict__.update(annots)
+            case set():
+                if not hasattr(fn, JGDV_ANNOTATIONS):
+                    setattr(fn, JGDV_ANNOTATIONS, set())
+
+                annotations = getattr(fn, JGDV_ANNOTATIONS)
+                annotations.update(annots)
+        return fn
+
+    @staticmethod
+    def truncate_signature(fn):
+        """
+           actions are (self?, spec, state)
+          with and extracted keys from the spec and state.
+          This truncates the signature of the action to what is *called*, not what is *used*.
+
+          TODO: could take a callable as the prototype to build the signature from
+        """
+        sig = inspect.signature(fn)
+        min_index = len(sig.parameters) - len(getattr(fn, KEY_ANNOTS))
+        newsig = sig.replace(parameters=list(sig.parameters.values())[:min_index])
+        fn.__signature__ = newsig
+        return fn
+
+    @staticmethod
+    def _update_key_annotations(fn, keys:list[JGDVKey]) -> True:
+        """ update the declared expansion keys on the wrapped action """
+        sig = inspect.signature(fn)
+
+        # prepend annotations, so written decorator order is the same as written arg order:
+        # (ie: @wrap(x) @wrap(y) @wrap(z) def fn (x, y, z), even though z's decorator is applied first
+        new_annotations = keys + getattr(fn, KEY_ANNOTS, [])
+        setattr(fn, KEY_ANNOTS, new_annotations)
 
-        assert(image_path.exists()), f"File Doesn't Exist {image_path}"
-        assert(image_path.stat().st_size < TOOT_IMAGE_SIZE), "Image to large, needs to be smaller than 8MB"
-        assert(image_path.suffix.lower() in TOOT_IMAGE_TYPES), "Bad Type, needs to be a jpg, png or gif"
-
-        media_id = instance.media_post(str(image_path), description=image_desc)
-        instance.status_post(text, media_ids=media_id)
-        logging.debug("Image Toot Posted")
-        return True
+        if not DecorationUtils.verify_action_signature(sig, new_annotations):
+            raise doot.errors.DootKeyError("Annotations do not match signature", sig)
 
-    def _handle_resolution(self, task):
-        # post to mastodon
-        with open(RESOLUTION_BLACKLIST, 'r') as f:
-            resolution_blacklist = {x.strip() for x in f.readlines()}
-
-        min_x, min_y = inf, inf
-
-        if bool(resolution_blacklist):
-            min_x        = min(int(res.split("x")[0]) for res in resolution_blacklist)
-            min_y        = min(int(res.split("x")[1]) for res in resolution_blacklist)
-
-        res : str    = _get_resolution(selected_file)
-        res_x, res_y = res.split("x")
-        res_x, res_y = int(res_x), int(res_y)
-        if res in resolution_blacklist or (min_x <= res_x and min_y <= res_y):
-            logging.warning("Image is too big %s: %s", selected_file, res)
-            return
-
-    def _get_resolution(self, filepath:Path) -> str:
-        result = subprocess.run(["file", str(filepath)], capture_output=True, shell=False)
-        if result.returncode == 0:
-            res = RESOLUTION_RE.match(result.stdout.decode())
-            return res[1]
-
-        raise djerror.DootActionError("Couldn't get image resolution", filepath, result.stdout.decode(), result.stderr.decode())
-
-    def _maybe_compress_file(self, task):
-        image = task.values['image']
-        logging.debug("Attempting compression of: %s", image)
-        assert(isinstance(filepath, pl.Path) and filepath.exists())
-        ext               = filepath.suffix
-        conversion_target = doot.locs.image_temp.with_suffix(ext)
-        convert_cmd = self.make_cmd(["convert", str(filepath),
-                                    *conversion_args,
-                                    str(conversion_target)])
-        convert_cmd.execute()
+        return True
 
-        if doot.locs.image_temp.stat().st_size < 5000000:
-            return { 'image': doot.locs.image_temp }
+    @staticmethod
+    def prepare_expansion(keys:list[JGDVKey], fn):
+        """ used as a partial fn. adds declared keys to a function,
+          and idempotently adds the expansion decorator
+        """
+        is_func = True
+        match DecorationUtils._unwrap(fn):
+            case x if DecorationUtils.has_annotations(x, KEYS_HANDLED):
+                DecorationUtils._update_key_annotations(x, keys)
+                return fn
+            case orig:
+                is_func = inspect.signature(orig).parameters.get("self", None) is None
+                DecorationUtils._update_key_annotations(x, keys)
+                DecorationUtils.annotate(orig, {KEYS_HANDLED})
+
+        match is_func:
+            case False:
+                wrapper = DecorationUtils.add_method_expander(fn)
+            case True:
+                wrapper = DecorationUtils.add_fn_expander(fn)
+
+        return wrapper
+
+    @staticmethod
+    def add_method_expander(fn):
+
+        @ftz.wraps(fn)
+        def method_action_expansions(self, spec, state, *call_args, **kwargs):
+            try:
+                expansions = [x(spec, state) for x in getattr(fn, KEY_ANNOTS)]
+            except KeyError as err:
+                printer.warning("Action State Expansion Failure: %s", err)
+                return False
+            all_args = (*call_args, *expansions)
+            return fn(self, spec, state, *all_args, **kwargs)
+
+        # -
+        return method_action_expansions
+
+    @staticmethod
+    def add_fn_expander(fn):
+
+        @ftz.wraps(fn)
+        def fn_action_expansions(spec, state, *call_args, **kwargs):
+            try:
+                expansions = [x(spec, state) for x in getattr(fn, KEY_ANNOTS)]
+            except KeyError as err:
+                printer.warning("Action State Expansion Failure: %s", err)
+                return False
+            all_args = (*call_args, *expansions)
+            return fn(spec, state, *all_args, **kwargs)
 
-        return False
+        # -
+        return fn_action_expansions
```

### Comparing `jgdv-0.1.2/jgdv/apis/mastodon/error.py` & `jgdv-0.1.3/jgdv/structs/regex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
-"""
 
+"""
 
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
@@ -16,23 +16,39 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
+from dataclasses import dataclass
+import re
+
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
+
+@dataclass
+class RegexEqual(str):
+    """ https://martinheinz.dev/blog/78 """
+    string : str
+    match :  re.Match = None
+
+    def __eq__(self, pattern):
+        self.match = re.search(pattern, self.string)
+        return self.match is not None
+
+    def __getitem__(self, group):
+        return self.match[group]
```

### Comparing `jgdv-0.1.2/jgdv/apis/sphinx/directive.py` & `jgdv-0.1.3/jgdv/enums/loop_control.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -26,36 +25,31 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from docutils import nodes
-from docutils.parsers.rst import Directive, directives
-from docutils.statemachine import StringList
+from jgdv.enums.util import EnumBuilder_m, FlagsBuilder_m
 
-def setup(app):
-    """
-    Adds the directive `.. $1::` for use in rst-files
+class LoopControl(EnumBuilder_m, enum.Enum):
     """
-    app.add_directive("$1", $2Directive)
+      A Simple enum to descrbe results for testing in a maybe recursive loop
+      (like walking a a tree)
 
-class $2Directive(Directive):
-    has_content        = False
-    required_arguments = 0
-    optional_arguments = 0
-
-    the_text = ""
-
-    def run(self):
-        container          = nodes.literal_block()
-        translated_content = StringList($2Directive.the_text.splitlines(keepends=False))
-        self.state.nested_parse(translated_content, 0, container)
-        return [container]
+    accept  : is a result, and descend if recursive
+    keep    : is a result, don't descend
+    discard : not a result, descend
+    reject  : not a result, don't descend
+    """
+    yesAnd  = enum.auto()
+    yes     = enum.auto()
+    noBut   = enum.auto()
+    no      = enum.auto()
```

### Comparing `jgdv-0.1.2/jgdv/cli/repl/commands/tutorial_cmd.py` & `jgdv-0.1.3/jgdv/enums/location_meta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 #!/usr/bin/env python3
-##-- imports
+"""
+
+
+See EOF for license/metadata/notes as applicable
+"""
+
+##-- builtin imports
 from __future__ import annotations
 
-import abc
+# import abc
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
-from dataclasses import InitVar, dataclass, field
+import pathlib as pl
+import re
+import time
+import types
+import weakref
+# from copy import deepcopy
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
 
-##-- end imports
+##-- end builtin imports
 
+##-- lib imports
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
+
+##-- logging
 logging = logmod.getLogger(__name__)
+##-- end logging
+
+from jgdv.enums.util import EnumBuilder_m, FlagsBuilder_m
+
+class LocationMeta(FlagsBuilder_m, enum.Flag):
+    """ Available metadata attachable to a location """
 
-@register_class("tutorial")
-class TutorialCmd:
-    """
-    Print out a basic tutorial of Acab and this Repl
-    """
-
-    def __init__(self):
-        self._parser = self._gen_parser()
-
-    def _gen_parser(self):
-        pass
-
-    def __call__(self, line):
-        # Print a section, return to main loop,
-        # if tutorial is called again, continue
-        # if restart is passed in, restart the tutorial
-        # also include option to print tutorial for a module
-        return
+    default      = enum.auto()
+    file         = enum.auto()
+    protected    = enum.auto()
+    indefinite   = enum.auto()
+    cleanable    = enum.auto()
+    normOnLoad   = enum.auto()
```

### Comparing `jgdv-0.1.2/jgdv/debugging/frame_helper.py` & `jgdv-0.1.3/jgdv/enums/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 #!/usr/bin/env python3
 """
 
+
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
 # import abc
-# import datetime
-# import enum
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
+import weakref
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
+
+##-- end builtin imports
 
-##-- end imports
+##-- lib imports
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import sys
+class EnumBuilder_m:
+    """ A Mixin to add a .build(str) method for the enum """
 
-class FrameHelper:
-    """
-      Utility to work with python frames and tracebacks
-    """
-
-    def __init__(self):
-        self.frames = []
-        self.get_frames()
-
-    def __getitem__(self, val=None):
-        match val:
-            case None:
-                return self.to_tb()
-            case slice() | int():
-                return self.to_tb(self.frames[val])
-            case _:
-                raise TypeError("Bad value passed to TraceHelper")
-
-    def get_frames(self):
-        """ from https://stackoverflow.com/questions/27138440 """
-        tb    = None
-        depth = 0
-        while True:
+    @classmethod
+    def build(cls, val:str) -> Self:
+        try:
+            match val:
+                case str():
+                    return cls[val]
+                case cls():
+                    return val
+        except KeyError:
+            logging.warning("Can't Create a flag of (%s):%s. Available: %s", cls, val, list(cls.__members__.keys()))
+
+class FlagsBuilder_m:
+    """ A Mixin to add a .build(vals) method for EnumFlags """
+
+    @classmethod
+    def build(cls, vals:str|list|dict) -> Self:
+        match vals:
+            case str():
+                vals = [vals]
+            case list():
+                pass
+            case dict():
+                vals = [x for x,y in vals.items() if bool(y)]
+
+        base = cls.default
+        for x in vals:
             try:
-                frame = sys._getframe(depth)
-                depth += 1
-            except ValueError as exc:
-                break
-
-            self.frames.append(frame)
-
-    def to_tb(self, frames=None):
-        top = None
-        frames = frames or self.frames
-        for frame in frames:
-            top = types.TracebackType(top, frame,
-                                     frame.f_lasti,
-                                     frame.f_lineno)
-        return top
+                match x:
+                    case str():
+                        base |= cls[x]
+                    case cls():
+                        base |= x
+            except KeyError:
+                logging.warning("Can't create a flag of (%s):%s. Available: %s", cls, x, list(cls.__members__.keys()))
+
+        return base
```

### Comparing `jgdv-0.1.2/jgdv/debugging/human.py` & `jgdv-0.1.3/jgdv/debugging/human.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 
 class HumanNum:
     """
     Simple human number related functions
     """
 
     @staticmethod
-    def human_sizes(val, format=False):
+    def size(val:int, format=False) -> str:
         return tracemalloc._format_size(val, format)
 
     @staticmethod
-    def round_time(dt:DateTime=None, roundTo:Seconds=60) -> DateTime:
+    def time(dt:DateTime=None, roundTo:Seconds=60) -> DateTime:
         """Round a datetime object to any time lapse in seconds
         dt : datetime.datetime object, default now.
         roundTo : Closest number of seconds to round to, default 1 minute.
         Author: Thierry Husson 2012 - Use it as you want but don't blame me.
         from: https://stackoverflow.com/questions/3463930
         """
         dt       = dt or datetime.datetime.now()
```

### Comparing `jgdv-0.1.2/jgdv/decorators/base.py` & `jgdv-0.1.3/jgdv/decorators/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,19 +32,16 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-printer = logmod.getLogger("doot._printer")
-
 import inspect
 import abc
-import builtins
 from typing import Type
 import decorator
 
 FUNC_WRAPPED     : Final[str]                = "__wrapped__"
 jgdv_ANNOTATIONS : Final[str]                = "__JGDV_ANNOTATIONS__"
 WRAPPER          : Final[str]                = "__wrapper"
 
@@ -69,58 +66,49 @@
 
         if isinstance(fn, Type):
             return self.wrap_method(fn, fn.__call__, self._wrapper)
 
         decorated = decorator.decorate(fn, self._wrapper)
         return decorated
 
-    @staticmethod
-    def _strip_wrappers(fn:callable) -> callable:
-        # if not hasattr(fn, FUNC_WRAPPED):
-        #     return fn
-
-        # return getattr(fn, FUNC_WRAPPED)
+    def _strip_wrappers(self, fn:callable) -> callable:
         return inspect.unwrap(fn)
 
-    @staticmethod
-    def has_annotations(fn, *keys) -> bool:
-        base = JGDVDecorator._strip_wrappers(fn)
+    def has_annotations(self, fn, *keys) -> bool:
+        base = self._strip_wrappers(fn)
         if not hasattr(base, jgdv_ANNOTATIONS):
             return False
 
         annots = getattr(base, jgdv_ANNOTATIONS)
         return all(key in annots for key in keys)
 
-    @staticmethod
-    def annotate(fn:callable, annots:set) -> callable:
-        base = JGDVDecorator._strip_wrappers(fn)
+    def annotate(self, fn:callable, annots:set) -> callable:
+        base = self._strip_wrappers(fn)
         if not hasattr(base, jgdv_ANNOTATIONS):
             setattr(base, jgdv_ANNOTATIONS, set())
 
         annotations = getattr(base, jgdv_ANNOTATIONS)
         for cls in getattr(fn, '__mro__', []):
             annotations.update(getattr(cls, jgdv_ANNOTATIONS, {}))
 
         annotations.update(annots)
         return fn
 
-    @staticmethod
-    def wrap_method(obj:Type, method:callable, wrapper:callable) -> Type:
+    def wrap_method(self, obj:Type, method:callable, wrapper:callable) -> Type:
         wrapped = decorator.decorate(method, wrapper)
         setattr(obj, method.__name__, wrapped)
         return obj
 
-    @staticmethod
-    def truncate_signature(fn):
+    def truncate_signature(self, fn):
         """
            actions are (self?, spec, state)
           with and extracted keys from the spec and state.
           This truncates the signature of the action to what is *called*, not what is *used*.
 
           TODO: could take a callable as the prototype to build the signature from
         """
-        sig = inspect.signature(fn)
-        min_index = len(sig.parameters) - len(getattr(fn, "_doot_keys"))
-        newsig = sig.replace(parameters=list(sig.parameters.values())[:min_index])
+        sig              = inspect.signature(fn)
+        min_index        = len(sig.parameters) - len(getattr(fn, "_doot_keys"))
+        newsig           = sig.replace(parameters=list(sig.parameters.values())[:min_index])
         fn.__signature__ = newsig
         return fn
```

### Comparing `jgdv-0.1.2/jgdv/decorators/breakpoint.py` & `jgdv-0.1.3/jgdv/decorators/check_protocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
-See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
 import datetime
@@ -25,41 +23,19 @@
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
-
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from jgdv._interfaces.decorator import JGDVDecorator_i
-from jgdv.debugginer.running_debugger import RunningDebugger
-
-class JGDVBreakpoint(JGDVDecorator_i):
-    """
-      Decorator to attach a debugger to a function, without pausing execution
-    """
-
-    def __call__(self, *args, **kwargs):
-        # TODO handle repeats
-        if args[0].breakpoint:
-            f_code = f.__code__
-            db = RunningDebugger()
-            # Ensure trace function is set
-            sys.settrace(db.trace_dispatch)
-            if not db.get_break(f_code.co_filename, f_code.co_firstlineno+2):
-                db.set_break(f_code.co_filename,
-                            f_code.co_firstlineno+2,
-                            True)
-            else:
-                bp = Breakpoint.bplist[f_code.co_filename,
-                                    f_code.co_firstlineno+2][0]
-                bp.enable()
+def check_protocol(cls):
+    """ Decorator. Check the class implements all its methods / has no abstractmethods """
 
+    abstracts = [x for x in dir(cls) if hasattr(getattr(cls, x), "__isabstractmethod__") and getattr(cls, x).__isabstractmethod__]
+    if bool(abstracts):
+        raise NotImplementedError(f"Class has Abstract Methods: {cls.__module__} : {cls.__name__} : {abstracts}")
 
-        return self._func(self, *args, **kwargs)
+    return cls
```

### Comparing `jgdv-0.1.2/jgdv/enums/location_meta.py` & `jgdv-0.1.3/jgdv/enums/task_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,17 @@
 # from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from jgdv.mixins.enums import EnumBuilder_m, FlagsBuilder_m
+from jgdv.enums.util import EnumBuilder_m, FlagsBuilder_m
 
-class LocationMeta(FlagsBuilder_m, enum.Flag):
-    """ Available metadata attachable to a location """
-
-    default      = enum.auto()
-    file         = enum.auto()
-    protected    = enum.auto()
-    indefinite   = enum.auto()
-    cleanable    = enum.auto()
-    normOnLoad   = enum.auto()
+class TaskResponseEnum(EnumBuilder_m, enum.Enum):
+    """
+      Enums for how a task can describe its response
+    """
+    SUCCEED  = enum.auto()
+    FAIL     = enum.auto()
+    SKIP     = enum.auto()
+    HALT     = enum.auto()
```

### Comparing `jgdv-0.1.2/jgdv/enums/loop_control.py` & `jgdv-0.1.3/jgdv/util/slice.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 """
 
+
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -25,29 +26,19 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-# import more_itertools as mitz
-# from boltons import
+import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class LoopControl(enum.Enum):
+def build_slice(toks:dict) -> slice:
     """
-      A Simple enum to descrbe results for testing in a maybe recursive loop
-      (like walking a a tree)
-
-    accept  : is a result, and descend if recursive
-    keep    : is a result, don't descend
-    discard : not a result, descend
-    reject  : not a result, don't descend
+      Utility to create a slice from a dict(first=None|int(), second=None|int())
     """
-    yesAnd  = enum.auto()
-    yes     = enum.auto()
-    noBut   = enum.auto()
-    no      = enum.auto()
+    return slice(toks.get("first", None), toks.get("second", None))
```

### Comparing `jgdv-0.1.2/jgdv/enums/task_state.py` & `jgdv-0.1.3/jgdv/enums/task_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,20 +34,19 @@
 # from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from jgdv.mixins.enums import EnumBuilder_m, FlagsBuilder_m
+from jgdv.enums.util import EnumBuilder_m, FlagsBuilder_m
 
-class TaskStateEnum(enum.Enum):
+class TaskStateEnum(EnumBuilder_m, enum.Enum):
     """
       Enumeration of the different states a task can be in.
-      The state is stored in a TaskTracker_i, not the task itself
     """
     TEARDOWN        = enum.auto()
     SUCCESS         = enum.auto()
     FAILED          = enum.auto()
     HALTED          = enum.auto()
     WAIT            = enum.auto()
     READY           = enum.auto()
```

### Comparing `jgdv-0.1.2/jgdv/files/bookmarks/bookmark.py` & `jgdv-0.1.3/jgdv/files/bookmarks/bookmark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -16,85 +15,92 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+                    cast, final, overload, runtime_checkable, Generator, Self)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-TAG_NORM : Final[re.Pattern] = re.compile(" +")
+from pydantic import BaseModel, Field, model_validator, field_validator, ValidationError
 
-@dataclass
-class Bookmark:
-    url     : str      = field()
-    tags    : Set[str] = field(default_factory=set)
-    name    : str      = field(default="No Name")
-    sep     : str      = field(default=" : ")
+class Bookmark(BaseModel):
+    url              : str
+    tags             : set[str]              = set()
+    name             : str                   = "No Name"
+    _tag_sep         : ClassVar[str]         = " : "
+    _tag_norm_re     : ClassVar[re.Pattern]  = re.compile(" +")
 
     @staticmethod
     def build(line:str, sep=None):
         """
         Build a bookmark from a line of a bookmark file
         """
-        sep  = sep or Bookmark.sep
+        sep  = sep or Bookmark._tag_sep
         tags = []
         match [x.strip() for x in line.split(sep)]:
             case []:
                 raise TypeException("Bad line passed to Bookmark")
             case [url]:
                 logging.warning("No Tags for: %s", url)
             case [url, *tags]:
                 pass
 
-        return Bookmark(url,
-                        set(tags),
+        return Bookmark(url=url,
+                        tags=set(tags),
                         sep=sep)
 
-    def __post_init__(self):
-        self.tags = {TAG_NORM.sub("_", x.strip()) for x in self.tags}
+    @field_validator("tags", mode="before")
+    def _validate_tags(cls, val):
+        match val:
+            case list()|set():
+                return { Bookmark._tag_norm_re.sub("_", x.strip()) for x in val }
+            case str():
+                return { Bookmark._tag_norm_re.sub("_", x.strip()) for x in val.split(Boomark._tag_sep) }
+            case _:
+                raise ValueError("Unrecognized tags base", val)
 
     def __eq__(self, other):
         return self.url == other.url
 
     def __lt__(self, other):
         return self.url < other.url
 
     def __str__(self):
-        tags = self.sep.join(sorted(self.tags))
-        return f"{self.url}{self.sep}{tags}"
+        sep = Bookmark._tag_sep
+        tags = sep.join(sorted(self.tags))
+        return f"{self.url}{sep}{tags}"
 
     @property
     def url_comps(self) -> url_parse.ParseResult:
         return url_parse.urlparse(self.url)
 
-    def merge(self, other) -> 'Bookmark':
+    def merge(self, other) -> Self:
         """ Merge two bookmarks' tags together,
         creating a new bookmark
         """
         assert(self == other)
-        merged = Bookmark(self.url,
-                          self.tags.union(other.tags),
-                          self.name,
-                          sep=self.sep)
+        merged = Bookmark(url=self.url,
+                          tags=self.tags.union(other.tags),
+                          name=self.name)
         return merged
 
     def clean(self, subs):
         """
         run tag substitutions on all tags in the bookmark
         """
         cleaned_tags = set()
```

### Comparing `jgdv-0.1.2/jgdv/files/bookmarks/collection.py` & `jgdv-0.1.3/jgdv/files/bookmarks/collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -16,15 +15,15 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
@@ -33,19 +32,21 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-@dataclass
-class BookmarkCollection:
+from pydantic import BaseModel, Field, model_validator, field_validator, ValidationError
+from jgdv.files.bookmarks.bookmark import Bookmark
+
+class BookmarkCollection(BaseModel):
 
-    entries : List[Bookmark] = field(default_factory=list)
-    ext     : str            = field(default=".bookmarks")
+    entries : list[Bookmark] = []
+    ext     : str            = ".bookmarks"
 
     @staticmethod
     def read(fpath:pl.Path) -> BookmarkCollection:
         """ Read a file to build a bookmark collection """
         bookmarks = BookmarkCollection()
         for line in (x.strip() for x in fpath.read_text().split("\n")):
             if not bool(line):
@@ -70,14 +71,15 @@
         return value in self.entries
 
     def __len__(self):
         return len(self.entries)
 
     def __hash__(self):
         return id(self)
+
     def update(self, *values):
         for val in values:
             match val:
                 case Bookmark():
                     self.entries.append(val)
                 case BookmarkCollection():
                     self.entries += val.entries
```

### Comparing `jgdv-0.1.2/jgdv/files/metadata.py` & `jgdv-0.1.3/jgdv/logging/filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,41 +26,29 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import sh
-
-def exiftool_pdf_md(path) -> str:
-    result = ""
-    try:
-        response = subprocess.run(["exiftool", str(path), "-PDF:all"],
-                                  capture_output=True,
-                                  shell=False)
-        result = response.stdout.decode() if response.returncode == 0 else response.stderr.decode()
-
-    except Exception as err:
-        result = str(err)
-
-    return result
-
-def exiftool_xmp_md(path) -> str:
-    result = ""
-    try:
-        response = subprocess.run(["exiftool", str(path), "-XMP:all"],
-                                  capture_output=True,
-                                  shell=False)
-        result = response.stdout.decode() if response.returncode == 0 else response.stderr.decode()
-
-    except Exception as err:
-        result = str(err)
-
-    return result
+class JGDVAnyFilter:
+    """
+      A Logging filter to white and blacklist regexs of logger names
+    """
+
+    def __init__(self, names=None, reject=None):
+        self.names      = names or []
+        self.rejections = reject or []
+        self.name_re    = re.compile("^({})".format("|".join(self.names)))
+
+    def __call__(self, record):
+        return (record.name not in self.rejections) and (record.name == "root"
+                                                         or not bool(self.names)
+                                                        or self.name_re.match(record.name))
```

### Comparing `jgdv-0.1.2/jgdv/files/tags/base.py` & `jgdv-0.1.3/jgdv/files/tags/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+ #!/usr/bin/env python3
 """
 
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
@@ -15,54 +15,70 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
+from collections import defaultdict
+from pydantic import BaseModel, field_validator, model_validator
+
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 TAG_NORM : Final[re.Pattern] = re.compile(" +")
 
-@dataclass
-class TagFile:
+class TagFile(BaseModel):
     """ A Basic TagFile holds the counts for each tag use """
 
-    counts : dict[str, int] = field(default_factory=lambda: defaultdict(lambda: 0))
-    sep    : str            = field(default=" : ")
-    ext    : str            = field(default=".tags")
+    counts : dict[str, int] = defaultdict(lambda: 0)
+    sep    : str            = " : "
+    ext    : str            = ".tags"
 
-    norm_regex : re.Pattern  = TAG_NORM
+    norm_regex : ClassVar[re.Pattern]  = TAG_NORM
 
     @classmethod
     def read(cls, fpath:pl.Path, sep=None) -> TagFile:
         obj = cls(sep=sep or cls.sep)
         for i, line in enumerate(fpath.read_text().split("\n")):
             try:
                 obj.update(tuple(x.strip() for x in line.split(obj.sep)))
             except Exception as err:
-                logging.warning("Failure Tag Reading %s (l:%s) : %s : %s", fpath, i, err, line)
+                logging.warning("Failure Tag Read: (l:%s) : %s : %s : (file: %s)", i, err, line, fpath)
 
         return obj
 
+    @field_validator("counts", mode="before")
+    def _validate_counts(cls, val):
+        counts = defaultdict(lambda: 0)
+        match val:
+            case dict():
+                counts.update(val)
+        return counts
+
+    @model_validator(mode="after")
+    def _normalize_counts(self):
+        orig = self.counts
+        self.counts = defaultdict(lambda: 0)
+        self.counts.update({self.norm_tag(x):y for x,y in orig.items()})
+
     def __iter__(self):
         return iter(self.counts)
 
     def __str__(self):
         """
         Export the counts, 1 entry per line, as:
         `key` : `value`
@@ -73,46 +89,49 @@
                 continue
             all_lines.append(self.sep.join([key, str(self.counts[key])]))
         return "\n".join(all_lines)
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: {len(self)}>"
 
-    def __iadd__(self, values):
+    def __iadd__(self, values:TagFile|str|dict|set):
+        """  merge tags, updating their counts as well. """
         return self.update(values)
 
     def __len__(self):
         return len(self.counts)
 
     def __contains__(self, value):
         return self.norm_tag(value) in self.counts
 
-    def _inc(self, key, *, amnt=1):
+    def _inc(self, key, *, amnt=1) -> None|str:
         norm_key = self.norm_tag(key)
+        if not bool(norm_key):
+            return None
         self.counts[norm_key] += amnt
         return norm_key
 
-    def update(self, *values):
+    def update(self, *values:str|TagFile|set|dict):
         for val in values:
             match val:
                 case None | "":
                     continue
                 case str():
                     self._inc(val)
-                case [str() as key]:
-                    self._inc(key)
-                case (str() as key, str() as counts):
+                case list() | set():
+                    self.update(*val)
+                case dict():
+                    self.update(*val.items())
+                case (str() as key, int()|str() as counts):
                     self._inc(key, amnt=int(counts))
                 case TagFile():
-                    self.update(*values.counts.items())
-                case set():
-                    self.update(*val)
+                    self.update(*val.counts.items())
         return self
 
-    def to_set(self) -> Set[str]:
+    def to_set(self) -> set[str]:
         return set(self.counts.keys())
 
     def get_count(self, tag):
         return self.counts[self.norm_tag(tag)]
 
     def norm_tag(self, tag):
-        return self.norm_regex.sub("_", tag.strip())
+        return TagFile.norm_regex.sub("_", tag.strip())
```

### Comparing `jgdv-0.1.2/jgdv/files/twitter/structs/thread.py` & `jgdv-0.1.3/jgdv/util/chain_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 #!/usr/bin/env python3
-##-- imports
+"""
+
+See EOF for license/metadata/notes as applicable
+"""
+
+##-- builtin imports
 from __future__ import annotations
 
+# import abc
 import datetime
-import json
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
 import pathlib as pl
-from collections import defaultdict
-from dataclasses import InitVar, dataclass, field
-from typing import (Any, Callable, ClassVar, Dict, Generic, Iterable, Iterator,
-                    List, Mapping, Match, MutableMapping, Optional, Sequence,
-                    Set, Tuple, TypeVar, Union, cast)
-from uuid import uuid1
-
-import networkx as nx
-##-- end imports
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
 
+##-- logging
 logging = logmod.getLogger(__name__)
+##-- end logging
+
+class ChainedKeyGetter:
+    """
+      The core logic to turn a key into a value.
+      Doesn't perform repeated expansions.
 
-@dataclass
-class TwitterThreadObj:
-    """ Utility Class to hold a thread
-    doesn't hold the tweets themselves, just ID's
+      tries sources in order.
     """
-    main      : list[str]       = field(default_factory=list)
-    rest      : list[list[str]] = field(default_factory=list)
-    quotes    : list[str]       = field(default_factory=list)
-    component : pl.Path         = field(default=None)
-    base_user : str             = field(default=None)
 
     @staticmethod
-    def build(data):
-        assert(all([x in data for x in ["main_thread",
-                                        "rest",
-                                        "quotes"]]))
-
-        return TwitterThreadObj(data["main_thread"],
-                                data["rest"],
-                                data["quotes"])
-
-    def dump(self):
-        return {
-            'main_thread' : self.main,
-            'rest'        : self.rest,
-            'quotes'      : self.quotes,
-            'component'   : self.component,
-            'base_user'   : self.base_user,
-            }
+    def chained_get(key:str, *sources:dict|JGDVLocations) -> Any:
+        # cli   : dict          = doot.args.on_fail({}).tasks[str(state.get(STATE_TASK_NAME_K, None))]()
+        # replacement           = cli.get(key, None)
+        # *Not* elif's, want it to chain.
+        for source in sources:
+            if source is None:
+                continue
+            replacement = source.get(key, None)
+            if replacement is not None:
+                return replacement
 
+        return None
```

### Comparing `jgdv-0.1.2/jgdv/keys/formatter.py` & `jgdv-0.1.3/jgdv/files/tags/substitutions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -16,100 +15,99 @@
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 import weakref
 # from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-# import more_itertools as mitz
-# from boltons import
+import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class JGDVFormatter(string.Formatter):
-    """
-      A Formatter for expanding arguments based on action spec kwargs, and task state, and cli args
-    """
-    _fmt                = None
-
-    SPEC   : Final[str] = "_spec"
-    INSIST : Final[str] = "_insist"
-    STATE  : Final[str] = "_state"
-    LOCS   : Final[str] = "_locs"
-    REC    : Final[str] = "_rec"
-
-    @staticmethod
-    def fmt(fmt:str|DootKey|pl.Path, /, *args, **kwargs) -> str:
-        if not DootFormatter._fmt:
-            DootFormatter._fmt = DootFormatter()
-
-        return DootFormatter._fmt.format(fmt, *args, **kwargs)
-
-    def format(self, fmt:str|DootKey|pl.Path, /, *args, **kwargs) -> str:
-        """ expand and coerce keys """
-        self._depth = 0
-        match kwargs.get(self.SPEC, None):
-            case None:
-                kwargs['_spec'] = {}
-            case SpecStruct_p():
-                kwargs['_spec'] = kwargs[self.SPEC].params
-            case x:
-                raise TypeError("Bad Spec Type in Format Call", x)
-
-        match fmt:
-            case DootKey():
-                fmt = fmt.form
-                result = self.vformat(fmt, args, kwargs)
-            case str():
-                result = self.vformat(fmt, args, kwargs)
-            # case pl.Path():
-            #     result = str(ftz.reduce(pl.Path.joinpath, [self.vformat(x, args, kwargs) for x in fmt.parts], pl.Path()))
-            case _:
-                raise TypeError("Unrecognized expansion type", fmt)
-
-        return result
-
-    def get_value(self, key, args, kwargs):
-        """ lowest level handling of keys being expanded """
-        logging.debug("Expanding: %s", key)
-        if isinstance(key, int):
-            return args[key]
-
-        insist                = kwargs.get(self.INSIST, False)
-        spec  : dict          = kwargs.get(self.SPEC, None) or {}
-        state : dict          = kwargs.get(self.STATE, None) or {}
-        locs  : DootLocations = kwargs.get(self.LOCS,  None)
-        depth_check           = self._depth < MAX_KEY_EXPANSIONS
-        rec_allowed           = kwargs.get(self.REC, False) and depth_check
-
-        match (replacement:=DootKeyGetter.chained_get(key, spec, state, locs)):
-            case None if insist:
-                raise KeyError("Key Expansion Not Found")
-            case None:
-                return DootKey.build(key).form
-            case DootKey() if depth_check:
-                self._depth += 1
-                return self.vformat(replacement.form, args, kwargs)
-            case str() if rec_allowed:
-                self._depth += 1
-                return self.vformat(str(replacement), args, kwargs)
-            case str():
-                return replacement
-            case pl.Path() if depth_check:
-                self._depth += 1
-                return ftz.reduce(pl.Path.joinpath, map(lambda x: self.vformat(x, args, kwargs), replacement.parts), pl.Path())
-            case _:
-                return str(replacement)
-                # raise TypeError("Replacement Value isn't a string", args, kwargs)
+from collections import defaultdict
+from jgdv.files.tags.base import TagFile
+
+class SubstitutionFile(TagFile):
+    """ SubstitutionFiles add a replacement tag for some tags """
+
+    ext           : str                  = ".sub"
+    substitutions : dict[str, set[str]]  = defaultdict(set)
+
+    def __str__(self):
+        """
+        Export the substitutions, 1 entry per line, as:
+        `key` : `counts` : `substitution`
+        """
+        all_lines = []
+        for key in sorted(self.counts.keys()):
+            if not bool(self.substitutions[key]):
+                continue
+            line = [key, str(self.counts[key])]
+            line += sorted(self.substitutions[key])
+            all_lines.append(self.sep.join(line))
+
+        return "\n".join(all_lines)
+
+    def __getitem__(self, key) -> set[str]:
+        return self.sub(key)
+
+    def canonical(self) -> TagFile:
+        """ create a tagfile of just canonical tags"""
+        # All substitutes are canonical
+        canon = {x:1 for x in iter(self) if not self.has_sub(x)}
+        return TagFile(counts=canon)
+
+    def sub(self, value:str) -> set[str]:
+        """ apply a substitution if it exists """
+        normed = self.norm_tag(value)
+        if bool(self.substitutions.get(normed, None)):
+            return self.substitutions[normed]
+
+        return set([normed])
+
+    def has_sub(self, value):
+        normed = self.norm_tag(value)
+        if normed != value:
+            return True
+        return bool(self.substitutions.get(normed, None))
+
+    def update(self, *values:str|Tuple|dict|SubstitutionFile|TagFile|set):
+        for val in values:
+            match val:
+                case None | "": # empty line
+                    continue
+                case str(): # just a tag
+                    self._inc(val)
+                case list() | set():
+                    for key in val:
+                        self._inc(key)
+                case dict(): # tag and count
+                    for key, val in val.items():
+                        self._inc(key, amnt=val)
+                case (str() as key, int() | str() as counts): # tag and count
+                    self._inc(key, amnt=int(counts))
+                case (str() as key, int() | str() as counts, *subs):
+                    norm_key  = self._inc(key, amnt=int(counts))
+                    norm_subs = [normed for x in subs if (normed:=self.norm_tag(x)) is not None]
+                    self.update({x:1 for x in norm_subs}) # Add to normal counts too
+                    self.substitutions[norm_key].update(norm_subs)
+                case SubstitutionFile():
+                    self.update(val.counts)
+                    for tag, subs in val.substitutions.items():
+                        self.substitutions[tag].update(subs)
+                case TagFile():
+                    self.update(val.counts.items())
+
+        return self
```

### Comparing `jgdv-0.1.2/jgdv/logging/log_context.py` & `jgdv-0.1.3/jgdv/logging/context.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.2/jgdv.egg-info/PKG-INFO` & `jgdv-0.1.3/jgdv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgdv
-Version: 0.1.2
+Version: 0.1.3
 Author-email: John Grey <jgrey.n.plus.one+dejavu@gmail.com>
 License: * ACAB License
         
         © 2024-03-04 John Grey
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -52,14 +52,15 @@
 Requires-Dist: selenium
 Requires-Dist: numpy
 Requires-Dist: scrapy
 Requires-Dist: pyparsing
 Requires-Dist: construct
 Requires-Dist: networkx
 Requires-Dist: pygobject
+Requires-Dist: pydantic
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: doot; extra == "dev"
 Requires-Dist: pipreqs; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>7.0.0; extra == "test"
```

### Comparing `jgdv-0.1.2/pyproject.toml` & `jgdv-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "jgdv"
-version         = "0.1.2"
+version         = "0.1.3"
 description     = ""
 readme          = "README.md"
 requires-python = ">=3.10"
 license         = {file = "LICENSE"}
 keywords        = []
 authors         = [
   {name  = "John Grey", email = "jgrey.n.plus.one+dejavu@gmail.com"},
@@ -19,14 +19,15 @@
                "selenium",
                "numpy",
                "scrapy",
                "pyparsing",
                "construct",
                "networkx",
                "pygobject",
+               "pydantic",
 ]
 
 [project.optional-dependencies]
 docs = [ "sphinx" ]
 dev  = [ "doot", "pipreqs"]
 test = [ "pytest > 7.0.0" ]
 
@@ -147,15 +148,15 @@
 
 [tool.sphinx.html.options]
 
 ##-- end sphinx
 
 ##-- bumpver
 [tool.bumpver]
-current_version    = "0.1.2"
+current_version    = "0.1.3"
 version_pattern    = "MAJOR.MINOR.PATCH"
 commit_message     = "[bump]: version {old_version} -> {new_version}"
 tag_message        = "{new_version}"
 tag_scope          = "default"
 commit             = true
 tag                = true
 # pre_commit_hook  = ""
```

