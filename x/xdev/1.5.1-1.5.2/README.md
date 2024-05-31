# Comparing `tmp/xdev-1.5.1.tar.gz` & `tmp/xdev-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdev-1.5.1.tar", last modified: Sat Feb 10 23:39:19 2024, max compression
+gzip compressed data, was "xdev-1.5.2.tar", last modified: Fri May 31 16:04:02 2024, max compression
```

## Comparing `xdev-1.5.1.tar` & `xdev-1.5.2.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.514634 xdev-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-02-10 23:38:55.000000 xdev-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30784 2024-02-10 23:39:19.514634 xdev-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-02-10 23:38:55.000000 xdev-1.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-10 23:38:55.000000 xdev-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 23:39:19.514634 xdev-1.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10478 2024-02-10 23:38:55.000000 xdev-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.474633 xdev-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-10 23:38:55.000000 xdev-1.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-10 23:38:55.000000 xdev-1.5.1/tests/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.482633 xdev-1.5.1/xdev/
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/_ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/_ipython_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/algo.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/algo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/autojit.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/autojit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.482633 xdev-1.5.1/xdev/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6198 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/bin/freshpyenv.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/class_reloader.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/class_reloader.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.486634 xdev-1.5.1/xdev/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30409 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/available_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/available_package_versions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/dirstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    45976 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/docstr_stubgen.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/docstr_stubgen.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18393 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/cli/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/desktop_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/desktop_interaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28261 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/directory_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/embeding.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/embeding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/format_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/format_quotes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/interactive_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/interactive_iter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/introspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/introspect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/patterns.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/profiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/regex_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/regex_builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/search_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/search_replace.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/tracebacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24108 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util_networkx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util_networkx.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-10 23:38:55.000000 xdev-1.5.1/xdev/util_path.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 23:39:19.486634 xdev-1.5.1/xdev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30784 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-10 23:39:19.000000 xdev-1.5.1/xdev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.076956 xdev-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-31 16:03:39.000000 xdev-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31672 2024-05-31 16:04:02.072956 xdev-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-05-31 16:03:39.000000 xdev-1.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-31 16:03:39.000000 xdev-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:04:02.076956 xdev-1.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10478 2024-05-31 16:03:39.000000 xdev-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.028957 xdev-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 16:03:39.000000 xdev-1.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 16:03:39.000000 xdev-1.5.2/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.036957 xdev-1.5.2/xdev/
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/_ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/_ipython_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/algo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/autojit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/autojit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.036957 xdev-1.5.2/xdev/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6224 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/bin/freshpyenv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/class_reloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/class_reloader.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.040957 xdev-1.5.2/xdev/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/available_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/available_package_versions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/dirstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46455 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/docstr_stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/cli/pyversion_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/desktop_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/desktop_interaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28992 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/directory_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/embeding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/embeding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/format_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/format_quotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/interactive_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/interactive_iter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/introspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/patterns.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/profiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/regex_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/regex_builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/search_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/search_replace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/tracebacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24108 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_networkx.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25754 2024-05-31 16:03:39.000000 xdev-1.5.2/xdev/util_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:04:02.040957 xdev-1.5.2/xdev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31672 2024-05-31 16:04:01.000000 xdev-1.5.2/xdev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-31 16:04:02.000000 xdev-1.5.2/xdev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:04:01.000000 xdev-1.5.2/xdev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 16:04:01.000000 xdev-1.5.2/xdev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-31 16:04:02.000000 xdev-1.5.2/xdev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 16:04:02.000000 xdev-1.5.2/xdev.egg-info/top_level.txt
```

### Comparing `xdev-1.5.1/LICENSE` & `xdev-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/PKG-INFO` & `xdev-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdev
-Version: 1.5.1
+Version: 1.5.2
 Summary: An excellent developer tool for excellent developers
 Home-page: https://github.com/Erotemic/xdev
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 Requires-Dist: numpy>=1.26.0; python_version < "4.0" and python_version >= "3.12"
 Requires-Dist: numpy>=1.23.2; python_version < "3.12" and python_version >= "3.11"
 Requires-Dist: numpy>=1.21.1; python_version < "3.11" and python_version >= "3.10"
 Requires-Dist: numpy>=1.19.3; python_version < "3.10" and python_version >= "3.9"
 Requires-Dist: numpy>=1.19.2; python_version < "3.9" and python_version >= "3.8"
 Requires-Dist: numpy<2.0,>=1.14.5; python_version < "3.8" and python_version >= "3.7"
 Requires-Dist: numpy<2.0,>=1.12.0; python_version < "3.7" and python_version >= "3.6"
-Requires-Dist: networkx>=2.8.8; python_version < "4.0" and python_version >= "3.11"
+Requires-Dist: networkx>=2.8; python_version < "4.0" and python_version >= "3.11"
 Requires-Dist: networkx>=2.7; python_version < "3.11" and python_version >= "3.10"
 Requires-Dist: networkx>=2.5.1; python_version < "3.10" and python_version >= "3.9"
 Requires-Dist: networkx>=2.7; python_version < "3.9" and python_version >= "3.8"
 Requires-Dist: networkx>=2.6.2; python_version < "3.8" and python_version >= "3.7"
 Requires-Dist: networkx>=2.5; python_version < "3.7" and python_version >= "3.6"
 Requires-Dist: rich>=12.3.0
 Requires-Dist: progiter>=2.0.0
@@ -56,23 +56,23 @@
 Requires-Dist: numpy>=1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "all"
 Requires-Dist: numpy>=1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "all"
 Requires-Dist: numpy>=1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: numpy>=1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: numpy>=1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: numpy<2.0,>=1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: numpy<2.0,>=1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
-Requires-Dist: networkx>=2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
+Requires-Dist: networkx>=2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: networkx>=2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: networkx>=2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: networkx>=2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: networkx>=2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: networkx>=2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: rich>=12.3.0; extra == "all"
 Requires-Dist: progiter>=2.0.0; extra == "all"
-Requires-Dist: xdoctest>=0.14.0; extra == "all"
+Requires-Dist: xdoctest>=1.1.3; extra == "all"
 Requires-Dist: pytest>=7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: pytest>=6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "all"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "all"
 Requires-Dist: pytest-cov>=3.0.0; python_version >= "3.6.0" and extra == "all"
 Requires-Dist: coverage>=6.1.1; python_version >= "3.10" and extra == "all"
 Requires-Dist: coverage>=5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
@@ -84,26 +84,29 @@
 Requires-Dist: Levenshtein>=0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: fire>=0.5.0; python_version >= "3.10" and extra == "all"
 Requires-Dist: fire>=0.4.0; python_version < "3.10" and extra == "all"
-Requires-Dist: line_profiler>=4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
+Requires-Dist: line_profiler>=4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "all"
+Requires-Dist: line_profiler>=4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: yapf>=0.16.3; extra == "all"
 Requires-Dist: autoflake>=1.5.0; extra == "all"
 Requires-Dist: parso>=0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: parso>=0.8.0; python_version < "3.11" and extra == "all"
+Requires-Dist: pint>=0.18; extra == "all"
+Requires-Dist: python_dateutil>=2.8.2; extra == "all"
 Provides-Extra: tests
-Requires-Dist: xdoctest>=0.14.0; extra == "tests"
+Requires-Dist: xdoctest>=1.1.3; extra == "tests"
 Requires-Dist: pytest>=7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "tests"
 Requires-Dist: pytest>=6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "tests"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "tests"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; python_version >= "3.6.0" and extra == "tests"
 Requires-Dist: coverage>=6.1.1; python_version >= "3.10" and extra == "tests"
 Requires-Dist: coverage>=5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "tests"
@@ -116,24 +119,27 @@
 Requires-Dist: Levenshtein>=0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional"
 Requires-Dist: fire>=0.5.0; python_version >= "3.10" and extra == "optional"
 Requires-Dist: fire>=0.4.0; python_version < "3.10" and extra == "optional"
-Requires-Dist: line_profiler>=4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "optional"
+Requires-Dist: line_profiler>=4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "optional"
+Requires-Dist: line_profiler>=4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional"
 Requires-Dist: yapf>=0.16.3; extra == "optional"
 Requires-Dist: autoflake>=1.5.0; extra == "optional"
 Requires-Dist: parso>=0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "optional"
 Requires-Dist: parso>=0.8.0; python_version < "3.11" and extra == "optional"
+Requires-Dist: pint>=0.18; extra == "optional"
+Requires-Dist: python_dateutil>=2.8.2; extra == "optional"
 Provides-Extra: all-strict
 Requires-Dist: ubelt==1.3.3; extra == "all-strict"
 Requires-Dist: xinspect==0.2.0; extra == "all-strict"
 Requires-Dist: pyfiglet==0.7; extra == "all-strict"
 Requires-Dist: pygments==2.12.0; extra == "all-strict"
 Requires-Dist: IPython==7.16.2; extra == "all-strict"
 Requires-Dist: parse==1.19.0; extra == "all-strict"
@@ -143,23 +149,23 @@
 Requires-Dist: numpy==1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "all-strict"
 Requires-Dist: numpy==1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: numpy==1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: numpy==1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: numpy==1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: numpy<2.0,==1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: numpy<2.0,==1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
-Requires-Dist: networkx==2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
+Requires-Dist: networkx==2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: networkx==2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: networkx==2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: networkx==2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: rich==12.3.0; extra == "all-strict"
 Requires-Dist: progiter==2.0.0; extra == "all-strict"
-Requires-Dist: xdoctest==0.14.0; extra == "all-strict"
+Requires-Dist: xdoctest==1.1.3; extra == "all-strict"
 Requires-Dist: pytest==7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: pytest==6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "all-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "all-strict"
 Requires-Dist: pytest-cov==3.0.0; python_version >= "3.6.0" and extra == "all-strict"
 Requires-Dist: coverage==6.1.1; python_version >= "3.10" and extra == "all-strict"
 Requires-Dist: coverage==5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
@@ -171,24 +177,27 @@
 Requires-Dist: Levenshtein==0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: fire==0.5.0; python_version >= "3.10" and extra == "all-strict"
 Requires-Dist: fire==0.4.0; python_version < "3.10" and extra == "all-strict"
-Requires-Dist: line_profiler==4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
+Requires-Dist: line_profiler==4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "all-strict"
+Requires-Dist: line_profiler==4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: yapf==0.16.3; extra == "all-strict"
 Requires-Dist: autoflake==1.5.0; extra == "all-strict"
 Requires-Dist: parso==0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: parso==0.8.0; python_version < "3.11" and extra == "all-strict"
+Requires-Dist: pint==0.18; extra == "all-strict"
+Requires-Dist: python_dateutil==2.8.2; extra == "all-strict"
 Provides-Extra: runtime-strict
 Requires-Dist: ubelt==1.3.3; extra == "runtime-strict"
 Requires-Dist: xinspect==0.2.0; extra == "runtime-strict"
 Requires-Dist: pyfiglet==0.7; extra == "runtime-strict"
 Requires-Dist: pygments==2.12.0; extra == "runtime-strict"
 Requires-Dist: IPython==7.16.2; extra == "runtime-strict"
 Requires-Dist: parse==1.19.0; extra == "runtime-strict"
@@ -198,24 +207,24 @@
 Requires-Dist: numpy==1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "runtime-strict"
 Requires-Dist: numpy==1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "runtime-strict"
 Requires-Dist: numpy==1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "runtime-strict"
 Requires-Dist: numpy==1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "runtime-strict"
 Requires-Dist: numpy==1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "runtime-strict"
 Requires-Dist: numpy<2.0,==1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "runtime-strict"
 Requires-Dist: numpy<2.0,==1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "runtime-strict"
-Requires-Dist: networkx==2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "runtime-strict"
+Requires-Dist: networkx==2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "runtime-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "runtime-strict"
 Requires-Dist: networkx==2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "runtime-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "runtime-strict"
 Requires-Dist: networkx==2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "runtime-strict"
 Requires-Dist: networkx==2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "runtime-strict"
 Requires-Dist: rich==12.3.0; extra == "runtime-strict"
 Requires-Dist: progiter==2.0.0; extra == "runtime-strict"
 Provides-Extra: tests-strict
-Requires-Dist: xdoctest==0.14.0; extra == "tests-strict"
+Requires-Dist: xdoctest==1.1.3; extra == "tests-strict"
 Requires-Dist: pytest==7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "tests-strict"
 Requires-Dist: pytest==6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "tests-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "tests-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "tests-strict"
 Requires-Dist: pytest-cov==3.0.0; python_version >= "3.6.0" and extra == "tests-strict"
 Requires-Dist: coverage==6.1.1; python_version >= "3.10" and extra == "tests-strict"
 Requires-Dist: coverage==5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "tests-strict"
@@ -228,24 +237,27 @@
 Requires-Dist: Levenshtein==0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional-strict"
 Requires-Dist: fire==0.5.0; python_version >= "3.10" and extra == "optional-strict"
 Requires-Dist: fire==0.4.0; python_version < "3.10" and extra == "optional-strict"
-Requires-Dist: line_profiler==4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "optional-strict"
+Requires-Dist: line_profiler==4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "optional-strict"
+Requires-Dist: line_profiler==4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional-strict"
 Requires-Dist: yapf==0.16.3; extra == "optional-strict"
 Requires-Dist: autoflake==1.5.0; extra == "optional-strict"
 Requires-Dist: parso==0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "optional-strict"
 Requires-Dist: parso==0.8.0; python_version < "3.11" and extra == "optional-strict"
+Requires-Dist: pint==0.18; extra == "optional-strict"
+Requires-Dist: python_dateutil==2.8.2; extra == "optional-strict"
 
 Xdev - Excellent Developer
 --------------------------
 
 |GithubActions| |Codecov| |Pypi| |Downloads| |ReadTheDocs|
```

### Comparing `xdev-1.5.1/README.rst` & `xdev-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/pyproject.toml` & `xdev-1.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,21 @@
 ignore_missing_imports = true
 
 [tool.xcookie]
 tags = [ "erotemic", "purepy", "github",]
 mod_name = "xdev"
 repo_name = "xdev"
 rel_mod_parent_dpath = "."
-#os = [ "win", "osx", "linux", "all",]
+os = [ "win", "osx", "linux", "all",]
 min_python = '3.7'
-max_python = '3.11'
+max_python = '3.12'
 
 #supported_python_versions = ['3.7', '3.8', '3.9', '3.10', '3.11']
-
-
-os = [ "linux" ]
-ci_cpython_versions=[3.7, 3.11]
+# os = [ "linux" ]
+# ci_cpython_versions=[3.7, 3.11]
 
 author = "Jon Crall"
 author_email = "erotemic@gmail.com"
 description = "An excellent developer tool for excellent developers"
 license = "Apache 2"
 dev_status = "beta"
 ci_pypy_versions = []
@@ -31,16 +29,16 @@
 ]
 [tool.xcookie.entry_points]
 console_scripts = [
     "xdev = xdev.__main__:main",
 ]
 
 [tool.pytest.ini_options]
-addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=dev"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
+addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=dev --ignore-glob=docs"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
 filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
```

### Comparing `xdev-1.5.1/setup.py` & `xdev-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/tests/test_cli.py` & `xdev-1.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/_ipython_ext.py` & `xdev-1.5.2/xdev/_ipython_ext.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/algo.py` & `xdev-1.5.2/xdev/algo.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/algo.pyi` & `xdev-1.5.2/xdev/algo.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/autojit.py` & `xdev-1.5.2/xdev/autojit.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/bin/freshpyenv.sh` & `xdev-1.5.2/xdev/bin/freshpyenv.sh`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     does not incur multiple downloads.
 
 OPTIONS
      COMMAND:
          Defaults to 'start'. Can also be 'images'
 
      -i, --image=IMAGE_NAME
-          The docker image to use
+         The docker image to use (e.g. --image=python:3.12)
 
      -v, --version
             print the version information
 
      -h, --help
             view this help message
```

### Comparing `xdev-1.5.1/xdev/class_reloader.py` & `xdev-1.5.2/xdev/class_reloader.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/cli/__main__.py` & `xdev-1.5.2/xdev/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/cli/available_package_versions.py` & `xdev-1.5.2/xdev/cli/available_package_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 
             platform_tag = item.get('platform_tag', None)
             if platform_tag is not None:
                 platinfo = parse_platform_tag(platform_tag)
                 item['os'] = platinfo['os']
                 item['arch'] = platinfo['arch']
 
-            python_version = item['python_version']
+            # python_version = item['python_version']
 
             flat_table.append(item)
     table = pd.DataFrame(flat_table)
     return table
 
 
 def vectorize(func):
@@ -574,15 +574,14 @@
                 # fix it if it is not. Hack for scikit-image
                 if str(row['python_version']) == 'image/tools/scikit_image':
                     row['python_version'] = row['python_tag']
 
                 min_pyver = python_versions.cp_codes.get(row['python_version'], row['python_version'])
                 max_pyver = python_versions.cp_codes.get(row['python_version'], row['python_version'])
 
-
             upload_time = ub.timeparse(row['upload_time_iso_8601'])
             flags = [upload_time >= t for t in python_version_table['release_date']]
             contemporary_pyvers = python_version_table['pyver'][flags].tolist()
 
             heuristic_support = None
 
             if row['requires_python']:
```

### Comparing `xdev-1.5.1/xdev/cli/available_package_versions.pyi` & `xdev-1.5.2/xdev/cli/available_package_versions.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,32 @@
     ...
 
 
 def summarize_package_availability(package_name):
     ...
 
 
+class PythonVersions:
+    latest: Incomplete
+    cp_codes: Incomplete
+    table: Incomplete
+    python_vstrings: Incomplete
+    python_version_rows: Incomplete
+
+    def __init__(self) -> None:
+        ...
+
+    def resolve_pyversion(self, pyver, maximize: bool = ...):
+        ...
+
+
+def build_package_table(package_name, refresh: bool = ...):
+    ...
+
+
 def minimum_cross_python_versions(package_name,
                                   request_min: Incomplete | None = ...,
                                   refresh: bool = ...):
     ...
 
 
 def demo() -> None:
```

### Comparing `xdev-1.5.1/xdev/cli/dirstats.py` & `xdev-1.5.2/xdev/cli/dirstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 #!/usr/bin/env python3
 import scriptconfig as scfg
 import ubelt as ub
+import os
+
+if not os.environ.get('_ARGCOMPLETE', ''):
+    # Hack for backwards compat
+    from xdev.directory_walker import DirectoryWalker  # NOQA
 
 
 class DirectoryStatsCLI(scfg.DataConfig):
     """
     Analysis for code in a repository
 
     CommandLine:
@@ -17,15 +22,15 @@
     exclude_dnames = scfg.Value(None, help='A coercable multi-pattern. If "py:auto" chooses sensible defaults for a Python dev.', nargs='+', alias=['block_dnames'])
 
     exclude_fnames = scfg.Value(None, help='A coercable multi-pattern. If "py:auto" chooses sensible defaults for a Python dev.', nargs='+', alias=['block_fnames'])
 
     include_dnames = scfg.Value(None, help='A coercable multi-pattern. Only directory names matching this pattern will be considered', nargs='+')
     include_fnames = scfg.Value(None, help='A coercable multi-pattern. Only file names matching this pattern will be considered', nargs='+')
 
-    parse_content = scfg.Value(True, isflag=True, help='if True parse stats about the content of each file')
+    parse_content = scfg.Value(False, isflag=True, help='if True parse stats about the content of each file')
     max_files = scfg.Value(None)
     # parse_meta_stats = scfg.Value(True, isflag=True, help='if True parse stats about the content of each file')
 
     max_walk_depth = scfg.Value(None, short_alias=['L'], help='maximum depth to walk')
     max_display_depth = scfg.Value(None, short_alias=['D'], help='maximum depth to display')
 
     verbose = scfg.Value(0, isflag=True, short_alias=['-v'])
@@ -81,15 +86,15 @@
     config = DirectoryStatsCLI.cli(cmdline=cmdline, data=kwargs, strict=True)
 
     import rich
     if config.verbose:
         kwargs = {'dpath': ub.modname_to_modpath('kwarray')}
     rich.print('config = ' + ub.urepr(config, nl=1))
 
-    from xdev.directory_walker import DirectoryWalker
+    from xdev.directory_walker import DirectoryWalker  # NOQA
     kwargs = ub.udict(config) & {
         'dpath', 'exclude_dnames', 'exclude_fnames', 'include_dnames',
         'include_fnames', 'max_walk_depth', 'parse_content', 'max_files'
     }
     self = DirectoryWalker(**kwargs)
     self.build()
     nxtxt_kwargs = {'max_depth': config['max_display_depth']}
```

### Comparing `xdev-1.5.1/xdev/cli/docstr_stubgen.py` & `xdev-1.5.2/xdev/cli/docstr_stubgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# mypy: ignore-errors
 """
 Script for auto-generating pyi type extension files from google-style
 docstrings.
 
 This is a work in progress, but ultimately the goal is to be able to express
 concise typing information in docstrings and then explicitly expose that to
 Python.
 
+It seems that mypy updates break this code extremely frequently. It is hard to
+keep this maintained.
+
 Requirements:
     pip install mypy autoflake yapf
 
 CommandLine:
     # Run script to parse google-style docstrings and write pyi files
 
     xdev doctypes --module=xdev
@@ -33,17 +37,19 @@
     modpath = delayed_nodes.__file__
     name = 'DelayedVisionOperation'
     lib = liberator.Liberator()
     lib.add_static(name, modpath)
     print(lib.current_sourcecode())
 """
 
+
 try:
-    from mypy.stubgen import (StubGenerator, find_self_initializers, FUNC, EMPTY,
+    from mypy.stubgen import (ASTStubGenerator, find_self_initializers, FUNC, EMPTY,
                               METHODS_WITH_RETURN_VALUE,)
+    from mypy.stubgen import (is_none_expr)
     from mypy.nodes import (
         # Expression, IntExpr, UnaryExpr, StrExpr, BytesExpr, NameExpr, FloatExpr, MemberExpr,
         # TupleExpr, ListExpr, ComparisonExpr, CallExpr, IndexExpr, EllipsisExpr,
         # ClassDef, MypyFile, Decorator, AssignmentStmt, TypeInfo,
         # IfStmt, ImportAll, ImportFrom, Import,
         IS_ABSTRACT,
         FuncDef,
@@ -61,15 +67,15 @@
     )
     from mypy.traverser import (
         all_yield_expressions,
         has_return_statement,
         has_yield_expression
     )
 except Exception:
-    StubGenerator = object
+    ASTStubGenerator = object
     FuncDef = None
     METHODS_WITH_RETURN_VALUE = []
 
 import sys
 from typing import (List,)
 # from mypy.stubgenc import generate_stub_for_c_module
 # from mypy.stubutil import (
@@ -214,14 +220,15 @@
     else:
         output_dir = modpath.parent
     # print(f'output_dir={output_dir}')
 
     options = stubgen.Options(
         pyversion=defaults.PYTHON3_VERSION,
         no_import=True,
+        inspect=False,
         doc_dir='',
         search_path=[],
         interpreter=sys.executable,
         ignore_errors=False,
         parse_only=True,
         include_private=False,
         output_dir=os.fspath(output_dir),
@@ -232,15 +239,15 @@
         quiet=False,
         export_less=True,
         include_docstrings=True,
     )
     # generate_stubs(options)
 
     mypy_opts = stubgen.mypy_options(options)
-    py_modules, c_modules = stubgen.collect_build_targets(options, mypy_opts)
+    py_modules, pyc_modules, c_modules = stubgen.collect_build_targets(options, mypy_opts)
 
     # Collect info from docs (if given):
     sigs = class_sigs = None  # type: Optional[Dict[str, str]]
     if options.doc_dir:
         sigs, class_sigs = stubgen.collect_docs_signatures(options.doc_dir)
 
     # Use parsed sources to generate stubs for Python modules.
@@ -264,24 +271,25 @@
         # target = join(options.output_dir, target)
         if verbose > 1:
             print(f'target={target}')
         # print(f'options.output_dir={options.output_dir}')
         # print(f'target={target}')
         files.append(target)
         with stubgen.generate_guarded(mod.module, target, options.ignore_errors, options.verbose):
-            stubgen.generate_stub_from_ast(mod, target, options.parse_only,
-                                           # options.pyversion,
-                                           options.include_private,
-                                           options.export_less)
+            # stubgen.generate_stub_from_ast(mod, target, options.parse_only,
+            #                                # options.pyversion,
+            #                                options.include_private,
+            #                                options.export_less)
 
             gen = ExtendedStubGenerator(mod.runtime_all,
                                         # pyversion=options.pyversion,
                                         include_private=options.include_private,
                                         analyzed=not options.parse_only,
                                         export_less=options.export_less)
+            gen.module = mod.module
             assert mod.ast is not None, "This function must be used only with analyzed modules"
             mod.ast.accept(gen)
             # print('gen.import_tracker.required_names = {!r}'.format(gen.import_tracker.required_names))
             # print(gen.import_tracker.import_lines())
 
             # print('mod.path = {!r}'.format(mod.path))
 
@@ -339,16 +347,16 @@
 
 
 def delete_unpaired_pyi_files(modpath):
     """
     Cleanup pyi files corresponding to renamed or removed py files.
     """
     import os
-    from xdev.cli import dirstats
-    walker = dirstats.DirectoryWalker(modpath, block_dnames=['__pycache__'])
+    import xdev
+    walker = xdev.DirectoryWalker(modpath, exclude_dnames=['__pycache__'])
     walker._walk()
     dangling_pyi_fpaths = []
     for node in walker.graph.nodes():
         if node.endswith('.pyi'):
             pypath = ub.Path(os.fspath(node)[0:-1])
             if not pypath.exists():
                 dangling_pyi_fpaths.append(node)
@@ -455,16 +463,15 @@
     # })
 
     style = yapf.yapf_api.style.CreatePEP8Style()
     text, _ = yapf.yapf_api.FormatCode(
         text,
         filename='<stdin>',
         style_config=style,
-        lines=None,
-        verify=False)
+        lines=None)
     # print(text)
     return text
 
 
 @ub.memoize
 def stdlib_names():
     # https://stackoverflow.com/questions/6463918/how-to-get-a-list-of-all-the-python-standard-library-modules
@@ -755,27 +762,30 @@
     #     add_typing_import('Callable')
     #     add_import_line('from typing import {}\n'.format(typing_arg))
     result['type_name'] = type_name
 
     return result
 
 
-class ExtendedStubGenerator(StubGenerator):
+class ExtendedStubGenerator(ASTStubGenerator):
 
     def _hack_for_info(self, info):
         type_name = info['type']
         if type_name is not None:
 
             if type_name == 'NoParamType' and self.path == 'ubelt/util_const.py':
                 # hack: Ignore util const
                 return
 
             results = hacked_typing_info(type_name)
             for typing_arg in results['typing_imports']:
-                self.add_typing_import(typing_arg)
+                # FIXME: mypy removed this API
+                # self.add_typing_import(typing_arg)
+                ...
+
             for line in results['import_lines']:
                 self.add_import_line(line)
             for hack in results['hacks']:
                 if hack == 'sliceable':
                     hacked = ub.codeblock(
                         '''
                         from typing import Any
@@ -952,15 +962,16 @@
                 # handle None specificaly.
                 if hasattr(arg_.initializer, 'name') and arg_.initializer.name == 'None':
                     info = name_to_parsed_docstr_info[name]
                     if info['type'] is not None:
                         doctype_str = info['type'].replace(' ', '')
                         if all(n not in doctype_str for n in {'None', 'Optional'}):
                             info['type'] = info['type'] + ' | None'
-                            self.add_typing_import('Union')
+                            # FIXME: mypy removed this API
+                            # self.add_typing_import('Union')
         # ------------------------------------------
 
         args: List[str] = []
         for i, arg_ in enumerate(o.arguments):
             var = arg_.variable
             kind = arg_.kind
             name = var.name
@@ -1020,14 +1031,16 @@
                         # arg_.initializer.is_special_form
                         if isinstance(arg_.initializer, (mypy.nodes.IntExpr, mypy.nodes.FloatExpr)):
                             annotation += '={!r}'.format(arg_.initializer.value)
                         elif isinstance(arg_.initializer, mypy.nodes.StrExpr):
                             annotation += '={!r}'.format(arg_.initializer.value)
                         elif isinstance(arg_.initializer, mypy.nodes.NameExpr):
                             annotation += '={}'.format(arg_.initializer.name)
+                        elif isinstance(arg_.initializer, mypy.nodes.UnaryExpr):
+                            annotation += '={}'.format(arg_.initializer.expr.value)
                         else:
                             # fallback, unhandled default
                             print(f'todo: Unhandled arg_.initializer={type(arg_.initializer)}')
                             annotation += '=...'
                     else:
                         annotation += ' = ...'
                 arg = name + annotation
@@ -1050,29 +1063,32 @@
             # Always assume abstract methods return Any unless explicitly annotated. Also
             # some dunder methods should not have a None return type.
             retname = None  # implicit Any
         elif has_yield_expression(o) or force_yield:
             try:
                 self.add_abc_import('Generator')
             except AttributeError:
-                self.add_typing_import('Generator')
+                # FIXME: mypy removed this API
+                # self.add_typing_import('Generator')
+                ...
             yield_name = 'None'
             send_name = 'None'
             return_name = 'None'
             for expr, in_assignment in all_yield_expressions(o):
-                if expr.expr is not None and not self.is_none_expr(expr.expr):
-                    self.add_typing_import('Any')
+                if expr.expr is not None and not is_none_expr(expr.expr):
+                    # self.add_typing_import('Any')  # fixme
                     yield_name = 'Any'
                 if in_assignment:
-                    self.add_typing_import('Any')
+                    # self.add_typing_import('Any')  # fixme
                     send_name = 'Any'
             if has_return_statement(o):
-                self.add_typing_import('Any')
+                # self.add_typing_import('Any')  # fixme
                 return_name = 'Any'
-            generator_name = self.typing_name('Generator')
+            # generator_name = self.typing_name('Generator')
+            generator_name = "collections.abc.Generator"
             if return_parsed_docstr_info is not None:
                 yield_name = return_parsed_docstr_info[1]
             retname = f'{generator_name}[{yield_name}, {send_name}, {return_name}]'
             # print('o.name = {}'.format(ub.repr2(o.name, nl=1)))
             # print('retname = {!r}'.format(retname))
             # print('retfield = {!r}'.format(retfield))
         elif not has_return_statement(o) and not is_abstract:
@@ -1191,15 +1207,7 @@
                 modpath = modpath_coercable
             else:
                 raise ValueError('Cannot find module={}'.format(modpath_coercable))
     else:
         raise TypeError('{}'.format(type(modpath_coercable)))
     modpath = ub.util_import.normalize_modpath(modpath)
     return modpath
-
-if __name__ == '__main__':
-    """
-    CommandLine:
-        python -m xdev.cli.gen_typed_stubs
-    """
-    from xdev.cli.docstr_stubgen import DocstrStubgenCLI
-    DocstrStubgenCLI.main()
```

### Comparing `xdev-1.5.1/xdev/cli/main.py` & `xdev-1.5.2/xdev/cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -264,88 +264,15 @@
 
         @classmethod
         def main(cls, cmdline=False, **kwargs):
             args = cls.cli(cmdline=cmdline, data=kwargs)
             modpath = ub.modname_to_modpath(args['modname'])
             print(modpath)
 
-    class PyVersionCLI(scfg.DataConfig):
-        """
-        Detect and print the version of a Python module or package.
-
-        Note
-        ----
-        Different backends may produce different results, especially for packages
-        that are in development and were installed in development mode.
-
-        Alternatives
-        ------------
-        An alternative with no dependencies is to use the one-liner:
-
-        python -c "import <modname>; print(<modname>.__version__)"
-
-        Example Usage
-        -------------
-        xdev pyversion xdev
-        xdev pyversion numpy
-
-        # Both the module name and the package name can be used.
-        xdev pyversion cv2
-        xdev pyversion opencv-python-headless
-
-        xdev pyversion xdev --backend=import
-        xdev pyversion xdev --backend=pkg_resources
-        """
-        __command__ = 'pyversion'
-        __alias__ = ['modversion']
-        __default__ = {
-            'modname': scfg.Value(None, position=1, help='The name of the module or package'),
-            'backend': scfg.Value('auto', help=ub.paragraph(
-                '''
-                The method to lookup the version. The core methods are 'import'
-                which imports the module and looks for a ``__version__`` attribute
-                or 'pkg_resources', which uses pip metadata. Can also be 'auto'
-                which tries to find the first one that works.
-                '''), choices=['auto', 'import', 'pkg_resources']),
-        }
-
-        @classmethod
-        def main(cls, cmdline=False, **kwargs):
-            args = cls.cli(cmdline=cmdline, data=kwargs)
-            modname = args['modname']
-
-            if args['backend'] == 'auto':
-                candidate_backends  = ['import', 'pkg_resources']
-            else:
-                candidate_backends = [args['backend']]
-
-            def _getversion(modname, backend):
-                if backend == 'import':
-                    module = ub.import_module_from_name(modname)
-                    version = module.__version__
-                elif backend == 'pkg_resources':
-                    import pkg_resources
-                    version = pkg_resources.get_distribution(modname).version
-                else:
-                    raise KeyError(backend)
-                return version
-
-            version = None
-            for backend in candidate_backends:
-                try:
-                    version = _getversion(modname, backend)
-                except KeyError:
-                    raise
-                except Exception:
-                    ...
-                else:
-                    break
-            print(version)
-            if version is None:
-                raise Exception(f'No version was found for {modname}')
+    from xdev.cli.pyversion_cli import PyVersionCLI
 
     class EditfileCLI(scfg.DataConfig):
         """
         Opens a file in your visual editor determined by the ``VISUAL``
         environment variable.
 
         If ``VISUAL`` is unspecified it attempts to default to the first known
@@ -408,15 +335,15 @@
 
         SeeAlso
         -------
         The generic freshpyenv.sh bash script also installed with this package.
         """
         __command__ = 'freshpyenv'
         __default__ = {
-            'image': scfg.Value('__default__', help='The docker image to use')
+            'image': scfg.Value('__default__', help='The docker image to use. (e.g. --image=python:3.12)')
         }
 
         @classmethod
         def main(cls, cmdline=False, **kwargs):
             config = cls.cli(cmdline=cmdline, data=kwargs)
             import ubelt as ub
             ub.cmd(f'freshpyenv.sh --image={config["image"]}', system=True)
```

### Comparing `xdev-1.5.1/xdev/cli/main.pyi` & `xdev-1.5.2/xdev/cli/main.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -112,10 +112,22 @@
         __default__: Incomplete
         __doc__: Incomplete
 
         @classmethod
         def main(cls, cmdline: bool = ..., **kwargs) -> None:
             ...
 
+    class RegexCLI(scfg.DataConfig):
+        __command__: str
+        backend: Incomplete
+
+        @classmethod
+        def main(cls, cmdline: bool = ..., **kwargs) -> None:
+            ...
+
+
+def rprint(*args) -> None:
+    ...
+
 
 def main() -> None:
     ...
```

### Comparing `xdev-1.5.1/xdev/desktop_interaction.py` & `xdev-1.5.2/xdev/desktop_interaction.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/directory_walker.py` & `xdev-1.5.2/xdev/directory_walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,18 +170,38 @@
 
             disp_piv = _node_table(root_node)
             print('')
             rich.print(disp_piv[:-1])
             rich.print(disp_piv[-1:])
         print('root_node = {}'.format(ub.urepr(root_node, nl=1)))
 
+        if 0:
+            # Feature to show most recently modified files in a tree?
+            table = []
+            for node, node_data in self.graph.nodes(data=True):
+                node_data['path_stat'] = node.stat()
+                node_data['path'] = node
+                table.append(node_data)
+
+            table = sorted(table, key=lambda r: r['path_stat'].st_mtime)
+            for row in table:
+                import xdev
+                time = xdev.datetime.coerce(row['path_stat'].st_mtime)
+                if 'dev' in str(row['path']):
+                    print(time, row['path'])
+
+            [r['path'] for r in table]
+
         # disp_stats = self._humanize_stats(stats, 'dir', reduce_prefix=True)
         # rich.print('stats = {}'.format(ub.urepr(disp_stats, nl=1)))
 
     def build(self):
+        """
+        Build the internal graph structure with requested metadata
+        """
         self._walk()
         self._update_stats()
         self._update_labels()
         self._sort()
         return self
 
     def _inplace_filter_dnames(self, dnames):
```

### Comparing `xdev-1.5.1/xdev/embeding.py` & `xdev-1.5.2/xdev/embeding.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/embeding.pyi` & `xdev-1.5.2/xdev/embeding.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+from os import PathLike
 from _typeshed import Incomplete
 
 
 def embed(parent_locals: Incomplete | None = ...,
           parent_globals: Incomplete | None = ...,
           exec_lines: Incomplete | None = ...,
           remove_pyqt_hook: bool = ...,
           n: int = ...) -> None:
     ...
 
 
+def breakpoint():
+    ...
+
+
+def load_snapshot(fpath: str | PathLike,
+                  parent_globals: dict | None = None) -> None:
+    ...
+
+
+def snapshot(parent_ns: dict | None = None, n: int = 0) -> None:
+    ...
+
+
 def embed_if_requested(n: int = ...) -> None:
     ...
 
 
 class EmbedOnException:
     before_embed: Incomplete
```

### Comparing `xdev-1.5.1/xdev/format_quotes.py` & `xdev-1.5.2/xdev/format_quotes.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/format_quotes.pyi` & `xdev-1.5.2/xdev/format_quotes.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/interactive_iter.py` & `xdev-1.5.2/xdev/interactive_iter.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/interactive_iter.pyi` & `xdev-1.5.2/xdev/interactive_iter.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/introspect.py` & `xdev-1.5.2/xdev/introspect.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/misc.py` & `xdev-1.5.2/xdev/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         if dirblocklist is None:
             dirblocklist = MultiPattern.coerce('.*', hint='glob')
         else:
             dirblocklist = MultiPattern.coerce([dirblocklist, '.*'], hint='glob')
 
     walker = dirstats.DirectoryWalker(
         cwd,
-        block_dnames=dirblocklist,
+        exclude_dnames=dirblocklist,
         max_files=max_files,
         abs_root_label=abs_root_label,
         pathstyle=pathstyle,
         show_nfiles=show_nfiles,
         show_progress=False,
         show_types=with_type,
         colors=colors,
```

### Comparing `xdev-1.5.1/xdev/misc.pyi` & `xdev-1.5.2/xdev/misc.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -38,13 +38,15 @@
               dirblocklist: Incomplete | None = ...,
               show_nfiles: str = ...,
               return_text: bool = False,
               return_tree: bool = False,
               pathstyle: str = 'name',
               max_depth: Incomplete | None = ...,
               with_type: bool = ...,
+              abs_root_label: bool = True,
+              ignore_dotprefix: bool = ...,
               colors: bool = ...):
     ...
 
 
 def textfind(text, pattern) -> None:
     ...
```

### Comparing `xdev-1.5.1/xdev/patterns.py` & `xdev-1.5.2/xdev/patterns.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/patterns.pyi` & `xdev-1.5.2/xdev/patterns.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import ubelt as ub
 from _typeshed import Incomplete
 from collections.abc import Generator
 
 RE_Pattern: Incomplete
 
 
+class FakeParseModule:
+
+    def Parser(self, *args, **kwargs) -> None:
+        ...
+
+
 class PatternBase:
 
     def match(self, text) -> None:
         ...
 
     def search(self, text) -> None:
         ...
 
     def sub(self, repl, text) -> None:
         ...
 
 
-def our_extended_regex_compile() -> None:
-    ...
-
-
 class Pattern(PatternBase, ub.NiceRepr):
     pattern: Incomplete
     backend: Incomplete
 
     def __init__(self, pattern, backend) -> None:
         ...
 
-    def __nice__(self):
+    def __nice__(self) -> str:
         ...
 
-    def to_regex(self):
+    def to_regex(self) -> Pattern:
         ...
 
     @classmethod
     def from_regex(cls,
                    data,
                    flags: int = ...,
                    multiline: bool = ...,
@@ -47,27 +49,27 @@
     def from_glob(cls, data):
         ...
 
     @classmethod
     def coerce_backend(cls, data, hint: str = ...):
         ...
 
+    @classmethod
+    def coerce(cls, data, hint: str = 'auto'):
+        ...
+
     def match(self, text):
         ...
 
     def search(self, text):
         ...
 
     def sub(self, repl: str, text: str, count: int = ...):
         ...
 
-    @classmethod
-    def coerce(cls, data, hint: str = ...):
-        ...
-
     def paths(self,
               cwd: Incomplete | None = ...,
               recursive: bool = ...) -> Generator[ub.Path, None, None]:
         ...
 
 
 class MultiPattern(PatternBase, ub.NiceRepr):
@@ -85,9 +87,12 @@
 
     def paths(self,
               cwd: Incomplete | None = ...,
               recursive: bool = ...) -> None:
         ...
 
     @classmethod
-    def coerce(cls, data, hint: str = ..., predicate: str = ...):
+    def coerce(cls,
+               data,
+               hint: str = 'auto',
+               predicate: str = ...) -> MultiPattern:
         ...
```

### Comparing `xdev-1.5.1/xdev/profiler.py` & `xdev-1.5.2/xdev/profiler.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/regex_builder.py` & `xdev-1.5.2/xdev/regex_builder.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/regex_builder.pyi` & `xdev-1.5.2/xdev/regex_builder.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/search_replace.py` & `xdev-1.5.2/xdev/search_replace.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/search_replace.pyi` & `xdev-1.5.2/xdev/search_replace.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 
 def sed(regexpr: str | Pattern,
         repl: str,
         dpath: str | None = None,
         include: str | List[str] | MultiPattern | None = None,
         exclude: str | List[str] | MultiPattern | None = None,
+        dirblocklist: str | List[str] | MultiPattern | None = None,
         recursive: bool = True,
         dry: bool = False,
         verbose: int = 1) -> None:
     ...
 
 
 def grep(regexpr: str | Pattern,
```

### Comparing `xdev-1.5.1/xdev/tracebacks.py` & `xdev-1.5.2/xdev/tracebacks.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/util.py` & `xdev-1.5.2/xdev/util.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/util_networkx.py` & `xdev-1.5.2/xdev/util_networkx.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/util_networkx.pyi` & `xdev-1.5.2/xdev/util_networkx.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/util_path.py` & `xdev-1.5.2/xdev/util_path.py`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev/util_path.pyi` & `xdev-1.5.2/xdev/util_path.pyi`

 * *Files identical despite different names*

### Comparing `xdev-1.5.1/xdev.egg-info/PKG-INFO` & `xdev-1.5.2/xdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdev
-Version: 1.5.1
+Version: 1.5.2
 Summary: An excellent developer tool for excellent developers
 Home-page: https://github.com/Erotemic/xdev
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 Requires-Dist: numpy>=1.26.0; python_version < "4.0" and python_version >= "3.12"
 Requires-Dist: numpy>=1.23.2; python_version < "3.12" and python_version >= "3.11"
 Requires-Dist: numpy>=1.21.1; python_version < "3.11" and python_version >= "3.10"
 Requires-Dist: numpy>=1.19.3; python_version < "3.10" and python_version >= "3.9"
 Requires-Dist: numpy>=1.19.2; python_version < "3.9" and python_version >= "3.8"
 Requires-Dist: numpy<2.0,>=1.14.5; python_version < "3.8" and python_version >= "3.7"
 Requires-Dist: numpy<2.0,>=1.12.0; python_version < "3.7" and python_version >= "3.6"
-Requires-Dist: networkx>=2.8.8; python_version < "4.0" and python_version >= "3.11"
+Requires-Dist: networkx>=2.8; python_version < "4.0" and python_version >= "3.11"
 Requires-Dist: networkx>=2.7; python_version < "3.11" and python_version >= "3.10"
 Requires-Dist: networkx>=2.5.1; python_version < "3.10" and python_version >= "3.9"
 Requires-Dist: networkx>=2.7; python_version < "3.9" and python_version >= "3.8"
 Requires-Dist: networkx>=2.6.2; python_version < "3.8" and python_version >= "3.7"
 Requires-Dist: networkx>=2.5; python_version < "3.7" and python_version >= "3.6"
 Requires-Dist: rich>=12.3.0
 Requires-Dist: progiter>=2.0.0
@@ -56,23 +56,23 @@
 Requires-Dist: numpy>=1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "all"
 Requires-Dist: numpy>=1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "all"
 Requires-Dist: numpy>=1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: numpy>=1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: numpy>=1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: numpy<2.0,>=1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: numpy<2.0,>=1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
-Requires-Dist: networkx>=2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
+Requires-Dist: networkx>=2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: networkx>=2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: networkx>=2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: networkx>=2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: networkx>=2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: networkx>=2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: rich>=12.3.0; extra == "all"
 Requires-Dist: progiter>=2.0.0; extra == "all"
-Requires-Dist: xdoctest>=0.14.0; extra == "all"
+Requires-Dist: xdoctest>=1.1.3; extra == "all"
 Requires-Dist: pytest>=7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: pytest>=6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "all"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "all"
 Requires-Dist: pytest-cov>=3.0.0; python_version >= "3.6.0" and extra == "all"
 Requires-Dist: coverage>=6.1.1; python_version >= "3.10" and extra == "all"
 Requires-Dist: coverage>=5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
@@ -84,26 +84,29 @@
 Requires-Dist: Levenshtein>=0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: fire>=0.5.0; python_version >= "3.10" and extra == "all"
 Requires-Dist: fire>=0.4.0; python_version < "3.10" and extra == "all"
-Requires-Dist: line_profiler>=4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
+Requires-Dist: line_profiler>=4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "all"
+Requires-Dist: line_profiler>=4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all"
 Requires-Dist: yapf>=0.16.3; extra == "all"
 Requires-Dist: autoflake>=1.5.0; extra == "all"
 Requires-Dist: parso>=0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "all"
 Requires-Dist: parso>=0.8.0; python_version < "3.11" and extra == "all"
+Requires-Dist: pint>=0.18; extra == "all"
+Requires-Dist: python_dateutil>=2.8.2; extra == "all"
 Provides-Extra: tests
-Requires-Dist: xdoctest>=0.14.0; extra == "tests"
+Requires-Dist: xdoctest>=1.1.3; extra == "tests"
 Requires-Dist: pytest>=7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "tests"
 Requires-Dist: pytest>=6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "tests"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "tests"
 Requires-Dist: pytest>=4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; python_version >= "3.6.0" and extra == "tests"
 Requires-Dist: coverage>=6.1.1; python_version >= "3.10" and extra == "tests"
 Requires-Dist: coverage>=5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "tests"
@@ -116,24 +119,27 @@
 Requires-Dist: Levenshtein>=0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional"
 Requires-Dist: Levenshtein>=0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional"
 Requires-Dist: fire>=0.5.0; python_version >= "3.10" and extra == "optional"
 Requires-Dist: fire>=0.4.0; python_version < "3.10" and extra == "optional"
-Requires-Dist: line_profiler>=4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "optional"
+Requires-Dist: line_profiler>=4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "optional"
+Requires-Dist: line_profiler>=4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional"
 Requires-Dist: line_profiler>=4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional"
 Requires-Dist: yapf>=0.16.3; extra == "optional"
 Requires-Dist: autoflake>=1.5.0; extra == "optional"
 Requires-Dist: parso>=0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "optional"
 Requires-Dist: parso>=0.8.0; python_version < "3.11" and extra == "optional"
+Requires-Dist: pint>=0.18; extra == "optional"
+Requires-Dist: python_dateutil>=2.8.2; extra == "optional"
 Provides-Extra: all-strict
 Requires-Dist: ubelt==1.3.3; extra == "all-strict"
 Requires-Dist: xinspect==0.2.0; extra == "all-strict"
 Requires-Dist: pyfiglet==0.7; extra == "all-strict"
 Requires-Dist: pygments==2.12.0; extra == "all-strict"
 Requires-Dist: IPython==7.16.2; extra == "all-strict"
 Requires-Dist: parse==1.19.0; extra == "all-strict"
@@ -143,23 +149,23 @@
 Requires-Dist: numpy==1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "all-strict"
 Requires-Dist: numpy==1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: numpy==1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: numpy==1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: numpy==1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: numpy<2.0,==1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: numpy<2.0,==1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
-Requires-Dist: networkx==2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
+Requires-Dist: networkx==2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: networkx==2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: networkx==2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: networkx==2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: rich==12.3.0; extra == "all-strict"
 Requires-Dist: progiter==2.0.0; extra == "all-strict"
-Requires-Dist: xdoctest==0.14.0; extra == "all-strict"
+Requires-Dist: xdoctest==1.1.3; extra == "all-strict"
 Requires-Dist: pytest==7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: pytest==6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "all-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "all-strict"
 Requires-Dist: pytest-cov==3.0.0; python_version >= "3.6.0" and extra == "all-strict"
 Requires-Dist: coverage==6.1.1; python_version >= "3.10" and extra == "all-strict"
 Requires-Dist: coverage==5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
@@ -171,24 +177,27 @@
 Requires-Dist: Levenshtein==0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: fire==0.5.0; python_version >= "3.10" and extra == "all-strict"
 Requires-Dist: fire==0.4.0; python_version < "3.10" and extra == "all-strict"
-Requires-Dist: line_profiler==4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
+Requires-Dist: line_profiler==4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "all-strict"
+Requires-Dist: line_profiler==4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "all-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "all-strict"
 Requires-Dist: yapf==0.16.3; extra == "all-strict"
 Requires-Dist: autoflake==1.5.0; extra == "all-strict"
 Requires-Dist: parso==0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "all-strict"
 Requires-Dist: parso==0.8.0; python_version < "3.11" and extra == "all-strict"
+Requires-Dist: pint==0.18; extra == "all-strict"
+Requires-Dist: python_dateutil==2.8.2; extra == "all-strict"
 Provides-Extra: runtime-strict
 Requires-Dist: ubelt==1.3.3; extra == "runtime-strict"
 Requires-Dist: xinspect==0.2.0; extra == "runtime-strict"
 Requires-Dist: pyfiglet==0.7; extra == "runtime-strict"
 Requires-Dist: pygments==2.12.0; extra == "runtime-strict"
 Requires-Dist: IPython==7.16.2; extra == "runtime-strict"
 Requires-Dist: parse==1.19.0; extra == "runtime-strict"
@@ -198,24 +207,24 @@
 Requires-Dist: numpy==1.26.0; (python_version < "4.0" and python_version >= "3.12") and extra == "runtime-strict"
 Requires-Dist: numpy==1.23.2; (python_version < "3.12" and python_version >= "3.11") and extra == "runtime-strict"
 Requires-Dist: numpy==1.21.1; (python_version < "3.11" and python_version >= "3.10") and extra == "runtime-strict"
 Requires-Dist: numpy==1.19.3; (python_version < "3.10" and python_version >= "3.9") and extra == "runtime-strict"
 Requires-Dist: numpy==1.19.2; (python_version < "3.9" and python_version >= "3.8") and extra == "runtime-strict"
 Requires-Dist: numpy<2.0,==1.14.5; (python_version < "3.8" and python_version >= "3.7") and extra == "runtime-strict"
 Requires-Dist: numpy<2.0,==1.12.0; (python_version < "3.7" and python_version >= "3.6") and extra == "runtime-strict"
-Requires-Dist: networkx==2.8.8; (python_version < "4.0" and python_version >= "3.11") and extra == "runtime-strict"
+Requires-Dist: networkx==2.8; (python_version < "4.0" and python_version >= "3.11") and extra == "runtime-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.11" and python_version >= "3.10") and extra == "runtime-strict"
 Requires-Dist: networkx==2.5.1; (python_version < "3.10" and python_version >= "3.9") and extra == "runtime-strict"
 Requires-Dist: networkx==2.7; (python_version < "3.9" and python_version >= "3.8") and extra == "runtime-strict"
 Requires-Dist: networkx==2.6.2; (python_version < "3.8" and python_version >= "3.7") and extra == "runtime-strict"
 Requires-Dist: networkx==2.5; (python_version < "3.7" and python_version >= "3.6") and extra == "runtime-strict"
 Requires-Dist: rich==12.3.0; extra == "runtime-strict"
 Requires-Dist: progiter==2.0.0; extra == "runtime-strict"
 Provides-Extra: tests-strict
-Requires-Dist: xdoctest==0.14.0; extra == "tests-strict"
+Requires-Dist: xdoctest==1.1.3; extra == "tests-strict"
 Requires-Dist: pytest==7.0.0; (python_version < "4.0" and python_version >= "3.11") and extra == "tests-strict"
 Requires-Dist: pytest==6.2.5; (python_version < "3.11" and python_version >= "3.10") and extra == "tests-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == "tests-strict"
 Requires-Dist: pytest==4.6.0; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == "tests-strict"
 Requires-Dist: pytest-cov==3.0.0; python_version >= "3.6.0" and extra == "tests-strict"
 Requires-Dist: coverage==6.1.1; python_version >= "3.10" and extra == "tests-strict"
 Requires-Dist: coverage==5.3.1; (python_version < "3.10" and python_version >= "3.9") and extra == "tests-strict"
@@ -228,24 +237,27 @@
 Requires-Dist: Levenshtein==0.18.2; (python_version < "3.11" and python_version >= "3.10") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional-strict"
 Requires-Dist: Levenshtein==0.18.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional-strict"
 Requires-Dist: fire==0.5.0; python_version >= "3.10" and extra == "optional-strict"
 Requires-Dist: fire==0.4.0; python_version < "3.10" and extra == "optional-strict"
-Requires-Dist: line_profiler==4.1.0; (python_version < "4.0" and python_version >= "3.11") and extra == "optional-strict"
+Requires-Dist: line_profiler==4.1.2; (python_version < "4.0" and python_version >= "3.12") and extra == "optional-strict"
+Requires-Dist: line_profiler==4.1.0; (python_version < "3.12" and python_version >= "3.11") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.11" and python_version >= "3.10") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.10" and python_version >= "3.9") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.9" and python_version >= "3.8") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.8" and python_version >= "3.7") and extra == "optional-strict"
 Requires-Dist: line_profiler==4.1.0; (python_version < "3.7" and python_version >= "3.6") and extra == "optional-strict"
 Requires-Dist: yapf==0.16.3; extra == "optional-strict"
 Requires-Dist: autoflake==1.5.0; extra == "optional-strict"
 Requires-Dist: parso==0.8.3; (python_version < "4.0" and python_version >= "3.11") and extra == "optional-strict"
 Requires-Dist: parso==0.8.0; python_version < "3.11" and extra == "optional-strict"
+Requires-Dist: pint==0.18; extra == "optional-strict"
+Requires-Dist: python_dateutil==2.8.2; extra == "optional-strict"
 
 Xdev - Excellent Developer
 --------------------------
 
 |GithubActions| |Codecov| |Pypi| |Downloads| |ReadTheDocs|
```

### Comparing `xdev-1.5.1/xdev.egg-info/SOURCES.txt` & `xdev-1.5.2/xdev.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -41,24 +41,26 @@
 xdev/tracebacks.pyi
 xdev/util.py
 xdev/util.pyi
 xdev/util_networkx.py
 xdev/util_networkx.pyi
 xdev/util_path.py
 xdev/util_path.pyi
+xdev/util_random.py
+xdev/util_time.py
 xdev.egg-info/PKG-INFO
 xdev.egg-info/SOURCES.txt
 xdev.egg-info/dependency_links.txt
 xdev.egg-info/entry_points.txt
 xdev.egg-info/requires.txt
 xdev.egg-info/top_level.txt
 xdev/bin/freshpyenv.sh
 xdev/cli/__init__.py
 xdev/cli/__main__.py
 xdev/cli/__main__.pyi
 xdev/cli/available_package_versions.py
 xdev/cli/available_package_versions.pyi
 xdev/cli/dirstats.py
 xdev/cli/docstr_stubgen.py
-xdev/cli/docstr_stubgen.pyi
 xdev/cli/main.py
-xdev/cli/main.pyi
+xdev/cli/main.pyi
+xdev/cli/pyversion_cli.py
```

### Comparing `xdev-1.5.1/xdev.egg-info/requires.txt` & `xdev-1.5.2/xdev.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 networkx>=2.6.2
 
 [:python_version < "3.9" and python_version >= "3.8"]
 numpy>=1.19.2
 networkx>=2.7
 
 [:python_version < "4.0" and python_version >= "3.11"]
-networkx>=2.8.8
+networkx>=2.8
 
 [:python_version < "4.0" and python_version >= "3.12"]
 numpy>=1.26.0
 
 [:python_version >= "3.7"]
 lazy_loader>=0.1
 
@@ -48,32 +48,36 @@
 pygments>=2.12.0
 IPython>=7.16.2
 parse>=1.19.0
 pyflakes>=2.5.0
 scriptconfig>=0.7.10
 rich>=12.3.0
 progiter>=2.0.0
-xdoctest>=0.14.0
+xdoctest>=1.1.3
 yapf>=0.16.3
 autoflake>=1.5.0
+pint>=0.18
+python_dateutil>=2.8.2
 
 [all-strict]
 ubelt==1.3.3
 xinspect==0.2.0
 pyfiglet==0.7
 pygments==2.12.0
 IPython==7.16.2
 parse==1.19.0
 pyflakes==2.5.0
 scriptconfig==0.7.10
 rich==12.3.0
 progiter==2.0.0
-xdoctest==0.14.0
+xdoctest==1.1.3
 yapf==0.16.3
 autoflake==1.5.0
+pint==0.18
+python_dateutil==2.8.2
 
 [all-strict:python_version < "3.10"]
 fire==0.4.0
 
 [all-strict:python_version < "3.10" and python_version >= "3.9"]
 numpy==1.19.3
 networkx==2.5.1
@@ -93,14 +97,15 @@
 pytest==6.2.5
 Levenshtein==0.18.2
 line_profiler==4.1.0
 
 [all-strict:python_version < "3.12" and python_version >= "3.11"]
 numpy==1.23.2
 Levenshtein==0.20.3
+line_profiler==4.1.0
 
 [all-strict:python_version < "3.7" and python_version >= "3.6"]
 numpy<2.0,==1.12.0
 networkx==2.5
 coverage==6.1.1
 Levenshtein==0.18.0
 line_profiler==4.1.0
@@ -119,22 +124,22 @@
 numpy==1.19.2
 networkx==2.7
 coverage==6.1.1
 Levenshtein==0.18.0
 line_profiler==4.1.0
 
 [all-strict:python_version < "4.0" and python_version >= "3.11"]
-networkx==2.8.8
+networkx==2.8
 pytest==7.0.0
-line_profiler==4.1.0
 parso==0.8.3
 
 [all-strict:python_version < "4.0" and python_version >= "3.12"]
 numpy==1.26.0
 Levenshtein==0.23.0
+line_profiler==4.1.2
 
 [all-strict:python_version >= "3.10"]
 coverage==6.1.1
 fire==0.5.0
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
@@ -164,14 +169,15 @@
 pytest>=6.2.5
 Levenshtein>=0.18.2
 line_profiler>=4.1.0
 
 [all:python_version < "3.12" and python_version >= "3.11"]
 numpy>=1.23.2
 Levenshtein>=0.20.3
+line_profiler>=4.1.0
 
 [all:python_version < "3.7" and python_version >= "3.6"]
 numpy<2.0,>=1.12.0
 networkx>=2.5
 coverage>=6.1.1
 Levenshtein>=0.18.0
 line_profiler>=4.1.0
@@ -190,40 +196,44 @@
 numpy>=1.19.2
 networkx>=2.7
 coverage>=6.1.1
 Levenshtein>=0.18.0
 line_profiler>=4.1.0
 
 [all:python_version < "4.0" and python_version >= "3.11"]
-networkx>=2.8.8
+networkx>=2.8
 pytest>=7.0.0
-line_profiler>=4.1.0
 parso>=0.8.3
 
 [all:python_version < "4.0" and python_version >= "3.12"]
 numpy>=1.26.0
 Levenshtein>=0.23.0
+line_profiler>=4.1.2
 
 [all:python_version >= "3.10"]
 coverage>=6.1.1
 fire>=0.5.0
 
 [all:python_version >= "3.6.0"]
 pytest-cov>=3.0.0
 
 [all:python_version >= "3.7"]
 lazy_loader>=0.1
 
 [optional]
 yapf>=0.16.3
 autoflake>=1.5.0
+pint>=0.18
+python_dateutil>=2.8.2
 
 [optional-strict]
 yapf==0.16.3
 autoflake==1.5.0
+pint==0.18
+python_dateutil==2.8.2
 
 [optional-strict:python_version < "3.10"]
 fire==0.4.0
 
 [optional-strict:python_version < "3.10" and python_version >= "3.9"]
 Levenshtein==0.18.0
 line_profiler==4.1.0
@@ -233,33 +243,34 @@
 
 [optional-strict:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein==0.18.2
 line_profiler==4.1.0
 
 [optional-strict:python_version < "3.12" and python_version >= "3.11"]
 Levenshtein==0.20.3
+line_profiler==4.1.0
 
 [optional-strict:python_version < "3.7" and python_version >= "3.6"]
 Levenshtein==0.18.0
 line_profiler==4.1.0
 
 [optional-strict:python_version < "3.8" and python_version >= "3.7"]
 Levenshtein==0.18.0
 line_profiler==4.1.0
 
 [optional-strict:python_version < "3.9" and python_version >= "3.8"]
 Levenshtein==0.18.0
 line_profiler==4.1.0
 
 [optional-strict:python_version < "4.0" and python_version >= "3.11"]
-line_profiler==4.1.0
 parso==0.8.3
 
 [optional-strict:python_version < "4.0" and python_version >= "3.12"]
 Levenshtein==0.23.0
+line_profiler==4.1.2
 
 [optional-strict:python_version >= "3.10"]
 fire==0.5.0
 
 [optional:python_version < "3.10"]
 fire>=0.4.0
 
@@ -272,33 +283,34 @@
 
 [optional:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein>=0.18.2
 line_profiler>=4.1.0
 
 [optional:python_version < "3.12" and python_version >= "3.11"]
 Levenshtein>=0.20.3
+line_profiler>=4.1.0
 
 [optional:python_version < "3.7" and python_version >= "3.6"]
 Levenshtein>=0.18.0
 line_profiler>=4.1.0
 
 [optional:python_version < "3.8" and python_version >= "3.7"]
 Levenshtein>=0.18.0
 line_profiler>=4.1.0
 
 [optional:python_version < "3.9" and python_version >= "3.8"]
 Levenshtein>=0.18.0
 line_profiler>=4.1.0
 
 [optional:python_version < "4.0" and python_version >= "3.11"]
-line_profiler>=4.1.0
 parso>=0.8.3
 
 [optional:python_version < "4.0" and python_version >= "3.12"]
 Levenshtein>=0.23.0
+line_profiler>=4.1.2
 
 [optional:python_version >= "3.10"]
 fire>=0.5.0
 
 [runtime-strict]
 ubelt==1.3.3
 xinspect==0.2.0
@@ -331,27 +343,27 @@
 networkx==2.6.2
 
 [runtime-strict:python_version < "3.9" and python_version >= "3.8"]
 numpy==1.19.2
 networkx==2.7
 
 [runtime-strict:python_version < "4.0" and python_version >= "3.11"]
-networkx==2.8.8
+networkx==2.8
 
 [runtime-strict:python_version < "4.0" and python_version >= "3.12"]
 numpy==1.26.0
 
 [runtime-strict:python_version >= "3.7"]
 lazy_loader==0.1
 
 [tests]
-xdoctest>=0.14.0
+xdoctest>=1.1.3
 
 [tests-strict]
-xdoctest==0.14.0
+xdoctest==1.1.3
 
 [tests-strict:python_version < "3.10" and python_version >= "3.9"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
 pytest==4.6.0
```

