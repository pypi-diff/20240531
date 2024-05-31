# Comparing `tmp/dissect_cstruct-4.0.dev2.tar.gz` & `tmp/dissect_cstruct-4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect_cstruct-4.0.dev2.tar", last modified: Mon May 27 11:53:12 2024, max compression
+gzip compressed data, was "dissect_cstruct-4.0.dev3.tar", last modified: Fri May 31 12:01:24 2024, max compression
```

## Comparing `dissect_cstruct-4.0.dev2.tar` & `dissect_cstruct-4.0.dev3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.431345 dissect_cstruct-4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-27 11:53:12.431345 dissect_cstruct-4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.415345 dissect_cstruct-4.0.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.419345 dissect_cstruct-4.0.dev2/dissect/cstruct/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.423345 dissect_cstruct-4.0.dev2/dissect/cstruct/types/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/char.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/leb128.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23954 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/void.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/types/wchar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/dissect/cstruct/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.427345 dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-27 11:53:12.000000 dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-27 11:53:12.000000 dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:53:12.000000 dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 11:53:12.000000 dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.423345 dissect_cstruct-4.0.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/examples/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/examples/mirai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/examples/pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/examples/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/examples/secdesc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-27 11:53:07.000000 dissect_cstruct-4.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:53:12.431345 dissect_cstruct-4.0.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.427345 dissect_cstruct-4.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.427345 dissect_cstruct-4.0.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/data/testdef.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:53:12.427345 dissect_cstruct-4.0.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_bitfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_leb128.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_union.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_void.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_types_wchar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-27 11:53:00.000000 dissect_cstruct-4.0.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.150916 dissect_cstruct-4.0.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.154916 dissect_cstruct-4.0.dev3/dissect/cstruct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.158916 dissect_cstruct-4.0.dev3/dissect/cstruct/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23958 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/types/wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/dissect/cstruct/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-31 12:01:24.000000 dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-31 12:01:24.000000 dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:01:24.000000 dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 12:01:24.000000 dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.158916 dissect_cstruct-4.0.dev3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/examples/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/examples/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/examples/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/examples/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/examples/secdesc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-31 12:01:19.000000 dissect_cstruct-4.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.162916 dissect_cstruct-4.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/data/testdef.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:01:24.166916 dissect_cstruct-4.0.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_types_wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 12:01:14.000000 dissect_cstruct-4.0.dev3/tox.ini
```

### Comparing `dissect_cstruct-4.0.dev2/LICENSE` & `dissect_cstruct-4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/PKG-INFO` & `dissect_cstruct-4.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 4.0.dev2
+Version: 4.0.dev3
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect_cstruct-4.0.dev2/README.md` & `dissect_cstruct-4.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/__init__.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/bitbuffer.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/compiler.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/compiler.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/cstruct.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/cstruct.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/expression.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/expression.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/parser.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/parser.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/__init__.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/base.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/base.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/char.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/char.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/enum.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/enum.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/flag.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/flag.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/int.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/int.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/leb128.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/leb128.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/packed.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/packed.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/pointer.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/pointer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/structure.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     __align__: bool
     __anonymous__: bool
     __updating__ = False
     __compiled__ = False
 
     def __new__(metacls, name: str, bases: tuple[type, ...], classdict: dict[str, Any]) -> MetaType:
         if (fields := classdict.pop("fields", None)) is not None:
-            metacls._update_fields(metacls, fields, align=classdict.get("align", False), classdict=classdict)
+            metacls._update_fields(metacls, fields, align=classdict.get("__align__", False), classdict=classdict)
 
         return super().__new__(metacls, name, bases, classdict)
 
     def __call__(cls, *args, **kwargs) -> Structure:
         if (
             cls.__fields__
             and len(args) == len(cls.__fields__) == 1
```

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/types/wchar.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/types/wchar.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect/cstruct/utils.py` & `dissect_cstruct-4.0.dev3/dissect/cstruct/utils.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/PKG-INFO` & `dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 4.0.dev2
+Version: 4.0.dev3
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect_cstruct-4.0.dev2/dissect.cstruct.egg-info/SOURCES.txt` & `dissect_cstruct-4.0.dev3/dissect.cstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/examples/disk.py` & `dissect_cstruct-4.0.dev3/examples/disk.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/examples/mirai.py` & `dissect_cstruct-4.0.dev3/examples/mirai.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/examples/pe.py` & `dissect_cstruct-4.0.dev3/examples/pe.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/examples/protobuf.py` & `dissect_cstruct-4.0.dev3/examples/protobuf.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/examples/secdesc.py` & `dissect_cstruct-4.0.dev3/examples/secdesc.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/pyproject.toml` & `dissect_cstruct-4.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/docs/Makefile` & `dissect_cstruct-4.0.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/docs/conf.py` & `dissect_cstruct-4.0.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_align.py` & `dissect_cstruct-4.0.dev3/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_basic.py` & `dissect_cstruct-4.0.dev3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_bitbuffer.py` & `dissect_cstruct-4.0.dev3/tests/test_bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_bitfield.py` & `dissect_cstruct-4.0.dev3/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_compiler.py` & `dissect_cstruct-4.0.dev3/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_ctypes.py` & `dissect_cstruct-4.0.dev3/tests/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_expression.py` & `dissect_cstruct-4.0.dev3/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_parser.py` & `dissect_cstruct-4.0.dev3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_base.py` & `dissect_cstruct-4.0.dev3/tests/test_types_base.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_char.py` & `dissect_cstruct-4.0.dev3/tests/test_types_char.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_custom.py` & `dissect_cstruct-4.0.dev3/tests/test_types_custom.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_enum.py` & `dissect_cstruct-4.0.dev3/tests/test_types_enum.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_flag.py` & `dissect_cstruct-4.0.dev3/tests/test_types_flag.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_int.py` & `dissect_cstruct-4.0.dev3/tests/test_types_int.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_leb128.py` & `dissect_cstruct-4.0.dev3/tests/test_types_leb128.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_packed.py` & `dissect_cstruct-4.0.dev3/tests/test_types_packed.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_pointer.py` & `dissect_cstruct-4.0.dev3/tests/test_types_pointer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_structure.py` & `dissect_cstruct-4.0.dev3/tests/test_types_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from dissect.cstruct.cstruct import cstruct
 from dissect.cstruct.exceptions import ParserError
 from dissect.cstruct.types.base import Array, BaseType
 from dissect.cstruct.types.pointer import Pointer
-from dissect.cstruct.types.structure import Field, Structure
+from dissect.cstruct.types.structure import Field, Structure, StructureMetaType
 
 from .utils import verify_compiled
 
 
 @pytest.fixture
 def TestStruct(cs: cstruct) -> type[Structure]:
     return cs._make_struct(
@@ -525,7 +525,15 @@
         struct test * b;
     };
     """
     cs.load(cdef)
 
     assert issubclass(cs.test.fields["b"].type, Pointer)
     assert cs.test.fields["b"].type.type is cs.test
+
+
+def test_align_struct_in_struct(cs: cstruct) -> None:
+    with patch.object(StructureMetaType, "_update_fields") as update_fields:
+        cs._make_struct("test", [Field("a", cs.uint64)], align=True)
+
+        _, kwargs = update_fields.call_args
+        assert kwargs["align"]
```

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_union.py` & `dissect_cstruct-4.0.dev3/tests/test_types_union.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_types_wchar.py` & `dissect_cstruct-4.0.dev3/tests/test_types_wchar.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tests/test_utils.py` & `dissect_cstruct-4.0.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev2/tox.ini` & `dissect_cstruct-4.0.dev3/tox.ini`

 * *Files identical despite different names*

