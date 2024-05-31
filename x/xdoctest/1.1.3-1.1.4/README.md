# Comparing `tmp/xdoctest-1.1.3.tar.gz` & `tmp/xdoctest-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdoctest-1.1.3.tar", last modified: Tue Jan 30 18:32:53 2024, max compression
+gzip compressed data, was "xdoctest-1.1.4.tar", last modified: Fri May 31 17:01:26 2024, max compression
```

## Comparing `xdoctest-1.1.3.tar` & `xdoctest-1.1.4.tar`

### file list

```diff
@@ -1,139 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.481136 xdoctest-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-01-30 18:32:47.000000 xdoctest-1.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-01-30 18:32:47.000000 xdoctest-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-30 18:32:47.000000 xdoctest-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21767 2024-01-30 18:32:53.481136 xdoctest-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-01-30 18:32:47.000000 xdoctest-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.473136 xdoctest-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.477136 xdoctest-1.1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/installing_python.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoc_with_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.checker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.constants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.demo.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.directive.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.docstr.docscrape_google.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.docstr.docscrape_numpy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.docstr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.doctest_example.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.doctest_part.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.dynamic_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.global_state.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.static_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_deprecation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_notebook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_path.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_str.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/source/xdoctest.utils.util_stream.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-01-30 18:32:47.000000 xdoctest-1.1.3/docs/todo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-30 18:32:47.000000 xdoctest-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-30 18:32:47.000000 xdoctest-1.1.3/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.477136 xdoctest-1.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/jupyter.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/tests-binary.txt
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-30 18:32:47.000000 xdoctest-1.1.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-01-30 18:32:47.000000 xdoctest-1.1.3/run_doctests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-01-30 18:32:47.000000 xdoctest-1.1.3/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:32:53.481136 xdoctest-1.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10062 2024-01-30 18:32:47.000000 xdoctest-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.461136 xdoctest-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.469136 xdoctest-1.1.3/src/xdoctest/
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)    21443 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/demo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    32667 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/directive.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.473136 xdoctest-1.1.3/src/xdoctest/docstr/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/docstr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/docstr/docscrape_google.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/docstr/docscrape_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    55051 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/doctest_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/doctest_example.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/doctest_part.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/doctest_part.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/dynamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/dynamic_analysis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/global_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    42409 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30275 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    42107 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/static_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/static_analysis.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.473136 xdoctest-1.1.3/src/xdoctest/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37965 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-01-30 18:32:47.000000 xdoctest-1.1.3/src/xdoctest/utils/util_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.469136 xdoctest-1.1.3/src/xdoctest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21767 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-30 18:32:53.000000 xdoctest-1.1.3/src/xdoctest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.481136 xdoctest-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/notebook_with_doctests.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:32:53.481136 xdoctest-1.1.3/tests/pybind11_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/pybind11_test/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_binary_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_doctest_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_doctest_in_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_limitations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    57853 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_preimport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_pytest_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-01-30 18:32:47.000000 xdoctest-1.1.3/tests/test_traceback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.612839 xdoctest-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-05-31 17:01:18.000000 xdoctest-1.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-31 17:01:18.000000 xdoctest-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 17:01:18.000000 xdoctest-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    38457 2024-05-31 17:01:26.612839 xdoctest-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-05-31 17:01:18.000000 xdoctest-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.576839 xdoctest-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.580839 xdoctest-1.1.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/installing_python.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoc_with_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.checker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.constants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.demo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.directive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.docstr.docscrape_google.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.docstr.docscrape_numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.docstr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.doctest_example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.doctest_part.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.dynamic_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.global_state.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.static_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_deprecation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_path.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_str.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/source/xdoctest.utils.util_stream.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-31 17:01:18.000000 xdoctest-1.1.4/docs/todo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-31 17:01:18.000000 xdoctest-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 17:01:18.000000 xdoctest-1.1.4/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.580839 xdoctest-1.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/jupyter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/tests-binary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 17:01:18.000000 xdoctest-1.1.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-31 17:01:18.000000 xdoctest-1.1.4/run_doctests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-05-31 17:01:18.000000 xdoctest-1.1.4/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:01:26.612839 xdoctest-1.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10062 2024-05-31 17:01:18.000000 xdoctest-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.560839 xdoctest-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.572839 xdoctest-1.1.4/src/xdoctest/
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21443 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/demo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    32667 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/directive.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.572839 xdoctest-1.1.4/src/xdoctest/docstr/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/docstr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/docstr/docscrape_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/docstr/docscrape_google.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/docstr/docscrape_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/docstr/docscrape_numpy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    55051 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/doctest_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/doctest_example.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/doctest_part.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/doctest_part.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/dynamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/dynamic_analysis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/global_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    42409 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30275 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    42107 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/static_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/static_analysis.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.576839 xdoctest-1.1.4/src/xdoctest/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    39023 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_import.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_notebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_str.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-31 17:01:18.000000 xdoctest-1.1.4/src/xdoctest/utils/util_stream.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.584839 xdoctest-1.1.4/src/xdoctest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    38457 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 17:01:26.000000 xdoctest-1.1.4/src/xdoctest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.584839 xdoctest-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/notebook_with_doctests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:01:26.584839 xdoctest-1.1.4/tests/pybind11_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/pybind11_test/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_binary_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_doctest_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_doctest_in_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57853 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_preimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_pytest_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-31 17:01:18.000000 xdoctest-1.1.4/tests/test_traceback.py
```

### Comparing `xdoctest-1.1.3/CHANGELOG.md` & `xdoctest-1.1.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # Changelog
 
 We are currently working on porting this changelog to the specifications in
 [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## Version 1.1.3 - 
+
+## Version 1.1.4 - Unreleased
+
+### Fixed
+* Working around a `modname_to_modpath` issue.
+
+
+## Version 1.1.3 - Released 2024-01-30 
 
 ### Fixed
 * `modname_to_modpath` now handles cases where editable packages have modules where the name is different than the package.
 * Update `xdoctest.plugin` to support pytest 8.0
 * Fixed deprecated usage of `ast.Num`
 
 
-## Version 1.1.2 - Released 2023-010-25 
+## Version 1.1.2 - Released 2023-10-25 
 
 ### Added
 * Partial support for 3.12. New f-string syntax is not supported yet.
 
 ### Changed
 * Removed dependency on six and got rid of old Python 2 logic
```

### Comparing `xdoctest-1.1.3/LICENSE` & `xdoctest-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/PKG-INFO` & `xdoctest-1.1.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,7 @@
-Metadata-Version: 2.1
-Name: xdoctest
-Version: 1.1.3
-Summary: A rewrite of the builtin doctest module
-Home-page: https://github.com/Erotemic/xdoctest
-Author: Jon Crall
-Author-email: erotemic@gmail.com
-License: Apache 2
-Keywords: xdoctest,doctest,test,docstr,pytest
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Classifier: Framework :: Pytest
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-Provides-Extra: all-strict
-Provides-Extra: colors
-Provides-Extra: jupyter
-Provides-Extra: optional
-Provides-Extra: optional-strict
-Provides-Extra: runtime-strict
-Provides-Extra: tests
-Provides-Extra: tests-binary
-Provides-Extra: tests-binary-strict
-Provides-Extra: tests-strict
-License-File: LICENSE
-
 |GithubActions| |CircleCI| |Appveyor| |Codecov| |Pypi| |PypiDownloads| |ReadTheDocs|
 
 
 .. The large version wont work because github strips rst image rescaling.
 .. image:: https://i.imgur.com/u0tYYxM.png
    :height: 100px
    :align: left
@@ -542,9 +500,7 @@
    :target: https://pypistats.org/packages/xdoctest
 .. |CondaDownloads| image:: https://anaconda.org/conda-forge/xdoctest/badges/downloads.svg
    :target: https://anaconda.org/conda-forge/xdoctest
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/xdoctest/badge/?version=latest
     :target: https://xdoctest.readthedocs.io
 .. |GithubActions| image:: https://github.com/Erotemic/xdoctest/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/Erotemic/xdoctest/actions?query=branch%3Amain
-
-
```

### Comparing `xdoctest-1.1.3/docs/Makefile` & `xdoctest-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/docs/make.bat` & `xdoctest-1.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/docs/source/conf.py` & `xdoctest-1.1.4/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Notes:
     Based on template code in:
-        ~/code/xcookie/xcookie/builders/docs_conf.py
+        ~/code/xcookie/xcookie/builders/docs.py
         ~/code/xcookie/xcookie/rc/conf_ext.py
 
     http://docs.readthedocs.io/en/latest/getting_started.html
 
     pip install sphinx sphinx-autobuild sphinx_rtd_theme sphinxcontrib-napoleon
 
     cd ~/code/xdoctest
@@ -13,56 +13,82 @@
     cd docs
 
     sphinx-quickstart
 
     # need to edit the conf.py
 
     cd ~/code/xdoctest/docs
-    sphinx-apidoc --private -f -o ~/code/xdoctest/docs/source ~/code/xdoctest/src/xdoctest --separate
+    sphinx-apidoc --private --separate -f -o ~/code/xdoctest/docs/source/auto ~/code/xdoctest/src/xdoctest '_tokenize.py'
+
+    # Note: the module should importable before running this
+    # (e.g. install it in developer mode or munge the PYTHONPATH)
     make html
 
-    git add source/*.rst
+    git add source/auto/*.rst
 
     Also:
         To turn on PR checks
 
         https://docs.readthedocs.io/en/stable/guides/autobuild-docs-for-pull-requests.html
 
         https://readthedocs.org/dashboard/xdoctest/advanced/
 
         ensure your github account is connected to readthedocs
         https://readthedocs.org/accounts/social/connections/
 
         ### For gitlab
 
-        The user will need to enable the repo on their readthedocs account:
-        https://readthedocs.org/dashboard/import/manual/?
-
         To enable the read-the-docs go to https://readthedocs.org/dashboard/ and login
 
-        Make sure you have a .readthedocs.yml file
+        The user will need to enable the repo on their readthedocs account:
+        https://readthedocs.org/dashboard/import/manual/?
 
-        Click import project: (for github you can select, but gitlab you need to import manually)
+        Enter the following information:
             Set the Repository NAME: xdoctest
             Set the Repository URL: https://github.com/Erotemic/xdoctest
 
+        Make sure you have a .readthedocs.yml file
+
         For gitlab you also need to setup an integrations. Navigate to:
 
             https://readthedocs.org/dashboard/xdoctest/integrations/create/
 
         Then add gitlab incoming webhook and copy the URL (make sure
-        you copy the real url and not the text so https is included).
+        you copy the real url and not the text so https is included),
+        specifically:
+
+            In the "Integration type:" dropdown menu, select
+            "Gitlab incoming webhook"
+
+            Click "Add integration"
+
+            Copy the text in the "Webhook URL" box to be used later.
+
+            Copy the text in the "Secret" box to be used later.
 
         Then go to
 
             https://github.com/Erotemic/xdoctest/hooks
 
-        and add the URL
+            Click "Add new webhook".
+
+            Copy the text previously saved from the "Webhook URL" box
+            in the readthedocs form into the "URL" box in the gitlab
+            form.
+
+            Copy the text previously saved from the "Secret" box
+            in the readthedocs form into the "Secret token" box in the
+            gitlab form.
+
+            For trigger permissions select the following checkboxes:
+                push events,
+                tag push events,
+                merge request events
 
-        select push, tag, and merge request
+            Click the "Add webhook" button.
 
         See Docs for more details https://docs.readthedocs.io/en/stable/integrations.html
 
         Will also need to activate the main branch:
             https://readthedocs.org/projects/xdoctest/versions/
 """
 #
@@ -106,22 +132,27 @@
                 if getattr(target, 'id', None) == '__version__':
                     self.version = node.value.s
     visitor = VersionVisitor()
     visitor.visit(pt)
     return visitor.version
 
 project = 'xdoctest'
-copyright = '2023, Jon Crall'
+copyright = '2024, Jon Crall'
 author = 'Jon Crall'
 modname = 'xdoctest'
 
-modpath = join(dirname(dirname(dirname(__file__))), 'src/xdoctest', '__init__.py')
+repo_dpath = dirname(dirname(dirname(__file__)))
+mod_dpath = join(repo_dpath, 'src/xdoctest')
+src_dpath = dirname(mod_dpath)
+modpath = join(mod_dpath, '__init__.py')
 release = parse_version(modpath)
 version = '.'.join(release.split('.')[0:2])
 
+# Hack to ensure the module is importable
+# sys.path.insert(0, os.path.abspath(src_dpath))
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -132,41 +163,57 @@
     # 'autoapi.extension',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
     'sphinx.ext.todo',
     'sphinx.ext.viewcode',
-    # 'myst_parser',  # TODO
-
+    'myst_parser',  # For markdown docs
+    'sphinx.ext.imgconverter',  # For building latexpdf
     'sphinx.ext.githubpages',
     # 'sphinxcontrib.redirects',
     'sphinx_reredirects',
 ]
 
 todo_include_todos = True
 napoleon_google_docstring = True
 napoleon_use_param = False
 napoleon_use_ivar = True
 
+#autoapi_type = 'python'
+#autoapi_dirs = [mod_dpath]
+
 autodoc_inherit_docstrings = False
 
+# Hack for geowatch, todo configure
+autosummary_mock_imports = [
+    'geowatch.utils.lightning_ext._jsonargparse_ext_ge_4_24_and_lt_4_xx',
+    'geowatch.utils.lightning_ext._jsonargparse_ext_ge_4_22_and_lt_4_24',
+    'geowatch.utils.lightning_ext._jsonargparse_ext_ge_4_21_and_lt_4_22',
+    'geowatch.tasks.fusion.datamodules.temporal_sampling.affinity_sampling',
+    'geowatch.tasks.depth_pcd.model',
+    'geowatch.tasks.cold.export_change_map',
+]
+
 autodoc_member_order = 'bysource'
 autoclass_content = 'both'
 # autodoc_mock_imports = ['torch', 'torchvision', 'visdom']
 
 # autoapi_modules = {
 #     modname: {
 #         'override': False,
 #         'output': 'auto'
 #     }
 # }
 # autoapi_dirs = [f'../../src/{modname}']
 # autoapi_keep_files = True
 
+# References:
+# https://stackoverflow.com/questions/21538983/specifying-targets-for-intersphinx-links-to-numpy-scipy-and-matplotlib
+
 intersphinx_mapping = {
     # 'pytorch': ('http://pytorch.org/docs/master/', None),
     'python': ('https://docs.python.org/3', None),
     'click': ('https://click.palletsprojects.com/', None),
     # 'xxhash': ('https://pypi.org/project/xxhash/', None),
     # 'pygments': ('https://pygments.org/docs/', None),
     # 'tqdm': ('https://tqdm.github.io/', None),
@@ -177,18 +224,28 @@
     'ndsampler': ('https://ndsampler.readthedocs.io/en/latest/', None),
     'ubelt': ('https://ubelt.readthedocs.io/en/latest/', None),
     'xdoctest': ('https://xdoctest.readthedocs.io/en/latest/', None),
     'networkx': ('https://networkx.org/documentation/stable/', None),
     'scriptconfig': ('https://scriptconfig.readthedocs.io/en/latest/', None),
     'rich': ('https://rich.readthedocs.io/en/latest/', None),
 
+    'numpy': ('https://numpy.org/doc/stable/', None),
+    'sympy': ('https://docs.sympy.org/latest/', None),
+    'scikit-learn': ('https://scikit-learn.org/stable/', None),
+    'pandas': ('https://pandas.pydata.org/docs/', None),
+    'matplotlib': ('https://matplotlib.org/stable/', None),
+
     'pytest': ('https://docs.pytest.org/en/latest/', None),
+    'platformdirs': ('https://platformdirs.readthedocs.io/en/latest/', None),
+
+    'timerit': ('https://timerit.readthedocs.io/en/latest/', None),
+    'progiter': ('https://progiter.readthedocs.io/en/latest/', None),
+    'dateutil': ('https://dateutil.readthedocs.io/en/latest/', None),
     # 'pytest._pytest.doctest': ('https://docs.pytest.org/en/latest/_modules/_pytest/doctest.html', None),
     # 'colorama': ('https://pypi.org/project/colorama/', None),
-    # 'numpy': ('http://docs.scipy.org/doc/numpy/', None),
     # 'cv2' : ('http://docs.opencv.org/2.4/', None),
     # 'h5py' : ('http://docs.h5py.org/en/latest/', None)
 }
 __dev_note__ = """
 python -m sphinx.ext.intersphinx https://docs.python.org/3/objects.inv
 python -m sphinx.ext.intersphinx https://kwcoco.readthedocs.io/en/latest/objects.inv
 python -m sphinx.ext.intersphinx https://networkx.org/documentation/stable/objects.inv
@@ -242,14 +299,15 @@
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     'collapse_navigation': False,
     'display_version': True,
+    'navigation_depth': -1,
     # 'logo_only': True,
 }
 # html_logo = '.static/xdoctest.svg'
 # html_favicon = '.static/xdoctest.ico'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
@@ -271,14 +329,29 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = project + 'doc'
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
+# References:
+# https://tex.stackexchange.com/questions/546246/centos-8-the-font-freeserif-cannot-be-found
+
+"""
+# https://www.sphinx-doc.org/en/master/usage/builders/index.html#sphinx.builders.latex.LaTeXBuilder
+# https://tex.stackexchange.com/a/570691/83399
+sudo apt install fonts-freefont-otf texlive-luatex texlive-latex-extra texlive-fonts-recommended texlive-latex-recommended tex-gyre latexmk
+make latexpdf LATEXMKOPTS="-shell-escape --synctex=-1 -src-specials -interaction=nonstopmode"
+make latexpdf LATEXMKOPTS="-lualatex -interaction=nonstopmode"
+make LATEXMKOPTS="-lualatex -interaction=nonstopmode"
+
+"""
+# latex_engine = 'lualatex'
+# latex_engine = 'xelatex'
+
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
 
     # The font size ('10pt', '11pt' or '12pt').
     #
@@ -326,21 +399,32 @@
 
 # -- Extension configuration -------------------------------------------------
 from sphinx.domains.python import PythonDomain  # NOQA
 # from sphinx.application import Sphinx  # NOQA
 from typing import Any, List  # NOQA
 
 
+# HACK TO PREVENT EXCESSIVE TIME.
+# TODO: FIXME FOR REAL
+MAX_TIME_MINUTES = None
+if MAX_TIME_MINUTES:
+    import ubelt  # NOQA
+    TIMER = ubelt.Timer()
+    TIMER.tic()
+
+
 class PatchedPythonDomain(PythonDomain):
     """
     References:
         https://github.com/sphinx-doc/sphinx/issues/3866
     """
     def resolve_xref(self, env, fromdocname, builder, typ, target, node, contnode):
-        # TODO: can use this to resolve references nicely
+        """
+        Helps to resolves cross-references
+        """
         if target.startswith('ub.'):
             target = 'ubelt.' + target[3]
         if target.startswith('xdoc.'):
             target = 'xdoctest.' + target[3]
         return_value = super(PatchedPythonDomain, self).resolve_xref(
             env, fromdocname, builder, typ, target, node, contnode)
         return return_value
@@ -349,14 +433,15 @@
 class GoogleStyleDocstringProcessor:
     """
     A small extension that runs after napoleon and reformats erotemic-flavored
     google-style docstrings for sphinx.
     """
 
     def __init__(self, autobuild=1):
+        self.debug = 0
         self.registry = {}
         if autobuild:
             self._register_builtins()
 
     def register_section(self, tag, alias=None):
         """
         Decorator that adds a custom processing function for a non-standard
@@ -403,28 +488,39 @@
             # new_lines.append('')
             new_lines.append('.. rubric:: {}'.format(tag))
             new_lines.append('')
             new_text = textwrap.dedent('\n'.join(lines[1:]))
             redone = new_text.split('\n')
             new_lines.extend(redone)
             # import ubelt as ub
-            # print('new_lines = {}'.format(ub.repr2(new_lines, nl=1)))
+            # print('new_lines = {}'.format(ub.urepr(new_lines, nl=1)))
             # new_lines.append('')
             return new_lines
 
         @self.register_section(tag='TextArt', alias=['Ascii'])
         def text_art(lines):
             new_lines = []
             new_lines.append('.. rubric:: TextArt')
             new_lines.append('')
             new_lines.append('.. code-block:: bash')
             new_lines.append('')
             new_lines.extend(lines[1:])
             return new_lines
 
+        # @self.register_section(tag='TODO', alias=['.. todo::'])
+        # def todo_section(lines):
+        #     """
+        #     Fixup todo sections
+        #     """
+        #     import xdev
+        #     xdev.embed()
+        #     import ubelt as ub
+        #     print('lines = {}'.format(ub.urepr(lines, nl=1)))
+        #     return new_lines
+
         @self.register_section(tag='Ignore')
         def ignore(lines):
             return []
 
     def process(self, lines):
         """
         Example:
@@ -527,32 +623,38 @@
 
             lines (List[str]): the lines of the docstring, see above
 
         References:
             https://www.sphinx-doc.org/en/1.5.1/_modules/sphinx/ext/autodoc.html
             https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
         """
-        # print(f'name={name}')
+        if self.debug:
+            print(f'ProcessDocstring: name={name}, what_={what_}, num_lines={len(lines)}')
+
         # print('BEFORE:')
         # import ubelt as ub
-        # print('lines = {}'.format(ub.repr2(lines, nl=1)))
+        # print('lines = {}'.format(ub.urepr(lines, nl=1)))
 
         self.process(lines)
 
         # docstr = '\n'.join(lines)
         # if 'Convert the Mask' in docstr:
         #     import xdev
         #     xdev.embed()
 
         # if 'keys in this dictionary ' in docstr:
         #     import xdev
         #     xdev.embed()
 
-        RENDER_IMAGES = 0
-        if RENDER_IMAGES:
+        render_doc_images = 0
+
+        if MAX_TIME_MINUTES and TIMER.toc() > (60 * MAX_TIME_MINUTES):
+            render_doc_images = False  # FIXME too slow on RTD
+
+        if render_doc_images:
             # DEVELOPING
             if any('REQUIRES(--show)' in line for line in lines):
                 # import xdev
                 # xdev.embed()
                 create_doctest_figure(app, obj, name, lines)
 
         FIX_EXAMPLE_FORMATTING = 1
@@ -606,15 +708,15 @@
                         new_paragraph = indent + paragraph(para)
                         new_lines.append(new_paragraph)
                         new_lines.append('')
                     new_lines = new_lines[:-1]
                     lines[edit_slice] = new_lines
 
         # print('AFTER:')
-        # print('lines = {}'.format(ub.repr2(lines, nl=1)))
+        # print('lines = {}'.format(ub.urepr(lines, nl=1)))
 
         # if name == 'kwimage.Affine.translate':
         #     import sys
         #     sys.exit(1)
 
 
 class SphinxDocstring:
@@ -854,31 +956,78 @@
         if INSERT_AT == 'inline':
             # Try to insert after test
             insert_index = info['insert_line_index']
         elif INSERT_AT == 'end':
             insert_index = end_index
         else:
             raise KeyError(INSERT_AT)
-        lines.insert(insert_index, '.. image:: {}'.format(rel_to_root_fpath))
+        lines.insert(insert_index, '.. image:: {}'.format('..' / rel_to_root_fpath))
+        # lines.insert(insert_index, '.. image:: {}'.format(rel_to_root_fpath))
         # lines.insert(insert_index, '.. image:: {}'.format(rel_to_static_fpath))
         lines.insert(insert_index, '')
 
 
+def postprocess_hyperlinks(app, doctree, docname):
+    """
+    Extension to fixup hyperlinks.
+    This should be connected to the Sphinx application's
+    "autodoc-process-docstring" event.
+    """
+    # Your hyperlink postprocessing logic here
+    from docutils import nodes
+    import pathlib
+    for node in doctree.traverse(nodes.reference):
+        if 'refuri' in node.attributes:
+            refuri = node.attributes['refuri']
+            if '.rst' in refuri:
+                if 'source' in node.document:
+                    fpath = pathlib.Path(node.document['source'])
+                    parent_dpath = fpath.parent
+                    if (parent_dpath / refuri).exists():
+                        node.attributes['refuri'] = refuri.replace('.rst', '.html')
+                else:
+                    raise AssertionError
+
+
+def fix_rst_todo_section(lines):
+    new_lines = []
+    for line in lines:
+        ...
+    ...
+
+
 def setup(app):
     import sphinx
     app : sphinx.application.Sphinx = app
     app.add_domain(PatchedPythonDomain, override=True)
+
+    app.connect("doctree-resolved", postprocess_hyperlinks)
+
     docstring_processor = GoogleStyleDocstringProcessor()
     # https://stackoverflow.com/questions/26534184/can-sphinx-ignore-certain-tags-in-python-docstrings
     app.connect('autodoc-process-docstring', docstring_processor.process_docstring_callback)
 
+    def copy(src, dst):
+        import shutil
+        print(f'Copy {src} -> {dst}')
+        assert src.exists()
+        if not dst.parent.exists():
+            dst.parent.mkdir()
+        shutil.copy(src, dst)
+
     ### Hack for kwcoco: TODO: figure out a way for the user to configure this.
     HACK_FOR_KWCOCO = 0
     if HACK_FOR_KWCOCO:
         import pathlib
-        import shutil
-        doc_outdir = pathlib.Path(app.outdir)
-        doc_srcdir = pathlib.Path(app.srcdir)
-        schema_src = (doc_srcdir / '../../kwcoco/coco_schema.json')
-        shutil.copy(schema_src, doc_outdir / 'coco_schema.json')
-        shutil.copy(schema_src, doc_srcdir / 'coco_schema.json')
+        doc_outdir = pathlib.Path(app.outdir) / 'auto'
+        doc_srcdir = pathlib.Path(app.srcdir) / 'auto'
+
+        mod_dpath = doc_srcdir / '../../../kwcoco'
+
+        src_fpath = (mod_dpath / 'coco_schema.json')
+        copy(src_fpath, doc_outdir / src_fpath.name)
+        copy(src_fpath, doc_srcdir / src_fpath.name)
+
+        src_fpath = (mod_dpath / 'coco_schema_informal.rst')
+        copy(src_fpath, doc_outdir / src_fpath.name)
+        copy(src_fpath, doc_srcdir / src_fpath.name)
     return app
```

### Comparing `xdoctest-1.1.3/docs/source/installing_python.rst` & `xdoctest-1.1.4/docs/source/installing_python.rst`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/docs/source/xdoc_with_jupyter.rst` & `xdoctest-1.1.4/docs/source/xdoc_with_jupyter.rst`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/docs/source/xdoctest.rst` & `xdoctest-1.1.4/docs/source/xdoctest.rst`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/docs/todo.rst` & `xdoctest-1.1.4/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/pyproject.toml` & `xdoctest-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/pytest.ini` & `xdoctest-1.1.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/requirements/jupyter.txt` & `xdoctest-1.1.4/requirements/jupyter.txt`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/requirements/tests-binary.txt` & `xdoctest-1.1.4/requirements/tests-binary.txt`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/requirements/tests.txt` & `xdoctest-1.1.4/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/setup.py` & `xdoctest-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/__init__.py` & `xdoctest-1.1.4/src/xdoctest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 '''
 
 
 __autogen__ = '''
 mkinit xdoctest --nomods
 '''
 
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 
 # Expose only select submodules
 __submodules__ = [
     'runner',
     'exceptions',
 ]
```

### Comparing `xdoctest-1.1.3/src/xdoctest/__main__.py` & `xdoctest-1.1.4/src/xdoctest/__main__.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/_tokenize.py` & `xdoctest-1.1.4/src/xdoctest/_tokenize.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/checker.py` & `xdoctest-1.1.4/src/xdoctest/checker.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/checker.pyi` & `xdoctest-1.1.4/src/xdoctest/checker.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/constants.py` & `xdoctest-1.1.4/src/xdoctest/constants.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/core.py` & `xdoctest-1.1.4/src/xdoctest/core.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/core.pyi` & `xdoctest-1.1.4/src/xdoctest/core.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/demo.py` & `xdoctest-1.1.4/src/xdoctest/demo.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/directive.py` & `xdoctest-1.1.4/src/xdoctest/directive.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/directive.pyi` & `xdoctest-1.1.4/src/xdoctest/directive.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/docstr/__init__.py` & `xdoctest-1.1.4/src/xdoctest/docstr/__init__.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/docstr/docscrape_google.py` & `xdoctest-1.1.4/src/xdoctest/docstr/docscrape_google.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/doctest_example.py` & `xdoctest-1.1.4/src/xdoctest/doctest_example.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/doctest_example.pyi` & `xdoctest-1.1.4/src/xdoctest/doctest_example.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/doctest_part.py` & `xdoctest-1.1.4/src/xdoctest/doctest_part.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/doctest_part.pyi` & `xdoctest-1.1.4/src/xdoctest/doctest_part.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/dynamic_analysis.py` & `xdoctest-1.1.4/src/xdoctest/dynamic_analysis.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/dynamic_analysis.pyi` & `xdoctest-1.1.4/src/xdoctest/dynamic_analysis.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/exceptions.py` & `xdoctest-1.1.4/src/xdoctest/exceptions.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/exceptions.pyi` & `xdoctest-1.1.4/src/xdoctest/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/global_state.py` & `xdoctest-1.1.4/src/xdoctest/global_state.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/parser.py` & `xdoctest-1.1.4/src/xdoctest/parser.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/plugin.py` & `xdoctest-1.1.4/src/xdoctest/plugin.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/plugin.pyi` & `xdoctest-1.1.4/src/xdoctest/plugin.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/runner.py` & `xdoctest-1.1.4/src/xdoctest/runner.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/runner.pyi` & `xdoctest-1.1.4/src/xdoctest/runner.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/static_analysis.py` & `xdoctest-1.1.4/src/xdoctest/static_analysis.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/static_analysis.pyi` & `xdoctest-1.1.4/src/xdoctest/static_analysis.pyi`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/__init__.py` & `xdoctest-1.1.4/src/xdoctest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_deprecation.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_deprecation.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_import.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,42 +58,14 @@
     import importlib.util
     spec = importlib.util.spec_from_file_location(modname, modpath)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module
 
 
-def _pkgutil_modname_to_modpath(modname):  # nocover
-    """
-    faster version of :func:`_syspath_modname_to_modpath` using builtin python
-    mechanisms, but unfortunately it doesn't play nice with pytest.
-
-    Args:
-        modname (str): the module name.
-
-    Example:
-        >>> # xdoctest: +SKIP
-        >>> modname = 'xdoctest.static_analysis'
-        >>> _pkgutil_modname_to_modpath(modname)
-        ...static_analysis.py
-        >>> # xdoctest: +REQUIRES(CPython)
-        >>> _pkgutil_modname_to_modpath('_ctypes')
-        ..._ctypes...
-
-    Ignore:
-        >>> _pkgutil_modname_to_modpath('cv2')
-    """
-    import pkgutil
-    loader = pkgutil.find_loader(modname)
-    if loader is None:
-        raise Exception('No module named {} in the PYTHONPATH'.format(modname))
-    modpath = loader.get_filename().replace('.pyc', '.py')
-    return modpath
-
-
 class PythonPathContext(object):
     """
     Context for temporarily adding a dir to the PYTHONPATH.
 
     Used in testing, and used as a helper in certain ubelt functions.
 
     Warning:
@@ -316,16 +288,16 @@
         >>> modpath = zippath + ':' + internal
         >>> modpath = zippath + os.path.sep + internal
         >>> module = ub.import_module_from_path(modpath)
         >>> assert normpath(module.__name__) == normpath('folder/bar')
         >>> assert module.testvar == 1
 
     Example:
-        >>> import pytest
         >>> # xdoctest: +SKIP("ubelt dependency")
+        >>> import pytest
         >>> with pytest.raises(IOError):
         >>>     ub.import_module_from_path('does-not-exist')
         >>> with pytest.raises(IOError):
         >>>     ub.import_module_from_path('does-not-exist.zip/')
     """
     if not os.path.exists(modpath):
         import re
@@ -700,25 +672,29 @@
         if new_editable_finder_paths:  # nocover
             # This makes some assumptions, which may not hold in general
             # We may need to fallback entirely on pkgutil, which would
             # ultimately be good. Hopefully the new standards mean it does not
             # break with pytest anymore? Nope, pytest still doesn't work right
             # with it.
             for finder_fpath in new_editable_finder_paths:
-                mapping = _static_parse('MAPPING', finder_fpath)
                 try:
-                    target = dirname(mapping[_pkg_name])
-                except KeyError:
+                    mapping = _static_parse('MAPPING', finder_fpath)
+                except AttributeError:
                     ...
                 else:
-                    if not exclude or normalize(target) not in real_exclude:  # pragma: nobranch
-                        modpath = check_dpath(target)
-                        if modpath:  # pragma: nobranch
-                            found_modpath = modpath
-                            break
+                    try:
+                        target = dirname(mapping[_pkg_name])
+                    except KeyError:
+                        ...
+                    else:
+                        if not exclude or normalize(target) not in real_exclude:  # pragma: nobranch
+                            modpath = check_dpath(target)
+                            if modpath:  # pragma: nobranch
+                                found_modpath = modpath
+                                break
             if found_modpath is not None:
                 break
 
         # If a finder does not exist, then the __editable__ pth file might hold
         # the path itself. Check for that.
         new_editable_pth_paths = sorted(glob.glob(join(dpath, _editable_fname_pth_pat)))
         if new_editable_pth_paths:  # nocover
@@ -763,14 +739,59 @@
                 if modpath:
                     found_modpath = modpath
                     break
 
     return found_modpath
 
 
+def _importlib_modname_to_modpath(modname):  # nocover
+    import importlib.util
+    spec = importlib.util.find_spec(modname)
+    print(f'spec={spec}')
+    modpath = spec.origin.replace('.pyc', '.py')
+    return modpath
+
+
+def _pkgutil_modname_to_modpath(modname):  # nocover
+    """
+    faster version of :func:`_syspath_modname_to_modpath` using builtin python
+    mechanisms, but unfortunately it doesn't play nice with pytest.
+
+    Note:
+        pkgutil.find_loader is deprecated in 3.12 and removed in 3.14
+
+    Args:
+        modname (str): the module name.
+
+    Example:
+        >>> # xdoctest: +SKIP
+        >>> modname = 'xdoctest.static_analysis'
+        >>> _pkgutil_modname_to_modpath(modname)
+        ...static_analysis.py
+        >>> # xdoctest: +REQUIRES(CPython)
+        >>> _pkgutil_modname_to_modpath('_ctypes')
+        ..._ctypes...
+
+    Ignore:
+        >>> _pkgutil_modname_to_modpath('cv2')
+    """
+    import pkgutil
+    loader = pkgutil.find_loader(modname)
+    if loader is None:
+        raise Exception('No module named {} in the PYTHONPATH'.format(modname))
+    try:
+        modpath = loader.get_filename().replace('.pyc', '.py')
+    except Exception:
+        print('Issue in _pkgutil_modname_to_modpath')
+        print(f'loader = {loader!r}')
+        print(f'modname = {modname!r}')
+        raise
+    return modpath
+
+
 def modname_to_modpath(modname, hide_init=True, hide_main=False, sys_path=None):
     """
     Finds the path to a python module from its name.
 
     Determines the path to a python module without directly import it
 
     Converts the name of a module (__name__) to the path (__file__) where it is
@@ -804,15 +825,26 @@
         >>> modname = 'xdoctest'
         >>> modpath = modname_to_modpath(modname, hide_init=False)
         >>> assert modpath.endswith('__init__.py')
         >>> # xdoctest: +REQUIRES(CPython)
         >>> modpath = basename(modname_to_modpath('_ctypes'))
         >>> assert 'ctypes' in modpath
     """
-    modpath = _syspath_modname_to_modpath(modname, sys_path)
+    if hide_main or sys_path:
+        modpath = _syspath_modname_to_modpath(modname, sys_path)
+    else:
+        # import xdev
+        # with xdev.embed_on_exception_context:
+        # try:
+        #     modpath = _importlib_modname_to_modpath(modname)
+        # except Exception:
+        #     modpath = _syspath_modname_to_modpath(modname, sys_path)
+        # modpath = _pkgutil_modname_to_modpath(modname, sys_path)
+        modpath = _syspath_modname_to_modpath(modname, sys_path)
+
     if modpath is None:
         return None
 
     modpath = normalize_modpath(modpath, hide_init=hide_init,
                                 hide_main=hide_main)
     return modpath
```

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_misc.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_misc.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_mixins.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_notebook.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_notebook.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_path.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_path.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_str.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_str.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest/utils/util_stream.py` & `xdoctest-1.1.4/src/xdoctest/utils/util_stream.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/src/xdoctest.egg-info/SOURCES.txt` & `xdoctest-1.1.4/src/xdoctest.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -45,24 +45,34 @@
 ./src/xdoctest.egg-info/SOURCES.txt
 ./src/xdoctest.egg-info/dependency_links.txt
 ./src/xdoctest.egg-info/entry_points.txt
 ./src/xdoctest.egg-info/requires.txt
 ./src/xdoctest.egg-info/top_level.txt
 ./src/xdoctest/docstr/__init__.py
 ./src/xdoctest/docstr/docscrape_google.py
+./src/xdoctest/docstr/docscrape_google.pyi
 ./src/xdoctest/docstr/docscrape_numpy.py
+./src/xdoctest/docstr/docscrape_numpy.pyi
 ./src/xdoctest/utils/__init__.py
 ./src/xdoctest/utils/util_deprecation.py
+./src/xdoctest/utils/util_deprecation.pyi
 ./src/xdoctest/utils/util_import.py
+./src/xdoctest/utils/util_import.pyi
 ./src/xdoctest/utils/util_misc.py
+./src/xdoctest/utils/util_misc.pyi
 ./src/xdoctest/utils/util_mixins.py
+./src/xdoctest/utils/util_mixins.pyi
 ./src/xdoctest/utils/util_notebook.py
+./src/xdoctest/utils/util_notebook.pyi
 ./src/xdoctest/utils/util_path.py
+./src/xdoctest/utils/util_path.pyi
 ./src/xdoctest/utils/util_str.py
+./src/xdoctest/utils/util_str.pyi
 ./src/xdoctest/utils/util_stream.py
+./src/xdoctest/utils/util_stream.pyi
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/todo.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installing_python.rst
```

### Comparing `xdoctest-1.1.3/src/xdoctest.egg-info/requires.txt` & `xdoctest-1.1.4/src/xdoctest.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 [all-strict:python_version >= "3.10.0"]
 pytest==6.2.5
 
 [all-strict:python_version >= "3.5.0"]
 Pygments==2.4.1
 
 [all-strict:python_version >= "3.6"]
-attrs==19.2.0
 jedi==0.16
+attrs==19.2.0
 jupyter_core==4.7.0
 
 [all-strict:python_version >= "3.6" and platform_python_implementation != "PyPy"]
-ipython_genutils==0.2.0
 jinja2==3.0.0
+ipython_genutils==0.2.0
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [all-strict:python_version >= "3.6.1"]
 jupyter_client==7.0.0
 
@@ -133,21 +133,21 @@
 [all:python_version >= "3.10.0"]
 pytest>=6.2.5
 
 [all:python_version >= "3.5.0"]
 Pygments>=2.4.1
 
 [all:python_version >= "3.6"]
-attrs>=19.2.0
 jedi>=0.16
+attrs>=19.2.0
 jupyter_core>=4.7.0
 
 [all:python_version >= "3.6" and platform_python_implementation != "PyPy"]
-ipython_genutils>=0.2.0
 jinja2>=3.0.0
+ipython_genutils>=0.2.0
 
 [all:python_version >= "3.6.0"]
 pytest-cov>=3.0.0
 
 [all:python_version >= "3.6.1"]
 jupyter_client>=7.0.0
 
@@ -198,21 +198,21 @@
 [jupyter:python_version < "4.0" and python_version >= "3.12" and (platform_system != "Windows" or platform_python_implementation != "PyPy")]
 ipykernel
 
 [jupyter:python_version >= "3.10"]
 debugpy
 
 [jupyter:python_version >= "3.6"]
-attrs
 jedi
+attrs
 jupyter_core
 
 [jupyter:python_version >= "3.6" and platform_python_implementation != "PyPy"]
-ipython_genutils
 jinja2
+ipython_genutils
 
 [jupyter:python_version >= "3.6.1"]
 jupyter_client
 
 [jupyter:python_version >= "3.7"]
 IPython
 
@@ -265,21 +265,21 @@
 [optional-strict:python_version >= "3.10"]
 debugpy==1.6.0
 
 [optional-strict:python_version >= "3.5.0"]
 Pygments==2.4.1
 
 [optional-strict:python_version >= "3.6"]
-attrs==19.2.0
 jedi==0.16
+attrs==19.2.0
 jupyter_core==4.7.0
 
 [optional-strict:python_version >= "3.6" and platform_python_implementation != "PyPy"]
-ipython_genutils==0.2.0
 jinja2==3.0.0
+ipython_genutils==0.2.0
 
 [optional-strict:python_version >= "3.6.1"]
 jupyter_client==7.0.0
 
 [optional-strict:python_version >= "3.7"]
 IPython==7.23.1
 
@@ -326,21 +326,21 @@
 [optional:python_version >= "3.10"]
 debugpy>=1.6.0
 
 [optional:python_version >= "3.5.0"]
 Pygments>=2.4.1
 
 [optional:python_version >= "3.6"]
-attrs>=19.2.0
 jedi>=0.16
+attrs>=19.2.0
 jupyter_core>=4.7.0
 
 [optional:python_version >= "3.6" and platform_python_implementation != "PyPy"]
-ipython_genutils>=0.2.0
 jinja2>=3.0.0
+ipython_genutils>=0.2.0
 
 [optional:python_version >= "3.6.1"]
 jupyter_client>=7.0.0
 
 [optional:python_version >= "3.7"]
 IPython>=7.23.1
 
@@ -352,36 +352,36 @@
 [tests]
 
 [tests-binary]
 
 [tests-binary-strict]
 
 [tests-binary-strict:python_version < "3.11"]
-cmake==3.21.2
+scikit-build==0.11.1
 ninja==1.10.2
 pybind11==2.7.1
-scikit-build==0.11.1
+cmake==3.21.2
 
 [tests-binary-strict:python_version < "4.0" and python_version >= "3.11"]
-cmake==3.25.0
+scikit-build==0.16.1
 ninja==1.11.1
 pybind11==2.10.3
-scikit-build==0.16.1
+cmake==3.25.0
 
 [tests-binary:python_version < "3.11"]
-cmake
+scikit-build
 ninja
 pybind11
-scikit-build
+cmake
 
 [tests-binary:python_version < "4.0" and python_version >= "3.11"]
-cmake
+scikit-build
 ninja
 pybind11
-scikit-build
+cmake
 
 [tests-strict]
 
 [tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
 pytest==4.6.0
 
 [tests-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
```

### Comparing `xdoctest-1.1.3/tests/notebook_with_doctests.ipynb` & `xdoctest-1.1.4/tests/notebook_with_doctests.ipynb`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_binary_ext.py` & `xdoctest-1.1.4/tests/test_binary_ext.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_cases.py` & `xdoctest-1.1.4/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_checker.py` & `xdoctest-1.1.4/tests/test_checker.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_core.py` & `xdoctest-1.1.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_directive.py` & `xdoctest-1.1.4/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_doctest_example.py` & `xdoctest-1.1.4/tests/test_doctest_example.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_doctest_in_notebook.ipynb` & `xdoctest-1.1.4/tests/test_doctest_in_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_dynamic.py` & `xdoctest-1.1.4/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_entry_point.py` & `xdoctest-1.1.4/tests/test_entry_point.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_errors.py` & `xdoctest-1.1.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_limitations.py` & `xdoctest-1.1.4/tests/test_limitations.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_notebook.py` & `xdoctest-1.1.4/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_parser.py` & `xdoctest-1.1.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_plugin.py` & `xdoctest-1.1.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_preimport.py` & `xdoctest-1.1.4/tests/test_preimport.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_pytest_cli.py` & `xdoctest-1.1.4/tests/test_pytest_cli.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_runner.py` & `xdoctest-1.1.4/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_static.py` & `xdoctest-1.1.4/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `xdoctest-1.1.3/tests/test_traceback.py` & `xdoctest-1.1.4/tests/test_traceback.py`

 * *Files identical despite different names*

