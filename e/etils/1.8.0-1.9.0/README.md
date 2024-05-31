# Comparing `tmp/etils-1.8.0.tar.gz` & `tmp/etils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etils-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "etils-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `etils-1.8.0.tar` & `etils-1.9.0.tar`

### file list

```diff
@@ -1,91 +1,94 @@
--rw-r--r--   0        0        0    11357 2024-03-19 15:36:17.706324 etils-1.8.0/LICENSE
--rw-r--r--   0        0        0     2167 2024-03-19 15:36:17.706324 etils-1.8.0/README.md
--rw-r--r--   0        0        0      859 2024-03-19 15:36:17.710324 etils-1.8.0/etils/__init__.py
--rw-r--r--   0        0        0     1412 2024-03-19 15:36:17.710324 etils-1.8.0/etils/array_types/__init__.py
--rw-r--r--   0        0        0      720 2024-03-19 15:36:17.710324 etils-1.8.0/etils/eapp/__init__.py
--rw-r--r--   0        0        0     2743 2024-03-19 15:36:17.710324 etils-1.8.0/etils/eapp/dataclass_flags.py
--rw-r--r--   0        0        0     3770 2024-03-19 15:36:17.710324 etils-1.8.0/etils/eapp/logging_utils.py
--rw-r--r--   0        0        0     1484 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/__init__.py
--rw-r--r--   0        0        0     1848 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/adhoc_error.py
--rw-r--r--   0        0        0     3041 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/adhoc_lib/module_deps_utils.py
--rw-r--r--   0        0        0     8516 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/adhoc_lib/reload_workspace_lib.py
--rw-r--r--   0        0        0     6551 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/array_as_img.py
--rw-r--r--   0        0        0    14241 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/auto_display_utils.py
--rw-r--r--   0        0        0     5846 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/cell_autoreload.py
--rw-r--r--   0        0        0     5491 2024-03-19 15:36:17.710324 etils-1.8.0/etils/ecolab/colab_utils.py
--rw-r--r--   0        0        0     1569 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/highlight_util.py
--rw-r--r--   0        0        0    11522 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inplace_reload.py
--rw-r--r--   0        0        0      583 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/__init__.py
--rw-r--r--   0        0        0     1500 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/attrs.py
--rw-r--r--   0        0        0     2354 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/auto_utils.py
--rw-r--r--   0        0        0     2050 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/core.py
--rw-r--r--   0        0        0     2047 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/html_helper.py
--rw-r--r--   0        0        0    14853 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/nodes.py
--rw-r--r--   0        0        0     1540 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/resource_utils.py
--rw-r--r--   0        0        0      191 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/static/auto_activate.css
--rw-r--r--   0        0        0     1500 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/static/auto_activate.js
--rw-r--r--   0        0        0     2487 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/static/main.js
--rw-r--r--   0        0        0     2557 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/inspects/static/theme.css
--rw-r--r--   0        0        0     1713 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/ip_utils.py
--rw-r--r--   0        0        0     5676 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/lazy_imports.py
--rw-r--r--   0        0        0    11309 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/lazy_utils.py
--rw-r--r--   0        0        0     1459 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/mock_colab.py
--rw-r--r--   0        0        0     2441 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/patch_utils.py
--rw-r--r--   0        0        0      756 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/pyjs_com/__init__.py
--rw-r--r--   0        0        0     3031 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/pyjs_com/py_js_com.js
--rw-r--r--   0        0        0     4460 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/pyjs_com/py_js_com.py
--rw-r--r--   0        0        0     1074 2024-03-19 15:36:17.714324 etils-1.8.0/etils/ecolab/static/highlight.css
--rw-r--r--   0        0        0      872 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/__init__.py
--rw-r--r--   0        0        0     1678 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/cast_utils.py
--rw-r--r--   0        0        0     2621 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/context.py
--rw-r--r--   0        0        0     8036 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/dataclass_utils.py
--rw-r--r--   0        0        0     5668 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/field_utils.py
--rw-r--r--   0        0        0     8178 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/frozen_utils.py
--rw-r--r--   0        0        0     5001 2024-03-19 15:36:17.714324 etils-1.8.0/etils/edc/helpers.py
--rw-r--r--   0        0        0     1919 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/__init__.py
--rw-r--r--   0        0        0     5435 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/array_spec.py
--rw-r--r--   0        0        0      603 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/array_types/__init__.py
--rw-r--r--   0        0        0     7867 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/array_types/dtypes.py
--rw-r--r--   0        0        0     3725 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/array_types/typing.py
--rw-r--r--   0        0        0     9794 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/checking.py
--rw-r--r--   0        0        0     4233 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/compat.py
--rw-r--r--   0        0        0     2726 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/geo_utils.py
--rw-r--r--   0        0        0     4128 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/interp_utils.py
--rw-r--r--   0        0        0     1034 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/linalg.py
--rw-r--r--   0        0        0    10941 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/numpy_utils.py
--rw-r--r--   0        0        0     2804 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/testing.py
--rw-r--r--   0        0        0     2086 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/type_parsing.py
--rw-r--r--   0        0        0     2063 2024-03-19 15:36:17.718325 etils-1.8.0/etils/enp/typing.py
--rw-r--r--   0        0        0     1033 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/__init__.py
--rw-r--r--   0        0        0     6736 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/abstract_path.py
--rw-r--r--   0        0        0    18337 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/backend.py
--rw-r--r--   0        0        0     3159 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/flags.py
--rw-r--r--   0        0        0    10227 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/gpath.py
--rw-r--r--   0        0        0     3550 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/register.py
--rw-r--r--   0        0        0     5341 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/resource_utils.py
--rw-r--r--   0        0        0     1142 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/stat_utils.py
--rw-r--r--   0        0        0     5471 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/testing.py
--rw-r--r--   0        0        0      940 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epath/typing.py
--rw-r--r--   0        0        0     1919 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/__init__.py
--rw-r--r--   0        0        0     1860 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/_internal.py
--rw-r--r--   0        0        0     2157 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/adhoc_utils/binary_import.py
--rw-r--r--   0        0        0     4505 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/adhoc_utils/module_utils.py
--rw-r--r--   0        0        0     1907 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/adhoc_utils/utils.py
--rw-r--r--   0        0        0     2173 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/contextlib.py
--rw-r--r--   0        0        0     1070 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/env_utils.py
--rw-r--r--   0        0        0     3777 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/itertools.py
--rw-r--r--   0        0        0     6615 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/lazy_imports_utils.py
--rw-r--r--   0        0        0     5290 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/py_utils.py
--rw-r--r--   0        0        0     1381 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/re_utils.py
--rw-r--r--   0        0        0     4859 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/reraise_utils.py
--rw-r--r--   0        0        0     2843 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/testing.py
--rw-r--r--   0        0        0     9666 2024-03-19 15:36:17.718325 etils-1.8.0/etils/epy/text_utils.py
--rw-r--r--   0        0        0      642 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etqdm/__init__.py
--rw-r--r--   0        0        0     1454 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etqdm/tqdm_utils.py
--rw-r--r--   0        0        0     1195 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etree/__init__.py
--rw-r--r--   0        0        0     9735 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etree/backend.py
--rw-r--r--   0        0        0     5329 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etree/tree_utils.py
--rw-r--r--   0        0        0      961 2024-03-19 15:36:17.718325 etils-1.8.0/etils/etree/typing.py
--rw-r--r--   0        0        0      965 2024-03-19 15:36:17.718325 etils-1.8.0/etils/lazy_imports/__init__.py
--rw-r--r--   0        0        0     3310 2024-03-19 15:36:17.718325 etils-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     6383 1970-01-01 00:00:00.000000 etils-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 14:30:52.832723 etils-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2167 2024-05-31 14:30:52.832723 etils-1.9.0/README.md
+-rw-r--r--   0        0        0      859 2024-05-31 14:30:52.832723 etils-1.9.0/etils/__init__.py
+-rw-r--r--   0        0        0     1412 2024-05-31 14:30:52.832723 etils-1.9.0/etils/array_types/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-31 14:30:52.832723 etils-1.9.0/etils/eapp/__init__.py
+-rw-r--r--   0        0        0     2743 2024-05-31 14:30:52.832723 etils-1.9.0/etils/eapp/dataclass_flags.py
+-rw-r--r--   0        0        0     3770 2024-05-31 14:30:52.832723 etils-1.9.0/etils/eapp/logging_utils.py
+-rw-r--r--   0        0        0     1535 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/__init__.py
+-rw-r--r--   0        0        0     1848 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/adhoc_error.py
+-rw-r--r--   0        0        0     3041 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/adhoc_lib/module_deps_utils.py
+-rw-r--r--   0        0        0    10051 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/adhoc_lib/reload_workspace_lib.py
+-rw-r--r--   0        0        0     6551 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/array_as_img.py
+-rw-r--r--   0        0        0    14241 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/auto_display_utils.py
+-rw-r--r--   0        0        0     5846 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/cell_autoreload.py
+-rw-r--r--   0        0        0     6502 2024-05-31 14:30:52.832723 etils-1.9.0/etils/ecolab/colab_utils.py
+-rw-r--r--   0        0        0     1569 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/highlight_util.py
+-rw-r--r--   0        0        0    11522 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inplace_reload.py
+-rw-r--r--   0        0        0      583 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/__init__.py
+-rw-r--r--   0        0        0     1500 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/attrs.py
+-rw-r--r--   0        0        0     2354 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/auto_utils.py
+-rw-r--r--   0        0        0     2050 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/core.py
+-rw-r--r--   0        0        0     2047 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/html_helper.py
+-rw-r--r--   0        0        0    14853 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/nodes.py
+-rw-r--r--   0        0        0     1536 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/resource_utils.py
+-rw-r--r--   0        0        0      191 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/static/auto_activate.css
+-rw-r--r--   0        0        0     1500 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/static/auto_activate.js
+-rw-r--r--   0        0        0     2487 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/static/main.js
+-rw-r--r--   0        0        0     2557 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/inspects/static/theme.css
+-rw-r--r--   0        0        0     1713 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/ip_utils.py
+-rw-r--r--   0        0        0     5696 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/lazy_imports.py
+-rw-r--r--   0        0        0    11309 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/lazy_utils.py
+-rw-r--r--   0        0        0     1459 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/mock_colab.py
+-rw-r--r--   0        0        0     2441 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/patch_utils.py
+-rw-r--r--   0        0        0      756 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/pyjs_com/__init__.py
+-rw-r--r--   0        0        0     3031 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/pyjs_com/py_js_com.js
+-rw-r--r--   0        0        0     4460 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/pyjs_com/py_js_com.py
+-rw-r--r--   0        0        0     1074 2024-05-31 14:30:52.840723 etils-1.9.0/etils/ecolab/static/highlight.css
+-rw-r--r--   0        0        0      872 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/__init__.py
+-rw-r--r--   0        0        0     1678 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/cast_utils.py
+-rw-r--r--   0        0        0     2621 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/context.py
+-rw-r--r--   0        0        0     8036 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/dataclass_utils.py
+-rw-r--r--   0        0        0     5668 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/field_utils.py
+-rw-r--r--   0        0        0     8178 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/frozen_utils.py
+-rw-r--r--   0        0        0     5001 2024-05-31 14:30:52.840723 etils-1.9.0/etils/edc/helpers.py
+-rw-r--r--   0        0        0     1919 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/__init__.py
+-rw-r--r--   0        0        0     5435 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/array_spec.py
+-rw-r--r--   0        0        0      603 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/array_types/__init__.py
+-rw-r--r--   0        0        0     7867 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/array_types/dtypes.py
+-rw-r--r--   0        0        0     3725 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/array_types/typing.py
+-rw-r--r--   0        0        0     9794 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/checking.py
+-rw-r--r--   0        0        0     4289 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/compat.py
+-rw-r--r--   0        0        0     2726 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/geo_utils.py
+-rw-r--r--   0        0        0     4128 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/interp_utils.py
+-rw-r--r--   0        0        0     1034 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/linalg.py
+-rw-r--r--   0        0        0    10941 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/numpy_utils.py
+-rw-r--r--   0        0        0     2804 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/testing.py
+-rw-r--r--   0        0        0     2086 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/type_parsing.py
+-rw-r--r--   0        0        0     2063 2024-05-31 14:30:52.840723 etils-1.9.0/etils/enp/typing.py
+-rw-r--r--   0        0        0     1033 2024-05-31 14:30:52.840723 etils-1.9.0/etils/epath/__init__.py
+-rw-r--r--   0        0        0     6736 2024-05-31 14:30:52.840723 etils-1.9.0/etils/epath/abstract_path.py
+-rw-r--r--   0        0        0    18339 2024-05-31 14:30:52.840723 etils-1.9.0/etils/epath/backend.py
+-rw-r--r--   0        0        0     3159 2024-05-31 14:30:52.840723 etils-1.9.0/etils/epath/flags.py
+-rw-r--r--   0        0        0    10576 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/gpath.py
+-rw-r--r--   0        0        0     3550 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/register.py
+-rw-r--r--   0        0        0     5675 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/resource_utils.py
+-rw-r--r--   0        0        0     1142 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/stat_utils.py
+-rw-r--r--   0        0        0     5471 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/testing.py
+-rw-r--r--   0        0        0      940 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epath/typing.py
+-rw-r--r--   0        0        0     1981 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/__init__.py
+-rw-r--r--   0        0        0     1860 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/_internal.py
+-rw-r--r--   0        0        0      583 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/adhoc_utils/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/adhoc_utils/binary_import.py
+-rw-r--r--   0        0        0     2373 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/adhoc_utils/curr_args.py
+-rw-r--r--   0        0        0     4826 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/adhoc_utils/module_utils.py
+-rw-r--r--   0        0        0     1907 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/adhoc_utils/utils.py
+-rw-r--r--   0        0        0     2173 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/contextlib.py
+-rw-r--r--   0        0        0     1070 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/env_utils.py
+-rw-r--r--   0        0        0     3777 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/itertools.py
+-rw-r--r--   0        0        0     4272 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/lazy_api_imports_utils.py
+-rw-r--r--   0        0        0     7219 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/lazy_imports_utils.py
+-rw-r--r--   0        0        0     5290 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/py_utils.py
+-rw-r--r--   0        0        0     1381 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/re_utils.py
+-rw-r--r--   0        0        0     4859 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/reraise_utils.py
+-rw-r--r--   0        0        0     2843 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/testing.py
+-rw-r--r--   0        0        0     9666 2024-05-31 14:30:52.844724 etils-1.9.0/etils/epy/text_utils.py
+-rw-r--r--   0        0        0      642 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etqdm/__init__.py
+-rw-r--r--   0        0        0     1454 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etqdm/tqdm_utils.py
+-rw-r--r--   0        0        0     1195 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etree/__init__.py
+-rw-r--r--   0        0        0     9735 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etree/backend.py
+-rw-r--r--   0        0        0     5329 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etree/tree_utils.py
+-rw-r--r--   0        0        0      961 2024-05-31 14:30:52.844724 etils-1.9.0/etils/etree/typing.py
+-rw-r--r--   0        0        0      965 2024-05-31 14:30:52.844724 etils-1.9.0/etils/lazy_imports/__init__.py
+-rw-r--r--   0        0        0     3310 2024-05-31 14:30:52.844724 etils-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6383 1970-01-01 00:00:00.000000 etils-1.9.0/PKG-INFO
```

### Comparing `etils-1.8.0/LICENSE` & `etils-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/README.md` & `etils-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/__init__.py` & `etils-1.9.0/etils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Etils API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 # Do NOT add anything to this file. This is left empty on purpose.
 # Users should import subprojects directly.
```

### Comparing `etils-1.8.0/etils/array_types/__init__.py` & `etils-1.9.0/etils/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/eapp/__init__.py` & `etils-1.9.0/etils/eapp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/eapp/dataclass_flags.py` & `etils-1.9.0/etils/eapp/dataclass_flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/eapp/logging_utils.py` & `etils-1.9.0/etils/eapp/logging_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/__init__.py` & `etils-1.9.0/etils/ecolab/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # pylint: disable=g-importing-member
 
 from etils.ecolab.array_as_img import auto_plot_array
 from etils.ecolab.auto_display_utils import auto_display
 from etils.ecolab.auto_display_utils import disp
 from etils.ecolab.colab_utils import collapse
+from etils.ecolab.colab_utils import get_permalink
 from etils.ecolab.colab_utils import interruptible
 from etils.ecolab.colab_utils import json
 from etils.ecolab.highlight_util import highlight_html
 from etils.ecolab.inplace_reload import ReloadMode
 from etils.ecolab.inspects.auto_utils import auto_inspect
 from etils.ecolab.inspects.core import inspect
 from etils.ecolab.patch_utils import patch_graphviz
```

### Comparing `etils-1.8.0/etils/ecolab/adhoc_error.py` & `etils-1.9.0/etils/ecolab/adhoc_error.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/adhoc_lib/module_deps_utils.py` & `etils-1.9.0/etils/ecolab/adhoc_lib/module_deps_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/adhoc_lib/reload_workspace_lib.py` & `etils-1.9.0/etils/ecolab/adhoc_lib/reload_workspace_lib.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Reload workspace util."""
 
 from __future__ import annotations
 
-from collections.abc import Iterable
-import functools
+from collections.abc import Iterable, Iterator
+import contextlib
 import importlib
 import inspect
 import re
 import sys
 import types
 import typing
 
 from etils.ecolab import inplace_reload
 from etils.ecolab.adhoc_lib import module_deps_utils
 from etils.epy import py_utils
+from etils.epy.adhoc_utils import module_utils
 import IPython
 
 
 if typing.TYPE_CHECKING:
   # Do not import here to avoid circular deps:
   # `g3_utils` uses `epy.lazy_imports` that call `get_curr_adhoc_kwargs()` from
   # `ecolab`.
@@ -74,15 +75,24 @@
 
   # TODO(epot): When loading from workspace, then from HEAD, how to detect
   # which files should be reloaded ?
   # Especially when there's 2 different `ecolab.adhoc` scope!
   # Could detect all modules that are adhoc-imported (through the
   # `module.__file__` and reload them)
   if not isinstance(citc_info, g3_utils.Workspace):
-    return
+    if prev_modules := _find_modules_imported_in_different_source(source):
+      prev_module_name = next(iter(prev_modules))
+      prev_source = sys.modules[prev_module_name]._etils_workspace_reload_source  # pylint: disable=protected-access
+      raise ValueError(
+          f'Source was changed from {prev_source!r} to {source!r}.'
+          ' `reload_workspace=True` cannot auto-infer which modules to reload.'
+          ' Please restart your kernel.'
+      )
+    else:
+      return
 
   # Step 1: List all modules to reload
   modules_to_reload = _get_modules_to_reload(
       restrict=restrict,
       citc_info=citc_info,
   )
   if not modules_to_reload:
@@ -97,15 +107,15 @@
       reload_recursive=False,
       reload_mode=reload_mode,
       verbose=verbose,
       collapse_prefix=f'Reload workspace ({len(modules_to_reload)} modules): ',
   ):
     for module_name in modules_to_reload:
       module = importlib.import_module(module_name)
-      module._etils_is_workspace_reloaded = True  # pylint: disable=protected-access
+      module._etils_workspace_reload_source = source  # pylint: disable=protected-access
 
   # Step 3: Replace the reloaded modules in the Colab kernel.
   update_global_namespace(reload=modules_to_reload, verbose=verbose)
 
 
 def _get_modules_to_reload(
     *,
@@ -135,32 +145,21 @@
 def _filter_only_imported_modules(opened_files: Iterable[str]) -> list[str]:
   """Restrict the list of files to Python modules already in sys.modules."""
   all_opened_modules = []
   for path in opened_files:
     # TODO(epot): supports proto
     if not path.endswith('.py'):
       continue
-    if _path_to_module_name(path) not in sys.modules:
+    if module_utils.path_to_module_name(path) not in sys.modules:
       continue
     all_opened_modules.append(path)
 
   return all_opened_modules
 
 
-@functools.cache
-def _path_to_module_name(path: str) -> str:
-  """Normalizes paths to module names."""
-  return (
-      path.lstrip('/')
-      .removesuffix('.py')
-      .removesuffix('/__init__')
-      .replace('/', '.')
-  )
-
-
 # Note that reloading etils will reset the cache, triggering a full reload of
 # all edited modules. This is likely the best behavior.
 # Otherwise, we could try to attach the cache to the `sys.modules` directly.
 _MODULES_EDIT_TIME = {}
 
 
 def _filter_recently_edited(
@@ -170,15 +169,15 @@
 ) -> list[str]:
   """Only keep modules that have been updated."""
   recently_edited = []
 
   for module_path in module_paths:
     # TODO(epot): could also check that `sys.modules[].__file__` matches
     # `citc_info.g3_path`, otherwise, should force reload.
-    module_name = _path_to_module_name(module_path)
+    module_name = module_utils.path_to_module_name(module_path)
     curr_time = (citc_info.g3_path.parent / module_path).stat().mtime
     prev_time = _MODULES_EDIT_TIME.get(module_name)
 
     if prev_time == curr_time:  # File already cached. No updates
       continue
     _MODULES_EDIT_TIME[module_name] = curr_time
     recently_edited.append(module_name)
@@ -224,14 +223,55 @@
 
     imported_in = _filter_restrict(module_deps.imported_in)
     modules_to_process.update(imported_in)
     affected_modules.update(imported_in)
   return affected_modules
 
 
+def _find_modules_imported_in_different_source(
+    source: g3_utils.Source,
+) -> set[str]:
+  """Extract all modules imported in a different source."""
+  sentinel = object()
+  other_previous_modules = set()
+  for module_name, module in sys.modules.items():
+    old_source = inspect.getattr_static(
+        module, '_etils_workspace_reload_source', sentinel
+    )
+    if old_source is sentinel:
+      continue
+    if old_source != source:
+      other_previous_modules.add(module_name)
+  return other_previous_modules
+
+
+@contextlib.contextmanager
+def mark_adhoc_imported_modules(
+    source: None | g3_utils.Source,
+) -> Iterator[None]:
+  """Mark modules that were adhoc imported from this context.
+
+  This allow `reload_workspace=True` to raise an error if the source change.
+
+  Args:
+    source: The source of the adhoc import
+
+  Yields:
+    None
+  """
+  old_modules = set(sys.modules)
+  try:
+    yield
+  finally:
+    adhoc_imported_modules = set(sys.modules) - old_modules
+    for module_name in adhoc_imported_modules:
+      # TODO(epot): Could check that the `source` and `.__file__` match
+      sys.modules[module_name]._etils_workspace_reload_source = source  # pylint: disable=protected-access
+
+
 def update_global_namespace(
     *,
     reload: list[str],
     verbose: bool,
 ) -> None:
   """Overwrite the imported modules in the current Colab global namespace."""
   reload = set(reload)
```

### Comparing `etils-1.8.0/etils/ecolab/array_as_img.py` & `etils-1.9.0/etils/ecolab/array_as_img.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/auto_display_utils.py` & `etils-1.9.0/etils/ecolab/auto_display_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/cell_autoreload.py` & `etils-1.9.0/etils/ecolab/cell_autoreload.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/colab_utils.py` & `etils-1.9.0/etils/ecolab/colab_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 import contextlib
 import html
 import json as json_std
 import signal
 import threading
 import typing
-from typing import Iterator, Iterable, TypeVar
+from typing import Any, Iterable, Iterator, TypeVar
+import urllib
 import uuid
 
 import IPython.display
 
 if typing.TYPE_CHECKING:
   JsonValue = str | float | int | bool | None
   Json = JsonValue | dict[JsonValue, 'Json'] | list['Json']
@@ -183,7 +184,41 @@
   try:
     for i in inner:
       yield i
       if interrupted.is_set():
         return
   finally:
     signal.signal(signal.SIGINT, previous_handler)
+
+
+def get_permalink(
+    *,
+    url: str,
+    template_params: dict[str, Any] | tuple[tuple[str, Any, Any], ...],
+) -> str:
+  """Get the permalink for the current colab.
+
+  Args:
+    url: The base URL.
+    template_params: A dict of name to value. Can also be a list of (name,
+      value, default) tuples, in which case only the value != default are added
+      (to make the url shorter).
+
+  Returns:
+    The permalink.
+  """
+
+  # TODO(epot): If url is missing, should auto-extract it from the colab URL.
+  if url.startswith('go/'):
+    url = f'http://{url}'
+
+  # Normalize the template params to a dict.
+  if not isinstance(template_params, dict):
+    template_params = {
+        name: value
+        for name, value, default in template_params
+        if value != default  # Only add params which are different from default
+    }
+
+  template_params = json_std.dumps(template_params)
+  template_params = urllib.parse.quote(template_params)
+  return f'{url}#templateParams={template_params}'
```

### Comparing `etils-1.8.0/etils/ecolab/highlight_util.py` & `etils-1.9.0/etils/ecolab/highlight_util.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inplace_reload.py` & `etils-1.9.0/etils/ecolab/inplace_reload.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/__init__.py` & `etils-1.9.0/etils/ecolab/inspects/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/attrs.py` & `etils-1.9.0/etils/ecolab/inspects/attrs.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/auto_utils.py` & `etils-1.9.0/etils/ecolab/inspects/auto_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/core.py` & `etils-1.9.0/etils/ecolab/inspects/core.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/html_helper.py` & `etils-1.9.0/etils/ecolab/inspects/html_helper.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/nodes.py` & `etils-1.9.0/etils/ecolab/inspects/nodes.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/resource_utils.py` & `etils-1.9.0/etils/ecolab/inspects/resource_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Optional
 
 from etils import epath
 
 
 def _static_path() -> epath.Path:
   """Path to the static resources (`.js`, `.css`)."""
-  return epath.resource_path('etils') / 'ecolab' / 'inspects' / 'static'
+  return epath.resource_path('etils.ecolab') / 'inspects' / 'static'
 
 
 # TODO(epot): Use gstatic to serve those files.
 # TODO(epot): Expose in public API ?
 @functools.lru_cache()
 def resource_import(
     filename: str,
```

#### html2text {}

```diff
@@ -4,16 +4,16 @@
 www.apache.org/licenses/LICENSE-2.0 # # Unless required by applicable law or
 agreed to in writing, software # distributed under the License is distributed
 on an "AS IS" BASIS, # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. # See the License for the specific language governing
 permissions and # limitations under the License. """Resource utils.""" import
 functools from typing import Optional from etils import epath def _static_path
 () -> epath.Path: """Path to the static resources (`.js`, `.css`).""" return
-epath.resource_path('etils') / 'ecolab' / 'inspects' / 'static' # TODO(epot):
-Use gstatic to serve those files. # TODO(epot): Expose in public API ?
+epath.resource_path('etils.ecolab') / 'inspects' / 'static' # TODO(epot): Use
+gstatic to serve those files. # TODO(epot): Expose in public API ?
 @functools.lru_cache() def resource_import( filename: str, *, module: Optional
 [epath.PathLike] = None, ) -> str: """Returns the `HTML` associated with the
 resource. Args: filename: Path to the `.css`, `.js` resource module: Python
 module name from which the filename is relative too. """ path =
 epath.resource_path(module) if module else _static_path() path = path.joinpath
 (filename) content = path.read_text() if path.suffix == '.css': return f'
 ' elif path.suffix == '.js': return f'
```

### Comparing `etils-1.8.0/etils/ecolab/inspects/static/auto_activate.js` & `etils-1.9.0/etils/ecolab/inspects/static/auto_activate.js`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/static/main.js` & `etils-1.9.0/etils/ecolab/inspects/static/main.js`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/inspects/static/theme.css` & `etils-1.9.0/etils/ecolab/inspects/static/theme.css`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/ip_utils.py` & `etils-1.9.0/etils/ecolab/ip_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/lazy_imports.py` & `etils-1.9.0/etils/ecolab/lazy_imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,15 +200,15 @@
   tqdm.notebook  # pylint: disable=pointless-statement
   import tree
   import typeguard
   import typing_extensions
   import plotly
   from plotly import express as px
   from plotly import graph_objects as go
-  import pydantic
+  from pydantic import v1 as pydantic
   import requests
   import sunds
   import visu3d as v3d
   from xmanager.contrib import flow as xmflow
   from xmanager import xm
   # pytype: enable=import-error
   # pylint: enable=g-import-not-at-top,unused-import,reimported
```

### Comparing `etils-1.8.0/etils/ecolab/lazy_utils.py` & `etils-1.9.0/etils/ecolab/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/mock_colab.py` & `etils-1.9.0/etils/ecolab/mock_colab.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/patch_utils.py` & `etils-1.9.0/etils/ecolab/patch_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/pyjs_com/__init__.py` & `etils-1.9.0/etils/ecolab/pyjs_com/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/pyjs_com/py_js_com.js` & `etils-1.9.0/etils/ecolab/pyjs_com/py_js_com.js`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/ecolab/pyjs_com/py_js_com.py` & `etils-1.9.0/etils/ecolab/pyjs_com/py_js_com.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,9 +163,9 @@
 
 # TODO(epot): Host on gstatic and dynamically generate the URL from the
 # local file hash.
 # Auto-detect adhoc import or add a flag to load locally modified `.js`
 @functools.lru_cache()
 def js_import() -> str:
   """`<script></script>` to import to add in the HTML."""
-  path = epath.resource_path('etils') / 'ecolab/pyjs_com/py_js_com.js'
+  path = epath.resource_path('etils.ecolab') / 'pyjs_com/py_js_com.js'
   return f'<script>{path.read_text()}</script>'
```

### Comparing `etils-1.8.0/etils/ecolab/static/highlight.css` & `etils-1.9.0/etils/ecolab/static/highlight.css`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/__init__.py` & `etils-1.9.0/etils/edc/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/cast_utils.py` & `etils-1.9.0/etils/edc/cast_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/context.py` & `etils-1.9.0/etils/edc/context.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/dataclass_utils.py` & `etils-1.9.0/etils/edc/dataclass_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
   Note:
 
   * Only the last `.frozen()` call resolve the dataclass by calling `.replace`
     recursivelly.
   * Dataclass returned by `.unfrozen()` and nested attributes are not the
     original dataclass but proxy objects which track the mutations. As such,
-    those object are not compatible with `isinstance()`, `jax.tree_map`,...
+    those object are not compatible with `isinstance()`, `jax.tree.map`,...
   * Only the top-level dataclass need to be `allow_unfrozen=True`
   * Avoid using `unfrozen` if 2 attributes of the dataclass point to the
     same nested dataclass. Updates on one attribute might not be reflected on
     the other.
 
     ```python
     y = Y(y=123)
```

### Comparing `etils-1.8.0/etils/edc/field_utils.py` & `etils-1.9.0/etils/edc/field_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/frozen_utils.py` & `etils-1.9.0/etils/edc/frozen_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/edc/helpers.py` & `etils-1.9.0/etils/edc/helpers.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/__init__.py` & `etils-1.9.0/etils/enp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/array_spec.py` & `etils-1.9.0/etils/enp/array_spec.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/array_types/__init__.py` & `etils-1.9.0/etils/enp/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/array_types/dtypes.py` & `etils-1.9.0/etils/enp/array_types/dtypes.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/array_types/typing.py` & `etils-1.9.0/etils/enp/array_types/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/checking.py` & `etils-1.9.0/etils/enp/checking.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/compat.py` & `etils-1.9.0/etils/enp/compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
     return isinstance(x, xnp.ndarray)
 
 
 def astype(x: Array['*d'], dtype) -> Array['*d']:
   """`x.astype(dtype)`."""
   if lazy.is_torch(x):
     return x.type(dtype)
+  elif lazy.is_tf(x):
+    return lazy.tf.cast(x, dtype)
   else:
     return x.astype(dtype)
 
 
 def expand_dims(x: Array['*d'], *, axis) -> Array['*d']:
   """`xnp.expand_dims(x, axis=axis)`."""
   xnp = lazy.get_xnp(x)
```

### Comparing `etils-1.8.0/etils/enp/geo_utils.py` & `etils-1.9.0/etils/enp/geo_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/interp_utils.py` & `etils-1.9.0/etils/enp/interp_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/linalg.py` & `etils-1.9.0/etils/enp/linalg.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/numpy_utils.py` & `etils-1.9.0/etils/enp/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/testing.py` & `etils-1.9.0/etils/enp/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/type_parsing.py` & `etils-1.9.0/etils/enp/type_parsing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/enp/typing.py` & `etils-1.9.0/etils/enp/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/__init__.py` & `etils-1.9.0/etils/epath/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/abstract_path.py` & `etils-1.9.0/etils/epath/abstract_path.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/backend.py` & `etils-1.9.0/etils/epath/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
       self,
       top: PathLike,
       *,
       top_down: bool = True,
       on_error: Callable[[OSError], object] | None = None,
   ) -> Iterator[tuple[PathLike, list[str], list[str]]]:
     if hasattr(pathlib.Path, 'walk'):  # Python 3.12
-      yield from pathlib.Path(top).walk(topdown=top_down, onerror=on_error)
+      yield from pathlib.Path(top).walk(top_down=top_down, on_error=on_error)
     else:  # Backward compatibility
       # Note that `os.walk` is inconsistent for `symlinks` (always marked as
       # filenames), but should be fine.
       yield from os.walk(top, topdown=top_down, onerror=on_error)
 
   def makedirs(
       self,
```

### Comparing `etils-1.8.0/etils/epath/flags.py` & `etils-1.9.0/etils/epath/flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/gpath.py` & `etils-1.9.0/etils/epath/gpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import functools
 import importlib.util
 import ntpath
 import os
 import pathlib
 import posixpath
+import sys
 import types
 import typing
 from typing import Any, Callable, ClassVar, Iterator, Optional, Type, TypeVar, Union
 
 from etils import epy
 from etils.epath import abstract_path
 from etils.epath import backend as backend_lib
@@ -40,14 +41,23 @@
 
 _URI_MAP_ROOT = {
     'gs://': '/gs/',
     's3://': '/s3/',
     'az://': '/az/',
 }
 
+
+def _epath_use_tf() -> bool:
+  return os.environ.get('EPATH_USE_TF', '').lower() not in [
+      'false',
+      'no',
+      'f',
+      '0',
+  ]
+
 _PREFIX_TO_BACKEND = {
     'gs': backend_lib.fsspec_backend,
     's3': backend_lib.fsspec_backend,
     'az': backend_lib.fsspec_backend,
     None: backend_lib.os_backend,
 }
 _GCS_BACKENDS = frozenset({
@@ -56,40 +66,32 @@
 })
 
 # Available modes (from tensorflow/python/lib/io/file_io.py;l=55)
 # Also exclude `+` as broken in gfile
 _OPEN_MODES = ('r', 'w', 'a')
 
 
-@functools.cache
-def _is_tf_installed() -> bool:
-  """Checks whether TensorFlow is installed."""
-  if os.environ.get('EPATH_USE_TF', '').lower() in ['false', 'no', 'f', '0']:
-    return False
-  return importlib.util.find_spec('tensorflow') is not None
-
-
 class _GPath(abstract_path.Path):
   """Pathlib like api with gs://, s3://, az:// support."""
 
   # `_PATH` is `posixpath` or `ntpath`.
   # Use explicit `join()` rather than `super().joinpath()` to avoid infinite
   # recursion.
   # Do not use `os.path`, so `PosixGPath('gs://abc')` works on windows.
   _PATH: ClassVar[types.ModuleType]
 
-  def __new__(cls: Type[_P], *parts: PathLike) -> _P:
-    full_path = '/'.join(os.fspath(p) for p in parts)
-    if full_path.startswith(_URI_PREFIXES):
-      prefix, _ = full_path.split('://', maxsplit=1)
-      prefix = f'{prefix}://'
-      new_prefix = _URI_MAP_ROOT[prefix]
-      return super().__new__(cls, full_path.replace(prefix, new_prefix, 1))
-    else:
-      return super().__new__(cls, *parts)
+  if sys.version_info < (3, 12):
+
+    def __new__(cls: Type[_P], *parts: PathLike) -> _P:
+      return super().__new__(cls, *_process_parts(*parts))
+
+  else:
+
+    def __init__(self, *parts: PathLike) -> None:
+      super().__init__(*_process_parts(*parts))
 
   def _new(self: _P, *parts: PathLike) -> _P:
     """Create a new `Path` child of same type."""
     return type(self)(*parts)
 
   # Could try to use `cached_property` when beam is compatible (currently
   # raise mutable input error when used with beam).
@@ -168,15 +170,15 @@
   def glob(self: _P, pattern: str) -> Iterator[_P]:
     """Yielding all matching files (of any kind)."""
     pattern = self._PATH.join(self._path_str, pattern)
 
     if '**' in pattern:
       raise NotImplementedError(
           'Recursive `**` pattern not supported as this could trigger '
-          'thoushands of RPC requests on GCS. Use `*` instead. '
+          'thousands of RPC requests on GCS. Use `*` instead. '
           f'Got: {pattern!r}'
       )
 
     for f in self._backend.glob(pattern):
       yield self._new(f)
 
   def walk(
@@ -280,14 +282,48 @@
     return dst
 
   def stat(self) -> stat_utils.StatResult:
     """Returns metadata for the file/directory."""
     return self._backend.stat(self._path_str)
 
 
+@register.register_path_cls(_URI_PREFIXES)
+class PosixGPath(_GPath):
+  """Pathlib like api with gs://, s3:// support."""
+
+  _PATH = posixpath
+
+
+@register.register_path_cls
+class WindowsGPath(pathlib.PureWindowsPath, _GPath):
+  """Pathlib like api with gs://, s3:// support."""
+
+  _PATH = ntpath
+
+
+@functools.cache
+def _is_tf_installed() -> bool:
+  """Checks whether TensorFlow is installed."""
+  if not _epath_use_tf():
+    return False
+  return importlib.util.find_spec('tensorflow') is not None
+
+
+def _process_parts(*parts: PathLike) -> tuple[PathLike, ...]:
+  """Supports the `xx://` prefix."""
+  full_path = '/'.join(os.fspath(p) for p in parts)
+  if full_path.startswith(_URI_PREFIXES):
+    prefix, _ = full_path.split('://', maxsplit=1)
+    prefix = f'{prefix}://'
+    new_prefix = _URI_MAP_ROOT[prefix]
+    return (full_path.replace(prefix, new_prefix, 1),)
+  else:
+    return parts
+
+
 def _get_backend(p0: _GPath, p1: _GPath) -> backend_lib.Backend:
   """When composing with another backend, GCS win.
 
   To allow `Path('.').replace('gs://')`
 
   Args:
     p0: Path to compare
@@ -300,21 +336,7 @@
   if p0._backend in _GCS_BACKENDS:
     return p0._backend
   elif p1._backend in _GCS_BACKENDS:
     return p1._backend
   else:
     return p0._backend
   # pylint: enable=protected-access
-
-
-@register.register_path_cls(_URI_PREFIXES)
-class PosixGPath(_GPath):
-  """Pathlib like api with gs://, s3:// support."""
-
-  _PATH = posixpath
-
-
-@register.register_path_cls
-class WindowsGPath(pathlib.PureWindowsPath, _GPath):
-  """Pathlib like api with gs://, s3:// support."""
-
-  _PATH = ntpath
```

### Comparing `etils-1.8.0/etils/epath/register.py` & `etils-1.9.0/etils/epath/register.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/resource_utils.py` & `etils-1.9.0/etils/epath/resource_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,14 +141,20 @@
     # In practice, it is trickier to do as `__fspath__` and `__str__` are
     # called internally.
     # Convert to `GPath` for consistency and compatibility with `MockFs`.
     return abstract_path.Path(path)
   elif isinstance(path, zipfile.Path):
     path = ResourcePath(path.root, path.at)
     return typing.cast(abstract_path.Path, path)
+  elif isinstance(path, importlib_resources.abc.Traversable):
+    # Is seems like `importlib_resources.files` can return additional types,
+    # like `MultiplexedPath`.
+    # Fallback to avoid failure, however those objects might not implement
+    # `__fspath__`, so might fail later.
+    return typing.cast(abstract_path.Path, path)
   else:
     raise TypeError(f'Unknown resource path: {type(path)}: {path}')
   # pylint: enable=undefined-variable
 
 
 def to_write_path(path: abstract_path.Path) -> abstract_path.Path:
   """Cast the `epath.resource_path` to a read-write Path."""
```

### Comparing `etils-1.8.0/etils/epath/stat_utils.py` & `etils-1.9.0/etils/epath/stat_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/testing.py` & `etils-1.9.0/etils/epath/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epath/typing.py` & `etils-1.9.0/etils/epath/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/__init__.py` & `etils-1.9.0/etils/epy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from etils.epy import _internal
 from etils.epy.adhoc_utils.binary_import import binary_adhoc
 from etils.epy.contextlib import ContextManager
 from etils.epy.env_utils import is_notebook
 from etils.epy.itertools import groupby
 from etils.epy.itertools import splitby
 from etils.epy.itertools import zip_dict
+from etils.epy.lazy_api_imports_utils import lazy_api_imports
 from etils.epy.lazy_imports_utils import lazy_imports
 from etils.epy.py_utils import frozen
 from etils.epy.py_utils import is_namedtuple
 from etils.epy.py_utils import issubclass_ as issubclass  # pylint: disable=redefined-builtin
 from etils.epy.py_utils import StrEnum
 from etils.epy.py_utils import wraps_cls
 from etils.epy.re_utils import reverse_fstring
```

### Comparing `etils-1.8.0/etils/epy/_internal.py` & `etils-1.9.0/etils/epy/_internal.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/adhoc_utils/binary_import.py` & `etils-1.9.0/etils/epy/adhoc_utils/binary_import.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from collections.abc import Iterator
 import contextlib
 import functools
 import sys
 from typing import Any
 
 from etils.epy import py_utils
+from etils.epy.adhoc_utils import curr_args
 from etils.epy.adhoc_utils import module_utils
 from etils.epy.adhoc_utils import utils as adhoc_utils
 
 import __main__  # pylint: disable=g-bad-import-order
 
 
 @functools.cache
```

### Comparing `etils-1.8.0/etils/epy/adhoc_utils/module_utils.py` & `etils-1.9.0/etils/epy/adhoc_utils/module_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,37 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Adhoc imports utils."""
 
 from __future__ import annotations
 
+import functools
 import sys
 import types
 import typing
 from typing import NoReturn
 
 from etils.epy import py_utils
 
 
+@functools.cache
+def path_to_module_name(path: str) -> str:
+  """Normalizes paths to module names."""
+  if '/' not in path:  # Already a module name
+    return path
+  path = path.lstrip('/')
+  return (
+      path
+      .removesuffix('.py')
+      .removesuffix('/__init__')
+      .replace('/', '.')
+  )
+
+
 def get_module_names(
     restrict: py_utils.StrOrStrList, *, recursive: bool = True
 ) -> list[str]:
   """Returns all `sys.modules` matching the restrict name."""
 
   modules = py_utils.normalize_str_to_list(restrict)
   assert all('/' not in module for module in modules)
```

### Comparing `etils-1.8.0/etils/epy/adhoc_utils/utils.py` & `etils-1.9.0/etils/epy/adhoc_utils/utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/contextlib.py` & `etils-1.9.0/etils/epy/contextlib.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/env_utils.py` & `etils-1.9.0/etils/epy/env_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/itertools.py` & `etils-1.9.0/etils/epy/itertools.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/lazy_imports_utils.py` & `etils-1.9.0/etils/epy/lazy_imports_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,66 +28,77 @@
 import dataclasses
 import functools
 import importlib
 import sys
 import types
 from typing import Any, Callable, ContextManager, Iterator
 
+from etils.epy import reraise_utils
+from etils.epy.adhoc_utils import curr_args
+
 
 _ErrorCallback = Callable[[Exception], None]
 _SuccessCallback = Callable[[str], None]
 
 
 @dataclasses.dataclass(kw_only=True)
 class LazyModule:
   """Module loaded lazily during first call."""
 
   module_name: str
   adhoc_kwargs: dict[str, Any] | None
-  error_callback: _ErrorCallback | None
+  error_callback: str | _ErrorCallback | None
   success_callback: _SuccessCallback | None
   _submodules: dict[str, LazyModule] = dataclasses.field(default_factory=dict)
 
   def __post_init__(self):
     if self.adhoc_kwargs is not None:
       self.adhoc_kwargs = dict(self.adhoc_kwargs)
       # Whe the lazy import is triggered, do not reload modules, nor trigger a
       # full build.
       self.adhoc_kwargs.pop("reload", None)
-      self.adhoc_kwargs.pop("cell_autoreload", None)
       self.adhoc_kwargs.pop("build_targets", None)
+      self.adhoc_kwargs.pop("reload_workspace", None)
+      self.adhoc_kwargs.pop("cell_autoreload", None)
+      self.adhoc_kwargs.pop("restrict_reload", None)
 
   @functools.cached_property
   def _module(self) -> types.ModuleType:
     """Resolve the module."""
     # Try to import the module, eventually replaying the adhoc scope
     with self._maybe_adhoc():
       try:
         module = importlib.import_module(self.module_name)
       except ImportError as e:
         if self.error_callback is not None:
-          self.error_callback(e)
+          if isinstance(self.error_callback, str):
+            reraise_utils.reraise(e, suffix=f"\n{self.error_callback}")
+          else:
+            self.error_callback(e)
         raise
+      except AttributeError as e:
+        # If `self._module` raises an `AttributeError`, this will trigger
+        # `self.__getattr__('_module')`, triggering an infinite recursion.
+        # To avoid this, we re-raise the `AttributeError` as an `ImportError`.
+        raise ImportError(f"Error importing {self.module_name}: {e!r}") from e
     if self.success_callback is not None:
       self.success_callback(self.module_name)
     return module
 
   def _maybe_adhoc(self) -> ContextManager[None]:
     """Recreate the adhoc import context used during the original import."""
     if self.adhoc_kwargs is None or self.module_name in sys.modules:
       adhoc = contextlib.nullcontext()
     else:
-      from etils import ecolab  # pylint: disable=g-import-not-at-top  # pytype: disable=import-error
-
       # If the lazy-import is resolved from within an adhoc, keep the adhoc.
       # Is it the right thing to do ?
-      if ecolab.adhoc_imports.get_curr_adhoc_kwargs() is not None:
+      if curr_args.get_curr_adhoc_kwargs() is not None:
         adhoc = contextlib.nullcontext()
       else:
-        adhoc = ecolab.adhoc(
+        adhoc = curr_args.replay_adhoc_ctx(
             **self.adhoc_kwargs,
             collapse_prefix=f"Lazy-import {self.module_name!r}: ",
         )
 
     return adhoc
 
   def __getattr__(self, name: str) -> Any:
@@ -110,15 +121,15 @@
   module._submodules[name] = child_module  # pylint: disable=protected-access
   return child_module
 
 
 @contextlib.contextmanager
 def lazy_imports(
     *,
-    error_callback: _ErrorCallback | None = None,
+    error_callback: str | _ErrorCallback | None = None,
     success_callback: _SuccessCallback | None = None,
 ) -> Iterator[None]:
   """Context Manager which lazy loads packages.
 
   Their import is not executed immediately, but is postponed to the first
   call of one of their attributes.
 
@@ -133,20 +144,34 @@
   with epy.lazy_imports():
     import tensorflow as tf
 
   with epy.lazy_imports(success_callback=check_tf_version):
     import tensorflow as tf
   ```
 
+  When using type annotations, make sure to also use
+  `from __future__ import annotations`, otherwise the lazy-import will be
+  triggered at import time when used in typing annotations:
+
+  ```pthon
+  with epy.lazy_imports():
+    import tensorflow as tf
+
+  # !!! Resolve the lazy-import when `__future__.annotations` isn't present
+  def get_dataset() -> tf.data.Dataset:
+  ```
+
   This support `ecolab.adhoc` imports: When the lazy-import is resolved,
   the original `ecolab.adhoc` context is re-created to import the lazy module.
 
   Args:
-    error_callback: a callback to trigger when an import fails. The exception is
-      passed as an arg, so user can use `epy.reraise(e, 'Additional message')`.
+    error_callback: A additional message to append to the `ImportError` if the
+      import fails. Can also be a `Callable[[Exception], None]`. The exception
+      is passed as an arg, so user can use `epy.reraise(e, 'Additional
+      message')`.
     success_callback: a callback to trigger when an import succeeds. The
       callback is passed the name of the imported module as an arg.
 
   Yields:
     None
   """
   # Need to mock `__import__` (instead of `sys.meta_path`, as we do not want
@@ -166,40 +191,27 @@
 def _lazy_import(
     name: str,
     globals_=None,
     locals_=None,
     fromlist: tuple[str, ...] = (),
     level: int = 0,
     *,
-    error_callback: _ErrorCallback | None,
+    error_callback: str | _ErrorCallback | None,
     success_callback: _SuccessCallback | None,
 ):
   """Mock of `builtins.__import__`."""
   del globals_, locals_  # Unused
 
   if level:
     raise ValueError(f"Relative import statements not supported ({name}).")
 
-  if adhoc_imports := sys.modules.get("etils.ecolab.adhoc_imports", None):
-    adhoc_kwargs = adhoc_imports.get_curr_adhoc_kwargs()
-
-    # Lazy-imports don't trigger reload
-    if adhoc_kwargs is not None:
-      adhoc_kwargs.pop("reload", None)
-      adhoc_kwargs.pop("restrict_reload", None)
-      adhoc_kwargs.pop("build_targets", None)
-      adhoc_kwargs.pop("reload_workspace", None)
-      adhoc_kwargs.pop("cell_autoreload", None)
-  else:
-    adhoc_kwargs = None
-
   root_name, *parts = name.split(".")
   root = LazyModule(
       module_name=root_name,
-      adhoc_kwargs=adhoc_kwargs,
+      adhoc_kwargs=curr_args.get_curr_adhoc_kwargs(),
       error_callback=error_callback,
       success_callback=success_callback,
   )
 
   # Extract inner-most module
   child = root
   for name in parts:
```

### Comparing `etils-1.8.0/etils/epy/py_utils.py` & `etils-1.9.0/etils/epy/py_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/re_utils.py` & `etils-1.9.0/etils/epy/re_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/reraise_utils.py` & `etils-1.9.0/etils/epy/reraise_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/testing.py` & `etils-1.9.0/etils/epy/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/epy/text_utils.py` & `etils-1.9.0/etils/epy/text_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etqdm/__init__.py` & `etils-1.9.0/etils/etqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etqdm/tqdm_utils.py` & `etils-1.9.0/etils/etqdm/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etree/__init__.py` & `etils-1.9.0/etils/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etree/backend.py` & `etils-1.9.0/etils/etree/backend.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etree/tree_utils.py` & `etils-1.9.0/etils/etree/tree_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/etree/typing.py` & `etils-1.9.0/etils/etree/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/etils/lazy_imports/__init__.py` & `etils-1.9.0/etils/lazy_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/pyproject.toml` & `etils-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `etils-1.8.0/PKG-INFO` & `etils-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etils
-Version: 1.8.0
+Version: 1.9.0
 Summary: Collection of common python utils
 Keywords: utils,jax,tensorflow,tf,machine learning,deep learning
 Author-email: Conchylicultor <etils@google.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

