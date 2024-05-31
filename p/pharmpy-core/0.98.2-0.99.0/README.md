# Comparing `tmp/pharmpy-core-0.98.2.tar.gz` & `tmp/pharmpy-core-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.98.2.tar", last modified: Sun Jul 23 09:57:35 2023, max compression
+gzip compressed data, was "pharmpy-core-0.99.0.tar", last modified: Wed Aug 23 14:55:36 2023, max compression
```

## Comparing `pharmpy-core-0.98.2.tar` & `pharmpy-core-0.99.0.tar`

### file list

```diff
@@ -1,1199 +1,1204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.558932 pharmpy-core-0.98.2/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    46815 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    48730 2023-07-23 09:57:35.558932 pharmpy-core-0.98.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-23 09:57:35.558932 pharmpy-core-0.98.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3204 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80672 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.378932 pharmpy-core-0.98.2/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.354932 pharmpy-core-0.98.2/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.382932 pharmpy-core-0.98.2/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    30947 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/external/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/external/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/external/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/generic/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.386932 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.390932 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25255 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.390932 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    68481 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.390932 pharmpy-core-0.98.2/src/pharmpy/model/external/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/rxode/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/external/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    74441 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.394932 pharmpy-core-0.98.2/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    51755 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    37809 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.394932 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    74416 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/parameter_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.394932 pharmpy-core-0.98.2/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/external/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/external/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nlmixr/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7225 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.398932 pharmpy-core-0.98.2/src/pharmpy/tools/external/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/external/rxode/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39054 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.402932 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    33694 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/simfit/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/pkpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.406932 pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48730 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    47497 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 09:49:54.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-23 09:57:35.000000 pharmpy-core-0.98.2/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.410932 pharmpy-core-0.98.2/tests/external/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/external/test_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/external/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/external/test_rxode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.414932 pharmpy-core-0.98.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/integration/test_structsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.414932 pharmpy-core-0.98.2/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.414932 pharmpy-core-0.98.2/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.414932 pharmpy-core-0.98.2/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.418932 pharmpy-core-0.98.2/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.422932 pharmpy-core-0.98.2/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    34423 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29609 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    68275 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_odes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_parameter_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.426932 pharmpy-core-0.98.2/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.426932 pharmpy-core-0.98.2/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.434932 pharmpy-core-0.98.2/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35981 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.434932 pharmpy-core-0.98.2/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.434932 pharmpy-core-0.98.2/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.442932 pharmpy-core-0.98.2/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.442932 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.442932 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.446932 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.450932 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/failed_run.ext
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/failed_run.mod
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.450932 pharmpy-core-0.98.2/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.450932 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.450932 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.454932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.366932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.458932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.458932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.462932 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.462932 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.474932 pharmpy-core-0.98.2/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_conc.mod
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_des_assignments.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_pd.csv
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_pd.mod
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.486932 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.486932 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.486932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.490932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.490932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.490932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.490932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.494932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.494932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.494932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.494932 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.498932 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.370932 pharmpy-core-0.98.2/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.502932 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.514932 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.518932 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.518932 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.526932 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.530932 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.530932 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.530932 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.534932 pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.534932 pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.534932 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.538932 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.370932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.370932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:53:28.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.542932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.546932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.546932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.546932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.546932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.550932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.550932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.550932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.554932 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.558932 pharmpy-core-0.98.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_structsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:57:35.558932 pharmpy-core-0.98.2/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-23 09:48:31.000000 pharmpy-core-0.98.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.717354 pharmpy-core-0.99.0/
+-rw-r--r--   0 runner    (1001) docker     (999)      419 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      227 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (999)      973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    47364 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2852 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    35196 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     7652 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (999)      524 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)    49279 2023-08-23 14:55:36.717354 pharmpy-core-0.99.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2933 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.597348 pharmpy-core-0.99.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (999)    10512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    14367 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (999)    14872 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.597348 pharmpy-core-0.99.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (999)     7108 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4723 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5230 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    24284 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      741 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       30 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       33 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       30 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     4317 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2807 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       76 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      413 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       58 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3921 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     6067 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       47 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    10790 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      644 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1290 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (999)     5302 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      177 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    10499 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     8137 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1624 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      854 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12790 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.597348 pharmpy-core-0.99.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (999)     5937 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (999)   179150 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (999)     1509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    11603 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2827 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      967 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     8102 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     3653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    16627 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    16031 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     4434 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    12416 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (999)     1072 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1248 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     5585 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2758 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      157 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     7786 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     2697 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1416 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      109 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (999)    15280 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     4212 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)     2492 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      813 2023-08-23 14:55:36.717354 pharmpy-core-0.99.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (999)     3225 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.597348 pharmpy-core-0.99.0/src/
+-rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.597348 pharmpy-core-0.99.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)      219 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      125 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    80672 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3593 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (999)      579 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      518 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (999)      213 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (999)      165 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (999)      261 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      413 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (999)      909 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1922 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      352 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1397 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (999)      955 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (999)      632 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (999)      697 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (999)      264 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2959 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2273 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (999)      585 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2335 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5576 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19768 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (999)      770 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3611 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.581347 pharmpy-core-0.99.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      758 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (999)      327 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (999)      425 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1192 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6508 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.601348 pharmpy-core-0.99.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1380 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (999)      297 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15783 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3503 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (999)      964 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2519 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1044 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4340 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2114 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (999)     1498 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1413 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6365 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (999)     1353 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      922 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (999)    30947 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1053 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19145 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15932 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/external/
+-rw-r--r--   0 runner    (1001) docker     (999)       60 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/external/fcon/
+-rw-r--r--   0 runner    (1001) docker     (999)      104 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2117 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/external/generic/
+-rw-r--r--   0 runner    (1001) docker     (999)      164 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/generic/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.605348 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10767 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5571 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8908 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16669 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (999)      408 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11271 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.609348 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (999)      155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24604 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11551 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (999)      297 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14169 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6712 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (999)    29071 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.609348 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      866 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)    25255 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5455 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      423 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      361 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3476 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.609348 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (999)     2904 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     6372 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     2232 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)      360 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     3216 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)      318 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)      146 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     1397 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     1921 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (999)     1692 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17000 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20087 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2841 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (999)      840 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      565 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      426 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      952 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1002 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2803 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5335 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11765 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (999)    68481 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.609348 pharmpy-core-0.99.0/src/pharmpy/model/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7165 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1186 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/external/utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23813 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13285 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (999)    34378 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8281 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    74605 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.613348 pharmpy-core-0.99.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (999)    10967 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4589 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6781 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9011 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17485 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1127 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21351 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (999)    56271 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (999)    40189 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5087 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9130 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15348 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (999)    50310 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (999)     1392 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (999)      680 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21259 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    90151 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (999)   298562 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     2384 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14564 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      605 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    47500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2751 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11217 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1572 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19639 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2671 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (999)    74415 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12116 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (999)    35807 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/parameter_variability.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19188 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5975 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/pd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4939 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (999)    25760 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8420 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4920 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1628 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (999)    11165 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (999)      361 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)      643 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (999)     5634 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9087 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)     3816 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (999)       99 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6511 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4945 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (999)      458 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16735 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (999)      157 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     8798 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1842 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (999)       98 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8392 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4863 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.617349 pharmpy-core-0.99.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      192 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20023 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (999)      147 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1449 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (999)      171 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5863 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (999)      583 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     7542 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      746 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/external/
+-rw-r--r--   0 runner    (1001) docker     (999)       82 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (999)      783 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20571 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nlmixr/run.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (999)      782 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      635 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21360 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18254 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)     7225 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (999)      332 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (999)      779 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6598 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/external/rxode/run.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1897 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (999)      505 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    39054 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2913 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (999)      372 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9605 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (999)    91484 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (999)    93596 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (999)     9949 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      172 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6668 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.621349 pharmpy-core-0.99.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      171 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12805 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (999)      104 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2012 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2381 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5067 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1405 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (999)      209 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (999)      430 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (999)      577 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1269 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (999)      636 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2619 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2166 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1275 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (999)      603 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      596 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      751 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (999)      780 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2010 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (999)      253 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (999)      342 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (999)      444 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (999)      269 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (999)      850 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (999)      134 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2105 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (999)      671 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4183 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      177 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11496 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5431 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6174 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (999)       83 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19639 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2372 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (999)      848 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (999)    33766 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.625349 pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      191 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4507 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18481 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (999)      164 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2422 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (999)    27707 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (999)       98 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2870 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (999)      110 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      687 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/simfit/results.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      181 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2632 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/pkpd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4746 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5173 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2152 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5676 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (999)     2499 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      830 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1209 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (999)      325 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4460 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2843 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2805 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (999)      289 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9287 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12310 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      807 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1390 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1332 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (999)      229 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1540 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2922 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7332 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.629349 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)    49279 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    47674 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      114 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-23 14:46:28.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (999)      270 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       17 2023-08-23 14:55:36.000000 pharmpy-core-0.99.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (999)     8805 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (999)      403 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/external/
+-rw-r--r--   0 runner    (1001) docker     (999)      505 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/external/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2338 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/external/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1721 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/external/test_rxode.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (999)     1152 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1522 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1557 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1096 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (999)      640 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1115 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4025 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7912 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1772 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7834 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8845 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3551 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1070 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/integration/test_structsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (999)    15348 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (999)      223 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5505 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3863 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (999)      485 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.633350 pharmpy-core-0.99.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10111 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5597 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3047 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8855 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (999)    29709 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.637350 pharmpy-core-0.99.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4950 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1023 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6657 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4448 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (999)      246 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (999)    34423 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14266 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (999)    30999 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4679 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4191 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22068 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1301 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3651 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4607 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (999)      522 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (999)    68275 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_odes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3142 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (999)    54979 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_parameter_variability.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7614 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4462 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_pd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1154 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7765 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1751 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.637350 pharmpy-core-0.99.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (999)      495 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.637350 pharmpy-core-0.99.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (999)    13614 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.641350 pharmpy-core-0.99.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (999)      295 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (999)      834 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (999)    28308 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6044 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (999)      587 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1525 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2372 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10795 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7717 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      974 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (999)      339 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1080 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (999)      490 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4609 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10121 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2673 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (999)      361 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2045 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8868 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (999)    36833 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3822 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1734 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5595 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.641350 pharmpy-core-0.99.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.641350 pharmpy-core-0.99.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (999)    52275 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.645350 pharmpy-core-0.99.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (999)     4053 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (999)    59142 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.645350 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21259 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      668 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.645350 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.653351 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    22061 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1009 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21670 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1005 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21677 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1012 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    22067 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21680 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21680 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21680 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21680 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2978 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    22454 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    22067 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1020 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1016 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1023 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1026 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1730 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)      168 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.653351 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (999)     1210 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    10369 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     9105 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1014 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/failed_run.ext
+-rw-r--r--   0 runner    (1001) docker     (999)      422 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/failed_run.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    23702 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    19648 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    13342 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (999)      345 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    10316 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.653351 pharmpy-core-0.99.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (999)     6241 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (999)    39432 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (999)    22896 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1277 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    11250 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1623 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     4861 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2884 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    26246 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1553 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13993 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (999)    24625 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     4861 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (999)     4861 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2884 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    26183 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1599 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13993 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     2472 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14234 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      618 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9547 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      733 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      190 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.589347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (999)     2032 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (999)     1615 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17620 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      815 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.657351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (999)    14783 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    91887 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.661351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (999)    36515 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1963 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    16505 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      384 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13947 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    59168 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    37889 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (999)   115118 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    82511 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     2273 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    75841 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.661351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     5179 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      648 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.585347 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.665351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (999)    15883 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    18122 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    15469 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    26695 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      688 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     8760 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      661 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      972 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1564 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17548 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      691 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6956 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    13203 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    14451 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     2492 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    11801 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1393 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     5460 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1170 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17299 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      735 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6933 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    16143 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    14090 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    54699 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    31702 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    19741 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    31702 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (999)    13140 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.665351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (999)   178666 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (999)  1091059 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.665351 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (999)     4152 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    38485 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      841 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    41718 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.669352 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      884 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      665 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      846 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      707 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      701 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      719 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      735 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      769 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      826 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      784 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    18812 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (999)      937 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.673352 pharmpy-core-0.99.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (999)     1546 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)     3072 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (999)     1716 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1827 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    19098 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    12566 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1306 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    90456 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      703 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    12377 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1716 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1827 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21336 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      704 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    12566 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (999)   175384 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (999)   185992 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (999)     4764 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)   105888 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (999)     2816 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)    70155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (999)    11500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (999)      189 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1346 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    12218 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    10093 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      367 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_conc.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      557 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_des_assignments.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6107 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (999)      982 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    10527 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      428 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      709 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    10693 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      273 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     4633 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      763 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (999)      982 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    10540 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      345 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      470 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      629 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      341 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      947 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      736 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (999)      633 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.csv
+-rw-r--r--   0 runner    (1001) docker     (999)      975 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.ctl
+-rw-r--r--   0 runner    (1001) docker     (999)     1619 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    12138 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      461 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.mod
+-rw-r--r--   0 runner    (1001) docker     (999)      631 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1959 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd_mytab
+-rw-r--r--   0 runner    (1001) docker     (999)    36053 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     2851 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21259 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      666 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    90151 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (999)    22114 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (999)   298562 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    28308 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      712 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6933 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    17010 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.677352 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (999)   370034 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     4838 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    16579 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      873 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     2350 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14595 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      803 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    11716 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     2824 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17210 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     2620 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    12617 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    24133 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (999)   262826 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     2472 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    15014 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      638 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     3943 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     2198 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)   392990 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     3262 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17544 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1045 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.677352 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)     1512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    13182 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      672 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    12417 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)   276902 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (999)   180553 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)      337 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (999)     1812 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     3068 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)    10037 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     5383 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (999)      565 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      434 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      215 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      809 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      761 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     3813 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     2723 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      325 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)      260 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (999)     1896 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)    38957 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (999)      187 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (999)     1882 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)    20500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     2115 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)      318 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (999)     1819 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     1762 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)     8045 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.681352 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)     6870 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (999)   108031 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.685353 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    16221 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    16509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      365 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1454 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17071 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      484 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    16730 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.589347 pharmpy-core-0.99.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.685353 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)       50 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (999)    13424 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    13450 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    13336 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    13843 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.689353 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17040 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      394 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     5263 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17040 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      394 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     5263 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17040 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      394 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     5263 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    17040 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      394 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     5377 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      767 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    11625 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      407 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      767 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    11637 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      406 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      767 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    11623 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (999)      995 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    15116 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     1856 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     4615 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     4589 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     4703 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     4196 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1579 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      265 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.689353 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)       50 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      353 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.689353 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (999)     1983 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14761 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1110 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13993 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    19440 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     3246 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.693353 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9040 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6946 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    93135 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    16221 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      393 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      393 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     4392 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (999)     4392 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    21654 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1083 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    13826 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1225 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    10472 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1162 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1225 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    10750 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1188 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    14006 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1816 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     2970 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1852 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)       39 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (999)     5485 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)      705 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    12131 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (999)     1280 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (999)   137744 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (999)   316422 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1856 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    13850 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      700 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    11536 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (999)     1985 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (999)    11647 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.697353 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.701354 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (999)    63331 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (999)      591 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6973 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    54391 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    38720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (999)     1306 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14039 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13972 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)     1306 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    14039 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    13972 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (999)      653 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (999)     9500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (999)     6986 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    73024 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    73024 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    36512 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (999)    21489 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.705354 pharmpy-core-0.99.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (999)    24788 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)    50648 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)   130598 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)    12291 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)  1360720 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     6524 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)   205797 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)   197228 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)    12639 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)      787 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)   105603 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     7841 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (999)    57352 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.589347 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (999)      787 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.589347 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (999)   183701 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (999)     4639 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:50:52.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)     7143 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (999)      707 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)     7120 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     1488 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    91188 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      881 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    12377 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    70155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (999)      169 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (999)     1796 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.709354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)     7112 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     1761 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    91119 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      834 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    17187 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    70155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (999)      169 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (999)     1796 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.713354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.713354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)    53630 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     1943 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    91754 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      975 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    17187 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    70155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (999)      169 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (999)     2012 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.713354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.713354 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)    54979 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (999)     1943 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (999)    91879 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (999)    17187 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (999)    70155 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (999)      169 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (999)     2012 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (999)    47403 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (999)   105597 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.717354 pharmpy-core-0.99.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2400 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7559 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1369 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8607 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3914 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)      500 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3020 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (999)      956 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (999)    28369 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9657 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3536 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4328 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11786 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1096 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10258 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10900 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1799 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16689 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2622 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6858 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19845 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (999)      247 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (999)      985 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3385 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_structsearch.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2962 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1535 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 14:55:36.717354 pharmpy-core-0.99.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (999)     2051 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7060 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (999)      318 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3173 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)      198 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4384 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3971 2023-08-23 14:45:05.000000 pharmpy-core-0.99.0/tox.ini
```

### Comparing `pharmpy-core-0.98.2/AUTHORS.rst` & `pharmpy-core-0.99.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/CHANGELOG.rst` & `pharmpy-core-0.99.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+0.99.0 (2023-08-23)
+-------------------
+
+New features
+============
+
+* Add function modeling.set_reference_values
+* Add function modeling.set_lloq_data
+* Parse IV+oral models using CMT column
+* Specify DV in RUVSearch
+* Option to add logit IIV in ``add_iiv``
+* New options for remove_loq_data
+
+Changes
+=======
+
+* Make Task and Workflow immutable
+* Ignore fixed IIVs/IOVs in IIVSearch and IOVSearch
+
+Bugfixes
+========
+
+* Fix bug where epsilons where removed in ``remove_iiv``
+* Fix bug in ``create_basic_pk_model`` to handle space separated datasets
+
 0.98.0 (2023-07-21)
 -------------------
 
 New features
 ============
 
 * Support for multiple doses
```

### Comparing `pharmpy-core-0.98.2/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.99.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/LICENSE` & `pharmpy-core-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/LICENSE.LESSER` & `pharmpy-core-0.99.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/MANIFEST.in` & `pharmpy-core-0.99.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/PKG-INFO` & `pharmpy-core-0.99.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.98.2
+Version: 0.99.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,39 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.99.0 (2023-08-23)
+-------------------
+
+New features
+============
+
+* Add function modeling.set_reference_values
+* Add function modeling.set_lloq_data
+* Parse IV+oral models using CMT column
+* Specify DV in RUVSearch
+* Option to add logit IIV in ``add_iiv``
+* New options for remove_loq_data
+
+Changes
+=======
+
+* Make Task and Workflow immutable
+* Ignore fixed IIVs/IOVs in IIVSearch and IOVSearch
+
+Bugfixes
+========
+
+* Fix bug where epsilons where removed in ``remove_iiv``
+* Fix bug in ``create_basic_pk_model`` to handle space separated datasets
+
 0.98.0 (2023-07-21)
 -------------------
 
 New features
 ============
 
 * Support for multiple doses
```

### Comparing `pharmpy-core-0.98.2/README.rst` & `pharmpy-core-0.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/NONMEM.rst` & `pharmpy-core-0.99.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/Pharmpy_logo.svg` & `pharmpy-core-0.99.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.99.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/_ext/conversion.py` & `pharmpy-core-0.99.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.99.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/allometry.rst` & `pharmpy-core-0.99.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/amd.rst` & `pharmpy-core-0.99.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/api.rst` & `pharmpy-core-0.99.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/bootstrap.rst` & `pharmpy-core-0.99.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/cdd.rst` & `pharmpy-core-0.99.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/cli.rst` & `pharmpy-core-0.99.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/conf.py` & `pharmpy-core-0.99.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.98.2'
+version = release = '0.99.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.98.2/docs/configuration.rst` & `pharmpy-core-0.99.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/contribute.rst` & `pharmpy-core-0.99.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/covsearch.rst` & `pharmpy-core-0.99.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/crossval.rst` & `pharmpy-core-0.99.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/custom.css` & `pharmpy-core-0.99.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/data.rst` & `pharmpy-core-0.99.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/design.rst` & `pharmpy-core-0.99.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/estmethod.rst` & `pharmpy-core-0.99.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/frem.rst` & `pharmpy-core-0.99.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/getting_started.rst` & `pharmpy-core-0.99.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/help_functions.py` & `pharmpy-core-0.99.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/iivsearch.rst` & `pharmpy-core-0.99.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.99.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/images/tools.png` & `pharmpy-core-0.99.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/index.rst` & `pharmpy-core-0.99.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/iovsearch.rst` & `pharmpy-core-0.99.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/license.rst` & `pharmpy-core-0.99.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/linearize.rst` & `pharmpy-core-0.99.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/model.rst` & `pharmpy-core-0.99.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/modelfit.rst` & `pharmpy-core-0.99.0/docs/modelfit.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/modeling.rst` & `pharmpy-core-0.99.0/docs/modeling.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/modelsearch.rst` & `pharmpy-core-0.99.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/nonmem_plugin.rst` & `pharmpy-core-0.99.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/pharmr_logo.svg` & `pharmpy-core-0.99.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/plots.rst` & `pharmpy-core-0.99.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/plugins.rst` & `pharmpy-core-0.99.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/projects.rst` & `pharmpy-core-0.99.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/qa.rst` & `pharmpy-core-0.99.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/ruvsearch.rst` & `pharmpy-core-0.99.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/scm.rst` & `pharmpy-core-0.99.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/simeval.rst` & `pharmpy-core-0.99.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/tools.rst` & `pharmpy-core-0.99.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/docs/using_r.rst` & `pharmpy-core-0.99.0/docs/using_r.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/requirements.txt` & `pharmpy-core-0.99.0/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,107 +3,110 @@
 appdirs==1.4.4
 asttokens==2.2.1
 attrs==23.1.0
 Babel==2.12.1
 backcall==0.2.0
 beautifulsoup4==4.12.2
 bleach==6.0.0
-certifi==2023.5.7
+certifi==2023.7.22
 charset-normalizer==3.2.0
-click==8.1.6
+click==8.1.7
 cloudpickle==2.2.1
-comm==0.1.3
-commonmark==0.9.1
+comm==0.1.4
 csscompressor==0.9.5
 dask==2023.7.0
-debugpy==1.6.7
+debugpy==1.6.7.post1
 decorator==5.1.1
 defusedxml==0.7.1
 distributed==2023.7.0
 docutils==0.20.1
-entrypoints==0.4
 executing==1.2.0
-fastjsonschema==2.17.1
+fastjsonschema==2.18.0
 fsspec==2023.6.0
-HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
 importlib_metadata==6.8.0
-ipykernel==6.24.0
+ipykernel==6.25.1
 ipython==8.14.0
-ipywidgets==8.0.7
-jedi==0.18.2
+ipywidgets==8.1.0
+jedi==0.19.0
 Jinja2==3.1.2
 jsonschema==4.17.3
+jsonschema-specifications==2023.7.1
 jupyter-client==8.3.0
 jupyter-core==5.3.1
 jupyter-sphinx==0.4.0
 jupyterlab-pygments==0.2.2
 jupyterlab-widgets==3.0.8
 lark==1.1.7
 locket==1.0.0
 lxml==4.9.3
+markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 matplotlib-inline==0.1.6
+mdurl==0.1.2
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
 nbclient==0.8.0
-nbconvert==7.7.2
-nbformat==5.9.1
-nest-asyncio==1.5.6
+nbconvert==7.7.4
+nbformat==5.9.2
+nest-asyncio==1.5.7
 networkx==3.1
-numexpr==2.8.4
+numexpr==2.8.5
 numpy==1.24.3
 packaging==23.1
-pandas==1.5.3
+pandas==2.0.3
 pandocfilters==1.5.0
 parso==0.8.3
 partd==1.4.0
 pexpect==4.8.0
 pickleshare==0.7.5
-platformdirs==3.9.1
+platformdirs==3.10.0
 prompt-toolkit==3.0.39
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
-Pygments==2.15.1
-pyreadr==0.4.7
-pyrsistent==0.19.3
+Pygments==2.16.1
+pyreadr==0.4.9
 python-dateutil==2.8.2
 pytz==2023.3
 pywin32>=302,!=304; sys_platform == 'win32' and platform_python_implementation != 'PyPy'
 PyYAML==6.0.1
+referencing==0.30.2
 requests==2.31.0
-pyzmq==25.1.0
-rich==13.4.2
-scipy==1.11.1
+pyzmq==25.1.1
+rich==13.5.2
+rpds-py==0.9.2
+scipy==1.11.2
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 soupsieve==2.4.1
-Sphinx==7.0.1
-sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.1
+Sphinx==7.2.2
+sphinxcontrib-applehelp==1.0.7
+sphinxcontrib-devhelp==1.0.5
+sphinxcontrib-htmlhelp==2.0.4
 sphinxcontrib-jsmath==1.0.1
-sphinxcontrib-qthelp==1.0.3
-sphinxcontrib-serializinghtml==1.1.5
-sphinxcontrib.applehelp==1.0.4
+sphinxcontrib-qthelp==1.0.6
+sphinxcontrib-serializinghtml==1.1.9
 stack-data==0.6.2
 symengine==0.10.0
 sympy==1.12
 tblib==2.0.0
 tinycss2==1.2.1
 toolz==0.12.0
-tornado==6.3.2
+tornado==6.3.3
 traitlets==5.9.0
+typing-extensions==4.7.1
+tzdata==2023.3
 urllib3==2.0.4
 wcwidth==0.2.6
 webencodings==0.5.1
 widgetsnbextension==4.0.8
 zict==3.0.0
 zipp==3.16.2
-tflite-runtime==2.12.0; sys_platform == 'linux' and python_version == '3.9'
+tflite-runtime==2.13.0; sys_platform == 'linux' and python_version == '3.9'
 tflite_runtime @ https://github.com/hjonnala/snippets/raw/main/wheels/python3.10/tflite_runtime-2.5.0.post1-cp310-cp310-linux_x86_64.whl ; sys_platform == 'linux' and python_version == '3.10'
 --extra-index-url https://google-coral.github.io/py-repo/
 tflite_runtime==2.5.0.post1; sys_platform == 'darwin' and python_version == '3.9'
 tflite_runtime==2.5.0.post1; sys_platform == 'win32' and python_version == '3.9'
```

### Comparing `pharmpy-core-0.98.2/setup.cfg` & `pharmpy-core-0.99.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/setup.py` & `pharmpy-core-0.99.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.98.2',
+    version='0.99.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
@@ -83,14 +83,15 @@
         'scipy',
         'dask>=2022.12.1, <=2023.7.0',
         'distributed>=2022.12.1, <=2023.7.0',
         'networkx',
         'appdirs',
         'rich',
         'jupyter-sphinx',
+        'ipykernel',
     ],
     extras_require={
         'nlmixr': ["pyreadr"],
     },
     entry_points={
         'console_scripts': [
             'pharmpy             = pharmpy.__main__:run',
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/cli.py` & `pharmpy-core-0.99.0/src/pharmpy/cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/config.py` & `pharmpy-core-0.99.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/deps/altair.py` & `pharmpy-core-0.99.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/df.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/fn/type.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/fs/tmp.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/math.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/ignored.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.99.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/data.py` & `pharmpy-core-0.99.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.99.0/src/pharmpy/model/datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.99.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.99.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/estimation.py` & `pharmpy-core-0.99.0/src/pharmpy/model/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/fcon/model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/fcon/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/generic/generic.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/generic/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/error_model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/error_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/ini.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/ini.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/model_block.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/model_block.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nlmixr/sanity_checks.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nlmixr/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/advan.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/advan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+import warnings
 from typing import TYPE_CHECKING, Optional, Tuple
 
 from pharmpy.deps import sympy
 from pharmpy.model import (
     Assignment,
     Bolus,
     Compartment,
@@ -34,53 +35,55 @@
     dataset,
     control_stream: NMTranControlStream,
     advan: str,
     trans,
     des=None,
 ):
     if advan == 'ADVAN1':
-        dose = dosing(di, dataset, 1)
+        # FIXME : Require multiple doses per comp before IV+ORAL
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         central = Compartment.create(
             'CENTRAL',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=1),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         cb.add_compartment(central)
         cb.add_flow(central, output, _advan1and2_trans(trans))
         ass = _f_link_assignment(control_stream, central, 1)
         comp_map = {'CENTRAL': 1, 'OUTPUT': 2}
     elif advan == 'ADVAN2':
-        dose = dosing(di, dataset, 1)
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         depot = Compartment.create(
             'DEPOT',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=1),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         central = Compartment.create(
             'CENTRAL',
-            dose=None,
+            dose=find_dose(doses, comp_number=2, admid=2),
             lag_time=_get_alag(control_stream, 2),
             bioavailability=_get_bioavailability(control_stream, 2),
         )
         cb.add_compartment(depot)
         cb.add_compartment(central)
         cb.add_flow(central, output, _advan1and2_trans(trans))
         cb.add_flow(depot, central, sympy.Symbol('KA'))
         ass = _f_link_assignment(control_stream, central, 2)
         comp_map = {'DEPOT': 1, 'CENTRAL': 2, 'OUTPUT': 3}
     elif advan == 'ADVAN3':
-        dose = dosing(di, dataset, 1)
+        # FIXME : Multiple doses per compartment IV+ORAL
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         central = Compartment.create(
             'CENTRAL',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=2),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         peripheral = Compartment.create(
             'PERIPHERAL',
             dose=None,
             lag_time=_get_alag(control_stream, 2),
@@ -91,25 +94,25 @@
         k, k12, k21 = _advan3_trans(trans)
         cb.add_flow(central, output, k)
         cb.add_flow(central, peripheral, k12)
         cb.add_flow(peripheral, central, k21)
         ass = _f_link_assignment(control_stream, central, 1)
         comp_map = {'CENTRAL': 1, 'PERIPHERAL': 2, 'OUTPUT': 3}
     elif advan == 'ADVAN4':
-        dose = dosing(di, dataset, 1)
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         depot = Compartment.create(
             'DEPOT',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=1),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         central = Compartment.create(
             'CENTRAL',
-            dose=None,
+            dose=find_dose(doses, comp_number=2, admid=2),
             lag_time=_get_alag(control_stream, 2),
             bioavailability=_get_bioavailability(control_stream, 2),
         )
         peripheral = Compartment.create(
             'PERIPHERAL',
             dose=None,
             lag_time=_get_alag(control_stream, 3),
@@ -160,19 +163,19 @@
             if defdepot is not None:
                 defdose = defdepot
             elif deffirst_dose is not None:
                 defdose = deffirst_dose
             else:
                 raise ModelSyntaxError('Dosing compartment is unknown')
 
-        dose = dosing(di, dataset, defdose[1])
+        doses = dosing(di, dataset, defdose[1])
         obscomp = None
         for i, name in enumerate(comp_names):
             if name == defdose[0]:
-                curdose = dose
+                curdose = find_dose(doses, defdose[1])
             else:
                 curdose = None
             comp = Compartment.create(
                 name,
                 dose=curdose,
                 lag_time=_get_alag(control_stream, i),
                 bioavailability=_get_bioavailability(control_stream, i),
@@ -184,35 +187,36 @@
         compartments.append(output)
 
         assert obscomp is not None
         for from_n, to_n, rate in _find_rates(control_stream, len(compartments)):
             cb.add_flow(compartments[from_n - 1], compartments[to_n - 1], rate)
         ass = _f_link_assignment(control_stream, obscomp, defobs[1])
     elif advan == 'ADVAN10':
-        dose = dosing(di, dataset, 1)
+        # FIXME : Multiple doses per compartment needed
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         central = Compartment.create(
             'CENTRAL',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=2),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         cb.add_compartment(central)
         vm = sympy.Symbol('VM')
         km = sympy.Symbol('KM')
         t = sympy.Symbol('t')
         cb.add_flow(central, output, vm / (km + sympy.Function(central.amount.name)(t)))
         ass = _f_link_assignment(control_stream, central, 1)
         comp_map = {'CENTRAL': 1, 'OUTPUT': 2}
     elif advan == 'ADVAN11':
-        dose = dosing(di, dataset, 1)
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         central = Compartment.create(
             'CENTRAL',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=2),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         per1 = Compartment.create(
             'PERIPHERAL1',
             dose=None,
             lag_time=_get_alag(control_stream, 2),
@@ -232,25 +236,25 @@
         cb.add_flow(central, per1, k12)
         cb.add_flow(per1, central, k21)
         cb.add_flow(central, per2, k13)
         cb.add_flow(per2, central, k31)
         ass = _f_link_assignment(control_stream, central, 1)
         comp_map = {'CENTRAL': 1, 'PERIPHERAL1': 2, 'PERIPHERAL2': 3, 'OUTPUT': 4}
     elif advan == 'ADVAN12':
-        dose = dosing(di, dataset, 1)
+        doses = dosing(di, dataset, 1)
         cb = CompartmentalSystemBuilder()
         depot = Compartment.create(
             'DEPOT',
-            dose=dose,
+            dose=find_dose(doses, comp_number=1, admid=1),
             lag_time=_get_alag(control_stream, 1),
             bioavailability=_get_bioavailability(control_stream, 1),
         )
         central = Compartment.create(
             'CENTRAL',
-            dose=None,
+            dose=find_dose(doses, comp_number=2, admid=2),
             lag_time=_get_alag(control_stream, 2),
             bioavailability=_get_bioavailability(control_stream, 2),
         )
         per1 = Compartment.create(
             'PERIPHERAL1',
             dose=None,
             lag_time=_get_alag(control_stream, 3),
@@ -272,14 +276,16 @@
         cb.add_flow(central, per1, k23)
         cb.add_flow(per1, central, k32)
         cb.add_flow(central, per2, k24)
         cb.add_flow(per2, central, k42)
         ass = _f_link_assignment(control_stream, central, 2)
         comp_map = {'DEPOT': 1, 'CENTRAL': 2, 'PERIPHERAL1': 3, 'PERIPHERAL2': 4, 'OUTPUT': 5}
     elif des:
+        # FIXME : Add dose based on presence of CMT column
+
         rec_model = control_stream.get_records('MODEL')[0]
 
         subs_dict, comp_names = {}, {}
         comps = [c for c, _ in rec_model.compartments()]
         func_to_name = {}
 
         t = sympy.Symbol('t')
@@ -298,18 +304,21 @@
 
         cs = to_compartmental_system(func_to_name, eqs)
         cb = CompartmentalSystemBuilder(cs)
         for i, comp_name in enumerate(comps, start=1):
             comp = cs.find_compartment(comp_name)
             if comp is None:  # Compartments can be in $MODEL but not used in $DES
                 continue
-            if i == 1:
-                dose = dosing(di, dataset, 1)  # FIXME: Only one dose to 1st compartment
-                cb.set_dose(comp, dose)
-                comp = cb.find_compartment(comp_name)
+            admid = 1
+            if i == len(comps) and len(comps) != 1:
+                # FIXME : Always assume last comp to be CENTRAL and IV?
+                admid = 2
+            doses = dosing(di, dataset, i)
+            cb.set_dose(comp, find_dose(doses, i, admid=admid))
+            comp = cb.find_compartment(comp_name)
             f = _get_bioavailability(control_stream, i)
             cb.set_bioavailability(comp, f)
             comp = cb.find_compartment(comp_name)
             alag = _get_alag(control_stream, i)
             cb.set_lag_time(comp, alag)
 
         # Search for DEFOBSERVATION, default to first
@@ -577,30 +586,65 @@
             sympy.Symbol('K24'),
             sympy.Symbol('K42'),
             sympy.Symbol('KA'),
         )
 
 
 def dosing(di: DataInfo, dataset, dose_comp: int):
+    if 'CMT' not in di.names or di['CMT'].drop or dataset is None:
+        return ({'comp_number': dose_comp, 'dose': _dosing(di, dataset, dose_comp)},)
+    else:
+        # CMT column present
+        cmt = dataset['CMT']
+        if len(cmt.unique()) < 1:
+            # Single compartment dose
+            # Overwrite dose_comp
+            warnings.warn(
+                "CMT column present with only one value"
+                "Need ADMID column to determine doses (if multiple)"
+            )
+            comp_number = cmt[0]
+            return ({'comp_number': comp_number, 'dose': _dosing(di, dataset, comp_number)},)
+        else:
+            # Multiple different compartments
+            doses = ()
+            for comp_number in cmt.unique():
+                doses += ({'comp_number': comp_number, 'dose': _dosing(di, dataset, comp_number)},)
+            return doses
+
+
+def _dosing(di, dataset, dose_comp, cmt=False):
     if 'RATE' not in di.names or di['RATE'].drop:
         return Bolus(sympy.Symbol('AMT'))
 
-    df = dataset
+    if cmt is False:
+        df = dataset
+    else:
+        df = dataset[dataset['CMT'] == dose_comp]
+
     if df is None:
         return Bolus(sympy.Symbol('AMT'))
     elif (df['RATE'] == 0).all():
         return Bolus(sympy.Symbol('AMT'))
     elif (df['RATE'] == -1).any():
         return Infusion(sympy.Symbol('AMT'), rate=sympy.Symbol(f'R{dose_comp}'))
     elif (df['RATE'] == -2).any():
         return Infusion(sympy.Symbol('AMT'), duration=sympy.Symbol(f'D{dose_comp}'))
     else:
         return Infusion(sympy.Symbol('AMT'), rate=sympy.Symbol('RATE'))
 
 
+def find_dose(doses, comp_number, admid=1):
+    for dose in doses:
+        if dose['comp_number'] == comp_number:
+            comp_dose = dose['dose']
+            return comp_dose.replace(admid=admid)
+    return None
+
+
 def _get_alag(control_stream: NMTranControlStream, n: int):
     """Check if ALAGn is defined in model and return it else return 0"""
     alag = f'ALAG{n}'
     pkrec = control_stream.get_records('PK')[0]
     if pkrec.statements.find_assignment(alag):
         return sympy.Symbol(alag)
     else:
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/dataset.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.fs.path import path_absolute, path_relative_to
+from pharmpy.internals.immutable import frozenmapping
 from pharmpy.model import Assignment, DataInfo, EstimationSteps
 from pharmpy.model import Model as BaseModel
 from pharmpy.model import NormalDistribution, Parameter, Parameters, RandomVariables, Statements
 from pharmpy.model.model import compare_before_after_params, update_datainfo
 from pharmpy.modeling.write_csv import write_csv
 
 from .nmtran_parser import NMTranControlStream, NMTranParser
@@ -88,22 +89,21 @@
     nm_model = parse_model(code, dataset=model.dataset)
     assert isinstance(nm_model, Model)
     nm_model._datainfo = model.datainfo
     nm_model._parameters = model.parameters
     nm_model._dataset = model.dataset
     nm_model._estimation_steps = model.estimation_steps
     nm_model._initial_individual_estimates = model.initial_individual_estimates
-    # FIXME: This is handled equivalently to dependent variables, should handle multiple DVs
-    new_obs_trans = {sympy.Symbol('Y'): sympy.Symbol('Y')}
+    new_obs_trans = frozenmapping({dv: dv for dv in model.dependent_variables.keys()})
     internals = nm_model.internals.replace(old_parameters=Parameters())
     nm_model = nm_model.replace(
         name=model.name,
         value_type=model.value_type,
         observation_transformation=new_obs_trans,
-        dependent_variables={sympy.Symbol('Y'): 1},
+        dependent_variables=model.dependent_variables,
         random_variables=model.random_variables,
         statements=model.statements,
         description=model.description,
         internals=internals,
     )
     nm_model = nm_model.update_source()
     if model.statements.ode_system:
@@ -373,14 +373,15 @@
         name=name,
         parameters=parameters,
         random_variables=rvs,
         statements=statements,
         dataset=dataset,
         datainfo=di,
         dependent_variables=dependent_variables,
+        observation_transformation=obs_trans,
         estimation_steps=estimation_steps,
         parent_model=None,
         initial_individual_estimates=init_etas,
         filename_extension=filename_extension,
         value_type=value_type,
         description=description,
         internals=internals,
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/nmtran_parser.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/parsing.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
             cond = expr.args[0][1]
             if cond.lhs == sympy.Symbol("DVID") and cond.rhs == 1:
                 ass1 = s.replace(symbol=sympy.Symbol('Y_1'), expression=expr.args[0][0])
                 ass2 = s.replace(symbol=sympy.Symbol('Y_2'), expression=expr.args[1][0])
                 kept.append(ass1)
                 kept.append(ass2)
                 dvs = frozenmapping({sympy.Symbol('Y_1'): 1, sympy.Symbol('Y_2'): 2})
-                obs_trans = {sympy.Symbol('Y_1'): sympy.Symbol('Y_1')}
+                obs_trans = frozenmapping({dv: dv for dv in dvs.keys()})
                 change = True
                 continue
         kept.append(s)
     after = Statements(tuple(kept))
     if statements.ode_system is not None:
         statements = statements.before_odes + statements.ode_system + after
         if change:  # $ERROR
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/code_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/code_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/data_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/factory.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/model_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/omega_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/omega_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/option_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/parsers.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/problem_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/sizes_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/subroutine_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/table_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/table_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/records/theta_record.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/table.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/nonmem/update.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/nonmem/update.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/rxode/model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/rxode/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/external/utils.py` & `pharmpy-core-0.99.0/src/pharmpy/model/external/utils.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/model.py` & `pharmpy-core-0.99.0/src/pharmpy/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import json
 import warnings
 from pathlib import Path
 
 import pharmpy
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
-from pharmpy.internals.immutable import Immutable, frozenmapping
+from pharmpy.internals.df import hash_df_runtime
+from pharmpy.internals.immutable import Immutable, cache_method, frozenmapping
 from pharmpy.model.external import detect_model
 
 from .datainfo import ColumnInfo, DataInfo
 from .estimation import EstimationSteps
 from .parameters import Parameters
 from .random_variables import RandomVariables
 from .statements import ODESystem, Statements
@@ -95,15 +96,15 @@
     def create(
         cls,
         name,
         parameters=None,
         random_variables=None,
         statements=None,
         dataset=None,
-        datainfo=None,
+        datainfo=DataInfo(),
         dependent_variables=None,
         observation_transformation=None,
         estimation_steps=None,
         modelfit_results=None,
         parent_model=None,
         initial_individual_estimates=None,
         filename_extension='',
@@ -140,17 +141,20 @@
             statements=statements,
             modelfit_results=modelfit_results,
             description=description,
             parent_model=parent_model,
             filename_extension=filename_extension,
             internals=internals,
             initial_individual_estimates=initial_individual_estimates,
+            dataset=dataset,
+            datainfo=datainfo,
         )
 
-    def _canonicalize_value_type(self, value):
+    @staticmethod
+    def _canonicalize_value_type(value):
         allowed_strings = ('PREDICTION', 'LIKELIHOOD', '-2LL')
         if isinstance(value, str):
             if value.upper() not in allowed_strings:
                 raise ValueError(
                     f"Cannot set value_type to {value}. Must be one of {allowed_strings} "
                     f"or a symbol"
                 )
@@ -319,15 +323,15 @@
         initial_individual_estimates = kwargs.get(
             'initial_individual_estimates', self.initial_individual_estimates
         )
         filename_extension = kwargs.get('filename_extension', self.filename_extension)
         if not isinstance(filename_extension, str):
             raise TypeError("Filename extension has to be of string type")
         if 'value_type' in kwargs:
-            value_type = self._canonicalize_value_type(kwargs['value_type'])
+            value_type = Model._canonicalize_value_type(kwargs['value_type'])
         else:
             value_type = self.value_type
         description = kwargs.get('description', self.description)
         internals = kwargs.get('internals', self._internals)
         return self.__class__(
             name=name,
             dependent_variables=dependent_variables,
@@ -410,25 +414,27 @@
         if self.datainfo != other.datainfo:
             return False
         if self.value_type != other.value_type:
             return False
 
         return True
 
+    @cache_method
     def __hash__(self):
         return hash(
             (
                 self._parameters,
                 self._random_variables,
                 self._statements,
                 self._dependent_variables,
                 self._observation_transformation,
                 self._estimation_steps,
                 self._initial_individual_estimates,
                 self._datainfo,
+                hash_df_runtime(self._dataset),
                 self._value_type,
             )
         )
 
     def to_dict(self):
         if self._initial_individual_estimates is not None:
             ie = self._initial_individual_estimates.to_dict()
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/parameters.py` & `pharmpy-core-0.99.0/src/pharmpy/model/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.99.0/src/pharmpy/model/random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/results.py` & `pharmpy-core-0.99.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/model/statements.py` & `pharmpy-core-0.99.0/src/pharmpy/model/statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -924,15 +924,18 @@
         >>> model.statements.ode_system.dosing_compartment[0]
         Compartment(CENTRAL, amount=A_CENTRAL, dose=Bolus(AMT, admid=1))
         """
         dosing_comps = tuple()
         for node in _comps(self._g):
             if node.dose is not None:
                 if node.name != self.central_compartment.name:
-                    dosing_comps = (node,) + dosing_comps
+                    if len(dosing_comps) >= 2:
+                        dosing_comps = dosing_comps[:-1] + (node,) + dosing_comps[-1:]
+                    else:
+                        dosing_comps = (node,) + dosing_comps
                 else:
                     dosing_comps = dosing_comps + (node,)
 
         if len(dosing_comps) != 0:
             return dosing_comps
 
         raise ValueError('No dosing compartment exists')
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     get_number_of_observations_per_individual,
     get_observations,
     list_time_varying_covariates,
     read_dataset_from_datainfo,
     remove_loq_data,
     set_covariates,
     set_dvid,
+    set_lloq_data,
+    set_reference_values,
     translate_nmtran_time,
     undrop_columns,
 )
 from .error import (
     has_additive_error_model,
     has_combined_error_model,
     has_proportional_error_model,
@@ -361,23 +363,25 @@
     'set_estimation_step',
     'set_evaluation_step',
     'set_first_order_absorption',
     'set_first_order_elimination',
     'set_iiv_on_ruv',
     'set_initial_condition',
     'set_initial_estimates',
+    'set_lloq_data',
     'set_lower_bounds',
     'set_upper_bounds',
     'set_michaelis_menten_elimination',
     'set_mixed_mm_fo_elimination',
     'set_name',
     'set_ode_solver',
     'set_peripheral_compartments',
     'set_power_on_ruv',
     'set_proportional_error_model',
+    'set_reference_values',
     'set_seq_zo_fo_absorption',
     'set_time_varying_error_model',
     'set_tmdd',
     'set_transit_compartments',
     'set_weighted_error_model',
     'set_zero_order_absorption',
     'set_zero_order_elimination',
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/basic_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         interaction=True,
         maximum_evaluations=99999,
         predictions=['CIPREDI'],
         residuals=['CWRES'],
     )
     eststeps = EstimationSteps.create([est])
 
-    model = Model(
+    model = Model.create(
         name='start',
         statements=stats,
         estimation_steps=eststeps,
         dependent_variables={y_ass.symbol: 1},
         random_variables=rvs,
         parameters=params,
         description='Start model',
@@ -138,49 +138,61 @@
         model = set_first_order_absorption(model)
         model = set_initial_estimates(model, {'POP_MAT': mat_init})
         model = add_iiv(model, list_of_parameters='MAT', expression='exp', initial_estimate=0.1)
 
     return model
 
 
-def _create_default_datainfo(path):
-    path = path_absolute(path)
-    datainfo_path = path.with_suffix('.datainfo')
-    if datainfo_path.is_file():
-        di = DataInfo.read_json(datainfo_path)
-        di = di.replace(path=path)
-    else:
-        colnames = list(pd.read_csv(path, nrows=0))
-        column_info = []
-        for colname in colnames:
-            if colname == 'ID' or colname == 'L1':
-                info = ColumnInfo.create(colname, type='id', scale='nominal', datatype='int32')
-            elif colname == 'DV':
-                info = ColumnInfo.create(colname, type='dv')
-            elif colname == 'TIME':
-                if not set(colnames).isdisjoint({'DATE', 'DAT1', 'DAT2', 'DAT3'}):
-                    datatype = 'nmtran-time'
-                else:
-                    datatype = 'float64'
-                info = ColumnInfo.create(colname, type='idv', scale='ratio', datatype=datatype)
-            elif colname == 'EVID':
-                info = ColumnInfo.create(colname, type='event', scale='nominal')
-            elif colname == 'MDV':
-                if 'EVID' in colnames:
-                    info = ColumnInfo.create(colname, type='mdv')
+def _create_default_datainfo(path_or_df):
+    if not isinstance(path_or_df, pd.DataFrame):
+        path = path_absolute(path_or_df)
+        datainfo_path = path.with_suffix('.datainfo')
+        if datainfo_path.is_file():
+            di = DataInfo.read_json(datainfo_path)
+            di = di.replace(path=path)
+            return di
+        else:
+            with open(path) as file:
+                first_line = file.readline()
+                if ',' not in first_line:
+                    colnames = list(pd.read_csv(path, nrows=0, sep=r'\s+'))
+                    separator = r'\s+'
                 else:
-                    info = ColumnInfo.create(
-                        colname, type='event', scale='nominal', datatype='int32'
-                    )
-            elif colname == 'AMT':
-                info = ColumnInfo.create(colname, type='dose', scale='ratio')
+                    colnames = list(pd.read_csv(path, nrows=0))
+                    separator = ','
+    else:
+        colnames = path_or_df.columns
+        separator = None
+        path = None
+
+    column_info = []
+    for colname in colnames:
+        if colname == 'ID' or colname == 'L1':
+            info = ColumnInfo.create(colname, type='id', scale='nominal', datatype='int32')
+        elif colname == 'DV':
+            info = ColumnInfo.create(colname, type='dv')
+        elif colname == 'TIME':
+            if not set(colnames).isdisjoint({'DATE', 'DAT1', 'DAT2', 'DAT3'}):
+                datatype = 'nmtran-time'
+            else:
+                datatype = 'float64'
+            info = ColumnInfo.create(colname, type='idv', scale='ratio', datatype=datatype)
+        elif colname == 'EVID':
+            info = ColumnInfo.create(colname, type='event', scale='nominal')
+        elif colname == 'MDV':
+            if 'EVID' in colnames:
+                info = ColumnInfo.create(colname, type='mdv')
             else:
-                info = ColumnInfo.create(colname)
-            column_info.append(info)
-        di = DataInfo.create(column_info, path=path, separator=',')
+                info = ColumnInfo.create(colname, type='event', scale='nominal', datatype='int32')
+        elif colname == 'AMT':
+            info = ColumnInfo.create(colname, type='dose', scale='ratio')
+        else:
+            info = ColumnInfo.create(colname)
+        column_info.append(info)
+    di = DataInfo.create(column_info, path=path, separator=separator)
     return di
 
 
 def dosing(di: DataInfo, dataset, dose_comp: int):
     # FIXME: Copied from plugins.nonmem.advan
     if di is None:
         return Bolus(sympy.Symbol('AMT'))
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,205 +1,228 @@
-"""
-:meta private:
-"""
-from typing import Optional
-
-from pharmpy.deps import sympy
-from pharmpy.internals.expr.funcs import PHI
-from pharmpy.model import Assignment, EstimationSteps, JointNormalDistribution, Model
-
-from .data import remove_loq_data
-from .expressions import _simplify_expression_from_parameters, create_symbol
-
-SUPPORTED_METHODS = frozenset(['m1', 'm3', 'm4'])
-
-
-def transform_blq(model: Model, method: str = 'm4', lloq: Optional[float] = None):
-    """Transform for BLQ data
-
-    Transform a given model, methods available are m1, m3, and m4 [1]_. Current limits of the
-    m3 and m4 method:
-
-    * Does not support covariance between epsilons
-    * Supports additive, proportional, combined, and power error model
-
-    .. [1] Beal SL. Ways to fit a PK model with some data below the quantification
-    limit. J Pharmacokinet Pharmacodyn. 2001 Oct;28(5):481-504. doi: 10.1023/a:1012299115260.
-    Erratum in: J Pharmacokinet Pharmacodyn 2002 Jun;29(3):309. PMID: 11768292.
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Any, List, Optional, Union
+
+import pharmpy.tools.estmethod.algorithms as algorithms
+from pharmpy.deps import numpy as np
+from pharmpy.deps import pandas as pd
+from pharmpy.internals.fn.signature import with_same_arguments_as
+from pharmpy.internals.fn.type import with_runtime_arguments_type_check
+from pharmpy.model import Model
+from pharmpy.modeling import has_linear_odes
+from pharmpy.results import ModelfitResults
+from pharmpy.tools import summarize_errors, summarize_modelfit_results
+from pharmpy.tools.common import ToolResults
+from pharmpy.tools.modelfit import create_fit_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
+
+EST_METHODS = ('FOCE', 'FO', 'IMP', 'IMPMAP', 'ITS', 'SAEM', 'LAPLACE', 'BAYES')
+SOLVERS = ('CVODES', 'DGEAR', 'DVERK', 'IDA', 'LSODA', 'LSODI')
+COVS = ('SANDWICH', 'CPG', 'OFIM')
+
+ALGORITHMS = frozenset(['exhaustive', 'exhaustive_with_update', 'exhaustive_only_eval'])
+
+
+def create_workflow(
+    algorithm: str,
+    methods: Optional[Union[List[str], str]] = None,
+    solvers: Optional[Union[List[str], str]] = None,
+    covs: Optional[Union[List[str], str]] = None,
+    results: Optional[ModelfitResults] = None,
+    model: Optional[Model] = None,
+):
+    """Run estmethod tool.
 
     Parameters
     ----------
+    algorithm : str
+        The algorithm to use (can be 'exhaustive', 'exhaustive_with_update' or 'exhaustive_only_eval')
+    methods : list or None
+        List of estimation methods to test. Can be specified as 'all', a list of methods, or
+        None (to not test any estimation method)
+    solvers : list, str or None
+        List of solver to test. Can be specified as 'all', a list of solvers, or None (to
+        not test any solver)
+    covs : list, str or None
+        List of covariance to test. Can be specified as 'all', a list of covs, or None (to
+        not evaluate any covariance)
+    results : ModelfitResults
+        Results for model
     model : Model
         Pharmpy model
-    method : str
-        Which BLQ method to use
-    lloq : float, optional
-        LLOQ limit to use, if None Pharmpy will use the BLQ/LLOQ column in the dataset
-
-    Return
-    ------
-    Model
-        Pharmpy model object
+
+    Returns
+    -------
+    EstMethodResults
+        Estmethod tool result object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import run_estmethod, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> model = transform_blq(model, method='m4', lloq=0.1)
-    >>> model.statements.find_assignment("Y")
-        ⎧ EPS₁⋅W + F   for DV ≥ LLOQ
-        ⎪
-        ⎨CUMD - CUMDZ
-        ⎪────────────   otherwise
-    Y = ⎩ 1 - CUMDZ
-
-    See also
-    --------
-    remove_loq_data
+    >>> results = load_example_modelfit_results("pheno")
+    >>> methods = ['imp', 'saem']
+    >>> covs = None
+    >>> run_estmethod( # doctest: +SKIP
+    >>>     'reduced', methods=methods, solvers='all', covs=covs, results=results, model=model # doctest: +SKIP
+    >>> ) # doctest: +SKIP
 
     """
-    if method not in SUPPORTED_METHODS:
-        raise ValueError(
-            f'Invalid `method`: got `{method}`,' f' must be one of {sorted(SUPPORTED_METHODS)}.'
-        )
-    if method == 'm1' and not isinstance(lloq, float):
-        raise ValueError('Invalid type of `lloq` when combined with m1 method, must be float')
+    wb = WorkflowBuilder(name="estmethod")
 
-    if method == 'm1':
-        model = _m1_method(model, lloq)
-    if method in ('m3', 'm4'):
-        _verify_model(model, method)
-        model = _m3_m4_method(model, lloq, method)
+    algorithm_func = getattr(algorithms, algorithm)
 
-    return model
+    if model is not None:
+        start_task = Task('start_estmethod', start, model)
+    else:
+        start_task = Task('start_estmethod', start)
 
+    wb.add_task(start_task)
 
-def _m1_method(model, lloq):
-    return remove_loq_data(model, lloq)
+    if methods is None:
+        methods = [model.estimation_steps[-1].method]
 
+    wf_algorithm, task_base_model_fit = algorithm_func(
+        _format_input(methods, EST_METHODS),
+        _format_input(solvers, SOLVERS),
+        _format_input(covs, COVS),
+    )
+    wb.insert_workflow(wf_algorithm, predecessors=start_task)
 
-def _m3_m4_method(model, lloq, method):
-    sset = model.statements
+    wf_fit = create_fit_workflow(n=len(wb.output_tasks))
+    wb.insert_workflow(wf_fit, predecessors=wb.output_tasks)
 
-    est_steps = model.estimation_steps
-    est_steps_new = EstimationSteps([est_step.replace(laplace=True) for est_step in est_steps])
-    model = model.replace(estimation_steps=est_steps_new)
+    if task_base_model_fit:
+        model_tasks = wb.output_tasks + task_base_model_fit
+    else:
+        model_tasks = wb.output_tasks
 
-    # FIXME: handle other DVs?
-    y_symb = list(model.dependent_variables.keys())[0]
-    y = sset.find_assignment(y_symb)
-    ipred = y.expression.subs({rv: 0 for rv in model.random_variables.epsilons.names})
+    task_post_process = Task('post_process', post_process, model)
+    wb.add_task(task_post_process, predecessors=model_tasks)
 
-    if isinstance(lloq, float):
-        blq_symb = create_symbol(model, 'LLOQ')
-        blq_type = 'lloq'
-    else:
-        blq_symb, blq_type = get_blq_symb_and_type(model)
+    return Workflow(wb)
 
-    sd = _get_sd(model, y)
-    symb_dv = sympy.Symbol(model.datainfo.dv_column.name)
-    symb_fflag = create_symbol(model, 'F_FLAG')
-    symb_cumd = create_symbol(model, 'CUMD')
 
-    if blq_type == 'lloq':
-        is_above_lloq = sympy.GreaterThan(symb_dv, blq_symb)
+def _format_input(input_option, default_option):
+    if input_option == 'all':
+        return default_option
+    elif input_option is None:
+        return [None]
     else:
-        is_above_lloq = sympy.Equality(blq_symb, 0)
+        return [entry.upper() for entry in input_option]
 
-    assignments = [sd]
 
-    if isinstance(lloq, float):
-        lloq = Assignment(blq_symb, sympy.Float(lloq))
-        assignments.append(lloq)
+def start(model):
+    return model
 
-    assignments += Assignment(symb_fflag, sympy.Piecewise((0, is_above_lloq), (1, True)))
 
-    cumd = Assignment(symb_cumd, PHI((blq_symb - ipred) / sd.symbol))
-    if method == 'm3':
-        assignments += Assignment(
-            y.symbol, sympy.Piecewise((y.expression, is_above_lloq), (cumd.expression, True))
-        )
-    else:
-        assignments += cumd
-        symb_cumdz = create_symbol(model, 'CUMDZ')
-        assignments += Assignment(symb_cumdz, PHI(-ipred / sd.symbol))
-
-        y_below_lloq = (symb_cumd - symb_cumdz) / (1 - symb_cumdz)
-        assignments += Assignment(
-            y.symbol, sympy.Piecewise((y.expression, is_above_lloq), (y_below_lloq, True))
-        )
+def post_process(input_model, *models):
+    res_models = []
+    base_model = input_model
+    for model in models:
+        if model.name == 'base_model':
+            base_model = model
+        else:
+            res_models.append(model)
+
+    summary_tool = summarize_tool(models)
+    summary_models = summarize_modelfit_results(
+        [base_model.modelfit_results] + [model.modelfit_results for model in res_models],
+        include_all_estimation_steps=True,
+    )
+    summary_errors = summarize_errors(m.modelfit_results for m in models)
+    summary_settings = summarize_estimation_steps([base_model] + res_models)
 
-    y_idx = sset.find_assignment_index(y.symbol)
-    sset_new = sset[:y_idx] + assignments + sset[y_idx + 1 :]
-    model = model.replace(statements=sset_new)
-
-    return model.update_source()
-
-
-def has_blq_transformation(model: Model):
-    # FIXME: make more general
-    y = list(model.dependent_variables.keys())[0]
-    y_expr = model.statements.error.find_assignment(y).expression
-    if not isinstance(y_expr, sympy.Piecewise):
-        return False
-    for statement, cond in y_expr.args:
-        blq_symb, _ = get_blq_symb_and_type(model)
-        if blq_symb in cond.free_symbols:
-            break
+    if base_model.name == input_model.name:
+        models = res_models
     else:
-        return False
+        models = [base_model] + res_models
 
-    expected_m3 = ['SD', 'F_FLAG']
-    expected_m4 = ['SD', 'F_FLAG', 'CUMD', 'CUMDZ']
-    return _has_all_expected_symbs(model.statements.error, expected_m3) or _has_all_expected_symbs(
-        model.statements.error, expected_m4
+    return EstMethodResults(
+        summary_tool=summary_tool,
+        summary_models=summary_models,
+        summary_settings=summary_settings,
+        summary_errors=summary_errors,
+        models=models,
     )
 
 
-def get_blq_symb_and_type(model: Model):
-    try:
-        blq_datainfo = model.datainfo.typeix['lloq']
-        return sympy.Symbol(blq_datainfo[0].name), 'lloq'
-    except IndexError:
-        try:
-            blq_datainfo = model.datainfo.typeix['blqdv']
-            return sympy.Symbol(blq_datainfo[0].name), 'blqdv'
-        except IndexError:
-            return sympy.Symbol('LLOQ'), 'lloq'
-
-
-def _has_all_expected_symbs(sset, expected_symbs):
-    symb_names = [s.symbol.name for s in sset]
-    return all(symb in symb_names for symb in expected_symbs)
-
-
-def _verify_model(model, method):
-    rvs = model.random_variables.epsilons
-    if any(isinstance(rv, JointNormalDistribution) for rv in rvs):
+@dataclass(frozen=True)
+class EstMethodResults(ToolResults):
+    rst_path = Path(__file__).resolve().parent / 'report.rst'
+
+    summary_settings: Optional[Any] = None
+
+
+def summarize_tool(models):
+    rows = {}
+
+    for model in models:
+        description, parent_model = model.description, model.parent_model
+        res = model.modelfit_results
+        if res is not None:
+            ofv = res.ofv
+            runtime_est = res.estimation_runtime_iterations.iloc[0]
+        else:
+            ofv, runtime_est = np.nan, np.nan
+        rows[model.name] = (description, ofv, runtime_est, parent_model)
+
+    colnames = ['description', 'ofv', 'runtime_estimation', 'parent_model']
+    index = pd.Index(rows.keys(), name='model')
+    df = pd.DataFrame(rows.values(), index=index, columns=colnames)
+
+    return df.sort_values(by=['ofv'])
+
+
+def summarize_estimation_steps(models):
+    dfs = {}
+    for model in models:
+        df = model.estimation_steps.to_dataframe()
+        df.index = range(1, len(df) + 1)
+        dfs[model.name] = df.drop(columns=['tool_options'])
+
+    return pd.concat(dfs.values(), keys=dfs.keys())
+
+
+@with_runtime_arguments_type_check
+@with_same_arguments_as(create_workflow)
+def validate_input(algorithm, methods, solvers, covs, model):
+    if solvers is not None and has_linear_odes(model):
         raise ValueError(
-            f'Invalid input model: covariance between epsilons not supported in `method` {method}'
+            'Invalid input `model`: testing non-linear solvers on linear system is not supported'
         )
 
+    if algorithm not in ALGORITHMS:
+        raise ValueError(
+            f'Invalid `algorithm`: got `{algorithm}`, must be one of {sorted(ALGORITHMS)}.'
+        )
 
-def _get_sd(model, y):
-    y_expr = model.statements.find_assignment(y.symbol).expression
-    sd_expr = get_sd_expr(y_expr, model.random_variables, model.parameters)
-    symb_sd = create_symbol(model, 'SD')
-    return Assignment(symb_sd, sd_expr)
+    if methods is None and solvers is None and covs is None:
+        raise ValueError(
+            'Invalid search space options: please specify at least one of `methods`, `solvers`, or `covs`'
+        )
+
+    if methods is not None:
+        _validate_search_space(methods, EST_METHODS, 'methods')
 
+    if solvers is not None:
+        _validate_search_space(solvers, SOLVERS, 'solvers')
 
-def get_sd_expr(y_expr, rvs, params):
-    rv_terms = [arg for arg in y_expr.args if arg.free_symbols.intersection(rvs.free_symbols)]
-    sd_expr = []
-    for i, term in enumerate(rv_terms, 1):
-        rvs_in_term = rvs.free_symbols.intersection(term.free_symbols)
-        if len(rvs_in_term) > 1:
+    if covs is not None:
+        _validate_search_space(covs, COVS, 'covs')
+
+
+def _validate_search_space(input_search_space, allowed_search_space, option_name):
+    if isinstance(input_search_space, str):
+        if input_search_space != 'all':
             raise ValueError(
-                'Invalid input model: error model not supported, terms in error model cannot contain '
-                'more than one random variable'
+                f'Invalid `{option_name}`: if option is str it must be `all`, got {input_search_space}'
+            )
+    else:
+        option_diff = {option.upper() for option in input_search_space}.difference(
+            allowed_search_space
+        )
+        if option_diff:
+            raise ValueError(
+                f'Invalid `{option_name}`: {option_diff} not in {sorted(allowed_search_space)}'
             )
-        expr = rvs.replace_with_sympy_rvs(term)
-        sd_expr.append(sympy.stats.std(expr))
-
-    return _simplify_expression_from_parameters(
-        sympy.sqrt(sympy.Add(*[expr**2 for expr in sd_expr])), params
-    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/common.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/data.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     55   0.0  25.0  1.1   4.0  0.0  1.0  1.0
     56   0.0  12.0  0.6   4.0  0.0  1.0  1.0
     57   0.0  20.0  2.1   6.0  0.0  1.0  1.0
     58   0.0  14.0  1.4   8.0  0.0  1.0  1.0
     59   0.0  22.8  1.1   6.0  0.0  1.0  1.0
     """
     idlab = model.datainfo.id_column.name
-    baselines = model.dataset.groupby(idlab).nth(0)
+    baselines = model.dataset.groupby(idlab).nth(0).set_index(idlab)
     return baselines
 
 
 def set_covariates(model: Model, covariates: List[str]):
     """Set columns in the dataset to be covariates in the datainfo
 
     Parameters
@@ -1395,53 +1395,196 @@
         timecol = timecol.replace(unit='h')
     timecol = timecol.replace(datatype='float64')
     di = di.set_column(timecol)
     model = model.replace(datainfo=di, dataset=df)
     return model.update_source()
 
 
-def remove_loq_data(model: Model, lloq: Optional[float] = None, uloq: Optional[float] = None):
+def _loq_mask(
+    model: Model,
+    lloq: Optional[Union[float, str]] = None,
+    uloq: Optional[Union[float, str]] = None,
+    blq: Optional[str] = None,
+    alq: Optional[str] = None,
+):
+    """Boolean series with False for lloq records and True for non-lloq
+    Options as remove_loq_data
+    """
+    if blq and lloq:
+        raise ValueError("Cannot specify blq and lloq at the same time")
+    if alq and uloq:
+        raise ValueError("Cannot specify alq and uloq at the same time")
+    df = model.dataset
+    if lloq is not None or uloq is not None:
+        dv = model.datainfo.dv_column.name
+    mdv = get_mdv(model)
+    which_keep = pd.Series(True, index=df.index)
+    if isinstance(lloq, str):
+        lloq = df[lloq]
+    if isinstance(uloq, str):
+        uloq = df[uloq]
+    if lloq is not None:
+        which_keep &= (df[dv] > lloq) | mdv
+    elif blq is not None:
+        which_keep &= (df[blq] == 0) | mdv
+    if uloq is not None:
+        which_keep &= (df[dv] < uloq) | mdv
+    elif alq is not None:
+        which_keep &= (df[alq] == 0) | mdv
+    return which_keep
+
+
+def remove_loq_data(
+    model: Model,
+    lloq: Optional[Union[float, str]] = None,
+    uloq: Optional[Union[float, str]] = None,
+    blq: Optional[str] = None,
+    alq: Optional[str] = None,
+    keep: Optional[int] = 0,
+):
     """Remove loq data records from the dataset
 
-    Does nothing if none of the limits is specified.
+    Does nothing if none of the limits are specified.
 
     Parameters
     ----------
     model : Model
         Pharmpy model object
-    lloq : float
-        Lower limit of quantification. Default not specified.
-    uloq : float
-        Upper limit of quantification. Default not specified.
+    lloq : float or str
+        Value or column name for lower limit of quantification.
+    uloq : float or str
+        Value or column name for upper limit of quantification.
+    blq : str
+        Column name for below limit of quantification indicator.
+    alq : str
+        Column name for above limit of quantification indicator.
+    keep : int
+        Number of loq records to keep for each individual.
 
     Returns
     -------
     Model
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = remove_loq_data(model, lloq=10, uloq=40)
     >>> len(model.dataset)
     736
     """
-    df = model.dataset
-    dv = model.datainfo.dv_column.name
-    mdv = get_mdv(model)
-    keep = pd.Series(True, index=df.index)
-    if lloq:
-        keep &= (df[dv] >= lloq) | mdv
-    if uloq:
-        keep &= (df[dv] <= uloq) | mdv
-    model = model.replace(dataset=df[keep])
+    which_keep = _loq_mask(model, lloq=lloq, uloq=uloq, blq=blq, alq=alq)
+    df = model.dataset.copy()
+    if keep > 0:
+        idcol = model.datainfo.id_column.name
+        keep_df = pd.DataFrame({'ID': df[idcol], 'remove': ~which_keep})
+        obj = keep_df.groupby(idcol).cumsum().le(keep)['remove']
+        which_keep = obj | which_keep
+    model = model.replace(dataset=df[which_keep])
     return model.update_source()
 
 
+def set_lloq_data(
+    model: Model,
+    value: Union[str, float, sympy.Expr],
+    lloq: Optional[Union[float, str]] = None,
+    blq: Optional[str] = None,
+):
+    """Set a dv value for lloq data records
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model object
+    value : float or sympy.Expression
+        The new dv value
+    lloq : float or str
+        Value or column name for lower limit of quantification.
+    blq : str
+        Column name for below limit of quantification indicator.
+
+    Returns
+    -------
+    Model
+        Pharmpy model object
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = set_lloq_data(model, 0, lloq=10)
+    """
+    which_keep = _loq_mask(model, lloq=lloq, blq=blq)
+    df = model.dataset.copy()
+    dv = model.datainfo.dv_column.name
+    if isinstance(value, sympy.Expr) or isinstance(value, str):
+        value = df.eval(str(value))
+    df[dv] = df[dv].where(which_keep, value)
+    model = model.replace(dataset=df)
+    return model
+
+
+def set_reference_values(model: Model, refs: dict):
+    """Set reference values for selected columns
+
+        All values for each selected column will be replaced. For dose columns
+        only the values for dosing events will be replaced.
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model object
+    refs : dict
+        Pairs of column names and reference values
+
+    Returns
+    -------
+    Model
+        Pharmpy model object
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = set_reference_values(model, {'WGT': 0.5, 'AMT': 4.0})
+    >>> model.dataset
+         ID   TIME  AMT  WGT  APGR    DV  FA1  FA2
+    0     1    0.0  4.0  0.5   7.0   0.0  1.0  1.0
+    1     1    2.0  0.0  0.5   7.0  17.3  0.0  0.0
+    2     1   12.5  4.0  0.5   7.0   0.0  1.0  1.0
+    3     1   24.5  4.0  0.5   7.0   0.0  1.0  1.0
+    4     1   37.0  4.0  0.5   7.0   0.0  1.0  1.0
+    ..   ..    ...  ...  ...   ...   ...  ...  ...
+    739  59  108.3  4.0  0.5   6.0   0.0  1.0  1.0
+    740  59  120.5  4.0  0.5   6.0   0.0  1.0  1.0
+    741  59  132.3  4.0  0.5   6.0   0.0  1.0  1.0
+    742  59  144.8  4.0  0.5   6.0   0.0  1.0  1.0
+    743  59  146.8  0.0  0.5   6.0  40.2  0.0  0.0
+    <BLANKLINE>
+    [744 rows x 8 columns]
+
+    """
+    df = model.dataset
+    di = model.datainfo
+    newcols = dict()
+    dtypes = dict()
+    for colname, value in refs.items():
+        if di[colname].type == 'dose':
+            newdose = df[colname].mask(df[colname] > 0, value)
+            newcols[colname] = newdose
+        else:
+            newcols[colname] = value
+        datatype = ColumnInfo.convert_datatype_to_pd_dtype(di[colname].datatype)
+        dtypes[colname] = datatype
+    df = df.assign(**newcols).astype(dtypes)
+    model = model.replace(dataset=df)
+    return model
+
+
 class Checker:
     _all_checks = (
         ('A1', 'Body weight has unit'),
         ('A2', 'Body weight has mass unit'),
         ('A3', 'Body weight >0 and <700kg'),
         ('A4', 'Age has unit'),
         ('A5', 'Age has time unit'),
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/error.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 :meta private:
 """
 from __future__ import annotations
 
+import warnings
 from typing import List, Optional, Union
 
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.parse import parse as parse_expr
 from pharmpy.internals.expr.subs import subs
 from pharmpy.model import Assignment, Model, NormalDistribution, Parameter, Parameters, Statements
 
@@ -891,30 +892,39 @@
 
     return model.update_source()
 
 
 def set_power_on_ruv(
     model: Model,
     list_of_eps: Optional[Union[str, list]] = None,
+    dv: Union[sympy.Symbol, str, int, None] = None,
     lower_limit: Optional[float] = 0.01,
     ipred: Optional[Union[str, sympy.Symbol]] = None,
     zero_protection: bool = False,
 ):
-    """Applies a power effect to provided epsilons.
+    """Applies a power effect to provided epsilons. If a dependent variable
+    is provided, then only said epsilons affecting said variable will be changed.
 
     Initial estimates for new thetas are 1 if the error
     model is proportional, otherwise they are 0.1.
 
+    NOTE : If no DVs or epsilons are specified, all epsilons with the same name
+    will be connected to the same theta. Running the function per DV will give
+    each epsilon a specific theta.
+
     Parameters
     ----------
     model : Model
         Pharmpy model to create block effect on.
     list_of_eps : str or list or None
         Name/names of epsilons to apply power effect. If None, all epsilons will be used.
         None is default.
+    dv : Union[sympy.Symbol, str, int, None]
+        Name or DVID of dependent variable. None will change the epsilon on all occurences
+        regardless of affected dependent variable.
     lower_limit : float or None
         Lower limit of power (theta). None for no limit.
     ipred : Symbol
         Symbol to use as IPRED. Default is to autodetect expression for IPRED.
     zero_protection : bool
         Set to True to add code protecting from IPRED=0
 
@@ -934,25 +944,57 @@
 
     See also
     --------
     set_iiv_on_ruv
 
     """
     list_of_eps = _format_input_list(list_of_eps)
-    eps = model.random_variables.epsilons
-    if list_of_eps is not None:
-        eps = eps[list_of_eps]
+    eps = _get_epsilons(model, list_of_eps)
+    eps = [e for e in eps]
+    dv_symb = get_dv_symbol(model, dv)
+    y = model.statements.find_assignment(dv_symb)
     pset, sset = list(model.parameters), model.statements
 
     if ipred is None:
-        ipred = get_ipred(model)
+        # Extract ipred based on the dv
+        ipred = get_ipred(model, dv=dv_symb)
     else:
         ipred = parse_expr(ipred)
 
-    if has_proportional_error_model(model):
+    # Assert that the provided epsilons are used for the corresponding DV
+    # Else give warning
+    if (
+        dv is not None
+        and list_of_eps is not None
+        and any(
+            [
+                sympy.Symbol(e.names[0])
+                not in model.statements.after_odes.full_expression(dv_symb).free_symbols
+                for e in eps
+            ]
+        )
+    ):
+        warnings.warn(f'Some provided epsilons are not connected to the supplied DV ({dv_symb})')
+    elif dv is not None and any(
+        [
+            sympy.Symbol(e.names[0])
+            not in model.statements.after_odes.full_expression(dv_symb).free_symbols
+            for e in eps
+        ]
+    ):
+        # Only analyze epsilons connected to the given DV
+        eps = [
+            e
+            for e in eps
+            if sympy.Symbol(e.names[0])
+            in model.statements.after_odes.full_expression(dv_symb).free_symbols
+        ]
+
+    # Check for used DV, not just the first one
+    if has_proportional_error_model(model, dv=dv_symb):
         theta_init = 1
     else:
         theta_init = 0.1
 
     # Find for example W = IPRED
     ipredadj = None
     alternative = None
@@ -975,53 +1017,74 @@
                         ipredadj = s.symbol
                         break
 
         if has_blq_transformation(model):
             _, _, f = _preparations(model)
             ipred = _get_f_above_lloq(model, f)
 
-    for e in eps.names:
+    for e in eps:
+        e = e.names[0]
         theta_name = str(
             _create_symbol(
                 sset, pset, model.random_variables, model.datainfo, 'power', force_numbering=True
             )
         )
         if lower_limit is None:
             theta = Parameter(theta_name, theta_init)
         else:
             theta = Parameter(theta_name, theta_init, lower=lower_limit)
         pset.append(theta)
-        sset = sset.subs(
-            {sympy.Symbol(e) * ipred: sympy.Symbol(e)}
-        )  # To avoid getting F*EPS*F**THETA
+
+        subs_dict = {sympy.Symbol(e) * ipred: sympy.Symbol(e)}  # To avoid getting F*EPS*F**THETA
+        if not dv:
+            sset = sset.subs(subs_dict)
+        else:
+            y = y.subs(subs_dict)
+            sset = sset.reassign(y.symbol, y.expression)
+
         if alternative:  # To avoid getting W*EPS*F**THETA
-            sset = sset.subs({sympy.Symbol(e) * alternative: sympy.Symbol(e)})
+            subs_dict = {sympy.Symbol(e) * alternative: sympy.Symbol(e)}
+            if not dv:
+                sset = sset.subs(subs_dict)
+            else:
+                y = y.subs(subs_dict)
+                sset = sset.reassign(y.symbol, y.expression)
 
         if ipredadj:
-            sset = sset.subs(
-                {sympy.Symbol(e) * ipredadj: ipredadj ** sympy.Symbol(theta.name) * sympy.Symbol(e)}
-            )
+            subs_dict = {
+                sympy.Symbol(e) * ipredadj: ipredadj ** sympy.Symbol(theta.name) * sympy.Symbol(e)
+            }
+            if not dv:
+                sset = sset.subs(subs_dict)
+            else:
+                y = y.subs(subs_dict)
+                sset = sset.reassign(y.symbol, y.expression)
         else:
-            sset = sset.subs({sympy.Symbol(e): ipred ** sympy.Symbol(theta.name) * sympy.Symbol(e)})
+            subs_dict = {sympy.Symbol(e): ipred ** sympy.Symbol(theta.name) * sympy.Symbol(e)}
+            if not dv:
+                sset = sset.subs(subs_dict)
+            else:
+                y = y.subs(subs_dict)
+                sset = sset.reassign(y.symbol, y.expression)
 
         if has_blq_transformation(model):
             # FIXME: make more general
             y_above_lloq, _ = sset.find_assignment('Y').expression.args[0]
             sd = model.statements.find_assignment('SD')
             sd_new = get_sd_expr(y_above_lloq, model.random_variables, Parameters.create(pset))
             sset = sset.reassign(sd.symbol, sd_new)
-
     model = model.replace(parameters=Parameters.create(pset), statements=sset)
 
     return model.update_source()
 
 
-def get_ipred(model):
+def get_ipred(model, dv=None):
     # FIXME: handle other DVs?
-    dv = list(model.dependent_variables.keys())[0]
+    if dv is None:
+        dv = list(model.dependent_variables.keys())[0]
     expr = model.statements.after_odes.full_expression(dv)
     ipred = subs(
         expr, {sympy.Symbol(rv): 0 for rv in model.random_variables.names}, simultaneous=True
     )
     for s in model.statements:
         if isinstance(s, Assignment) and s.expression == ipred:
             ipred = s.symbol
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/evaluation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.99.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,25 +327,29 @@
     statements = model.statements
     for old_ind, assignment in _find_eta_assignments(model):
         # NOTE The sequence of old_ind must be increasing
         eta = next(iter(etas.intersection(assignment.expression.free_symbols)))
         old_def = assignment.expression
         dep = old_def.as_independent(eta)[1]
         mu = sympy.Symbol(f'mu_{index[eta]}')
-        new_def = subs(dep, {eta: mu + eta})
-        mu_expr = sympy.solve(old_def - new_def, mu)[0]
-        insertion_ind = offset + old_ind
-        statements = (
-            statements[0:insertion_ind]
-            + Assignment(mu, mu_expr)
-            + Assignment(assignment.symbol, new_def)
-            + statements[insertion_ind + 1 :]
-        )
-        offset += 1  # NOTE We need this offset because we replace one
-        # statement by two statements
+        if mu in old_def.free_symbols:
+            # If mu reference is already used, ignore
+            pass
+        else:
+            new_def = subs(dep, {eta: mu + eta})
+            mu_expr = sympy.solve(old_def - new_def, mu)[0]
+            insertion_ind = offset + old_ind
+            statements = (
+                statements[0:insertion_ind]
+                + Assignment(mu, mu_expr)
+                + Assignment(assignment.symbol, new_def)
+                + statements[insertion_ind + 1 :]
+            )
+            offset += 1  # NOTE We need this offset because we replace one
+            # statement by two statements
     model = model.replace(statements=statements).update_source()
     return model
 
 
 def simplify_expression(model: Model, expr: Union[int, float, str, sympy.Expr]):
     """Simplify expression given constraints in model
 
@@ -1197,15 +1201,15 @@
 
     Example
     -------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = set_direct_effect(model, "linear")
     >>> get_pd_parameters(model)
-    ['E0', 'S']
+    ['E0', 'Slope']
 
     See also
     --------
     get_pk_parameters
 
     """
     # FIXME: this function needs to be updated. Currently uses fixed parameter names.
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/help_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def _get_eta_symbs(eta_str, rvs, sset):
     try:
         exp_symbs = sset.find_assignment(eta_str).expression.free_symbols
     except AttributeError:
         raise KeyError(f'Symbol "{eta_str}" does not exist')
-    return [str(e) for e in exp_symbs.intersection(rvs.free_symbols)]
+    return [str(e) for e in exp_symbs.intersection(rvs.etas.free_symbols)]
 
 
 def _has_fixed_params(model, rv):
     param_names = model.random_variables[rv].parameter_names
 
     for p in model.parameters:
         if p.name in param_names and p.fix:
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/math.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/odes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1460,15 +1460,15 @@
     try:
         time_label = model.datainfo.idv_column.name
     except IndexError:
         time_min = 1.0
     else:
         obs = get_observations(model)
         time = obs.index.get_level_values(level=time_label)
-        time_min = time[time != 0].min()
+        time_min = time[time > 0].min()
 
     if param_name == 'MDT':
         return float(time_min) / 2
     elif param_name == 'MAT':
         return float(time_min) * 2
 
     raise NotImplementedError('param_name must be MDT or MAT')
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/parameter_variability.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/parameter_variability.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
     Effects that currently have templates are:
 
     - Additive (*add*)
     - Proportional (*prop*)
     - Exponential (*exp*)
     - Logit (*log*)
+    - Rescaled logit (*re_log*)
 
     For all except exponential the operation input is not needed. Otherwise user specified
     input is supported. Initial estimates for new etas are 0.09.
 
     Parameters
     ----------
     model : Model
@@ -123,19 +124,32 @@
         index = sset.find_assignment_index(list_of_parameters[i])
 
         if index is None:
             raise ValueError(f'Could not find parameter: {list_of_parameters[i]}')
         statement = sset[index]
 
         eta_addition = _create_template(expression[i], operation[i])
-        eta_addition.apply(statement.expression, eta.names[0])
 
-        sset = (
-            sset[0:index] + Assignment(statement.symbol, eta_addition.template) + sset[index + 1 :]
-        )
+        if expression[i] == "re_log":
+            # Need to add phi as well
+            phi = sympy.Symbol(f'phi_{statement.expression}')
+            eta_addition.apply(phi, eta.names[0])
+            sset = (
+                sset[0:index]
+                + Assignment(phi, sympy.log(statement.expression / (1 - statement.expression)))
+                + Assignment(statement.symbol, eta_addition.template)
+                + sset[index + 1 :]
+            )
+        else:
+            eta_addition.apply(statement.expression, eta.names[0])
+            sset = (
+                sset[0:index]
+                + Assignment(statement.symbol, eta_addition.template)
+                + sset[index + 1 :]
+            )
 
     model = model.replace(random_variables=rvs, parameters=Parameters.create(pset), statements=sset)
 
     return model.update_source()
 
 
 def add_iov(
@@ -452,14 +466,16 @@
         return EtaAddition.additive()
     elif expression == 'prop':
         return EtaAddition.proportional()
     elif expression == 'exp':
         return EtaAddition.exponential(operation_func)
     elif expression == 'log':
         return EtaAddition.logit()
+    elif expression == 're_log':
+        return EtaAddition.re_logit()
     else:
         expression = parse_expr(f'original {operation} {expression}')
         return EtaAddition(expression)
 
 
 def _get_operation_func(operation):
     """Gets sympy operation based on string"""
@@ -535,14 +551,21 @@
     def logit(cls):
         template = sympy.Symbol('original') * (
             sympy.exp(sympy.Symbol('eta_new')) / (1 + sympy.exp(sympy.Symbol('eta_new')))
         )
 
         return cls(template)
 
+    @classmethod
+    def re_logit(cls):
+        template = sympy.exp(sympy.Symbol('eta_new') * sympy.Symbol('original')) / (
+            1 + sympy.exp(sympy.Symbol('eta_new') * sympy.Symbol('original'))
+        )
+        return cls(template)
+
 
 def remove_iiv(model: Model, to_remove: Optional[Union[List[str], str]] = None):
     """
     Removes all IIV etas given a list with eta names and/or parameter names.
 
     Parameters
     ----------
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional, Union
 
 from pharmpy.deps import pandas as pd
-from pharmpy.model import Model, Parameter, Parameters
+from pharmpy.model import Model, Parameter, Parameters, RandomVariables
 
 
 def get_thetas(model: Model):
     """Get all thetas (structural parameters) of a model
 
     Parameters
     ----------
@@ -174,16 +174,23 @@
         parameter_estimates = _move_est_close_to_bounds(model, parameter_estimates)
 
     model = model.replace(parameters=model.parameters.set_initial_estimates(parameter_estimates))
 
     return model.update_source()
 
 
+def _get_nonfixed_rvs(model):
+    fixed_omegas = get_omegas(model).fixed.names
+    rvs = model.random_variables
+    nonfixed_rvs = [rv for rv in rvs if str(list(rv.variance.free_symbols)[0]) not in fixed_omegas]
+    return RandomVariables.create(nonfixed_rvs)
+
+
 def _move_est_close_to_bounds(model: Model, pe):
-    rvs, pset = model.random_variables, model.parameters
+    rvs, pset = _get_nonfixed_rvs(model), model.parameters
     est = pe.to_dict()
     sdcorr = rvs.parameters_sdcorr(est)
     newdict = est.copy()
     for dist in rvs:
         rvs = dist.names
         if len(rvs) > 1:
             sigma_sym = dist.variance
@@ -198,16 +205,17 @@
                             sd_i, sd_j = sdcorr[name_i], sdcorr[name_j]
                             newdict[param_name] = corr_new * sd_i * sd_j
                     else:
                         if not _is_zero_fix(pset[param_name]) and est[param_name] < 0.001:
                             newdict[param_name] = 0.01
         else:
             param_name = dist.variance.name
-            if not _is_zero_fix(pset[param_name]) and est[param_name] < 0.001:
-                newdict[param_name] = 0.01
+            if not pset[param_name].fix:
+                if not _is_zero_fix(pset[param_name]) and est[param_name] < 0.001:
+                    newdict[param_name] = 0.01
     return newdict
 
 
 def _is_zero_fix(param):
     return param.init == 0 and param.fix
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/pd.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/pd.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,27 @@
 
 
 def add_effect_compartment(model: Model, expr: str):
     r"""Add an effect compartment.
 
     Implemented PD models are:
 
-    * Baseline: :math:`E = E_0`
-    * Linear: :math:`E = E_0 + S \cdot C`
-    * Emax: :math:`E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }`
-    * Step effect: :math:`E = \Biggl \lbrace { E_0 \quad  \text{ if C } < 0 \atop E_0 + E_{max} \quad  \text{else}}`
-    * Sigmoidal: :math:`E = \frac {E_{max} C^n} { EC_{50}^n + C^n}`
-    * Log-linear: :math:`E = m \cdot  \text{log}(C + C_0)`
+    * Baseline:
+    .. math:: E = E_0
+    * Linear:
+    .. math:: E = E_0 + \text{slope} \cdot C
+    * Emax:
+    .. math:: E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }
+    * Step effect:
+    .. math:: E = \Biggl \lbrace {E_0 \quad \text{if C} \leq 0 \atop E_0 + E_{max} \quad \text{else}}
+    * Sigmoidal:
+    .. math::  E=\Biggl \lbrace {E_0+\frac{E_{max} \cdot C^n}{EC_{50}^n+C^n} \quad \text{if C}>0 \atop \
+            E_0 \quad \text{else}}
+    * Log-linear:
+    .. math:: E = \text{slope} \cdot \text{log}(C + C_0)
 
     Parameters
     ----------
     model : Model
         Pharmpy model
     expr : str
         Name of the PD effect function. Valid names are: baseline, linear, Emax, sigmoid, step, loglin
@@ -42,53 +49,60 @@
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = add_effect_compartment(model, "linear")
     >>> model.statements.ode_system.find_compartment("EFFECT")
-    Compartment(EFFECT, amount=A_EFFECT, input=KE0*A_CENTRAL(t))
+    Compartment(EFFECT, amount=A_EFFECT, input=KE0*A_CENTRAL(t)/V)
     """
     vc, cl = _get_central_volume_and_cl(model)
 
     odes = model.statements.ode_system
     central = odes.central_compartment
     central_amount = sympy.Function(central.amount.name)(sympy.Symbol('t'))
     cb = CompartmentalSystemBuilder(odes)
 
     ke0 = sympy.Symbol("KE0")
     model = add_individual_parameter(model, ke0.name)
 
-    effect = Compartment.create("EFFECT", input=ke0 * central_amount)
+    effect = Compartment.create("EFFECT", input=ke0 * central_amount / vc)
     cb.add_compartment(effect)
     cb.add_flow(effect, output, ke0)
 
     model = model.replace(
         statements=Statements(
             model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
         )
     )
 
-    conc_e = model.statements.ode_system.find_compartment("EFFECT").amount / vc
+    conc_e = model.statements.ode_system.find_compartment("EFFECT").amount
 
     model = _add_effect(model, expr, conc_e)
     return model
 
 
 def set_direct_effect(model: Model, expr: str):
     r"""Add an effect to a model.
 
     Implemented PD models are:
 
-    * Baseline: :math:`E = E_0`
-    * Linear: :math:`E = E_0 + S \cdot C`
-    * Emax: :math:`E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }`
-    * Step effect: :math:`E = \Biggl \lbrace { E_0 \quad  \text{ if C } < 0 \atop E_0 + E_{max} \quad  \text{else}}`
-    * Sigmoidal: :math:`E = \frac {E_{max} C^n} { EC_{50}^n + C^n}`
-    * Log-linear: :math:`E = m \cdot  \text{log}(C + C_0)`
+    * Baseline:
+    .. math:: E = E_0
+    * Linear:
+    .. math:: E = E_0 + \text{slope} \cdot C
+    * Emax:
+    .. math:: E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }
+    * Step effect:
+    .. math:: E = \Biggl \lbrace {E_0 \quad \text{if C} \leq 0 \atop E_0 + E_{max} \quad \text{else}}
+    * Sigmoidal:
+    .. math::  E=\Biggl \lbrace {E_0+\frac{E_{max} \cdot C^n}{EC_{50}^n+C^n} \quad \text{if C}>0 \atop \
+            E_0 \quad \text{else}}
+    * Log-linear:
+    .. math:: E = \text{slope} \cdot \text{log}(C + C_0)
 
     Parameters
     ----------
     model : Model
         Pharmpy model
     expr : str
         Name of PD effect function. Valid names are: baseline, linear, Emax, sigmoid, step, loglin
@@ -100,17 +114,17 @@
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = set_direct_effect(model, "linear")
     >>> model.statements.find_assignment("E")
-        A_CENTRAL⋅S
-        ─────────── + E₀
-    E =      V
+        A_CENTRAL⋅Slope
+        ─────────────── + E₀
+    E =         V
 
     """
     vc, cl = _get_central_volume_and_cl(model)
     conc = model.statements.ode_system.central_compartment.amount / vc
 
     model = _add_effect(model, expr, conc)
 
@@ -140,30 +154,35 @@
         ec50 = sympy.Symbol("EC_50")
         model = add_individual_parameter(model, ec50.name)
 
     # Add effect E
     if expr == "baseline":
         E = Assignment(sympy.Symbol('E'), e0)
     elif expr == "linear":
-        s = sympy.Symbol("S")  # slope
+        s = sympy.Symbol("Slope")
         model = add_individual_parameter(model, s.name)
         E = Assignment(sympy.Symbol('E'), e0 + s * conc)
     elif expr == "Emax":
         E = Assignment(sympy.Symbol("E"), e0 + emax * conc / (ec50 + conc))
     elif expr == "step":
-        E = Assignment(sympy.Symbol("E"), sympy.Piecewise((e0, conc < 0), (e0 + emax, True)))
+        E = Assignment(sympy.Symbol("E"), sympy.Piecewise((e0, conc <= 0), (e0 + emax, True)))
     elif expr == "sigmoid":
         n = sympy.Symbol("n")  # Hill coefficient
         model = add_individual_parameter(model, n.name)
         model = set_initial_estimates(model, {"POP_n": 1})
-        E = Assignment(sympy.Symbol("E"), emax * conc**n / (ec50**n + conc**n))
+        E = Assignment(
+            sympy.Symbol("E"),
+            sympy.Piecewise(
+                ((e0 + emax * conc**n / (ec50**n + conc**n)), conc > 0), (e0, True)
+            ),
+        )
     elif expr == "loglin":
-        m = sympy.Symbol("m")  # slope
-        model = add_individual_parameter(model, m.name)
-        E = Assignment(sympy.Symbol("E"), m * sympy.log(conc + sympy.exp(e0 / m)))
+        s = sympy.Symbol("slope")
+        model = add_individual_parameter(model, s.name)
+        E = Assignment(sympy.Symbol("E"), s * sympy.log(conc + sympy.exp(e0 / s)))
     else:
         raise ValueError(f'Unknown model "{expr}".')
 
     # Add dependent variable Y_2
     y_2 = sympy.Symbol('Y_2')
     y = Assignment(y_2, E.symbol)
     dvs = model.dependent_variables.replace(y_2, 2)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/results.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/tmdd.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/units.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.99.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.99.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.99.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.99.0/src/pharmpy/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/results.py` & `pharmpy-core-0.99.0/src/pharmpy/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 def mfr(model: Model) -> ModelfitResults:
     res = model.modelfit_results
     assert isinstance(res, ModelfitResults)
     return res
 
 
 def _df_read_json(obj) -> pd.DataFrame:
+    # Convert time strings to naive datetime and then to string
+    # Needed because of https://github.com/pandas-dev/pandas/issues/52595
+    for row in obj['data']:
+        if 'time' in row:
+            row['time'] = pd.to_datetime(row['time']).tz_localize(None)
+            row['time'] = row['time'].isoformat()
+
     return pd.read_json(json.dumps(obj), typ='frame', orient='table', precise_float=True)
 
 
 def _multi_index_read_json(obj) -> pd.MultiIndex:
     return pd.MultiIndex.from_frame(_df_read_json(obj))
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/allometry/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     summarize_errors,
     summarize_individuals,
     summarize_individuals_count_table,
     summarize_modelfit_results,
 )
 from pharmpy.tools.common import ToolResults, update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def create_workflow(
     model: Optional[Model] = None,
     results: Optional[ModelfitResults] = None,
     allometric_variable: Union[str, sympy.Expr] = 'WT',
     reference_value: Union[str, int, float, sympy.Expr] = 70,
@@ -68,16 +68,15 @@
     >>> from pharmpy.tools import run_allometry, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_allometry(model=model, results=results, allometric_variable='WGT') # doctest: +SKIP
 
     """
 
-    wf = Workflow()
-    wf.name = "allometry"
+    wb = WorkflowBuilder(name="allometry")
     if model is not None:
         start_task = Task('start_allometry', start, model)
     else:
         start_task = Task('start_allometry', start)
     _add_allometry = partial(
         _add_allometry_on_model,
         allometric_variable=allometric_variable,
@@ -85,20 +84,20 @@
         parameters=parameters,
         initials=initials,
         lower_bounds=lower_bounds,
         upper_bounds=upper_bounds,
         fixed=fixed,
     )
     task_add_allometry = Task('add allometry', _add_allometry)
-    wf.add_task(task_add_allometry, predecessors=start_task)
+    wb.add_task(task_add_allometry, predecessors=start_task)
     fit_wf = create_fit_workflow(n=1)
-    wf.insert_workflow(fit_wf, predecessors=task_add_allometry)
+    wb.insert_workflow(fit_wf, predecessors=task_add_allometry)
     results_task = Task('results', globals()['results'])
-    wf.add_task(results_task, predecessors=[start_task] + fit_wf.output_tasks)
-    return wf
+    wb.add_task(results_task, predecessors=[start_task] + fit_wf.output_tasks)
+    return Workflow(wb)
 
 
 def start(model):
     return model
 
 
 def _add_allometry_on_model(
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/amd/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Parameters,
     RandomVariables,
     Statements,
     output,
 )
 
 # FIXME: This shouldn't be used here
-from pharmpy.model.external.nonmem.advan import dosing
+from pharmpy.model.external.nonmem.advan import dosing, find_dose
 from pharmpy.modeling import (
     add_iiv,
     create_joint_distribution,
     set_first_order_absorption,
     set_initial_estimates,
     set_proportional_error_model,
 )
@@ -53,15 +53,16 @@
 
     CL = sympy.Symbol('CL')
     VC = sympy.Symbol('VC')
     cl_ass = Assignment(CL, pop_cl.symbol * sympy.exp(sympy.Symbol(eta_cl_name)))
     vc_ass = Assignment(VC, pop_vc.symbol * sympy.exp(sympy.Symbol(eta_vc_name)))
 
     cb = CompartmentalSystemBuilder()
-    central = Compartment.create('CENTRAL', dose=dosing(di, df, 1))
+    doses = dosing(di, df, 1)
+    central = Compartment.create('CENTRAL', dose=find_dose(doses, 1))
     cb.add_compartment(central)
     cb.add_flow(central, output, CL / VC)
 
     ipred = Assignment(sympy.Symbol('IPRED'), central.amount / VC)
     y_ass = Assignment(sympy.Symbol('Y'), ipred.symbol)
 
     stats = Statements([cl_ass, vc_ass, CompartmentalSystem(cb), ipred, y_ass])
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/amd/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from pharmpy.model import Model
 from pharmpy.modeling import resample_data
 from pharmpy.results import ModelfitResults
 from pharmpy.tools.bootstrap.results import calculate_results
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def create_workflow(model: Model, results: Optional[ModelfitResults] = None, resamples: int = 1):
     """Run bootstrap tool
 
     Parameters
     ----------
@@ -30,28 +30,27 @@
     >>> from pharmpy.modeling import load_example_model
     >>> from pharmpy.tools import run_bootstrap, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_bootstrap(model, res, resamples=500) # doctest: +SKIP
     """
 
-    wf = Workflow()
-    wf.name = 'bootstrap'
+    wb = WorkflowBuilder(name='bootstrap')
 
     for i in range(resamples):
         task_resample = Task('resample', resample_model, model, f'bs_{i + 1}')
-        wf.add_task(task_resample)
+        wb.add_task(task_resample)
 
     wf_fit = create_fit_workflow(n=resamples)
-    wf.insert_workflow(wf_fit)
+    wb.insert_workflow(wf_fit)
 
     task_result = Task('results', post_process_results, model)
-    wf.add_task(task_result, predecessors=wf.output_tasks)
+    wb.add_task(task_result, predecessors=wb.output_tasks)
 
-    return wf
+    return Workflow(wb)
 
 
 def resample_model(model, name):
     resample = resample_data(model, model.datainfo.id_column.name, resamples=1, name=name)
     model, _ = next(resample)
     return model
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/cdd/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/common.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     all_covariate_effects,
     parse_spec,
     spec,
 )
 from pharmpy.tools.mfl.parse import parse as mfl_parse
 from pharmpy.tools.modelfit import create_fit_workflow
 from pharmpy.tools.scm.results import candidate_summary_dataframe, ofv_summary_dataframe
-from pharmpy.workflows import Task, Workflow, call_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow
 
 from ..mfl.filter import covsearch_statement_types
 from .results import COVSearchResults
 
 NAME_WF = 'covsearch'
 
 DataFrame = Any  # NOTE should be pd.DataFrame but we want lazy loading
@@ -138,52 +138,51 @@
     >>> from pharmpy.tools import run_covsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> effects = 'COVARIATE([CL, V], [AGE, WT], EXP)'
     >>> res = run_covsearch(effects, model=model, results=results)      # doctest: +SKIP
     """
 
-    wf = Workflow()
-    wf.name = NAME_WF
+    wb = WorkflowBuilder(name=NAME_WF)
 
     init_task = init(model)
-    wf.add_task(init_task)
+    wb.add_task(init_task)
 
     forward_search_task = Task(
         'forward-search',
         task_greedy_forward_search,
         effects,
         p_forward,
         max_steps,
     )
 
-    wf.add_task(forward_search_task, predecessors=init_task)
-    search_output = wf.output_tasks
+    wb.add_task(forward_search_task, predecessors=init_task)
+    search_output = wb.output_tasks
 
     if algorithm == 'scm-forward-then-backward':
         backward_search_task = Task(
             'backward-search',
             task_greedy_backward_search,
             p_backward,
             max_steps,
         )
 
-        wf.add_task(backward_search_task, predecessors=search_output)
-        search_output = wf.output_tasks
+        wb.add_task(backward_search_task, predecessors=search_output)
+        search_output = wb.output_tasks
 
     results_task = Task(
         'results',
         task_results,
         p_forward,
         p_backward,
     )
 
-    wf.add_task(results_task, predecessors=search_output)
+    wb.add_task(results_task, predecessors=search_output)
 
-    return wf
+    return Workflow(wb)
 
 
 def _init_search_state(model: Model) -> SearchState:
     candidate = Candidate(model, ())
     return SearchState(model, candidate, [candidate])
 
 
@@ -313,33 +312,33 @@
         all_candidates_so_far,
     )
 
 
 def wf_effects_addition(
     model: Model, candidate: Candidate, candidate_effects: List[EffectLiteral], index_offset: int
 ):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     for i, effect in enumerate(candidate_effects, 1):
         task = Task(
             repr(effect),
             task_add_covariate_effect,
             model,
             candidate,
             effect,
             index_offset + i,
         )
-        wf.add_task(task)
+        wb.add_task(task)
 
     wf_fit = create_fit_workflow(n=len(candidate_effects))
-    wf.insert_workflow(wf_fit)
+    wb.insert_workflow(wf_fit)
 
     task_gather = Task('gather', lambda *models: models)
-    wf.add_task(task_gather, predecessors=wf.output_tasks)
-    return wf
+    wb.add_task(task_gather, predecessors=wb.output_tasks)
+    return Workflow(wb)
 
 
 def task_add_covariate_effect(
     model: Model, candidate: Candidate, effect: EffectLiteral, effect_index: int
 ):
     name = f'covsearch_run{effect_index}'
     description = _create_description(effect, candidate.steps)
@@ -378,33 +377,33 @@
         effects.append(effect_new_str)
     return ';'.join(effects)
 
 
 def wf_effects_removal(
     base_model: Model, parent: Candidate, candidate_effects: List[EffectLiteral], index_offset: int
 ):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     for i, effect in enumerate(candidate_effects, 1):
         task = Task(
             repr(effect),
             task_remove_covariate_effect,
             base_model,
             parent,
             effect,
             index_offset + i,
         )
-        wf.add_task(task)
+        wb.add_task(task)
 
     wf_fit = create_fit_workflow(n=len(candidate_effects))
-    wf.insert_workflow(wf_fit)
+    wb.insert_workflow(wf_fit)
 
     task_gather = Task('gather', lambda *models: models)
-    wf.add_task(task_gather, predecessors=wf.output_tasks)
-    return wf
+    wb.add_task(task_gather, predecessors=wb.output_tasks)
+    return Workflow(wb)
 
 
 def task_remove_covariate_effect(
     base_model: Model, candidate: Candidate, effect: EffectLiteral, effect_index: int
 ):
     model = candidate.model
     name = f'covsearch_run{effect_index}'
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/crossval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 import itertools
 
 from pharmpy.modeling import add_estimation_step, remove_estimation_step, set_ode_solver
 from pharmpy.tools.common import update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def exhaustive(methods, solvers, covs):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     task_start = Task('start', start)
-    wf.add_task(task_start)
+    wb.add_task(task_start)
 
     candidate_no = 1
     for method, solver, cov in itertools.product(methods, solvers, covs):
         wf_estmethod = _create_candidate_model_wf(candidate_no, method, solver, cov, update=False)
-        wf.insert_workflow(wf_estmethod, predecessors=task_start)
+        wb.insert_workflow(wf_estmethod, predecessors=task_start)
         candidate_no += 1
 
-    return wf, None
+    return Workflow(wb), None
 
 
 def exhaustive_with_update(methods, solvers, covs):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     task_base_model = Task('create_base_model', _create_base_model)
-    wf.add_task(task_base_model)
+    wb.add_task(task_base_model)
     wf_fit = create_fit_workflow(n=1)
-    wf.insert_workflow(wf_fit, predecessors=task_base_model)
-    task_base_model_fit = wf.output_tasks
+    wb.insert_workflow(wf_fit, predecessors=task_base_model)
+    task_base_model_fit = wb.output_tasks
 
     candidate_no = 1
     for method, solver, cov in itertools.product(methods, solvers, covs):
         # This is equivalent to the base model
         if not (method == 'FOCE' and solver is None):
             # Create model with original estimates
             wf_estmethod_original = _create_candidate_model_wf(
                 candidate_no, method, solver, cov, update=False
             )
-            wf.insert_workflow(wf_estmethod_original, predecessors=task_base_model_fit)
+            wb.insert_workflow(wf_estmethod_original, predecessors=task_base_model_fit)
             candidate_no += 1
 
         # Create model with updated estimates from FOCE
         wf_estmethod_update = _create_candidate_model_wf(
             candidate_no, method, solver, cov, update=True
         )
-        wf.insert_workflow(wf_estmethod_update, predecessors=task_base_model_fit)
+        wb.insert_workflow(wf_estmethod_update, predecessors=task_base_model_fit)
         candidate_no += 1
 
-    return wf, task_base_model_fit
+    return Workflow(wb), task_base_model_fit
 
 
 def exhaustive_only_eval(methods, solvers, covs):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     task_start = Task('start', start)
-    wf.add_task(task_start)
+    wb.add_task(task_start)
 
     candidate_no = 1
     for method, solver, cov in itertools.product(methods, solvers, covs):
         wf_estmethod = _create_candidate_model_wf(
             candidate_no, method, solver, cov, update=False, is_eval_candidate=True
         )
-        wf.insert_workflow(wf_estmethod, predecessors=task_start)
+        wb.insert_workflow(wf_estmethod, predecessors=task_start)
         candidate_no += 1
 
-    return wf, None
+    return Workflow(wb), None
 
 
 def start(model):
     return model
 
 
 def _create_candidate_model_wf(candidate_no, method, solver, cov, update, is_eval_candidate=False):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     model_name = f'estmethod_run{candidate_no}'
     task_copy = Task('copy_model', _copy_model, model_name)
-    wf.add_task(task_copy)
+    wb.add_task(task_copy)
 
     if update:
         task_update_inits = Task('update_inits', update_initial_estimates)
-        wf.add_task(task_update_inits, predecessors=task_copy)
+        wb.add_task(task_update_inits, predecessors=task_copy)
         task_prev = task_update_inits
     else:
         task_prev = task_copy
     task_create_candidate = Task(
         'create_candidate', _create_candidate_model, method, solver, cov, update, is_eval_candidate
     )
-    wf.add_task(task_create_candidate, predecessors=task_prev)
-    return wf
+    wb.add_task(task_create_candidate, predecessors=task_prev)
+    return Workflow(wb)
 
 
 def _copy_model(name, model):
     return model.replace(name=name)
 
 
 def _create_base_model(model):
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.99.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from dataclasses import dataclass
 from typing import Any, Optional
 
 from pharmpy.model import Model, Results
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def create_workflow(model: Model):
-    wf = Workflow()
-    wf.name = 'evaldesign'
+    wb = WorkflowBuilder(name="evaldesign")
 
     from pharmpy.tools.external.nonmem.run import evaluate_design
 
     task = Task('run', evaluate_design, model)
-    wf.add_task(task)
+    wb.add_task(task)
 
     task_result = Task('results', post_process_results)
-    wf.add_task(task_result, predecessors=[task])
-    return wf
+    wb.add_task(task_result, predecessors=[task])
+    return Workflow(wb)
 
 
 def post_process_results(res):
     return res
 
 
 @dataclass(frozen=True)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nlmixr/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nlmixr/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nlmixr/run.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nlmixr/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/config.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/results_file.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/nonmem/run.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/nonmem/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/rxode/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/rxode/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/external/rxode/run.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/external/rxode/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/frem/models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/frem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/frem/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.99.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,110 @@
 from typing import Dict, List, Set, Tuple
 
 import pharmpy.tools.modelfit as modelfit
 from pharmpy.internals.expr.subs import subs
 from pharmpy.internals.set.partitions import partitions
 from pharmpy.internals.set.subsets import non_empty_subsets
 from pharmpy.model import Model, RandomVariables
-from pharmpy.modeling import create_joint_distribution, remove_iiv, split_joint_distribution
+from pharmpy.modeling import (
+    create_joint_distribution,
+    get_omegas,
+    remove_iiv,
+    split_joint_distribution,
+)
 from pharmpy.modeling.expressions import get_rv_parameters
 from pharmpy.results import mfr
 from pharmpy.tools.common import update_initial_estimates
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def brute_force_no_of_etas(base_model, index_offset=0, keep=None):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     base_model = base_model.replace(description=create_description(base_model))
 
     iivs = base_model.random_variables.iiv
     iiv_names = iivs.names
     if keep:
-        iiv_names = set(iiv_names) - _get_eta_from_parameter(base_model, keep)
+        iiv_names = _remove_sublist(iiv_names, _get_eta_from_parameter(base_model, keep))
+
+    # Remove fixed etas
+    fixed_etas = _get_fixed_etas(base_model)
+    iiv_names = _remove_sublist(iiv_names, fixed_etas)
 
     for i, to_remove in enumerate(non_empty_subsets(iiv_names), 1):
         model_name = f'iivsearch_run{i + index_offset}'
         task_copy = Task('copy', copy, model_name)
-        wf.add_task(task_copy)
+        wb.add_task(task_copy)
 
         task_update_inits = Task('update_inits', update_initial_estimates)
-        wf.add_task(task_update_inits, predecessors=task_copy)
+        wb.add_task(task_update_inits, predecessors=task_copy)
 
         task_remove_eta = Task('remove_eta', remove_eta, to_remove)
-        wf.add_task(task_remove_eta, predecessors=task_update_inits)
+        wb.add_task(task_remove_eta, predecessors=task_update_inits)
 
         task_update_description = Task('update_description', update_description)
-        wf.add_task(task_update_description, predecessors=task_remove_eta)
+        wb.add_task(task_update_description, predecessors=task_remove_eta)
 
-    wf_fit = modelfit.create_fit_workflow(n=len(wf.output_tasks))
-    wf.insert_workflow(wf_fit)
-    return wf
+    wf_fit = modelfit.create_fit_workflow(n=len(wb.output_tasks))
+    wb.insert_workflow(wf_fit)
+    return Workflow(wb)
 
 
 def brute_force_block_structure(base_model, index_offset=0):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     base_model = base_model.replace(description=create_description(base_model))
 
     iivs = base_model.random_variables.iiv
     model_no = 1 + index_offset
 
-    for block_structure in _rv_block_structures(iivs):
-        if _is_rv_block_structure(iivs, block_structure):
+    fixed_etas = _get_fixed_etas(base_model)
+    iiv_names = _remove_sublist(iivs.names, fixed_etas)
+
+    for block_structure in _rv_block_structures(iiv_names):
+        if _is_rv_block_structure(iivs, block_structure, fixed_etas):
             continue
 
         model_name = f'iivsearch_run{model_no}'
         task_copy = Task('copy', copy, model_name)
-        wf.add_task(task_copy)
+        wb.add_task(task_copy)
 
         task_update_inits = Task('update_inits', update_initial_estimates)
-        wf.add_task(task_update_inits, predecessors=task_copy)
+        wb.add_task(task_update_inits, predecessors=task_copy)
 
         task_joint_dist = Task('create_eta_blocks', create_eta_blocks, block_structure)
-        wf.add_task(task_joint_dist, predecessors=task_update_inits)
+        wb.add_task(task_joint_dist, predecessors=task_update_inits)
 
         task_update_description = Task('update_description', update_description)
-        wf.add_task(task_update_description, predecessors=task_joint_dist)
+        wb.add_task(task_update_description, predecessors=task_joint_dist)
 
         model_no += 1
 
-    wf_fit = modelfit.create_fit_workflow(n=len(wf.output_tasks))
-    wf.insert_workflow(wf_fit)
-    return wf
+    wf_fit = modelfit.create_fit_workflow(n=len(wb.output_tasks))
+    wb.insert_workflow(wf_fit)
+    return Workflow(wb)
 
 
 def _rv_block_structures(etas: RandomVariables):
     # NOTE All possible partitions of etas into block structures
-    return partitions(etas.names)
+    return partitions(etas)
 
 
-def _is_rv_block_structure(etas: RandomVariables, partition: Tuple[Tuple[str, ...], ...]):
+def _is_rv_block_structure(
+    etas: RandomVariables, partition: Tuple[Tuple[str, ...], ...], fixed_etas
+):
     parts = set(partition)
-    return all(map(lambda dist: dist.names in parts, etas))
+    # Remove fixed etas from etas
+    list_of_tuples = list(
+        filter(
+            None, list(map(lambda dist: tuple(_remove_sublist(list(dist.names), fixed_etas)), etas))
+        )
+    )
+    return all(map(lambda dist: dist in parts, list_of_tuples))
 
 
 def _create_param_dict(model: Model, dists: RandomVariables) -> Dict[str, str]:
     param_subs = {
         parameter.symbol: parameter.init for parameter in model.parameters if parameter.fix
     }
     param_dict = {}
@@ -159,7 +179,23 @@
     iiv_set = set()
     iiv_names = model.random_variables.names
     for iiv_name in iiv_names:
         param = get_rv_parameters(model, iiv_name)
         if set(param).issubset(parameters) and len(param) > 0:
             iiv_set.add(iiv_name)
     return iiv_set
+
+
+def _get_fixed_etas(model: Model) -> List[str]:
+    fixed_omegas = get_omegas(model).fixed.names
+    iivs = model.random_variables.iiv
+    if len(fixed_omegas) > 0:
+        fixed_etas = [
+            iiv.names for iiv in iivs if str(list(iiv.variance.free_symbols)[0]) in fixed_omegas
+        ]
+        return [item for tup in fixed_etas for item in tup]
+    else:
+        return []
+
+
+def _remove_sublist(list_a, list_b):
+    return [x for x in list_a if x not in list_b]
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.model import Model
 from pharmpy.modeling import add_pk_iiv, calculate_bic, create_joint_distribution, has_random_effect
 from pharmpy.modeling.results import RANK_TYPES
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import summarize_modelfit_results
 from pharmpy.tools.common import ToolResults, create_results, update_initial_estimates
+from pharmpy.tools.iivsearch.algorithms import _get_fixed_etas
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow, call_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow
 
 IIV_STRATEGIES = frozenset(('no_add', 'add_diagonal', 'fullblock'))
 IIV_ALGORITHMS = frozenset(('brute_force',) + tuple(dir(algorithms)))
 
 
 @dataclass
 class State:
@@ -68,56 +69,54 @@
     >>> from pharmpy.modeling import *
     >>> from pharmpy.tools import run_iivsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_iivsearch('brute_force', results=results, model=model)   # doctest: +SKIP
     """
 
-    wf = Workflow()
-    wf.name = 'iivsearch'
+    wb = WorkflowBuilder(name='iivsearch')
     start_task = Task('start_iiv', start, model, algorithm, iiv_strategy, rank_type, cutoff, keep)
-    wf.add_task(start_task)
+    wb.add_task(start_task)
     task_results = Task('results', _results)
-    wf.add_task(task_results, predecessors=[start_task])
-    return wf
+    wb.add_task(task_results, predecessors=[start_task])
+    return Workflow(wb)
 
 
 def create_algorithm_workflow(
     input_model, base_model, state, iiv_strategy, rank_type, cutoff, keep
 ):
-    wf: Workflow[IIVSearchResults] = Workflow()
-
+    wb = WorkflowBuilder()
     start_task = Task(f'start_{state.algorithm}', _start_algorithm, base_model)
-    wf.add_task(start_task)
+    wb.add_task(start_task)
 
     if iiv_strategy != 'no_add':
         wf_fit = create_fit_workflow(n=1)
-        wf.insert_workflow(wf_fit)
+        wb.insert_workflow(wf_fit)
         base_model_task = wf_fit.output_tasks[0]
     else:
         base_model_task = start_task
 
     index_offset = len(
         [model_name for model_name in state.model_names_so_far if 'base' not in model_name]
     )
     algorithm_func = getattr(algorithms, state.algorithm)
     if state.algorithm == "brute_force_no_of_etas":
         wf_method = algorithm_func(base_model, index_offset, keep)
     else:
         wf_method = algorithm_func(base_model, index_offset)
-    wf.insert_workflow(wf_method)
+    wb.insert_workflow(wf_method)
 
     task_result = Task(
         'results', post_process, state, rank_type, cutoff, input_model, base_model.name
     )
 
-    post_process_tasks = [base_model_task] + wf.output_tasks
-    wf.add_task(task_result, predecessors=post_process_tasks)
+    post_process_tasks = [base_model_task] + wb.output_tasks
+    wb.add_task(task_result, predecessors=post_process_tasks)
 
-    return wf
+    return Workflow(wb)
 
 
 def start(context, input_model, algorithm, iiv_strategy, rank_type, cutoff, keep):
     if iiv_strategy != 'no_add':
         model_iiv = input_model.replace(name='base_model')
         model_iiv = update_initial_estimates(model_iiv)
         base_model = _add_iiv(iiv_strategy, model_iiv)
@@ -163,15 +162,18 @@
         )
 
         base_model = final_model
         iiv_strategy = 'no_add'
         last_res = res
 
         assert base_model is not None
-        if len(base_model.random_variables.iiv.names) <= 1:
+        if (
+            len(set(base_model.random_variables.iiv.names).difference(_get_fixed_etas(base_model)))
+            <= 1
+        ):
             break
 
     assert last_res is not None
     assert final_model is not None
 
     res_modelfit_input = input_model.modelfit_results
     res_modelfit_final = final_model.modelfit_results
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 import pharmpy.tools.iivsearch.algorithms
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.internals.set.subsets import non_empty_proper_subsets, non_empty_subsets
-from pharmpy.model import Assignment, Model
-from pharmpy.modeling import add_iov, get_pk_parameters, remove_iiv, remove_iov
+from pharmpy.model import Assignment, Model, RandomVariables
+from pharmpy.modeling import add_iov, get_omegas, get_pk_parameters, remove_iiv, remove_iov
 from pharmpy.modeling.parameter_variability import ADD_IOV_DISTRIBUTION
 from pharmpy.modeling.results import RANK_TYPES
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import rank_models, summarize_modelfit_results
 from pharmpy.tools.common import (
     ToolResults,
     create_results,
     summarize_tool,
     update_initial_estimates,
 )
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow, call_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow
 
 NAME_WF = 'iovsearch'
 
 T = TypeVar('T')
 
 
 def create_workflow(
@@ -68,46 +68,45 @@
     >>> from pharmpy.modeling import load_example_model
     >>> from pharmpy.tools import run_iovsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_iovsearch('OCC', results=results, model=model)      # doctest: +SKIP
     """
 
-    wf = Workflow()
-    wf.name = NAME_WF
+    wb = WorkflowBuilder(name=NAME_WF)
 
     init_task = init(model)
-    wf.add_task(init_task)
+    wb.add_task(init_task)
 
     bic_type = 'random'
     search_task = Task(
         'search',
         task_brute_force_search,
         column,
         list_of_parameters,
         rank_type,
         cutoff,
         bic_type,
         distribution,
     )
 
-    wf.add_task(search_task, predecessors=init_task)
-    search_output = wf.output_tasks
+    wb.add_task(search_task, predecessors=init_task)
+    search_output = wb.output_tasks
 
     results_task = Task(
         'results',
         task_results,
         rank_type,
         cutoff,
         bic_type,
     )
 
-    wf.add_task(results_task, predecessors=search_output)
+    wb.add_task(results_task, predecessors=search_output)
 
-    return wf
+    return Workflow(wb)
 
 
 def init(model):
     return (
         Task('init', lambda model: model)
         if model is None
         else Task('init', lambda model: model, model)
@@ -122,15 +121,15 @@
     cutoff: Union[None, float],
     bic_type: Union[None, str],
     distribution: str,
     model: Model,
 ):
     # NOTE Default is to try all IIV ETAs.
     if list_of_parameters is None:
-        iiv = model.random_variables.iiv
+        iiv = _get_nonfixed_iivs(model)
         iiv_before_odes = iiv.free_symbols.intersection(model.statements.before_odes.free_symbols)
         list_of_parameters = [iiv.name for iiv in iiv_before_odes]
 
     current_step = 0
     step_mapping = {current_step: [model.name]}
 
     # NOTE Check that model has at least one IIV.
@@ -218,35 +217,35 @@
 
 def wf_etas_removal(
     remove: Callable[[Model, List[str]], None],
     model: Model,
     etas_subsets: Iterable[Tuple[str]],
     i: int,
 ):
-    wf = Workflow()
+    wb = WorkflowBuilder()
     j = i
     for subset_of_iiv_parameters in etas_subsets:
         task = Task(
             repr(subset_of_iiv_parameters),
             task_remove_etas_subset,
             remove,
             model,
             list(subset_of_iiv_parameters),
             j,
         )
-        wf.add_task(task)
+        wb.add_task(task)
         j += 1
 
     n = j - i
     wf_fit = create_fit_workflow(n=n)
-    wf.insert_workflow(wf_fit)
+    wb.insert_workflow(wf_fit)
 
     task_gather = Task('gather', lambda *models: models)
-    wf.add_task(task_gather, predecessors=wf.output_tasks)
-    return wf
+    wb.add_task(task_gather, predecessors=wb.output_tasks)
+    return Workflow(wb)
 
 
 def best_model(
     base: Model,
     models: List[Model],
     rank_type: str,
     cutoff: Union[None, float],
@@ -350,17 +349,26 @@
             else:
                 if all(s in iovs for s in expression_symbols):
                     yield statement.symbol
 
 
 def _get_iiv_etas_with_corresponding_iov(model: Model):
     iovs = set(_get_iov_piecewise_assignment_symbols(model))
-    iiv = model.random_variables.iiv
+    iiv = _get_nonfixed_iivs(model)
 
     for statement in model.statements:
         if isinstance(statement, Assignment) and isinstance(statement.expression, sympy.Add):
             for symbol in statement.expression.free_symbols:
                 if symbol in iovs:
                     rest = statement.expression - symbol
                     if isinstance(rest, sympy.Symbol) and rest in iiv:
                         yield rest
                     break
+
+
+def _get_nonfixed_iivs(model):
+    fixed_omegas = get_omegas(model).fixed.names
+    iivs = model.random_variables.iiv
+    nonfixed_iivs = [
+        iiv for iiv in iivs if str(list(iiv.variance.free_symbols)[0]) not in fixed_omegas
+    ]
+    return RandomVariables.create(nonfixed_iivs)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/linearize/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/linearize/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/linearize/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pharmpy.model
 from pharmpy.deps import sympy
 from pharmpy.model import Assignment, EstimationStep, EstimationSteps, Statements
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def create_workflow(model=None):
-    wf = Workflow()
-    wf.name = "linearize"
+    wb = WorkflowBuilder(name="linearize")
 
     if model is not None:
         start_task = Task('start_linearize', start_linearize, model)
     else:
         start_task = Task('start_linearize', start_linearize)
 
-    wf.add_task(start_task)
-    return wf
+    wb.add_task(start_task)
+    return Workflow(wb)
 
 
 def start_linearize(model):
     return model
 
 
 def create_linearized_model(model):
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterable, Literal, Optional, Tuple, Union
 
 from pharmpy.model import Model
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 SupportedPlugin = Literal['nonmem', 'nlmixr']
 
 
 def create_workflow(
     model_or_models: Optional[Union[Model, Iterable[Model]]] = None,
     n: Optional[int] = None,
@@ -32,44 +32,46 @@
     >>> from pharmpy.modeling import load_example_model
     >>> model = load_example_model("pheno")
     >>> from pharmpy.tools import run_modelfit     # doctest: +SKIP
     >>> run_modelfit(model)   # doctest: +SKIP
     """
 
     wf = create_fit_workflow(model_or_models, n, tool)
-    wf.name = "modelfit"
+    wf = wf.replace(name="modelfit")
     if isinstance(model_or_models, Model) or (model_or_models is None and n is None):
         post_process_results = post_process_results_one
     else:
         post_process_results = post_process_results_many
     task_result: Task[Union[Model, Tuple[Model, ...]]] = Task('results', post_process_results)
-    wf.add_task(task_result, predecessors=wf.output_tasks)
+    wb = WorkflowBuilder(wf)
+    wb.add_task(task_result, predecessors=wf.output_tasks)
+    wf = Workflow(wb)
     return wf
 
 
 def create_fit_workflow(models=None, n=None, tool=None):
     execute_model = retrieve_from_database_or_execute_model_with_tool(tool)
 
-    wf = Workflow()
+    wb = WorkflowBuilder()
     if models is None:
         if n is None:
             task = Task('run', execute_model)
-            wf.add_task(task)
+            wb.add_task(task)
         else:
             for i in range(n):
                 task = Task(f'run{i}', execute_model)
-                wf.add_task(task)
+                wb.add_task(task)
     elif isinstance(models, Model):
         task = Task('run', execute_model, models)
-        wf.add_task(task)
+        wb.add_task(task)
     else:
         for i, model in enumerate(models):
             task = Task(f'run{i}', execute_model, model)
-            wf.add_task(task)
-    return wf
+            wb.add_task(task)
+    return Workflow(wb)
 
 
 def post_process_results_one(context, *models: Model):
     return models[0]
 
 
 def post_process_results_many(context, *models: Model):
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List
 
 from pharmpy.model import Model
 from pharmpy.modeling import add_iiv, add_pk_iiv, create_joint_distribution, set_upper_bounds
 from pharmpy.tools.common import update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 from ..mfl.helpers import (
     all_combinations,
     funcs,
     get_funcs_same_type,
     key_to_str,
     modelsearch_features,
@@ -20,119 +20,119 @@
 
 def model_search_funcs(mfl_statements: List[Statement]):
     return funcs(Model(), mfl_statements, modelsearch_features)
 
 
 def exhaustive(mfl_statements: List[Statement], iiv_strategy: str):
     # TODO: rewrite using _create_model_workflow
-    wf_search = Workflow()
+    wb_search = WorkflowBuilder()
 
     model_tasks = []
 
     funcs = model_search_funcs(mfl_statements)
     combinations = list(all_combinations(funcs))
 
     for i, combo in enumerate(combinations, 1):
         model_name = f'modelsearch_run{i}'
 
         task_copy = Task('copy', _copy, model_name, combo)
-        wf_search.add_task(task_copy)
+        wb_search.add_task(task_copy)
 
         task_previous = task_copy
         for feat in combo:
             func = funcs[feat]
             task_function = Task(key_to_str(feat), func)
-            wf_search.add_task(task_function, predecessors=task_previous)
+            wb_search.add_task(task_function, predecessors=task_previous)
             if iiv_strategy != 'no_add':
                 task_add_iiv = Task('add_iivs', _add_iiv_to_func, iiv_strategy)
-                wf_search.add_task(task_add_iiv, predecessors=task_function)
+                wb_search.add_task(task_add_iiv, predecessors=task_function)
                 task_previous = task_add_iiv
             else:
                 task_previous = task_function
 
         wf_fit = create_fit_workflow(n=1)
-        wf_search.insert_workflow(wf_fit, predecessors=task_previous)
+        wb_search.insert_workflow(wf_fit, predecessors=task_previous)
 
         model_tasks += wf_fit.output_tasks
 
-    return wf_search, model_tasks
+    return Workflow(wb_search), model_tasks
 
 
 def exhaustive_stepwise(mfl_statements: List[Statement], iiv_strategy: str):
     mfl_funcs = model_search_funcs(mfl_statements)
 
-    wf_search = Workflow()
+    wb_search = WorkflowBuilder()
     model_tasks = []
 
     while True:
         no_of_trans = 0
-        actions = _get_possible_actions(wf_search, mfl_statements)
+        actions = _get_possible_actions(wb_search, mfl_statements)
         for task_parent, feat_new in actions.items():
             for feat in feat_new:
                 model_no = len(model_tasks) + 1
                 model_name = f'modelsearch_run{model_no}'
 
                 wf_create_model, _ = _create_model_workflow(
                     model_name, feat, mfl_funcs[feat], iiv_strategy
                 )
 
                 if task_parent:
-                    wf_search.insert_workflow(wf_create_model, predecessors=[task_parent])
+                    wb_search.insert_workflow(wf_create_model, predecessors=[task_parent])
                 else:
-                    wf_search += wf_create_model
+                    wb_search += WorkflowBuilder(wf_create_model)
 
                 model_tasks += wf_create_model.output_tasks
 
                 no_of_trans += 1
         if no_of_trans == 0:
             break
 
-    return wf_search, model_tasks
+    return Workflow(wb_search), model_tasks
 
 
 def reduced_stepwise(mfl_statements: List[Statement], iiv_strategy: str):
     mfl_funcs = model_search_funcs(mfl_statements)
 
-    wf_search = Workflow()
+    wb_search = WorkflowBuilder()
     model_tasks = []
 
     while True:
         no_of_trans = 0
-        actions = _get_possible_actions(wf_search, mfl_statements)
-        groups = _find_same_model_groups(wf_search, mfl_funcs)
+        actions = _get_possible_actions(wb_search, mfl_statements)
+        groups = _find_same_model_groups(wb_search, mfl_funcs)
         if len(groups) > 1:
             for group in groups:
                 # Only add collector nodes to tasks with possible actions (i.e. not to leaf nodes)
                 if all(len(actions[task]) > 0 for task in group):
                     task_best_model = Task('choose_best_model', _get_best_model)
-                    wf_search.add_task(task_best_model, predecessors=group)
+                    wb_search.add_task(task_best_model, predecessors=group)
             # Overwrite actions with new collector nodes
-            actions = _get_possible_actions(wf_search, mfl_statements)
+            actions = _get_possible_actions(wb_search, mfl_statements)
 
         for task_parent, feat_new in actions.items():
             for feat in feat_new:
                 model_no = len(model_tasks) + 1
                 model_name = f'modelsearch_run{model_no}'
 
                 wf_create_model, _ = _create_model_workflow(
                     model_name, feat, mfl_funcs[feat], iiv_strategy
                 )
 
                 if task_parent:
-                    wf_search.insert_workflow(wf_create_model, predecessors=[task_parent])
+                    wb_search.insert_workflow(wf_create_model, predecessors=[task_parent])
                 else:
-                    wf_search += wf_create_model
+                    wb_search += wf_create_model
 
                 model_tasks += wf_create_model.output_tasks
 
                 no_of_trans += 1
         if no_of_trans == 0:
             break
 
-    return wf_search, model_tasks
+    return Workflow(wb_search), model_tasks
 
 
 def _find_same_model_groups(wf, mfl_funcs):
     tasks = wf.output_tasks
     tasks_removed = []
     all_groups = []
     for task_start in tasks:
@@ -192,36 +192,36 @@
     features_previous = [
         tasks_dict[task.name] for task in tasks_upstream if task.name in tasks_dict
     ]
     return features_previous
 
 
 def _create_model_workflow(model_name, feat, func, iiv_strategy):
-    wf_stepwise_step = Workflow()
+    wb_stepwise_step = WorkflowBuilder()
 
     task_copy = Task('copy', _copy, model_name, (feat,))
-    wf_stepwise_step.add_task(task_copy)
+    wb_stepwise_step.add_task(task_copy)
 
     task_update_inits = Task('update_inits', update_initial_estimates)
-    wf_stepwise_step.add_task(task_update_inits, predecessors=task_copy)
+    wb_stepwise_step.add_task(task_update_inits, predecessors=task_copy)
 
     task_function = Task(key_to_str(feat), _apply_transformation, feat, func)
-    wf_stepwise_step.add_task(task_function, predecessors=task_update_inits)
+    wb_stepwise_step.add_task(task_function, predecessors=task_update_inits)
 
     if iiv_strategy != 'no_add':
         task_add_iiv = Task('add_iivs', _add_iiv_to_func, iiv_strategy)
-        wf_stepwise_step.add_task(task_add_iiv, predecessors=task_function)
+        wb_stepwise_step.add_task(task_add_iiv, predecessors=task_function)
         task_to_fit = task_add_iiv
     else:
         task_to_fit = task_function
 
     wf_fit = create_fit_workflow(n=1)
-    wf_stepwise_step.insert_workflow(wf_fit, predecessors=task_to_fit)
+    wb_stepwise_step.insert_workflow(wf_fit, predecessors=task_to_fit)
 
-    return wf_stepwise_step, task_function
+    return Workflow(wb_stepwise_step), task_function
 
 
 def _apply_transformation(feat, func, model):
     old_params = set(model.parameters)
     model = func(model)
     if feat[0] == 'PERIPHERALS':
         new_params = set(model.parameters)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.model import Model
 from pharmpy.modeling.results import RANK_TYPES
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import summarize_modelfit_results
 from pharmpy.tools.common import ToolResults, create_results
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 from ..mfl.filter import modelsearch_statement_types
 from ..mfl.parse import parse as mfl_parse
 
 
 def create_workflow(
     search_space: str,
@@ -57,40 +57,39 @@
     >>> from pharmpy.tools import run_modelsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_modelsearch('ABSORPTION(ZO);PERIPHERALS(1)', 'exhaustive', results=results, model=model) # doctest: +SKIP
 
     """
 
-    wf = Workflow()
-    wf.name = 'modelsearch'
+    wb = WorkflowBuilder(name='modelsearch')
 
     if model:
         start_task = Task('start_modelsearch', start, model)
     else:
         start_task = Task('start_modelsearch', start)
 
-    wf.add_task(start_task)
+    wb.add_task(start_task)
 
     algorithm_func = getattr(algorithms, algorithm)
 
     mfl_statements = mfl_parse(search_space)
     wf_search, candidate_model_tasks = algorithm_func(mfl_statements, iiv_strategy)
-    wf.insert_workflow(wf_search, predecessors=wf.output_tasks)
+    wb.insert_workflow(wf_search, predecessors=wb.output_tasks)
 
     task_result = Task(
         'results',
         post_process,
         rank_type,
         cutoff,
     )
 
-    wf.add_task(task_result, predecessors=[start_task] + candidate_model_tasks)
+    wb.add_task(task_result, predecessors=[start_task] + candidate_model_tasks)
 
-    return wf
+    return Workflow(wb)
 
 
 def start(model):
     return model
 
 
 def post_process(rank_type, cutoff, *models):
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/qa/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/reporting.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/run.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -769,32 +769,24 @@
     ...             rank_type='lrt') # doctest: +SKIP
     """
     models_all = [base_model] + models
 
     rank_values, delta_values = {}, {}
     models_to_rank = []
 
-    ref_value = _get_rankval(base_model, rank_type, bic_type)
+    ref_value = _get_rankval(base_model, errors_allowed, rank_type, bic_type)
     model_dict = {model.name: model for model in models_all}
 
     # Filter on strictness
     for model in models_all:
         # Exclude OFV etc. if model was not successful
-        if not model.modelfit_results or np.isnan(model.modelfit_results.ofv):
+        rank_value = _get_rankval(model, errors_allowed, rank_type, bic_type)
+        if np.isnan(rank_value):
             continue
-        if not model.modelfit_results.minimization_successful:
-            if errors_allowed:
-                if model.modelfit_results.termination_cause not in errors_allowed:
-                    continue
-                if np.isnan(model.modelfit_results.significant_digits):
-                    continue
-            else:
-                continue
 
-        rank_value = _get_rankval(model, rank_type, bic_type)
         if rank_type == 'lrt':
             parent = model_dict[model.parent_model]
             if cutoff is None:
                 co = 0.05 if lrt_df(parent, model) >= 0 else 0.01
             elif isinstance(cutoff, tuple):
                 co = cutoff[0] if lrt_df(parent, model) >= 0 else cutoff[1]
             else:
@@ -857,16 +849,30 @@
 
     if np.isnan(ref_value):
         return df.sort_values(by=[f'{rank_type_name}'])
     else:
         return df.sort_values(by=[f'd{rank_type_name}'], ascending=False)
 
 
-def _get_rankval(model, rank_type, bic_type):
-    if not model.modelfit_results:
+def _is_valid_res(res, errors_allowed):
+    if not res or np.isnan(res.ofv):
+        return False
+    if not res.minimization_successful:
+        if errors_allowed:
+            if res.termination_cause not in errors_allowed:
+                return False
+            if np.isnan(res.significant_digits):
+                return False
+        else:
+            return False
+    return True
+
+
+def _get_rankval(model, errors_allowed, rank_type, bic_type):
+    if not _is_valid_res(model.modelfit_results, errors_allowed):
         return np.nan
     if rank_type in ['ofv', 'lrt']:
         return model.modelfit_results.ofv
     elif rank_type == 'aic':
         return calculate_aic(model, model.modelfit_results.ofv)
     elif rank_type == 'bic':
         return calculate_bic(model, model.modelfit_results.ofv, bic_type)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,29 @@
     summarize_errors,
     summarize_individuals,
     summarize_individuals_count_table,
     summarize_modelfit_results,
 )
 from pharmpy.tools.common import summarize_tool, update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow, call_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow
 
 from .results import RUVSearchResults, calculate_results
 
 SKIP = frozenset(('IIV_on_RUV', 'power', 'combined', 'time_varying'))
 
 
 def create_workflow(
     model: Optional[Model] = None,
     results: Optional[ModelfitResults] = None,
     groups: int = 4,
     p_value: float = 0.05,
     skip: Optional[List[str]] = None,
     max_iter: Optional[int] = 3,
+    dv: Optional[int] = None,
 ):
     """Run the ruvsearch tool. For more details, see :ref:`ruvsearch`.
 
     Parameters
     ----------
     model : Model
         Pharmpy model
@@ -65,14 +66,16 @@
         The number of bins to use for the time varying models
     p_value : float
         The p-value to use for the likelihood ratio test
     skip : list
         A list of models to not attempt.
     max_iter :  int
         Number of iterations to run (1, 2, or 3). For models with BLQ only one iteration is supported.
+    dv : int
+        Which DV to assess the error model for.
 
     Returns
     -------
     RUVSearchResults
         Ruvsearch tool result object
 
     Examples
@@ -81,87 +84,91 @@
     >>> from pharmpy.tools import run_ruvsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_ruvsearch(model=model, results=results)      # doctest: +SKIP
 
     """
 
-    wf = Workflow()
-    wf.name = "ruvsearch"
-    start_task = Task('start_ruvsearch', start, model, groups, p_value, skip, max_iter)
-    wf.add_task(start_task)
+    wb = WorkflowBuilder(name="ruvsearch")
+    start_task = Task('start_ruvsearch', start, model, groups, p_value, skip, max_iter, dv)
+    wb.add_task(start_task)
     task_results = Task('results', _results)
-    wf.add_task(task_results, predecessors=[start_task])
-    return wf
+    wb.add_task(task_results, predecessors=[start_task])
+    return Workflow(wb)
 
 
-def create_iteration_workflow(model, groups, cutoff, skip, current_iteration):
-    wf = Workflow()
+def create_iteration_workflow(model, groups, cutoff, skip, current_iteration, dv):
+    wb = WorkflowBuilder()
 
     start_task = Task('start_iteration', _start_iteration, model)
-    wf.add_task(start_task)
+    wb.add_task(start_task)
 
     task_base_model = Task(
-        'create_base_model', partial(_create_base_model, current_iteration=current_iteration)
+        'create_base_model', partial(_create_base_model, current_iteration=current_iteration, dv=dv)
     )
-    wf.add_task(task_base_model, predecessors=start_task)
+    wb.add_task(task_base_model, predecessors=start_task)
 
     tasks = []
     if 'IIV_on_RUV' not in skip:
         task_iiv = Task(
             'create_iiv_on_ruv_model',
-            partial(_create_iiv_on_ruv_model, current_iteration=current_iteration),
+            partial(_create_iiv_on_ruv_model, current_iteration=current_iteration, dv=None),
         )
         tasks.append(task_iiv)
-        wf.add_task(task_iiv, predecessors=task_base_model)
+        wb.add_task(task_iiv, predecessors=task_base_model)
 
     if 'power' not in skip and 'combined' not in skip:
         task_power = Task(
-            'create_power_model', partial(_create_power_model, current_iteration=current_iteration)
+            'create_power_model',
+            partial(_create_power_model, current_iteration=current_iteration, dv=None),
         )
-        wf.add_task(task_power, predecessors=task_base_model)
+        wb.add_task(task_power, predecessors=task_base_model)
         tasks.append(task_power)
         task_combined = Task(
             'create_combined_error_model',
             partial(_create_combined_model, current_iteration=current_iteration),
         )
-        wf.add_task(task_combined, predecessors=task_base_model)
+        wb.add_task(task_combined, predecessors=task_base_model)
         tasks.append(task_combined)
 
     if 'time_varying' not in skip:
         for i in range(1, groups):
             tvar = partial(
-                _create_time_varying_model, groups=groups, i=i, current_iteration=current_iteration
+                _create_time_varying_model,
+                groups=groups,
+                i=i,
+                current_iteration=current_iteration,
+                dv=None,
             )
             task = Task(f"create_time_varying_model{i}", tvar)
             tasks.append(task)
-            wf.add_task(task, predecessors=task_base_model)
+            wb.add_task(task, predecessors=task_base_model)
 
     fit_wf = create_fit_workflow(n=1 + len(tasks))
-    wf.insert_workflow(fit_wf, predecessors=[task_base_model] + tasks)
-    post_pro = partial(post_process, cutoff=cutoff, current_iteration=current_iteration)
+    wb.insert_workflow(fit_wf, predecessors=[task_base_model] + tasks)
+    post_pro = partial(post_process, cutoff=cutoff, current_iteration=current_iteration, dv=dv)
     task_post_process = Task('post_process', post_pro)
-    wf.add_task(task_post_process, predecessors=[start_task] + fit_wf.output_tasks)
+    wb.add_task(task_post_process, predecessors=[start_task] + fit_wf.output_tasks)
 
-    return wf
+    return Workflow(wb)
 
 
-def start(context, model, groups, p_value, skip, max_iter):
+def start(context, model, groups, p_value, skip, max_iter, dv):
     cutoff = float(stats.chi2.isf(q=p_value, df=1))
     if skip is None:
         skip = []
 
     sum_models = []
     selected_models = [model]
     cwres_models = []
     tool_database = None
     last_iteration = 0
     for current_iteration in range(1, max_iter + 1):
         last_iteration = current_iteration
-        wf = create_iteration_workflow(model, groups, cutoff, skip, current_iteration)
+        wf = create_iteration_workflow(model, groups, cutoff, skip, current_iteration, dv=dv)
         res, best_model, selected_model_name = call_workflow(
             wf, f'results{current_iteration}', context
         )
         if current_iteration == 1:
             sum_models.append(summarize_modelfit_results(model.modelfit_results))
         sum_models.append(summarize_modelfit_results(best_model.modelfit_results))
 
@@ -221,18 +228,18 @@
     return model
 
 
 def _results(res):
     return res
 
 
-def post_process(context, start_model, *models, cutoff, current_iteration):
+def post_process(context, start_model, *models, cutoff, current_iteration, dv):
     res = calculate_results(models)
     best_model_unfitted, selected_model_name = _create_best_model(
-        start_model, res, current_iteration, cutoff=cutoff
+        start_model, res, current_iteration, cutoff=cutoff, dv=dv
     )
     if best_model_unfitted is not None:
         fit_wf = create_fit_workflow(models=[best_model_unfitted])
         best_model = call_workflow(fit_wf, f'fit{current_iteration}', context)
         if best_model.modelfit_results is not None:
             best_model_check = [
                 best_model.modelfit_results.ofv,
@@ -243,15 +250,15 @@
                 delta_ofv = start_model.modelfit_results.ofv - best_model.modelfit_results.ofv
                 if delta_ofv > cutoff:
                     return (res, best_model, selected_model_name)
 
     return (res, start_model, f"base_{current_iteration}")
 
 
-def _create_base_model(input_model, current_iteration):
+def _create_base_model(input_model, current_iteration, dv):
     theta = Parameter('theta', 0.1)
     omega = Parameter('omega', 0.01, lower=0)
     sigma = Parameter('sigma', 1, lower=0)
     params = Parameters((theta, omega, sigma))
 
     eta_name = 'eta_base'
     eta = NormalDistribution.create(eta_name, 'iiv', 0, omega.symbol)
@@ -264,45 +271,47 @@
     )
     statements = Statements([y])
 
     name = f'base_{current_iteration}'
 
     est = EstimationStep.create('foce', interaction=True, maximum_evaluations=9999)
 
-    base_model = Model(
+    base_model = Model.create(
         parameters=params,
         random_variables=rvs,
         statements=statements,
         name=name,
         description=name,
         estimation_steps=EstimationSteps.create([est]),
         dependent_variables={y.symbol: 1},
     )
-    base_model = base_model.replace(dataset=_create_dataset(input_model))
+    base_model = base_model.replace(dataset=_create_dataset(input_model, dv))
     return base_model
 
 
-def _create_iiv_on_ruv_model(input_model, current_iteration):
-    model = set_iiv_on_ruv(input_model)
+def _create_iiv_on_ruv_model(input_model, current_iteration, dv):
+    model = set_iiv_on_ruv(input_model, dv)
     name = f'IIV_on_RUV_{current_iteration}'
     model = model.replace(name=name, description=name)
     return model
 
 
-def _create_power_model(input_model, current_iteration):
-    model = set_power_on_ruv(input_model, ipred='IPRED', lower_limit=None, zero_protection=True)
+def _create_power_model(input_model, current_iteration, dv):
+    model = set_power_on_ruv(
+        input_model, ipred='IPRED', lower_limit=None, zero_protection=True, dv=dv
+    )
     name = f'power_{current_iteration}'
     model = model.replace(name=name, description=name)
     return model
 
 
-def _create_time_varying_model(input_model, groups, i, current_iteration):
+def _create_time_varying_model(input_model, groups, i, current_iteration, dv):
     quantile = i / groups
     cutoff = input_model.dataset['TAD'].quantile(q=quantile)
-    model = set_time_varying_error_model(input_model, cutoff=cutoff, idv='TAD')
+    model = set_time_varying_error_model(input_model, cutoff=cutoff, idv='TAD', dv=dv)
     name = f"time_varying{i}_{current_iteration}"
     model = model.replace(name=name, description=name)
     return model
 
 
 def _create_combined_model(input_model, current_iteration):
     model = remove_error_model(input_model)
@@ -331,17 +340,24 @@
         random_variables=model.random_variables + [eps_prop, eps_add],
         name=name,
         description=name,
     )
     return model
 
 
-def _create_dataset(input_model):
+def _create_dataset(input_model, dv):
     # Non-observations have already been filtered
     residuals = input_model.modelfit_results.residuals
+    if dv:
+        input_dataset = input_model.dataset
+        input_dataset = input_dataset[input_dataset['DV'] != 0].reset_index(
+            drop=True
+        )  # filter non-observations
+        indices = input_dataset.index[input_dataset['DVID'] == dv].tolist()
+        residuals = residuals.iloc[indices]
     cwres = residuals['CWRES'].reset_index(drop=True)
     if has_blq_transformation(input_model):
         cwres = cwres.loc[cwres != 0]
     predictions = input_model.modelfit_results.predictions
     if 'CIPREDI' in predictions:
         ipredcol = 'CIPREDI'
     elif 'IPRED' in predictions:
@@ -367,15 +383,15 @@
     if 'TAD' in model.dataset:
         pass
     else:
         model = add_time_after_dose(model)
     return model
 
 
-def _create_best_model(model, res, current_iteration, groups=4, cutoff=3.84):
+def _create_best_model(model, res, current_iteration, dv, groups=4, cutoff=3.84):
     if not res.cwres_models.empty and any(res.cwres_models['dofv'] > cutoff):
         model = update_initial_estimates(model)
         selected_model_name = f'base_{current_iteration}'
         idx = res.cwres_models['dofv'].idxmax()
         name = idx[0]
 
         if current_iteration == 1:
@@ -383,52 +399,52 @@
         else:
             base_description = model.description + '+'
         model = model.replace(
             name=f'best_ruvsearch_{current_iteration}', description=base_description + name
         )
 
         if name.startswith('power'):
-            model = set_power_on_ruv(model)
+            model = set_power_on_ruv(model, dv=dv)
             model = set_initial_estimates(
                 model,
                 {
                     'power1': res.cwres_models['parameters']
                     .loc['power', 1, current_iteration]
                     .get('theta')
                     + 1
                 },
             )
         elif name.startswith('IIV_on_RUV'):
-            model = set_iiv_on_ruv(model)
+            model = set_iiv_on_ruv(model, dv=dv)
             model = set_initial_estimates(
                 model,
                 {
                     'IIV_RUV1': res.cwres_models['parameters']
                     .loc['IIV_on_RUV', 1, current_iteration]
                     .get('omega')
                 },
             )
         elif name.startswith('time_varying'):
             model = _time_after_dose(model)
             i = int(name[-1])
             quantile = i / groups
-            df = _create_dataset(model)
+            df = _create_dataset(model, dv=dv)
             tad = df['TAD']
             cutoff_tvar = tad.quantile(q=quantile)
-            model = set_time_varying_error_model(model, cutoff=cutoff_tvar, idv='TAD')
+            model = set_time_varying_error_model(model, cutoff=cutoff_tvar, idv='TAD', dv=dv)
             model = set_initial_estimates(
                 model,
                 {
                     'time_varying': res.cwres_models['parameters']
                     .loc[f"time_varying{i}", 1, current_iteration]
                     .get('theta')
                 },
             )
         else:
-            model = set_combined_error_model(model)
+            model = set_combined_error_model(model, dv=dv)
             model = set_initial_estimates(
                 model,
                 {
                     'sigma_prop': res.cwres_models['parameters']
                     .loc['combined', 1, current_iteration]
                     .get('sigma_prop'),
                     'sigma_add': res.cwres_models['parameters']
@@ -442,15 +458,15 @@
         model = None
         selected_model_name = None
     return model, selected_model_name
 
 
 @with_runtime_arguments_type_check
 @with_same_arguments_as(create_workflow)
-def validate_input(model, groups, p_value, skip, max_iter):
+def validate_input(model, groups, p_value, skip, max_iter, dv):
     if groups <= 0:
         raise ValueError(f'Invalid `groups`: got `{groups}`, must be >= 1.')
 
     if not 0 < p_value <= 1:
         raise ValueError(f'Invalid `p_value`: got `{p_value}`, must be a float in range (0, 1].')
 
     if skip is not None and not set(skip).issubset(SKIP):
@@ -478,7 +494,14 @@
             )
 
         if has_blq_transformation(model) and max_iter > 1:
             raise ValueError(
                 f'Invalid `max_iter`: got `{max_iter}`,only 1 iteration is supported '
                 f'for models with BLQ transformation.'
             )
+
+        if dv:
+            if 'DVID' not in model.dataset.columns:
+                raise ValueError("No column DVID in dataset.")
+            else:
+                if dv not in set(model.dataset['DVID']):
+                    raise ValueError(f"No DVID = {dv} in dataset.")
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/simeval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/simfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/tmdd.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/structsearch/tool.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/structsearch/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.model import Model
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import summarize_modelfit_results
 from pharmpy.tools.common import ToolResults, create_results
 from pharmpy.tools.modelfit import create_fit_workflow
-from pharmpy.workflows import Task, Workflow, call_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow
 
-from .pkpd import create_pkpd_models
+from .pkpd import create_baseline_pd_model, create_pkpd_models
 from .tmdd import create_qss_models, create_remaining_models
 
 ROUTES = frozenset(('iv', 'oral'))
 TYPES = frozenset(('tmdd', 'pkpd'))
 
 
 def create_workflow(
@@ -50,22 +50,21 @@
     >>> from pharmpy.modeling import *
     >>> from pharmpy.tools import run_structsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_structsearch(model_type='tmdd', results=results, model=model)   # doctest: +SKIP
     """
 
-    wf = Workflow()
-    wf.name = 'structsearch'
+    wb = WorkflowBuilder(name="structsearch")
     if type == 'tmdd':
         start_task = Task('run_tmdd', run_tmdd, model)
     elif type == 'pkpd':
         start_task = Task('run_pkpd', run_pkpd, model)
-    wf.add_task(start_task)
-    return wf
+    wb.add_task(start_task)
+    return Workflow(wb)
 
 
 def run_tmdd(context, model):
     qss_candidate_models = create_qss_models(model)
 
     wf = create_fit_workflow(qss_candidate_models)
     task_results = Task('results', bundle_results)
@@ -95,31 +94,43 @@
         rank_type='bic',
         cutoff=None,
         summary_models=pd.concat([summary_input, summary_candidates], keys=[0, 1], names=['step']),
     )
 
 
 def run_pkpd(context, model):
-    pkpd_models = create_pkpd_models(model, model.modelfit_results.parameter_estimates)
+    baseline_pd_model = create_baseline_pd_model(model, model.modelfit_results.parameter_estimates)
+    wf = create_fit_workflow(baseline_pd_model)
+    wb = WorkflowBuilder(wf)
+    task_results = Task('results2', bundle_results)
+    wb.add_task(task_results, predecessors=wf.output_tasks)
+    pd_baseline_fit = call_workflow(Workflow(wb), 'results_remaining', context)
 
-    wf = create_fit_workflow(pkpd_models)
+    pkpd_models = create_pkpd_models(
+        model,
+        pd_baseline_fit[0].modelfit_results.parameter_estimates,
+        model.modelfit_results.parameter_estimates,
+    )
+
+    wf2 = create_fit_workflow(pkpd_models)
+    wb2 = WorkflowBuilder(wf2)
     task_results = Task('results2', bundle_results)
-    wf.add_task(task_results, predecessors=wf.output_tasks)
-    pkpd_models_fit = call_workflow(wf, 'results_remaining', context)
+    wb2.add_task(task_results, predecessors=wf2.output_tasks)
+    pkpd_models_fit = call_workflow(Workflow(wb2), 'results_remaining', context)
 
     summary_input = summarize_modelfit_results(model.modelfit_results)
     summary_candidates = summarize_modelfit_results(
-        [model.modelfit_results for model in pkpd_models_fit]
+        [model.modelfit_results for model in pd_baseline_fit + pkpd_models_fit]
     )
 
     return create_results(
         StructSearchResults,
         model,
         model,
-        list(pkpd_models_fit),
+        list(pd_baseline_fit + pkpd_models_fit),
         rank_type='bic',
         cutoff=None,
         summary_models=pd.concat([summary_input, summary_candidates], keys=[0, 1], names=["step"]),
     )
 
 
 def bundle_results(*args):
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.99.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/visualization.py` & `pharmpy-core-0.99.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     LocalDirectoryDatabase,
     LocalModelDirectoryDatabase,
     ModelDatabase,
     NullModelDatabase,
 )
 from .task import Task
 from .tool_database import LocalDirectoryToolDatabase, NullToolDatabase, ToolDatabase
-from .workflow import Workflow
+from .workflow import Workflow, WorkflowBuilder
 
 
 class WorkflowConfiguration(config.Configuration):
     module = 'pharmpy.workflows'
     default_dispatcher = config.ConfigItem(
         'pharmpy.workflows.local_dask', 'Name of default dispatcher module'
     )
@@ -87,8 +87,9 @@
     'Log',
     'NullModelDatabase',
     'NullToolDatabase',
     'ModelDatabase',
     'Task',
     'ToolDatabase',
     'Workflow',
+    'WorkflowBuilder',
 ]
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/args.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/call.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/call.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TypeVar
 
 from .context import insert_context
-from .workflow import Workflow
+from .workflow import Workflow, WorkflowBuilder
 
 T = TypeVar('T')
 
 
 def call_workflow(wf: Workflow[T], unique_name, db) -> T:
     """Dynamically call a workflow from another workflow.
 
@@ -25,15 +25,17 @@
     Any
         Whatever the dynamic workflow returns
     """
     from dask.distributed import get_client, rejoin, secede
 
     from .optimize import optimize_task_graph_for_dask_distributed
 
-    insert_context(wf, db)
+    wb = WorkflowBuilder(wf)
+    insert_context(wb, db)
+    wf = Workflow(wb)
 
     client = get_client()
     dsk = wf.as_dask_dict()
     dsk[unique_name] = dsk.pop('results')
     dsk_optimized = optimize_task_graph_for_dask_distributed(client, dsk)
     futures = client.get(dsk_optimized, unique_name, sync=False)
     secede()
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import replace
 from typing import TypeVar
 
 from pharmpy.model import Model, Results
 
 from .context import insert_context
-from .workflow import Workflow
+from .workflow import Workflow, WorkflowBuilder
 
 T = TypeVar('T')
 
 
 def execute_workflow(
     workflow: Workflow[T], dispatcher=None, database=None, path=None, resume=False
 ) -> T:
@@ -45,30 +45,33 @@
         database = default_tool_database(
             toolname=workflow.name, path=path, exist_ok=resume
         )  # TODO: database -> tool_database
 
     # For all input models set new database and read in results
     original_input_models = []
     input_models = []
+    wb = WorkflowBuilder(workflow)
     for task in workflow.tasks:
         new_inp = []
 
         for inp in task.task_input:
             if isinstance(inp, Model):
                 original_input_models.append(inp)
                 inp.modelfit_results  # To read in the results
                 new_model = inp.replace(parent_model=inp.name)
                 new_inp.append(new_model)
                 input_models.append(new_model)
             else:
                 new_inp.append(inp)
 
-        task.task_input = tuple(new_inp)
+        new_task = task.replace(task_input=tuple(new_inp))
+        wb.replace_task(task, new_task)
 
-    insert_context(workflow, database)
+    insert_context(wb, database)
+    workflow = Workflow(wb)
 
     res: T = dispatcher.run(workflow)
 
     if isinstance(res, Results):
         if hasattr(res, 'tool_database'):
             res = replace(res, tool_database=database)
         database.store_results(res)
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/log.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/local_directory.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.99.0/src/pharmpy/workflows/workflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,98 @@
 from __future__ import annotations
 
-import copy
 import uuid
-from typing import Generic, Iterable, List, Optional, TypeVar, Union
+from typing import Generic, List, Optional, TypeVar, Union
 
 from pharmpy.deps import networkx as nx
+from pharmpy.internals.immutable import Immutable
 
 from .task import Task
 
 T = TypeVar('T')
 
 
-class Workflow(Generic[T]):
-    """Workflow class
+class WorkflowBase:
+    """Common base class for Workflow and WorkflowBuilder"""
 
-    Representation of a directed acyclic graph with Tasks as nodes and
-    the flow of parameters as edges.
+    @property
+    def tasks(self) -> List[Task]:
+        """All tasks in workflow"""
+        return list(self._g.nodes())
 
-    Parameters
-    ----------
-    tasks : list
-        List of tasks for initialization
-    """
+    @property
+    def input_tasks(self) -> List[Task]:
+        """All input (source) tasks of entire workflow"""
+        return [node for node in self._g.nodes if self._g.in_degree(node) == 0]
+
+    @property
+    def output_tasks(self) -> List[Task]:
+        """All output tasks (sink) tasks of entire workflow"""
+        return [node for node in self._g.nodes if self._g.out_degree(node) == 0]
 
-    def __init__(self, tasks: Optional[Iterable[Task]] = None, name: Optional[str] = None):
-        self._g = nx.DiGraph()
-        self.name = name
+    def get_upstream_tasks(self, task: Task) -> List[Task]:
+        """Get all tasks upstream of a certain task
+
+        Parameters
+        ----------
+        task : Task
+            Downstream task
+
+        Returns
+        -------
+        list
+            Upstream tasks
+        """
+        edges = nx.edge_dfs(self._g, task, orientation='reverse')
+        return [node for node, _, _ in edges]
+
+    def get_predecessors(self, task: Task) -> List[Task]:
+        """Get all predecessors of task
+
+        Parameters
+        ----------
+        task : Task
+            Downstream task
+
+        Returns
+        -------
+        list
+            Predecessors of task
+        """
+        return list(self._g.predecessors(task))
+
+    def get_successors(self, task: Task) -> List[Task]:
+        """Get all successors of task
+
+        Parameters
+        ----------
+        task : Task
+            Upstream task
+
+        Returns
+        -------
+        list
+            Successors of task
+        """
+        return list(self._g.successors(task))
+
+    def __len__(self):
+        return len(self._g.nodes)
+
+
+class WorkflowBuilder(WorkflowBase):
+    """Builder class for Workflow"""
+
+    def __init__(self, workflow=None, tasks=None, name=None):
+        if workflow:
+            self._g = workflow._g.copy()
+            self.name = workflow.name
+        else:
+            self._g = nx.DiGraph()
+            self.name = name
         if tasks:
             for task in tasks:
                 self.add_task(task)
 
     def add_task(self, task: Task, predecessors: Optional[Union[Task, List[Task]]] = None):
         """Add a task to the workflow
 
@@ -46,14 +109,27 @@
         if predecessors is not None:
             if not isinstance(predecessors, list):
                 self._g.add_edge(predecessors, task)
             else:
                 for pred in predecessors:
                     self._g.add_edge(pred, task)
 
+    def replace_task(self, task: Task, new_task: Task):
+        """Replace a task with a new task
+
+        Parameters
+        ----------
+        task : Task
+            Task to replace
+        new_task : Task
+            New task
+        """
+        mapping = {task: new_task}
+        nx.relabel_nodes(self._g, mapping, copy=False)
+
     def insert_workflow(
         self, other: Workflow, predecessors: Optional[Union[Task, List[Task]]] = None
     ):
         """Insert other workflow
 
         Parameters
         ----------
@@ -81,14 +157,55 @@
                 self._g.add_edge(outp, input_tasks[0])
         elif len(output_tasks) == 1:
             for inp in input_tasks:
                 self._g.add_edge(output_tasks[0], inp)
         else:
             raise ValueError('Having N:M connections between workflows is currently not supported')
 
+    def __add__(self, other: Workflow):
+        wb_new = WorkflowBuilder()
+        wb_new._g = nx.compose(self._g, other._g)
+        wb_new.name = self.name
+        return wb_new
+
+
+class Workflow(WorkflowBase, Generic[T], Immutable):
+    """Workflow class
+
+    Representation of a directed acyclic graph with Tasks as nodes and
+    the flow of parameters as edges.
+
+    Parameters
+    ----------
+    tasks : list
+        List of tasks for initialization
+    """
+
+    def __init__(self, builder=None, graph=None, name: Optional[str] = None):
+        if builder is not None:
+            self._g = nx.freeze(builder._g.copy())
+            self._name = builder.name
+        elif graph is not None:
+            self._g = graph
+            self._name = name
+
+    @classmethod
+    def create(cls, builder=None, graph=None, name=None):
+        return cls(builder=builder, graph=graph, name=name)
+
+    def replace(self, **kwargs):
+        builder = kwargs.get('builder', None)
+        if builder is None:
+            g = kwargs.get('graph', self._g)
+            name = kwargs.get('name', self._name)
+        else:
+            g = None
+            name = None
+        return Workflow.create(builder=builder, graph=g, name=name)
+
     def as_dask_dict(self):
         """Create a dask workflow dictionary
 
         Returns
         -------
         dict
             Dask workflow dictionary
@@ -108,100 +225,30 @@
             input_list = list(task.task_input)
             input_list.extend(ids[t] for t in self._g.predecessors(task))
             value = (task.function, *input_list)
             as_dict[key] = value
         return as_dict
 
     @property
-    def input_tasks(self) -> List[Task]:
-        """All input (source) tasks of entire workflow"""
-        return [node for node in self._g.nodes if self._g.in_degree(node) == 0]
-
-    @property
-    def output_tasks(self) -> List[Task]:
-        """All output tasks (sink) tasks of entire workflow"""
-        return [node for node in self._g.nodes if self._g.out_degree(node) == 0]
-
-    def get_upstream_tasks(self, task: Task) -> List[Task]:
-        """Get all tasks upstream of a certain task
-
-        Parameters
-        ----------
-        task : Task
-            Downstream task
-
-        Returns
-        -------
-        list
-            Upstream tasks
-        """
-        edges = nx.edge_dfs(self._g, task, orientation='reverse')
-        return [node for node, _, _ in edges]
-
-    def get_predecessors(self, task: Task) -> List[Task]:
-        """Get all predecessors of task
-
-        Parameters
-        ----------
-        task : Task
-            Downstream task
-
-        Returns
-        -------
-        list
-            Predecessors of task
-        """
-        return list(self._g.predecessors(task))
-
-    def get_successors(self, task: Task) -> List[Task]:
-        """Get all successors of task
-
-        Parameters
-        ----------
-        task : Task
-            Upstream task
-
-        Returns
-        -------
-        list
-            Successors of task
-        """
-        return list(self._g.successors(task))
-
-    def copy(self) -> Workflow[T]:
-        """Deepcopy of workflow
-
-        Returns
-        -------
-        Workflow
-            Deepcopy
-        """
-        wf_copy = copy.deepcopy(self)
-        return wf_copy
+    def name(self):
+        """Name of Workflow"""
+        return self._name
 
     def plot_dask(self, filename: str):
         """Save a visualization of workflow to file
 
         Parameters
         ----------
         filename : str
             Path
         """
         from dask import visualize  # pyright: ignore [reportPrivateImportUsage]
 
         visualize(self.as_dask_dict(), filename=filename, collapse_outputs=True)
 
-    @property
-    def tasks(self) -> List[Task]:
-        """All tasks in workflow"""
-        return list(self._g.nodes())
-
-    def __len__(self):
-        return len(self._g.nodes)
-
     def __str__(self):
         return '\n'.join([str(task) for task in self._g])
 
     def __add__(self, other: Workflow):
-        wf_new = Workflow()
-        wf_new._g = nx.compose(self._g, other._g)
+        g = nx.compose(self._g, other._g)
+        wf_new = Workflow(graph=g)
         return wf_new
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.99.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.98.2
+Version: 0.99.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,39 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.99.0 (2023-08-23)
+-------------------
+
+New features
+============
+
+* Add function modeling.set_reference_values
+* Add function modeling.set_lloq_data
+* Parse IV+oral models using CMT column
+* Specify DV in RUVSearch
+* Option to add logit IIV in ``add_iiv``
+* New options for remove_loq_data
+
+Changes
+=======
+
+* Make Task and Workflow immutable
+* Ignore fixed IIVs/IOVs in IIVSearch and IOVSearch
+
+Bugfixes
+========
+
+* Fix bug where epsilons where removed in ``remove_iiv``
+* Fix bug in ``create_basic_pk_model`` to handle space separated datasets
+
 0.98.0 (2023-07-21)
 -------------------
 
 New features
 ============
 
 * Support for multiple doses
```

### Comparing `pharmpy-core-0.98.2/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.99.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,20 @@
 tests/testdata/nonmem/pheno_block.mod
 tests/testdata/nonmem/pheno_clashing_symbols.mod
 tests/testdata/nonmem/pheno_etas.mod
 tests/testdata/nonmem/pheno_multivariate_piecewise.mod
 tests/testdata/nonmem/pheno_nm750.mod
 tests/testdata/nonmem/pheno_no_obs_1stID.dta
 tests/testdata/nonmem/pheno_pd.csv
+tests/testdata/nonmem/pheno_pd.ctl
+tests/testdata/nonmem/pheno_pd.ext
+tests/testdata/nonmem/pheno_pd.lst
 tests/testdata/nonmem/pheno_pd.mod
+tests/testdata/nonmem/pheno_pd.phi
+tests/testdata/nonmem/pheno_pd_mytab
 tests/testdata/nonmem/pheno_rate.dta
 tests/testdata/nonmem/pheno_real.coi
 tests/testdata/nonmem/pheno_real.cor
 tests/testdata/nonmem/pheno_real.cov
 tests/testdata/nonmem/pheno_real.ext
 tests/testdata/nonmem/pheno_real.lst
 tests/testdata/nonmem/pheno_real.mod
```

### Comparing `pharmpy-core-0.98.2/tests/cli/test_cli.py` & `pharmpy-core-0.99.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/conftest.py` & `pharmpy-core-0.99.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/external/test_nlmixr.py` & `pharmpy-core-0.99.0/tests/external/test_nlmixr.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/external/test_rxode.py` & `pharmpy-core-0.99.0/tests/external/test_rxode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/conftest.py` & `pharmpy-core-0.99.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_allometry.py` & `pharmpy-core-0.99.0/tests/integration/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_amd.py` & `pharmpy-core-0.99.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_bootstrap.py` & `pharmpy-core-0.99.0/tests/integration/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_common.py` & `pharmpy-core-0.99.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_covsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_estmethod.py` & `pharmpy-core-0.99.0/tests/integration/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_evaldesign.py` & `pharmpy-core-0.99.0/tests/integration/test_evaldesign.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_fit.py` & `pharmpy-core-0.99.0/tests/integration/test_fit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_iivsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_iovsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_iovsearch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import shutil
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
+from pharmpy.modeling import fix_parameters
 from pharmpy.tools import fit, run_iovsearch
 
 
 def test_default_mox2(tmp_path, model_count, start_model):
     with chdir(tmp_path):
         res = run_iovsearch('VISI', results=start_model.modelfit_results, model=start_model)
         rundir = tmp_path / 'iovsearch_dir1'
         assert model_count(rundir) == 8
 
         assert res.final_model_name == 'iovsearch_run7'
 
 
+def test_ignore_fixed_iiv(tmp_path, model_count, start_model):
+    with chdir(tmp_path):
+        start_model = fix_parameters(start_model, 'IIV_CL')
+        res = run_iovsearch('VISI', results=start_model.modelfit_results, model=start_model)
+        assert len(res.summary_models) == 5
+
+
 def test_rank_type_ofv_mox2(tmp_path, model_count, start_model):
     with chdir(tmp_path):
         res = run_iovsearch(
             'VISI', results=start_model.modelfit_results, model=start_model, rank_type='ofv'
         )
         rundir = tmp_path / 'iovsearch_dir1'
         assert model_count(rundir) == 8
```

### Comparing `pharmpy-core-0.98.2/tests/integration/test_modelsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_resume.py` & `pharmpy-core-0.99.0/tests/integration/test_resume.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_ruvsearch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,44 @@
 import shutil
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
-from pharmpy.modeling import remove_covariance_step, transform_blq
-from pharmpy.tools import read_modelfit_results, retrieve_final_model, run_tool
+from pharmpy.modeling import (
+    convert_model,
+    create_basic_pk_model,
+    remove_covariance_step,
+    transform_blq,
+)
+from pharmpy.tools import (
+    fit,
+    read_modelfit_results,
+    retrieve_final_model,
+    run_structsearch,
+    run_tool,
+)
+from pharmpy.tools.structsearch.pkpd import create_pk_model
+
+
+def test_ruvsearch_dv(tmp_path, load_model_for_test, testdata):
+    with chdir(tmp_path):
+        dataset = testdata / "nonmem/pheno_pd.csv"
+        model = create_basic_pk_model("iv", dataset_path=dataset)
+        model = convert_model(model, 'nonmem')
+
+        # Fit pk model
+        pk_model = create_pk_model(model)
+        pk_res = fit(pk_model)
+
+        # structsearch
+        res_struct = run_structsearch(type='pkpd', route='iv', results=pk_res, model=model)
+        model = res_struct.models[1]
+
+        # ruvsearch
+        res_ruv = run_tool('ruvsearch', model=model, results=model.modelfit_results, dv=2)
+        assert res_ruv
 
 
 def test_ruvsearch(tmp_path, testdata):
     with chdir(tmp_path):
         for path in (testdata / 'nonmem' / 'ruvsearch').glob('mox3.*'):
             shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'ruvsearch' / 'moxo_simulated_resmod.csv', tmp_path)
```

### Comparing `pharmpy-core-0.98.2/tests/integration/test_structsearch.py` & `pharmpy-core-0.99.0/tests/integration/test_structsearch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from pharmpy.internals.fs.cwd import chdir
-from pharmpy.tools import fit, run_structsearch
+from pharmpy.modeling import convert_model, create_basic_pk_model
+from pharmpy.tools import fit  # , run_structsearch
 from pharmpy.tools.structsearch.pkpd import create_pk_model
 
 
 def test_pkpd(tmp_path, load_model_for_test, testdata):
     with chdir(tmp_path):
-        model = load_model_for_test(testdata / "nonmem" / "pheno_pd.mod")
+        model = create_basic_pk_model('iv', dataset_path=testdata / "nonmem" / "pheno_pd.csv")
+        model = convert_model(model, 'nonmem')
         pk_model = create_pk_model(model)  # NOTE: this step needs to be removed later
-        pk_res = fit(pk_model)
-        res = run_structsearch(type='pkpd', route='iv', results=pk_res, model=model)
+        fit(pk_model)
+    #    res = run_structsearch(type='pkpd', route='iv', results=pk_res, model=model)
 
-        no_of_models = 12
-        assert len(res.summary_models) == no_of_models + 1
-        assert len(res.summary_tool) == no_of_models + 1
-        assert len(res.models) == no_of_models
+    #    no_of_models = 9
+    #    assert len(res.summary_models) == no_of_models + 1
+    #    assert len(res.summary_tool) == no_of_models + 1
+    #    assert len(res.models) == no_of_models
 
-        rundir = tmp_path / 'structsearch_dir1'
-        assert rundir.is_dir()
-        assert (rundir / 'results.json').exists()
-        assert (rundir / 'results.csv').exists()
-        assert (rundir / 'metadata.json').exists()
+    #    rundir = tmp_path / 'structsearch_dir1'
+    #    assert rundir.is_dir()
+    #    assert (rundir / 'results.json').exists()
+    #    assert (rundir / 'results.csv').exists()
+    #    assert (rundir / 'metadata.json').exists()
```

### Comparing `pharmpy-core-0.98.2/tests/internals/fs/test_lock.py` & `pharmpy-core-0.99.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/internals/module/test_lazy.py` & `pharmpy-core-0.99.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/internals/test_math.py` & `pharmpy-core-0.99.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/internals/test_parse.py` & `pharmpy-core-0.99.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/model/test_datainfo.py` & `pharmpy-core-0.99.0/tests/model/test_datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/model/test_estimation.py` & `pharmpy-core-0.99.0/tests/model/test_estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/model/test_model.py` & `pharmpy-core-0.99.0/tests/model/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     nm_model = load_model_for_test(path)
     model = convert_model(nm_model, 'generic')
 
     assert model.parameters == nm_model.parameters
     assert model.random_variables == nm_model.random_variables
     assert model.name == nm_model.name
     assert model.statements == nm_model.statements
-    assert type(model) == Model
+    assert isinstance(model, Model)
 
 
 def test_model_equality():
     pheno1 = load_example_model("pheno")
     assert pheno1 == pheno1
 
     pheno2 = load_example_model("pheno")
```

### Comparing `pharmpy-core-0.98.2/tests/model/test_parameter.py` & `pharmpy-core-0.99.0/tests/model/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/model/test_random_variables.py` & `pharmpy-core-0.99.0/tests/model/test_random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/model/test_statements.py` & `pharmpy-core-0.99.0/tests/model/test_statements.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_allometry.py` & `pharmpy-core-0.99.0/tests/modeling/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_blq.py` & `pharmpy-core-0.99.0/tests/modeling/test_blq.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_common.py` & `pharmpy-core-0.99.0/tests/modeling/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.99.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_error.py` & `pharmpy-core-0.99.0/tests/modeling/test_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1018,14 +1018,73 @@
 ELSE
     Y = Y_2
 END IF
 """
     assert str(rec) == correct
 
 
+def test_set_power_on_ruv_multiple_dvs(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'models' / 'pheno_dvid.mod')
+    updated_model = set_power_on_ruv(model, dv=1)
+    rec = updated_model.internals.control_stream.get_records('ERROR')[0]
+    correct = """$ERROR
+Y_1 = F + EPS(1)*F**THETA(3)
+Y_2 = F + EPS(1)*F + EPS(2)
+
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+"""
+    assert str(rec) == correct
+
+    updated_model = set_power_on_ruv(model, dv=2)
+    rec = updated_model.internals.control_stream.get_records('ERROR')[0]
+    correct = """$ERROR
+Y_1 = F + EPS(1)*F
+Y_2 = F + EPS(1)*F**THETA(3) + EPS(2)*F**THETA(4)
+
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+"""
+    assert str(rec) == correct
+
+    updated_model = set_power_on_ruv(model)
+    rec = updated_model.internals.control_stream.get_records('ERROR')[0]
+    correct = """$ERROR
+Y_1 = F + EPS(1)*F**THETA(3)
+Y_2 = F + EPS(1)*F**THETA(3) + EPS(2)*F**THETA(4)
+
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+"""
+    assert str(rec) == correct
+
+    updated_model = set_power_on_ruv(model, list_of_eps=["EPS_2"])
+    rec = updated_model.internals.control_stream.get_records('ERROR')[0]
+    correct = """$ERROR
+Y_1 = F + EPS(1)*F
+Y_2 = F + EPS(1)*F + EPS(2)*F**THETA(3)
+
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+"""
+    assert str(rec) == correct
+
+
 @pytest.mark.parametrize(
     'epsilons, err_ref, theta_ref',
     [
         (
             ['EPS_1'],
             'IF (F.EQ.0) F = 2.22500000000000E-307\n'
             'Y = F + EPS(1)*F**THETA(4)\n'
```

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.99.0/tests/modeling/test_estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_evaluate.py` & `pharmpy-core-0.99.0/tests/modeling/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_expressions.py` & `pharmpy-core-0.99.0/tests/modeling/test_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,19 +345,18 @@
     assert 'KE0' not in get_pk_parameters(pkpd_model)
 
 
 @pytest.mark.parametrize(
     ('model_path', 'kind', 'expected'),
     (
         ('nonmem/pheno.mod', 'baseline', ['E0']),
-        ('nonmem/pheno.mod', 'linear', ['E0', 'S']),
+        ('nonmem/pheno.mod', 'linear', ['E0', 'Slope']),
         ('nonmem/pheno.mod', 'Emax', ['E0', 'E_max', 'EC_50']),
         ('nonmem/pheno.mod', 'step', ['E0', 'E_max']),
-        ('nonmem/pheno.mod', 'sigmoid', ['EC_50', 'E_max', 'n']),
-        ('nonmem/pheno.mod', 'loglin', ['E0', 'm']),
+        ('nonmem/pheno.mod', 'sigmoid', ['E0', 'EC_50', 'E_max', 'n']),
     ),
     ids=repr,
 )
 def test_get_pd_parameters(load_model_for_test, testdata, model_path, kind, expected):
     model = load_model_for_test(testdata / model_path)
     assert set(get_pd_parameters(set_direct_effect(model, kind))) == set(expected)
     assert set(get_pd_parameters(add_effect_compartment(model, kind))) == set(expected + ["KE0"])
```

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_help_functions.py` & `pharmpy-core-0.99.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_iterators.py` & `pharmpy-core-0.99.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_lrt.py` & `pharmpy-core-0.99.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_metabolite.py` & `pharmpy-core-0.99.0/tests/modeling/test_metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_odes.py` & `pharmpy-core-0.99.0/tests/modeling/test_odes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.99.0/tests/modeling/test_parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_parameter_variability.py` & `pharmpy-core-0.99.0/tests/modeling/test_parameter_variability.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,23 @@
         ('S1', 'add', None, None, 'V=TVV*EXP(ETA(2))\nS1 = V + ETA_S1', 2),
         ('S1', 'prop', None, None, 'V=TVV*EXP(ETA(2))\nS1 = ETA_S1*V', 2),
         ('S1', 'log', None, None, 'V=TVV*EXP(ETA(2))\nS1 = V*EXP(ETA_S1)/(EXP(ETA_S1) + 1)', 2),
         ('S1', 'eta_new', '+', None, 'V=TVV*EXP(ETA(2))\nS1 = V + ETA_S1', 2),
         ('S1', 'eta_new**2', '+', None, 'V=TVV*EXP(ETA(2))\nS1 = V + ETA_S1**2', 2),
         ('S1', 'exp', '+', 'ETA(3)', 'V=TVV*EXP(ETA(2))\nS1 = V + EXP(ETA(3))', 2),
         (
+            'S1',
+            're_log',
+            '+',
+            None,
+            'V=TVV*EXP(ETA(2))\nPHI_V = LOG(V/(1 - V))'
+            '\nS1 = EXP(ETA_S1*PHI_V)/(EXP(ETA_S1*PHI_V) + 1)',
+            2,
+        ),
+        (
             ['V', 'S1'],
             'exp',
             '+',
             None,
             'V = TVV*EXP(ETA(2)) + EXP(ETA_V)\nS1 = V + EXP(ETA_S1)',
             3,
         ),
```

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_parameters.py` & `pharmpy-core-0.99.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_pd.py` & `pharmpy-core-0.99.0/tests/modeling/test_pd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from pharmpy.deps import sympy
 from pharmpy.model import (
     Assignment,
     Compartment,
     CompartmentalSystem,
     CompartmentalSystemBuilder,
     output,
@@ -9,88 +11,90 @@
 from pharmpy.modeling import add_effect_compartment, set_direct_effect
 
 
 def S(x):
     return sympy.Symbol(x)
 
 
-def test_set_direct_effect(load_model_for_test, testdata):
+@pytest.mark.parametrize(
+    'pd_model',
+    [('baseline'), ('linear'), ('Emax'), ('sigmoid'), ('step'), ('loglin')],
+)
+def test_set_direct_effect(load_model_for_test, pd_model, testdata):
     model = load_model_for_test(testdata / "nonmem" / "pheno_pd.mod")
     conc = model.statements.ode_system.central_compartment.amount / S("V")
-    _test_effect_models(set_direct_effect(model, "baseline"), "baseline", conc)
-    _test_effect_models(set_direct_effect(model, "linear"), "linear", conc)
-    _test_effect_models(set_direct_effect(model, "Emax"), "Emax", conc)
-    _test_effect_models(set_direct_effect(model, "sigmoid"), "sigmoid", conc)
-    _test_effect_models(set_direct_effect(model, "step"), "step", conc)
-    _test_effect_models(set_direct_effect(model, "loglin"), "loglin", conc)
+    _test_effect_models(set_direct_effect(model, pd_model), pd_model, conc)
 
 
-def test_add_effect_compartment(load_model_for_test, testdata):
+@pytest.mark.parametrize(
+    'pd_model',
+    [('baseline'), ('linear'), ('Emax'), ('sigmoid'), ('step'), ('loglin')],
+)
+def test_add_effect_compartment(load_model_for_test, pd_model, testdata):
     model = load_model_for_test(testdata / "nonmem" / "pheno_pd.mod")
-    conc_e = S("A_EFFECT") / S("V")
+    conc_e = S("A_EFFECT")
     ke0 = S("KE0")
     central_amount = sympy.Function("A_CENTRAL")(S('t'))
-    comp_e = Compartment.create("EFFECT", input=ke0 * central_amount)
+    comp_e = Compartment.create("EFFECT", input=ke0 * central_amount / S("V"))
 
     model1 = add_effect_compartment(model, "baseline")
     compartments = CompartmentalSystemBuilder(model1.statements.ode_system)
     odes = model1.statements.ode_system
     assert odes.find_compartment("EFFECT") == comp_e
     assert odes.zero_order_inputs[0] == 0
-    assert odes.zero_order_inputs[1] == ke0 * central_amount
+    assert odes.zero_order_inputs[1] == ke0 * central_amount / S("V")
     assert odes.get_compartment_outflows("EFFECT")[0][0] == output
     assert odes.get_compartment_outflows("EFFECT")[0][1] == ke0
     assert CompartmentalSystem(compartments).compartment_names == ['CENTRAL', 'EFFECT']
 
-    _test_effect_models(add_effect_compartment(model, "baseline"), "baseline", conc_e)
-    _test_effect_models(add_effect_compartment(model, "linear"), "linear", conc_e)
-    _test_effect_models(add_effect_compartment(model, "Emax"), "Emax", conc_e)
-    _test_effect_models(add_effect_compartment(model, "sigmoid"), "sigmoid", conc_e)
-    _test_effect_models(add_effect_compartment(model, "step"), "step", conc_e)
-    _test_effect_models(add_effect_compartment(model, "loglin"), "loglin", conc_e)
+    _test_effect_models(add_effect_compartment(model, pd_model), pd_model, conc_e)
 
 
 def _test_effect_models(model, expr, conc):
     e = S("E")
     e0 = S("E0")
     emax = S("E_max")
     ec50 = S("EC_50")
 
     if expr == 'baseline':
         assert model.statements[0] == Assignment(e0, S("POP_E0"))
         assert model.statements.after_odes[-2] == Assignment(e, e0)
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
     elif expr == 'linear':
         assert model.statements[1] == Assignment(e0, S("POP_E0"))
-        assert model.statements[0] == Assignment(S("S"), S("POP_S"))
-        assert model.statements.after_odes[-2] == Assignment(e, e0 + S("S") * conc)
+        assert model.statements[0] == Assignment(S("Slope"), S("POP_Slope"))
+        assert model.statements.after_odes[-2] == Assignment(e, e0 + S("Slope") * conc)
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
     elif expr == "Emax":
         assert model.statements[0] == Assignment(ec50, S("POP_EC_50"))
         assert model.statements[2] == Assignment(e0, S("POP_E0"))
         assert model.statements[1] == Assignment(emax, S("POP_E_max"))
         assert model.statements.after_odes[-2] == Assignment(e, e0 + (emax * conc) / (ec50 + conc))
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
     elif expr == "sigmoid":
         assert model.statements[0] == Assignment(S("n"), S("POP_n"))
         assert model.statements[1] == Assignment(ec50, S("POP_EC_50"))
         assert model.statements[3] == Assignment(e0, S("POP_E0"))
         assert model.statements[2] == Assignment(emax, S("POP_E_max"))
         assert model.statements.after_odes[-2] == Assignment(
-            e, (emax * conc ** S("n")) / (ec50 ** S("n") + conc ** S("n"))
+            e,
+            sympy.Piecewise(
+                (e0 + ((emax * conc ** S("n")) / (ec50 ** S("n") + conc ** S("n"))), conc > 0),
+                (e0, True),
+            ),
         )
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
         assert model.parameters["POP_n"].init == 1
     elif expr == "step":
         assert model.statements[1] == Assignment(e0, S("POP_E0"))
         assert model.statements[0] == Assignment(emax, S("POP_E_max"))
         assert model.statements.after_odes[-2] == Assignment(
-            e, sympy.Piecewise((e0, conc < 0), (e0 + emax, True))
+            e, sympy.Piecewise((e0, conc <= 0), (e0 + emax, True))
         )
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
     elif expr == "loglin":
         assert model.statements[1] == Assignment(e0, S("POP_E0"))
-        assert model.statements[0] == Assignment(S("m"), S("POP_m"))
+        assert model.statements[0] == Assignment(S("slope"), S("POP_slope"))
         assert model.statements.after_odes[-2] == Assignment(
-            e, S("m") * sympy.log(conc + sympy.exp(e0 / S("m")))
+            e, S("slope") * sympy.log(conc + sympy.exp(e0 / S("slope")))
         )
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
```

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_plots.py` & `pharmpy-core-0.99.0/tests/modeling/test_plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_results.py` & `pharmpy-core-0.99.0/tests/modeling/test_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/modeling/test_tmdd.py` & `pharmpy-core-0.99.0/tests/modeling/test_tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.99.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_code.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_code.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_data.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.99.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_advan.py` & `pharmpy-core-0.99.0/tests/nonmem/test_advan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 import sympy
 
+from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import output
 from pharmpy.model.external.nonmem.advan import compartmental_model
 from pharmpy.modeling import get_initial_conditions
 
 
 def S(x):
     return sympy.Symbol(x)
@@ -234,7 +235,49 @@
 $OMEGA  0.001  ;    IIV_MAT
 $OMEGA  0.001 ; IIV_MDT
 $SIGMA  0.273617  ;   RUV_PROP
 """
     model = create_model_for_test(code)
     odes = model.statements.ode_system
     assert odes.get_flow(odes.central_compartment, output) == sympy.Symbol('K100')
+
+
+def test_multiple_dv_CMT_parsing(tmp_path, testdata, load_model_for_test, create_model_for_test):
+    with chdir(tmp_path):
+        code = f"""$PROB INOGATRAN HEALTHY VOLUNTEER MODEL
+        $INPUT ID TIME AMT DV CMT
+        $DATA {tmp_path / "data_iv_oral.csv"} IGNORE=@ ;IGN(ID.GT.30)
+        $SUBROUTINE ADVAN2 TRANS1
+        $PK
+                     F2=1
+           FU=0.75
+           TVCL  = THETA(4)*(WT/70)**.75 + THETA(1)*FU*CLCR*60/1000
+           TVV   = THETA(2)*WT/70
+           TVMAT = THETA(3)
+
+           CL    = TVCL *EXP(ETA(1))
+           V     = TVV  *EXP(ETA(2))
+           MAT   = TVMAT*EXP(ETA(3))
+           KA    = 1/MAT
+           K     = CL/V
+           S2    = V
+           HL    = LOG(2)/K
+        $ERROR (OBSERVATION ONLY)
+           Y     = F*(1+EPS(1)) ;conc in mg/L
+        $THETA  (0,.1)     ;1 TVCLR - RENAL COMPONENT
+        $THETA  (0,30)     ;2 TVV
+        $THETA  (0,1)      ;3 TVMAT
+        $THETA  (0,30)     ;4 TVCLH - HEPATIC COMPONENT
+        $OMEGA  .04        ;1 IIV_CL
+        $OMEGA  .04        ;2 IIV_V
+        $OMEGA  .02        ;3 IIV_MAT
+        $SIGMA  .015        ;1 SIGMA_PK
+        $EST METH=1 INTER MAXEVAL=9999"""
+
+        pheno = load_model_for_test(testdata / 'nonmem' / "pheno.mod")
+        dataset = pheno.dataset.copy()
+        dataset["CMT"] = 2
+        dataset.loc[(dataset["ID"] <= 20) & (dataset["AMT"] == 0), "CMT"] = 1
+        dataset.to_csv(tmp_path / "data_iv_oral.csv", index=False)
+        model = create_model_for_test(code)
+        odes = model.statements.ode_system
+        assert len(odes.dosing_compartment) == 2
```

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_des.py` & `pharmpy-core-0.99.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_input.py` & `pharmpy-core-0.99.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_modelfit_results.py` & `pharmpy-core-0.99.0/tests/nonmem/test_modelfit_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.99.0/tests/nonmem/test_nonmem_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 )
 from pharmpy.model.external.nonmem import convert_model
 from pharmpy.model.external.nonmem.nmtran_parser import NMTranParser
 from pharmpy.model.external.nonmem.records.factory import create_record
 from pharmpy.modeling import (
     add_iiv,
     add_population_parameter,
+    create_basic_pk_model,
     create_joint_distribution,
+    read_model,
     remove_iiv,
+    set_direct_effect,
     set_estimation_step,
     set_initial_condition,
     set_initial_estimates,
     set_transit_compartments,
     set_zero_order_absorption,
     set_zero_order_elimination,
     set_zero_order_input,
@@ -47,14 +50,32 @@
     return symbol(x)
 
 
 def test_source(pheno):
     assert pheno.model_code.startswith('$PROBLEM PHENOBARB')
 
 
+def test_convert_nonmem_model(testdata):
+    model = create_basic_pk_model('iv', testdata / 'nonmem/pheno_pd.csv')
+    model = set_direct_effect(model, 'linear')
+    model = convert_model(model)
+    assert model.dependent_variables == {S('Y'): 1, S('Y_2'): 2}
+    assert model.observation_transformation == {S('Y'): S('Y'), S('Y_2'): S('Y_2')}
+
+
+def test_parse_nonmem_model(testdata):
+    model = read_model(testdata / 'nonmem/pheno_pd.mod')
+    assert model.dependent_variables == {S('Y'): 1}
+    assert model.observation_transformation == {S('Y'): S('Y')}
+
+    model = read_model(testdata / 'nonmem/models/pheno_dvid.mod')
+    assert model.dependent_variables == {S('Y_1'): 1, S('Y_2'): 2}
+    assert model.observation_transformation == {S('Y_1'): S('Y_1'), S('Y_2'): S('Y_2')}
+
+
 def test_update_inits(load_model_for_test, pheno_path):
     from pharmpy.modeling import update_inits
 
     model = load_model_for_test(pheno_path)
     res = read_modelfit_results(pheno_path)
     model = update_inits(model, res.parameter_estimates)
 
@@ -1019,15 +1040,15 @@
 $THETA (0,0.984258)
 $THETA (0.15892)
 $OMEGA 0.0293508 0.027906
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION MAXEVALS=9999
 """
     model = Model.parse_model_from_string(code)
-    assert type(model.statements.ode_system.eqs[0].rhs) == sympy.Piecewise
+    assert isinstance(model.statements.ode_system.eqs[0].rhs, sympy.Piecewise)
     assert model.statements[3].symbol == sympy.Function("A_CENTRAL")(0)
     assert model.statements[3].expression == sympy.Integer(2)
 
 
 @pytest.mark.parametrize(
     'estline,likelihood',
     [
```

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.99.0/tests/nonmem/test_nonmem_table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_parser.py` & `pharmpy-core-0.99.0/tests/nonmem/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/nonmem/test_read.py` & `pharmpy-core-0.99.0/tests/nonmem/test_read.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/frem/results.json` & `pharmpy-core-0.99.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.99.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/failed_run.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/failed_run.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.99.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.99.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_des_assignments.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_des_assignments.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_pd.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_pd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.99.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.99.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.99.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.99.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.99.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/pheno_data.csv` & `pharmpy-core-0.99.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.99.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.99.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.99.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.99.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.99.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/amd_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/amd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/metadata.json` & `pharmpy-core-0.99.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/qa_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.99.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.99.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_allometry.py` & `pharmpy-core-0.99.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_amd.py` & `pharmpy-core-0.99.0/tests/tools/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_bootstrap.py` & `pharmpy-core-0.99.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_cdd.py` & `pharmpy-core-0.99.0/tests/tools/test_cdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_covsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_estmethod.py` & `pharmpy-core-0.99.0/tests/tools/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_exports.py` & `pharmpy-core-0.99.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_frem.py` & `pharmpy-core-0.99.0/tests/tools/test_frem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_iivsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_iivsearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pytest
 
 from pharmpy.modeling import (
     add_iiv,
+    add_individual_parameter,
     add_peripheral_compartment,
     add_pk_iiv,
     create_joint_distribution,
+    fix_parameters,
 )
 from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.iivsearch.algorithms import (
     _create_param_dict,
     _is_rv_block_structure,
     _rv_block_structures,
     brute_force_block_structure,
@@ -17,25 +19,49 @@
 )
 from pharmpy.tools.iivsearch.tool import create_workflow, validate_input
 from pharmpy.workflows import Workflow
 
 
 @pytest.mark.parametrize(
     'list_of_parameters, expected_values',
+    [([], 4), (['IVCL'], 1), (["IVCL", "IVV"], 0)],
+)
+def test_brute_force_block_structure_ignore_fixed_params(
+    load_model_for_test, testdata, list_of_parameters, expected_values
+):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    model = add_individual_parameter(model, 'PD1')
+    model = add_iiv(model, 'PD1', 'exp')
+    model = fix_parameters(model, list_of_parameters)
+    wf = brute_force_block_structure(model)
+    fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
+    assert len(fit_tasks) == expected_values
+
+
+@pytest.mark.parametrize(
+    'list_of_parameters, expected_values',
     [([], 3), (['CL'], 1), (["CL", "V"], 0)],
 )
 def test_brute_force_no_of_etas_keep(
     load_model_for_test, testdata, list_of_parameters, expected_values
 ):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
     wf = brute_force_no_of_etas(model, keep=list_of_parameters)
     fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
     assert len(fit_tasks) == expected_values
 
 
+def test_brute_force_no_of_etas_fixed(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    model = fix_parameters(model, 'IVCL')
+    wf = brute_force_no_of_etas(model)
+    fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
+    assert len(fit_tasks) == 1
+
+
 @pytest.mark.parametrize(
     'list_of_parameters, no_of_models',
     [([], 7), (['QP1'], 15)],
 )
 def test_brute_force_no_of_etas(load_model_for_test, testdata, list_of_parameters, no_of_models):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
     model = add_peripheral_compartment(model)
@@ -68,15 +94,15 @@
     assert len(fit_tasks) == no_of_models
 
 
 def test_rv_block_structures_4_etas(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
     model = add_iiv(model, ['TAD', 'S1'], 'exp')
 
-    block_structures = list(_rv_block_structures(model.random_variables.iiv))
+    block_structures = list(_rv_block_structures(model.random_variables.iiv.names))
 
     assert len(block_structures) == 15
 
     block_structures_integer_partitions = [
         tuple(map(len, block_structure)) for block_structure in block_structures
     ]
     assert block_structures_integer_partitions.count((4,)) == 1
@@ -86,15 +112,15 @@
     assert block_structures_integer_partitions.count((1, 1, 1, 1)) == 1
 
 
 def test_rv_block_structures_5_etas(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
     model = add_iiv(model, ['TVCL', 'TAD', 'S1'], 'exp')
 
-    block_structures = list(_rv_block_structures(model.random_variables.iiv))
+    block_structures = list(_rv_block_structures(model.random_variables.iiv.names))
     assert len(block_structures) == 52
 
     block_structures_integer_partitions = [
         tuple(map(len, block_structure)) for block_structure in block_structures
     ]
     assert block_structures_integer_partitions.count((5,)) == 1
     assert block_structures_integer_partitions.count((1, 4)) == 5
@@ -113,26 +139,26 @@
     etas_block_structure = (('ETA_1', 'ETA_2'), ('ETA_TAD',), ('ETA_S1',))
     model = create_joint_distribution(
         model,
         list(etas_block_structure[0]),
         individual_estimates=res.individual_estimates,
     )
     etas = model.random_variables.iiv
-    assert _is_rv_block_structure(etas, etas_block_structure)
+    assert _is_rv_block_structure(etas, etas_block_structure, [])
 
     etas_block_structure = (('ETA_1',), ('ETA_2',), ('ETA_TAD', 'ETA_S1'))
-    assert not _is_rv_block_structure(etas, etas_block_structure)
+    assert not _is_rv_block_structure(etas, etas_block_structure, [])
 
     etas_block_structure = (('ETA_1',), ('ETA_2', 'ETA_TAD'), ('ETA_S1',))
-    assert not _is_rv_block_structure(etas, etas_block_structure)
+    assert not _is_rv_block_structure(etas, etas_block_structure, [])
 
     model = create_joint_distribution(model, individual_estimates=res.individual_estimates)
     etas_block_structure = (('ETA_1', 'ETA_2', 'ETA_TAD', 'ETA_S1'),)
     etas = model.random_variables.iiv
-    assert _is_rv_block_structure(etas, etas_block_structure)
+    assert _is_rv_block_structure(etas, etas_block_structure, [])
 
 
 def test_create_joint_dist(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
     res = read_modelfit_results(testdata / 'nonmem' / 'models' / 'mox2.mod')
     # FIXME!!
     model = model.replace(modelfit_results=res)
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_iovsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_iovsearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import pytest
 from sympy import Symbol as S
 
-from pharmpy.modeling import add_iov, remove_iov
+from pharmpy.modeling import add_iov, fix_parameters, remove_iov
 from pharmpy.tools.iovsearch.tool import (
     _get_iiv_etas_with_corresponding_iov,
+    _get_nonfixed_iivs,
     create_workflow,
     validate_input,
 )
 from pharmpy.workflows import Workflow
 
 
+def test_ignore_fixed_iiv(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
+    assert len(model.random_variables.iiv.names) == 2
+    model = fix_parameters(model, 'IVCL')
+    nonfixed_iivs = _get_nonfixed_iivs(model)
+    assert len(nonfixed_iivs.names) == 1
+
+
 def test_iovsearch_github_issues_976(load_model_for_test, testdata):
     m = load_model_for_test(testdata / 'nonmem' / 'pheno_multivariate_piecewise.mod')
     assert not m.random_variables.iov
     assert set(_get_iiv_etas_with_corresponding_iov(m)) == set()
 
     m = add_iov(m, 'FA1', distribution='same-as-iiv')
     assert set(_get_iiv_etas_with_corresponding_iov(m)) == set(
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_linearize.py` & `pharmpy-core-0.99.0/tests/tools/test_linearize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_mfl.py` & `pharmpy-core-0.99.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_ml.py` & `pharmpy-core-0.99.0/tests/tools/test_ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_modelsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_qa.py` & `pharmpy-core-0.99.0/tests/tools/test_qa.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.99.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_run.py` & `pharmpy-core-0.99.0/tests/tools/test_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,14 +323,27 @@
     assert np.isnan(df.loc['m6']['rank'])
 
     # Test if base model failed, fall back to rank value
     base_nan = DummyModel('base_nan', parent='base_nan', parameter_names=['p1'], ofv=np.nan)
     df = rank_models(base_nan, models, errors_allowed=['rounding_errors'], rank_type='ofv')
     assert df.iloc[0].name == 'm1'
 
+    # Test if base model failed but still has OFV with a very high value, fall back to rank value
+    base_nan = DummyModel(
+        'base_nan',
+        parent='base_nan',
+        parameter_names=['p1'],
+        ofv=2e154,
+        minimization_successful=False,
+        termination_cause='something',
+    )
+    df = rank_models(base_nan, models, errors_allowed=['rounding_errors'], rank_type='ofv')
+    assert df.iloc[0].name == 'm1'
+    assert df.nunique()['ofv'] == df.nunique()['rank']
+
 
 def test_summarize_modelfit_results(
     load_model_for_test, create_model_for_test, testdata, pheno_path
 ):
     pheno = read_modelfit_results(pheno_path)
 
     summary_single = summarize_modelfit_results(pheno)
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_runtool.py` & `pharmpy-core-0.99.0/tests/tools/test_runtool.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 
 import pytest
 
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model, Results
 from pharmpy.tools.run import import_tool, run_tool_with_name
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 def test_import_tool():
     from pharmpy.tools import iivsearch
 
     tool = import_tool('iivsearch')
     assert tool == iivsearch
 
 
 def create_workflow_rename(new_name, name=None, model: Optional[Model] = None):
     def rename(m):
         m = m.replace(name=new_name)
         return m
 
-    wf = Workflow([Task('copy', lambda x: x, model)], name=name)
-    wf.insert_workflow(Workflow([Task('rename', rename)]))
-    return wf
+    wb = WorkflowBuilder(tasks=[Task('copy', lambda x: x, model)], name=name)
+    wb.insert_workflow(WorkflowBuilder(tasks=[Task('rename', rename)]))
+    return Workflow(wb)
 
 
 @with_same_arguments_as(create_workflow_rename)
 def validate_input_rename(model, new_name):
     assert isinstance(new_name, str)
     assert isinstance(model, Model)
 
 
 def create_workflow_generic(name=None, model: Optional[Model] = None):
-    return Workflow([Task('copy', lambda _: Results(), model)], name=name)
+    return Workflow(WorkflowBuilder(tasks=[Task('copy', lambda _: Results(), model)], name=name))
 
 
 @with_same_arguments_as(create_workflow_generic)
 def validate_input_generic(model):
     assert isinstance(model, Model)
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_ruvsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 from pharmpy.modeling import remove_covariance_step, transform_blq
 from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.ruvsearch.results import psn_resmod_results
 from pharmpy.tools.ruvsearch.tool import _create_dataset, create_workflow, validate_input
 from pharmpy.workflows import Workflow
 
 
+def test_filter_dataset(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem/pheno_pd.mod')
+    res = read_modelfit_results(testdata / 'nonmem/pheno_pd.mod')
+    model = model.replace(modelfit_results=res)
+    cwres = _create_dataset(model, dv=2)
+    expected_cwres = [-1.15490, 0.95703, -0.85365, 0.42327]
+    assert cwres['DV'].tolist() == expected_cwres
+
+
 def test_resmod_results(testdata):
     res = psn_resmod_results(testdata / 'psn' / 'resmod_dir1')
     assert list(res.cwres_models['dOFV']) == [
         -1.31,
         -3.34,
         -13.91,
         -18.54,
@@ -64,15 +73,15 @@
 
 
 def test_create_dataset(load_model_for_test, testdata, tmp_path):
     model = load_model_for_test(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
     res = read_modelfit_results(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
     model = model.replace(modelfit_results=res)
 
-    df = _create_dataset(model)
+    df = _create_dataset(model, dv=None)
 
     assert len(df) == 1006
     assert (df['DV'] != 0).all()
 
     with chdir(tmp_path):
         for path in (testdata / 'nonmem' / 'ruvsearch').glob('mox3.*'):
             shutil.copy2(path, tmp_path)
@@ -89,15 +98,15 @@
         model = load_model_for_test('mox3.mod')
         res = read_modelfit_results('mox3.mod')
 
         model = model.replace(modelfit_results=res)
 
         model = transform_blq(model, method='m3', lloq=0.05)
 
-        df = _create_dataset(model)
+        df = _create_dataset(model, dv=None)
 
         assert len(df) == 1005
         assert (df['DV'] != 0).all()
 
 
 @pytest.mark.parametrize(
     ('model_path', 'arguments', 'exception', 'match'),
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_scm.py` & `pharmpy-core-0.99.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_start_model.py` & `pharmpy-core-0.99.0/tests/tools/test_start_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_structsearch.py` & `pharmpy-core-0.99.0/tests/tools/test_structsearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,25 +67,27 @@
     models = create_remaining_models(model, ests)
     assert len(models) == 12
 
 
 def test_pkpd(load_model_for_test, testdata):
     res = read_modelfit_results(testdata / "nonmem" / "pheno.mod")
     ests = res.parameter_estimates
+    e0_init = pd.Series({'POP_E0': 5.75, 'IIV_E0': 0.01, 'sigma': 0.33})
     model = load_model_for_test(testdata / "nonmem" / "pheno_pd.mod")
-    pkpd_models = create_pkpd_models(model, ests)
-    assert len(pkpd_models) == 12
-    assert pkpd_models[0].name == "direct_effect_baseline"
-    assert pkpd_models[1].name == "direct_effect_linear"
-    assert pkpd_models[6].name == "effect_compartment_baseline"
-    assert pkpd_models[7].name == "effect_compartment_linear"
+    pkpd_models = create_pkpd_models(model, e0_init, ests)
+
+    assert len(pkpd_models) == 8
+    assert pkpd_models[0].name == "structsearch_run1"
+    assert pkpd_models[1].name == "structsearch_run2"
+    assert pkpd_models[4].name == "structsearch_run5"
+    assert pkpd_models[5].name == "structsearch_run6"
     assert pkpd_models[0].parameters[0].name == 'TVCL'
-    assert pkpd_models[6].parameters[0].name == 'TVCL'
+    assert pkpd_models[5].parameters[0].name == 'TVCL'
     assert pkpd_models[0].parameters[1].name == 'TVV'
-    assert pkpd_models[6].parameters[1].name == 'TVV'
+    assert pkpd_models[5].parameters[1].name == 'TVV'
 
 
 def test_create_workflow():
     assert isinstance(create_workflow('oral', 'pkpd'), Workflow)
 
 
 def test_create_workflow_pkpd(load_model_for_test, testdata):
```

### Comparing `pharmpy-core-0.98.2/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.99.0/tests/tools/test_summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/tools/test_wrap.py` & `pharmpy-core-0.99.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/workflows/test_call.py` & `pharmpy-core-0.99.0/tests/workflows/test_call.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from uuid import uuid4
 
 import pytest
 
 import pharmpy.workflows.dispatchers
 from pharmpy.config import ConfigurationContext
 from pharmpy.internals.fs.cwd import chdir
-from pharmpy.workflows import Task, Workflow, call_workflow, execute_workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder, call_workflow, execute_workflow
 
 
 def ignore_scratch_warning():
     warnings.filterwarnings(
         "ignore",
         message=".*creating scratch directories is taking a surprisingly long time",
         category=UserWarning,
     )
 
 
 def sub(a, b):
     t1 = Task('t1', lambda: a)
     t2 = Task('t2', lambda: b)
     t3 = Task('t3', lambda x, y: x + y)
-    wf = Workflow([t1, t2])
-    wf.add_task(t3, predecessors=[t1, t2])
-    return wf
+    wb = WorkflowBuilder(tasks=[t1, t2])
+    wb.add_task(t3, predecessors=[t1, t2])
+    return Workflow(wb)
 
 
 @pytest.mark.xdist_group(name="workflow")
 def f(context, a, b):
     wf = sub(a, b)
     name = uuid4()
     with warnings.catch_warnings():
@@ -36,17 +36,17 @@
     return res
 
 
 def add(a, b):
     t1 = Task('t1', lambda: a)
     t2 = Task('t2', lambda: b)
     t3 = Task('t3', f)
-    wf = Workflow([t1, t2], name='add')
-    wf.add_task(t3, predecessors=[t1, t2])
-    return wf
+    wb = WorkflowBuilder(tasks=[t1, t2], name='add')
+    wb.add_task(t3, predecessors=[t1, t2])
+    return Workflow(wb)
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_call_workflow_threaded(tmp_path):
     a, b = 1, 2
     wf = add(a, b)
```

### Comparing `pharmpy-core-0.98.2/tests/workflows/test_execute.py` & `pharmpy-core-0.99.0/tests/workflows/test_execute.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 import pytest
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Results
 from pharmpy.modeling import set_bolus_absorption
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import read_results
-from pharmpy.workflows import Task, ToolDatabase, Workflow, execute_workflow, local_dask
+from pharmpy.workflows import (
+    Task,
+    ToolDatabase,
+    Workflow,
+    WorkflowBuilder,
+    execute_workflow,
+    local_dask,
+)
 
 # All workflow tests are run by the same xdist test worker
 # This is to limit the number of sporadic failures on GHA on Windows
 # The failures seem like races in dask distributed because the tmp-dir takes to long to create
 # on C: (main drive is D:).
 
 
@@ -25,15 +32,16 @@
     )
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_constant(tmp_path):
     a = lambda: 1  # noqa E731
     t1 = Task('t1', a)
-    wf = Workflow([t1], name='test-workflow')
+    wb = WorkflowBuilder(tasks=[t1], name='test-workflow')
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res == a()
@@ -41,16 +49,17 @@
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_unary(tmp_path):
     a = lambda: 2  # noqa E731
     f = lambda x: x**2  # noqa E731
     t1 = Task('t1', a)
     t2 = Task('t2', f)
-    wf = Workflow([t1], name='test-workflow')
-    wf.add_task(t2, predecessors=[t1])
+    wb = WorkflowBuilder(tasks=[t1], name='test-workflow')
+    wb.add_task(t2, predecessors=[t1])
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res == f(a())
@@ -60,16 +69,17 @@
 def test_execute_workflow_binary(tmp_path):
     a = lambda: 1  # noqa E731
     b = lambda: 2  # noqa E731
     f = lambda x, y: x + y  # noqa E731
     t1 = Task('t1', a)
     t2 = Task('t2', b)
     t3 = Task('t3', f)
-    wf = Workflow([t1, t2], name='test-workflow')
-    wf.add_task(t3, predecessors=[t1, t2])
+    wb = WorkflowBuilder(tasks=[t1, t2], name='test-workflow')
+    wb.add_task(t3, predecessors=[t1, t2])
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res == f(a(), b())
@@ -78,17 +88,18 @@
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_map_reduce(tmp_path):
     n = 10
     f = lambda x: x**2  # noqa E731
     layer_init = list(map(lambda i: Task(f'x{i}', lambda: i), range(n)))
     layer_map = list(map(lambda i: Task(f'f(x{i})', f), range(n)))
     layer_reduce = [Task('reduce', lambda *y: sum(y))]
-    wf = Workflow(layer_init, name='test-workflow')
-    wf.insert_workflow(Workflow(layer_map))
-    wf.insert_workflow(Workflow(layer_reduce))
+    wb = WorkflowBuilder(tasks=layer_init, name='test-workflow')
+    wb.insert_workflow(WorkflowBuilder(tasks=layer_map))
+    wb.insert_workflow(WorkflowBuilder(tasks=layer_reduce))
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res == sum(map(f, range(n)))
@@ -99,17 +110,18 @@
     model1 = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan1.mod')
     model2 = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan2.mod')
     advan1_before = model1.model_code
 
     t1 = Task('init', lambda x: x, model2)
     t2 = Task('update', set_bolus_absorption)
     t3 = Task('postprocess', lambda x: x)
-    wf = Workflow([t1], name='test-workflow')
-    wf.insert_workflow(Workflow([t2]))
-    wf.insert_workflow(Workflow([t3]))
+    wb = WorkflowBuilder(tasks=[t1], name='test-workflow')
+    wb.insert_workflow(WorkflowBuilder(tasks=[t2]))
+    wb.insert_workflow(WorkflowBuilder(tasks=[t3]))
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res.model_code == advan1_before
@@ -126,18 +138,19 @@
 
     def fit(ofv, m):
         m = m.replace(modelfit_results=ModelfitResults(ofv=ofv))
         return m
 
     init = map(lambda i: Task(f'init_{i}', lambda x: x, models[i]), indices)
     process = map(lambda i: Task(f'fit{i}', fit, ofvs[i]), indices)
-    wf = Workflow(init, name='test-workflow')
-    wf.insert_workflow(Workflow(process))
+    wb = WorkflowBuilder(tasks=init, name='test-workflow')
+    wb.insert_workflow(WorkflowBuilder(tasks=process))
     gather = Task('gather', lambda *x: x)
-    wf.insert_workflow(Workflow([gather]))
+    wb.insert_workflow(WorkflowBuilder(tasks=[gather]))
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             execute_workflow(wf)
 
     # FIXME: These cannot be updated in place
@@ -148,15 +161,16 @@
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_results(tmp_path):
     ofv = 3
     mfr = ModelfitResults(ofv=ofv)
 
-    wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
+    wb = WorkflowBuilder(tasks=[Task('result', lambda: mfr)], name='test-workflow')
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
 
     assert res.ofv == ofv
@@ -170,38 +184,41 @@
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_results_with_tool_database(tmp_path):
     ofv = 3
     mfr = MyResults(ofv=ofv)
 
-    wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
+    wb = WorkflowBuilder(tasks=[Task('result', lambda: mfr)], name='test-workflow')
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
         assert res.tool_database is not None
 
     assert res.ofv == ofv
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_execute_workflow_results_with_report(testdata, tmp_path):
     mfr = replace(read_results(testdata / 'frem' / 'results.json'), tool_database=None)
 
-    wf = Workflow([Task('result', lambda: mfr)], name='test-workflow')
+    wb = WorkflowBuilder(tasks=[Task('result', lambda: mfr)], name='test-workflow')
+    wf = Workflow(wb)
 
     with chdir(tmp_path):
         with warnings.catch_warnings():
             ignore_scratch_warning()
             res = execute_workflow(wf)
         html = res.tool_database.path / 'results.html'
         assert html.is_file()
         assert html.stat().st_size > 500000
 
 
 @pytest.mark.xdist_group(name="workflow")
 def test_local_dispatcher():
-    wf = Workflow([Task('results', lambda x: x, 'input')])
+    wb = WorkflowBuilder(tasks=[Task('results', lambda x: x, 'input')])
+    wf = Workflow(wb)
     res = local_dask.run(wf)
     assert res == 'input'
```

### Comparing `pharmpy-core-0.98.2/tests/workflows/test_model_database.py` & `pharmpy-core-0.99.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.98.2/tests/workflows/test_workflow.py` & `pharmpy-core-0.99.0/tests/workflows/test_workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,155 @@
 import re
 
 import pytest
 
-from pharmpy.workflows import Task, Workflow
+from pharmpy.workflows import Task, Workflow, WorkflowBuilder
 
 
 @pytest.fixture
 def tasks():
     t1 = Task('t1', 'func', 'input')
     t2 = Task('t2', 'func', t1)
     t3 = Task('t3', 'func', t1)
     t4 = Task('t4', 'func', [t2, t3])
     return t1, t2, t3, t4
 
 
 def test_add_tasks(tasks):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     t1, t2, t3, _ = tasks
 
-    wf.add_task(t1)
-    assert len(wf) == 1
+    wb.add_task(t1)
+    assert len(wb) == 1
 
-    wf.add_task(t2)
-    wf.add_task(t3)
-    assert len(wf) == 3
+    wb.add_task(t2)
+    wb.add_task(t3)
+    assert len(wb) == 3
 
 
 def test_add_tasks_workflow(tasks):
     t1, t2, t3, _ = tasks
 
-    wf_sequential = Workflow([t1])
-    wf_sequential.add_task(t2, predecessors=t1)
-    wf_sequential.add_task(t3, predecessors=t1)
-    assert list(wf_sequential.get_successors(t1)) == [t2, t3]
+    wb_sequential = WorkflowBuilder(tasks=[t1])
+    wb_sequential.add_task(t2, predecessors=t1)
+    wb_sequential.add_task(t3, predecessors=t1)
+    assert list(Workflow(wb_sequential).get_successors(t1)) == [t2, t3]
 
     t4 = Task('t4', 'func', 'input')
-    wf_t4 = Workflow([t4])
+    wb_t4 = WorkflowBuilder(tasks=[t4])
 
-    wf_sequential.insert_workflow(wf_t4)
-    assert list(wf_sequential.get_predecessors(t4)) == [t2, t3]
-    assert len(wf_sequential) == 4
-
-    wf_parallel = Workflow([t1])
-    wf_parallel.add_task(t2, predecessors=t1)
-    wf_parallel.add_task(t3, predecessors=t1)
-    wf_parallel.insert_workflow(wf_t4, predecessors=[])
-    assert not list(wf_parallel.get_predecessors(t4))
-    assert len(wf_parallel) == 4
+    wb_sequential.insert_workflow(wb_t4)
+    assert list(Workflow(wb_sequential).get_predecessors(t4)) == [t2, t3]
+    assert len(wb_sequential) == 4
+
+    wb_parallel = WorkflowBuilder(tasks=[t1])
+    wb_parallel.add_task(t2, predecessors=t1)
+    wb_parallel.add_task(t3, predecessors=t1)
+    wb_parallel.insert_workflow(Workflow(wb_t4), predecessors=[])
+    assert not list(Workflow(wb_parallel).get_predecessors(t4))
+    assert len(wb_parallel) == 4
 
 
 def test_get_output(tasks):
     t1, t2, t3, t4 = tasks
-    wf = Workflow([t1])
-    wf.add_task(t2, predecessors=t1)
-    wf.add_task(t3, predecessors=t1)
+    wb = WorkflowBuilder(tasks=[t1])
+    wb.add_task(t2, predecessors=t1)
+    wb.add_task(t3, predecessors=t1)
 
-    assert wf.output_tasks == [t2, t3]
+    assert Workflow(wb).output_tasks == [t2, t3]
 
-    wf.add_task(t4, predecessors=[t2, t3])
+    wb.add_task(t4, predecessors=[t2, t3])
 
-    assert wf.output_tasks == [t4]
+    assert Workflow(wb).output_tasks == [t4]
 
 
 def test_as_dask_dict(tasks):
-    wf = Workflow()
+    wb = WorkflowBuilder()
 
     t1, t2, t3, t4 = tasks
 
-    wf.add_task(t1)
-    wf.add_task(t2, predecessors=t1)
-    wf.add_task(t3, predecessors=t1)
-    wf.add_task(t4, predecessors=[t2, t3])
+    wb.add_task(t1)
+    wb.add_task(t2, predecessors=t1)
+    wb.add_task(t3, predecessors=t1)
+    wb.add_task(t4, predecessors=[t2, t3])
 
-    wf_dict = wf.as_dask_dict()
+    wf_dict = Workflow(wb).as_dask_dict()
     assert re.match(
         r"\{'.*': \('func', 'input'\), '.*': \('func', t1, '.*'\), '.*': \('func', t1, '.*'\), 'results': \('func', \[t2, t3\], '.*', '.*'\)\}",  # noqa
         str(wf_dict),
     )
 
 
 def test_as_dask_dict_raises(tasks):
-    wf = Workflow(tasks)
+    wb = WorkflowBuilder(tasks=tasks)
 
     with pytest.raises(ValueError, match='.*one output task.*'):
-        wf.as_dask_dict()
+        Workflow(wb).as_dask_dict()
 
 
 def test_insert_workflow(tasks):
     t1, t2, t3, t4 = tasks
 
-    wf = Workflow([t1])
-    wf.insert_workflow(Workflow([t2, t3]))
-    wf.insert_workflow(Workflow([t4]))
+    wb = WorkflowBuilder(tasks=[t1])
+    wb.insert_workflow(WorkflowBuilder(tasks=[t2, t3]))
+    wb.insert_workflow(WorkflowBuilder(tasks=[t4]))
 
-    assert set(wf.input_tasks) == {t1}
-    assert set(wf.output_tasks) == {t4}
+    assert set(wb.input_tasks) == {t1}
+    assert set(wb.output_tasks) == {t4}
 
 
 def test_insert_workflow_with_single_predecessors(tasks):
     t1, t2, t3, t4 = tasks
 
-    wf = Workflow([t1])
-    wf.insert_workflow(Workflow([t2, t3]), predecessors=t1)
-    wf.insert_workflow(Workflow([t4]), predecessors=t2)
+    wb = WorkflowBuilder(tasks=[t1])
+    wb.insert_workflow(WorkflowBuilder(tasks=[t2, t3]), predecessors=t1)
+    wb.insert_workflow(WorkflowBuilder(tasks=[t4]), predecessors=t2)
 
-    assert set(wf.input_tasks) == {t1}
-    assert set(wf.output_tasks) == {t3, t4}
+    assert set(wb.input_tasks) == {t1}
+    assert set(wb.output_tasks) == {t3, t4}
 
 
 def test_insert_workflow_with_predecessors(tasks):
     t1, t2, t3, t4 = tasks
 
-    wf = Workflow([t1])
-    wf.insert_workflow(Workflow([t2, t3]), predecessors=[t1])
-    wf.insert_workflow(Workflow([t4]), predecessors=[t2, t3])
+    wb = WorkflowBuilder(tasks=[t1])
+    wb.insert_workflow(WorkflowBuilder(tasks=[t2, t3]), predecessors=[t1])
+    wb.insert_workflow(WorkflowBuilder(tasks=[t4]), predecessors=[t2, t3])
 
-    assert set(wf.input_tasks) == {t1}
-    assert set(wf.output_tasks) == {t4}
+    assert set(wb.input_tasks) == {t1}
+    assert set(wb.output_tasks) == {t4}
 
 
 def test_insert_workflow_nm():
     t1, t2, t3, t4, t5 = map(lambda i: Task(f't{i}', lambda: 0), range(5))
-    wf1 = Workflow([t1, t2])
-    wf2 = Workflow([t3, t4, t5])
+    wb1 = WorkflowBuilder(tasks=[t1, t2])
+    wb2 = WorkflowBuilder(tasks=[t3, t4, t5])
     with pytest.raises(ValueError, match='.*not supported.*'):
-        wf1.insert_workflow(wf2)
+        wb1.insert_workflow(wb2)
 
 
 def test_get_upstream_tasks():
     t1, t2, t3, t4, t5 = map(lambda i: Task(f't{i}', lambda: 0), range(5))
-    wf = Workflow([t1, t2])
-    wf.insert_workflow(Workflow([t3]))
-    wf.insert_workflow(Workflow([t4, t5]))
+    wb = WorkflowBuilder(tasks=[t1, t2])
+    wb.insert_workflow(WorkflowBuilder(tasks=[t3]))
+    wb.insert_workflow(WorkflowBuilder(tasks=[t4, t5]))
 
+    wf = Workflow(wb)
     assert set(wf.get_upstream_tasks(t4)) == set(wf.get_upstream_tasks(t5)) == {t1, t2, t3}
     assert set(wf.get_upstream_tasks(t1)) == set(wf.get_upstream_tasks(t2)) == set()
     assert set(wf.get_upstream_tasks(t3)) == {t1, t2}
 
 
-def test_copy(tasks):
-    t1, t2, t3, t4 = tasks
-    wf = Workflow([t1, t2, t3, t4])
-    wf2 = wf.copy()
-    assert len(wf) == len(wf2)
-    assert str(wf) == str(wf2)
-
-
 def test_add(tasks):
     t1, t2, t3, t4 = tasks
-    wf1 = Workflow([t1])
-    wf1.add_task(t2, predecessors=t1)
-    wf2 = Workflow([t3])
-    wf2.add_task(t4, predecessors=t3)
+    wb1 = WorkflowBuilder(tasks=[t1])
+    wb1.add_task(t2, predecessors=t1)
+    wb2 = WorkflowBuilder(tasks=[t3])
+    wb2.add_task(t4, predecessors=t3)
 
-    wf = wf1 + wf2
+    wb = wb1 + wb2
 
+    wf = Workflow(wb)
     assert len(wf.tasks) == 4
     assert len(wf.input_tasks) == 2
     assert len(wf.output_tasks) == 2
```

### Comparing `pharmpy-core-0.98.2/tox.ini` & `pharmpy-core-0.99.0/tox.ini`

 * *Files identical despite different names*

