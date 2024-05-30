# Comparing `tmp/pyTooling-6.1.0.tar.gz` & `tmp/pytooling-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTooling-6.1.0.tar", last modified: Tue Apr  9 22:31:52 2024, max compression
+gzip compressed data, was "pytooling-6.2.0.tar", last modified: Thu May 30 23:03:43 2024, max compression
```

## Comparing `pyTooling-6.1.0.tar` & `pytooling-6.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.887079 pyTooling-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-09 22:31:49.000000 pyTooling-6.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-04-09 22:31:52.887079 pyTooling-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-04-09 22:31:49.000000 pyTooling-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.871079 pyTooling-6.1.0/pyTooling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.875079 pyTooling-6.1.0/pyTooling/Attributes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.875079 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/CLIAbstraction/
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlagList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/CallByRef/
--rw-r--r--   0 runner    (1001) docker     (127)    20766 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CallByRef/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Common/
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/JSON.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/YAML.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/GenericPath/
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/GenericPath/URL.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/GenericPath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Graph/
--rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Graph/GraphML.py
--rw-r--r--   0 runner    (1001) docker     (127)    90663 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Licensing/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Licensing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/MetaClasses/
--rw-r--r--   0 runner    (1001) docker     (127)    36132 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/MetaClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Packaging/
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Packaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Platform/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/StateMachine/
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/StateMachine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/TerminalUI/
--rw-r--r--   0 runner    (1001) docker     (127)    35984 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/TerminalUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Timer/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Timer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Tree/
--rw-r--r--   0 runner    (1001) docker     (127)    34203 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Versioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:31:52.887079 pyTooling-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-09 22:31:49.000000 pyTooling-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.197213 pytooling-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-30 23:03:39.000000 pytooling-6.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-05-30 23:03:43.197213 pytooling-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-05-30 23:03:39.000000 pytooling-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.181213 pytooling-6.2.0/pyTooling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.181213 pytooling-6.2.0/pyTooling/Attributes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/Attributes/ArgParse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/CLIAbstraction/
+-rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlagList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17086 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/CallByRef/
+-rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CallByRef/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/Common/
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/JSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/YAML.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/GenericPath/
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/GenericPath/URL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/GenericPath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Graph/GraphML.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92485 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Licensing/
+-rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Licensing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/MetaClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)    36214 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/MetaClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Packaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Platform/
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/StateMachine/
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/StateMachine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/TerminalUI/
+-rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/TerminalUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Timer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Timer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Tree/
+-rw-r--r--   0 runner    (1001) docker     (127)    35173 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.193213 pytooling-6.2.0/pyTooling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:03:43.197213 pytooling-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-30 23:03:39.000000 pytooling-6.2.0/setup.py
```

### Comparing `pyTooling-6.1.0/LICENSE.md` & `pytooling-6.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/PKG-INFO` & `pytooling-6.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.1.0
+Version: 6.2.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,66 +21,65 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: docutils~=0.18.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: colorama>=0.4.6; extra == "test"
-Requires-Dist: lxml>=5.0; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: mypy>=1.8.0; extra == "test"
-Requires-Dist: ruamel.yaml>=0.18; extra == "test"
-Requires-Dist: Coverage>=7.4; extra == "test"
-Requires-Dist: typing_extensions>=4.9.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
+Requires-Dist: docutils~=0.18.0; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: Coverage>=7.4; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
 Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
-Requires-Dist: mypy>=1.8.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: lxml>=5.0; extra == "all"
-Requires-Dist: typing_extensions>=4.9.0; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pyTooling-6.1.0/README.md` & `pytooling-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Argument.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/Argument.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/BooleanFlag.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Flag.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/Flag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/ValuedFlag.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/__init__.py` & `pytooling-6.2.0/pyTooling/Attributes/ArgParse/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Attributes/__init__.py` & `pytooling-6.2.0/pyTooling/Attributes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,21 @@
 from enum   import IntFlag
 from sys    import version_info
 from types  import MethodType, FunctionType, ModuleType
 from typing import Callable, List, TypeVar, Dict, Any, Iterable, Union, Type, Tuple, Generator, ClassVar, Optional as Nullable
 
 try:
 	from pyTooling.Decorators import export, readonly
+	from pyTooling.Common     import getFullyQualifiedName
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Attributes] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators import export, readonly
+		from Common     import getFullyQualifiedName
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Attributes] Could not import directly!")
 		raise ex
 
 
 __all__ = ["Entity", "TAttr", "TAttributeFilter", "ATTRIBUTES_MEMBER_NAME"]
 
@@ -144,15 +146,18 @@
 		if isinstance(entity, MethodType):
 			attribute._methods.append(entity)
 		elif isinstance(entity, FunctionType):
 			attribute._functions.append(entity)
 		elif isinstance(entity, type):
 			attribute._classes.append(entity)
 		else:
-			raise TypeError(f"Parameter 'entity' is not a function, class nor method.")
+			ex = TypeError(f"Parameter 'entity' is not a function, class nor method.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(entity)}'.")
+			raise ex
 
 		if hasattr(entity, ATTRIBUTES_MEMBER_NAME):
 			getattr(entity, ATTRIBUTES_MEMBER_NAME).insert(0, attribute)
 		else:
 			setattr(entity, ATTRIBUTES_MEMBER_NAME,  [attribute, ])
 
 	if version_info < (3, 9):  # pragma: no cover
```

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/Argument.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/Argument.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,26 @@
 """
 This module implements command line arguments without prefix character(s).
 
 
 """
 from abc     import abstractmethod
 from pathlib import Path
+from sys     import version_info           # needed for versions before Python 3.11
 from typing  import ClassVar, List, Union, Iterable, TypeVar, Generic, Any, Optional as Nullable
 
 try:
 	from pyTooling.Decorators  import export, readonly
+	from pyTooling.Common      import getFullyQualifiedName
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Versioning] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators          import export, readonly
+		from Common              import getFullyQualifiedName
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Versioning] Could not import directly!")
 		raise ex
 
 
 __all__ = ["ValueT"]
 
@@ -146,15 +149,18 @@
 		"""
 		Initializes a ExecutableArgument instance.
 
 		:param executable: Path to the executable.
 		:raises TypeError: If parameter 'executable' is not of type :class:`~pathlib.Path`.
 		"""
 		if not isinstance(executable, Path):
-			raise TypeError("Parameter 'executable' is not of type 'Path'.")
+			ex = TypeError("Parameter 'executable' is not of type 'Path'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(executable)}'.")
+			raise ex
 
 		self._executable = executable
 
 	@property
 	def Executable(self) -> Path:
 		"""
 		Get the internal path to the wrapped executable.
@@ -168,15 +174,18 @@
 		"""
 		Set the internal path to the wrapped executable.
 
 		:param value:      Value to path to the executable.
 		:raises TypeError: If value is not of type :class:`~pathlib.Path`.
 		"""
 		if not isinstance(value, Path):
-			raise TypeError("Parameter 'value' is not of type 'Path'.")
+			ex = TypeError("Parameter 'value' is not of type 'Path'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+			raise ex
 
 		self._executable = value
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		"""
 		Convert this argument instance to a string representation with proper escaping using the matching pattern based on
 		the internal path to the wrapped executable.
@@ -314,15 +323,15 @@
 		"""
 		Initializes a ValuedArgument instance.
 
 		:param value:      Value to be stored internally.
 		:raises TypeError: If parameter 'value' is None.
 		"""
 		if value is None:
-			raise TypeError("Parameter 'value' is None.")
+			raise ValueError("Parameter 'value' is None.")
 
 		self._value = value
 
 	@property
 	def Value(self) -> ValueT:
 		"""
 		Get the internal value.
@@ -513,15 +522,18 @@
 
 		:param values:     An iterable of str instances.
 		:raises TypeError: If iterable parameter 'values' contains elements not of type :class:`str`.
 		"""
 		self._values = []
 		for value in values:
 			if not isinstance(value, str):
-				raise TypeError(f"Parameter 'values' contains elements which are not of type 'str'.")
+				ex = TypeError(f"Parameter 'values' contains elements which are not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(values)}'.")
+				raise ex
 
 			self._values.append(value)
 
 	@property
 	def Value(self) -> List[str]:
 		"""
 		Get the internal list of str objects.
@@ -539,15 +551,18 @@
 
 		:param value:      List of str objects to set.
 		:raises TypeError: If value contains elements, which are not of type :class:`str`.
 		"""
 		self._values.clear()
 		for value in value:
 			if not isinstance(value, str):
-				raise TypeError(f"Value contains elements which are not of type 'str'.")
+				ex = TypeError(f"Value contains elements which are not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+				raise ex
 			self._values.append(value)
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		"""
 		Convert this argument instance to a string representation with proper escaping using the matching pattern based on
 		the internal value.
 
@@ -587,15 +602,18 @@
 		"""
 		Initializes a PathArgument instance.
 
 		:param path:       Path to a filesystem object.
 		:raises TypeError: If parameter 'path' is not of type :class:`~pathlib.Path`.
 		"""
 		if not isinstance(path, Path):
-			raise TypeError("Parameter 'path' is not of type 'Path'.")
+			ex = TypeError("Parameter 'path' is not of type 'Path'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(path)}'.")
+			raise ex
 		self._path = path
 
 	@property
 	def Value(self) -> Path:
 		"""
 		Get the internal path object.
 
@@ -608,15 +626,18 @@
 		"""
 		Set the internal path object.
 
 		:param value:      Value to set.
 		:raises TypeError: If value is not of type :class:`~pathlib.Path`.
 		"""
 		if not isinstance(value, Path):
-			raise TypeError("Parameter 'value' is not of type 'Path'.")
+			ex = TypeError("Value is not of type 'Path'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+			raise ex
 
 		self._path = value
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		"""
 		Convert this argument instance to a string representation with proper escaping using the matching pattern based on
 		the internal value.
@@ -650,15 +671,18 @@
 
 		:param paths:      An iterable os Path instances.
 		:raises TypeError: If iterable parameter 'paths' contains elements not of type :class:`~pathlib.Path`.
 		"""
 		self._paths = []
 		for path in paths:
 			if not isinstance(path, Path):
-				raise TypeError(f"Parameter 'paths' contains elements which are not of type 'Path'.")
+				ex = TypeError(f"Parameter 'paths' contains elements which are not of type 'Path'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(path)}'.")
+				raise ex
 
 			self._paths.append(path)
 
 	@property
 	def Value(self) -> List[Path]:
 		"""
 		Get the internal list of path objects.
@@ -676,15 +700,18 @@
 
 		:param value:      List of path objects to set.
 		:raises TypeError: If value contains elements, which are not of type :class:`~pathlib.Path`.
 		"""
 		self._paths.clear()
 		for path in value:
 			if not isinstance(path, Path):
-				raise TypeError(f"Value contains elements which are not of type 'Path'.")
+				ex = TypeError(f"Value contains elements which are not of type 'Path'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(path)}'.")
+				raise ex
 			self._paths.append(path)
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		"""
 		Convert this argument instance to a string representation with proper escaping using the matching pattern based on
 		the internal value.
```

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/BooleanFlag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/Command.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/Command.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/Flag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/Flag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/KeyValueFlag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/KeyValueFlag.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,24 +37,27 @@
    * For flags with different pattern based on the boolean value itself. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.BooleanFlag`
    * For flags with a value. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.ValuedFlag`
    * For flags that have an optional value. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.NamedOptionalValuedFlag`
 """
+from sys    import version_info           # needed for versions before Python 3.11
 from typing import Union, Iterable, Dict, cast, Any, Optional as Nullable
 
 try:
 	from pyTooling.Decorators              import export
+	from pyTooling.Common                  import getFullyQualifiedName
 	from pyTooling.CLIAbstraction.Argument import NamedAndValuedArgument
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Versioning] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators                      import export
+		from Common                          import getFullyQualifiedName
 		from CLIAbstraction.Argument         import NamedAndValuedArgument
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Versioning] Could not import directly!")
 		raise ex
 
 
 @export
@@ -83,17 +86,23 @@
 		return super().__new__(cls, *args, **kwargs)
 
 	def __init__(self, keyValuePairs: Dict[str, str]) -> None:
 		super().__init__({})
 
 		for key, value in keyValuePairs.items():
 			if not isinstance(key, str):
-				raise TypeError(f"Parameter 'keyValuePairs' contains a pair, where the key is not of type 'str'.")
+				ex = TypeError(f"Parameter 'keyValuePairs' contains a pair, where the key is not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(key)}'.")
+				raise ex
 			elif not isinstance(value, str):
-				raise TypeError(f"Parameter 'keyValuePairs' contains a pair, where the value is not of type 'str'.")
+				ex = TypeError(f"Parameter 'keyValuePairs' contains a pair, where the value is not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+				raise ex
 
 			self._value[key] = value
 
 	@property
 	def Value(self) -> Dict[str, str]:
 		"""
 		Get the internal value.
@@ -110,17 +119,23 @@
 		:param keyValuePairs: Value to set.
 		:raises ValueError:   If value to set is None.
 		"""
 		innerDict = cast(Dict[str, str], self._value)
 		innerDict.clear()
 		for key, value in keyValuePairs.items():
 			if not isinstance(key, str):
-				raise TypeError(f"Parameter 'keyValuePairs' contains a pair, where the key is not of type 'str'.")
+				ex = TypeError(f"Parameter 'keyValuePairs' contains a pair, where the key is not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(key)}'.")
+				raise ex
 			elif not isinstance(value, str):
-				raise TypeError(f"Parameter 'keyValuePairs' contains a pair, where the value is not of type 'str'.")
+				ex = TypeError(f"Parameter 'keyValuePairs' contains a pair, where the value is not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+				raise ex
 
 			innerDict[key] = value
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		"""
 		Convert this argument instance to a string representation with proper escaping using the matching pattern based on
 		the internal name.
```

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlagList.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlagList.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,27 @@
    * For single valued flags. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.ValuedFlag`
    * For list of strings. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.Argument.StringListArgument`
    * For list of paths. |br|
      |rarr| :mod:`~pyTooling.CLIAbstraction.Argument.PathListArgument`
 """
+from sys    import version_info           # needed for versions before Python 3.11
 from typing import List, Union, Iterable, cast, Any
 
 try:
 	from pyTooling.Decorators              import export
+	from pyTooling.Common                  import getFullyQualifiedName
 	from pyTooling.CLIAbstraction.Argument import ValueT, NamedAndValuedArgument
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Versioning] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators                      import export
+		from Common                          import getFullyQualifiedName
 		from CLIAbstraction.Argument         import ValueT, NamedAndValuedArgument
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Versioning] Could not import directly!")
 		raise ex
 
 
 @export
@@ -109,15 +112,18 @@
 		:param values:       List of values to set.
 		:raises ValueError:  If a list element is not o type :class:`str`.
 		"""
 		innerList = cast(list, self._value)
 		innerList.clear()
 		for value in values:
 			if not isinstance(value, str):
-				raise TypeError(f"Value contains elements which are not of type 'str'.")
+				ex = TypeError(f"Value contains elements which are not of type 'str'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+				raise ex
 			innerList.append(value)
 
 	def AsArgument(self) -> Union[str, Iterable[str]]:
 		if self._name is None:
 			raise ValueError(f"")  # XXX: add message
 
 		return [self._pattern.format(self._name, value) for value in self._value]
```

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/CLIAbstraction/__init__.py` & `pytooling-6.2.0/pyTooling/CLIAbstraction/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,36 +29,39 @@
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Basic abstraction layer for executables."""
 
 # __keywords__ =  ["abstract", "executable", "cli", "cli arguments"]
 
-from os                    import environ as os_environ
-from pathlib               import Path
-from platform              import system
-from shutil                import which as shutil_which
-from subprocess            import Popen as Subprocess_Popen, PIPE as Subprocess_Pipe, STDOUT as Subprocess_StdOut
-from typing                import Dict, Optional as Nullable, ClassVar, Type, List, Tuple, Iterator, Generator, Any
+from os         import environ as os_environ
+from pathlib    import Path
+from platform   import system
+from shutil     import which as shutil_which
+from subprocess import Popen as Subprocess_Popen, PIPE as Subprocess_Pipe, STDOUT as Subprocess_StdOut
+from sys        import version_info           # needed for versions before Python 3.11
+from typing     import Dict, Optional as Nullable, ClassVar, Type, List, Tuple, Iterator, Generator, Any
 
 try:
 	from pyTooling.Decorators                import export, readonly
 	from pyTooling.MetaClasses               import ExtendedType
 	from pyTooling.Exceptions                import ToolingException, PlatformNotSupportedException
+	from pyTooling.Common                    import getFullyQualifiedName
 	from pyTooling.Attributes                import Attribute
 	from pyTooling.CLIAbstraction.Argument   import CommandLineArgument, ExecutableArgument
 	from pyTooling.CLIAbstraction.Argument   import NamedAndValuedArgument, ValuedArgument, PathArgument, PathListArgument, NamedTupledArgument
 	from pyTooling.CLIAbstraction.ValuedFlag import ValuedFlag
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.CLIAbstraction] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators                import export, readonly
 		from MetaClasses               import ExtendedType
 		from Exceptions                import ToolingException, PlatformNotSupportedException
+		from Common                    import getFullyQualifiedName
 		from Attributes                import Attribute
 		from CLIAbstraction.Argument   import CommandLineArgument, ExecutableArgument
 		from CLIAbstraction.Argument   import NamedAndValuedArgument, ValuedArgument, PathArgument, PathListArgument, NamedTupledArgument
 		from CLIAbstraction.ValuedFlag import ValuedFlag
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.CLIAbstraction] Could not import directly!")
 		raise ex
@@ -132,15 +135,18 @@
 			if isinstance(executablePath, Path):
 				if not executablePath.exists():
 					if dryRun:
 						self.LogDryRun(f"File check for '{executablePath}' failed. [SKIPPING]")
 					else:
 						raise CLIAbstractionException(f"Program '{executablePath}' not found.") from FileNotFoundError(executablePath)
 			else:
-				raise TypeError(f"Parameter 'executablePath' is not of type 'Path'.")
+				ex = TypeError(f"Parameter 'executablePath' is not of type 'Path'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(executablePath)}'.")
+				raise ex
 		elif binaryDirectoryPath is not None:
 			if isinstance(binaryDirectoryPath, Path):
 				if not binaryDirectoryPath.exists():
 					if dryRun:
 						self.LogDryRun(f"Directory check for '{binaryDirectoryPath}' failed. [SKIPPING]")
 					else:
 						raise CLIAbstractionException(f"Binary directory '{binaryDirectoryPath}' not found.") from FileNotFoundError(binaryDirectoryPath)
@@ -152,15 +158,18 @@
 
 				if not executablePath.exists():
 					if dryRun:
 						self.LogDryRun(f"File check for '{executablePath}' failed. [SKIPPING]")
 					else:
 						raise CLIAbstractionException(f"Program '{executablePath}' not found.") from FileNotFoundError(executablePath)
 			else:
-				raise TypeError(f"Parameter 'binaryDirectoryPath' is not of type 'Path'.")
+				ex = TypeError(f"Parameter 'binaryDirectoryPath' is not of type 'Path'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(binaryDirectoryPath)}'.")
+				raise ex
 		else:
 			try:
 				executablePath = Path(self._executableNames[self._platform])
 			except KeyError:
 				raise CLIAbstractionException(f"Program is not supported on platform '{self._platform}'.") from PlatformNotSupportedException(self._platform)
 
 			resolvedExecutable = shutil_which(str(executablePath))
@@ -193,22 +202,28 @@
 	@staticmethod
 	def _NeedsParameterInitialization(key):
 		return issubclass(key, (ValuedFlag, ValuedArgument, NamedAndValuedArgument, NamedTupledArgument, PathArgument, PathListArgument))
 
 	def __getitem__(self, key):
 		"""Access to a CLI parameter by CLI option (key must be of type :class:`CommandLineArgument`), which is already used."""
 		if not issubclass(key, CommandLineArgument):
-			raise TypeError(f"Key '{key}' is not a subclass of 'CommandLineArgument'.")
+			ex = TypeError(f"Key '{key}' is not a subclass of 'CommandLineArgument'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(key)}'.")
+			raise ex
 
 		# TODO: is nested check
 		return self.__cliParameters__[key]
 
 	def __setitem__(self, key, value):
 		if not issubclass(key, CommandLineArgument):
-			raise TypeError(f"Key '{key}' is not a subclass of 'CommandLineArgument'.")
+			ex = TypeError(f"Key '{key}' is not a subclass of 'CommandLineArgument'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(key)}'.")
+			raise ex
 		elif key not in self.__cliOptions__:
 			raise KeyError(f"Option '{key}' is not allowed on executable '{self.__class__.__name__}'")
 		elif key in self.__cliParameters__:
 			raise KeyError(f"Option '{key}' is already set to a value.")
 
 		if self._NeedsParameterInitialization(key):
 			self.__cliParameters__[key] = key(value)
```

### Comparing `pyTooling-6.1.0/pyTooling/CallByRef/__init__.py` & `pytooling-6.2.0/pyTooling/CallByRef/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -206,161 +206,221 @@
 
 	# Binary operators - logical
 	def __and__(self, other: Any) -> int:
 		"""And: self & other."""
 		if isinstance(other, int):
 			return self.Value & other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by and operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by and operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __or__(self, other: Any) -> int:
 		"""Or: self | other."""
 		if isinstance(other, int):
 			return self.Value | other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by or operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by or operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __xor__(self, other: Any) -> int:
 		"""Xor: self ^ other."""
 		if isinstance(other, int):
 			return self.Value ^ other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	# Binary inplace operators
 	def __iand__(self, other: Any) -> 'CallByRefIntParam':  # Starting with Python 3.11+, use typing.Self as return type
 		"""Inplace and: self &= other."""
 		if isinstance(other, int):
 			self.Value &= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by &= operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by &= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __ior__(self, other: Any) -> 'CallByRefIntParam':  # Starting with Python 3.11+, use typing.Self as return type
 		r"""Inplace or: self \|= other."""
 		if isinstance(other, int):
 			self.Value |= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by |= operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by |= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __ixor__(self, other: Any) -> 'CallByRefIntParam':  # Starting with Python 3.11+, use typing.Self as return type
 		r"""Inplace or: self \|= other."""
 		if isinstance(other, int):
 			self.Value ^= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by ^= operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by ^= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	# Binary operators - arithmetic
 	def __add__(self, other: Any) -> int:
 		"""Addition: self + other."""
 		if isinstance(other, int):
 			return self.Value + other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by + operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by + operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __sub__(self, other: Any) -> int:
 		"""Subtraction: self - other."""
 		if isinstance(other, int):
 			return self.Value - other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by - operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by - operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __truediv__(self, other: Any) -> int:
 		"""Division: self / other."""
 		if isinstance(other, int):
 			return self.Value / other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by / operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by / operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __floordiv__(self, other: Any) -> int:
 		"""Floor division: self // other."""
 		if isinstance(other, int):
 			return self.Value // other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by // operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by // operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __mul__(self, other: Any) -> int:
 		"""Multiplication: self * other."""
 		if isinstance(other, int):
 			return self.Value * other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by * operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by * operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __mod__(self, other: Any) -> int:
 		"""Modulo: self % other."""
 		if isinstance(other, int):
 			return self.Value % other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by % operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by % operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __pow__(self, other: Any) -> int:
 		"""Power: self ** other."""
 		if isinstance(other, int):
 			return self.Value ** other
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by ** operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by ** operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	# Binary inplace operators - arithmetic
 	def __iadd__(self, other: Any) -> 'CallByRefIntParam':
 		"""Addition: self += other."""
 		if isinstance(other, int):
 			self.Value += other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __isub__(self, other: Any) -> 'CallByRefIntParam':
 		"""Subtraction: self -= other."""
 		if isinstance(other, int):
 			self.Value -= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __idiv__(self, other: Any) -> 'CallByRefIntParam':
 		"""Division: self /= other."""
 		if isinstance(other, int):
 			self.Value /= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __ifloordiv__(self, other: Any) -> 'CallByRefIntParam':
 		"""Floor division: self // other."""
 		if isinstance(other, int):
 			self.Value //= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __imul__(self, other: Any) -> 'CallByRefIntParam':
 		r"""Multiplication: self \*= other."""
 		if isinstance(other, int):
 			self.Value *= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __imod__(self, other: Any) -> 'CallByRefIntParam':
 		"""Modulo: self %= other."""
 		if isinstance(other, int):
 			self.Value %= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	def __ipow__(self, other: Any) -> 'CallByRefIntParam':
 		r"""Power: self \*\*= other."""
 		if isinstance(other, int):
 			self.Value **= other
 			return self
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by xor operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: int")
+			raise ex
 
 	# Binary operators - comparison
 	def __eq__(self, other: Any) -> bool:
 		"""
 		Compare a CallByRefIntParam wrapped integer value with another instances (CallByRefIntParam) or non-wrapped integer value for equality.
 
 		:param other:      Parameter to compare against.
```

### Comparing `pyTooling-6.1.0/pyTooling/Common/__init__.py` & `pytooling-6.2.0/pyTooling/Common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,44 +33,82 @@
 
 .. hint:: See :ref:`high-level help <COMMON>` for explanations and usage examples.
 """
 __author__ =        "Patrick Lehmann"
 __email__ =         "Paebbels@gmail.com"
 __copyright__ =     "2017-2024, Patrick Lehmann"
 __license__ =       "Apache License, Version 2.0"
-__version__ =       "6.1.0"
+__version__ =       "6.2.0"
 __keywords__ =      ["abstract", "argparse", "attributes", "bfs", "cli", "console", "data structure", "decorators",
 					  "dfs", "exceptions", "generators", "generic library", "generic path", "graph", "installation",
 					  "iterators", "licensing", "message logging", "meta-classes", "overloading", "override", "packaging",
 					  "path", "platform", "setuptools", "shell", "singleton", "slots","terminal", "text user interface",
 					  "timer", "tree", "TUI", "url", "versioning", "wheel"]
 __issue_tracker__ = "https://GitHub.com/pyTooling/pyTooling/issues"
 
-from collections import deque
-from numbers     import Number
-from typing      import Type, TypeVar, Callable, Generator, overload, Hashable, Optional, List
-from typing      import Any, Dict, Tuple, Union, Mapping, Set, Iterable, Optional as Nullable
+from collections         import deque
+from numbers             import Number
+from pathlib             import Path
+from sys                 import version_info
+from types               import ModuleType
+from typing              import Type, TypeVar, Callable, Generator, overload, Hashable, Optional, List
+from typing              import Any, Dict, Tuple, Union, Mapping, Set, Iterable, Optional as Nullable
+
 
 try:
 	from pyTooling.Decorators import export
-	from pyTooling.Platform   import Platform
 except ModuleNotFoundError:  # pragma: no cover
 	print("[pyTooling.Common] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators         import export
-		from Platform           import Platform
 	except ModuleNotFoundError as ex:  # pragma: no cover
 		print("[pyTooling.Common] Could not import directly!")
 		raise ex
 
 
-__all__ = ["CurrentPlatform"]
+@export
+def getFullyQualifiedName(obj: Any):
+	try:
+		module = obj.__module__             # for class or function
+	except AttributeError:
+		module = obj.__class__.__module__
+
+	try:
+		name = obj.__qualname__             # for class or function
+	except AttributeError:
+		name = obj.__class__.__qualname__
+
+	# If obj is a method of builtin class, then module will be None
+	if module == "builtins" or module is None:
+		return name
+
+	return f"{module}.{name}"
+
+
+if version_info >= (3, 9):  # pragma: no cover
+	@export
+	def getResourceFile(module: Union[str, ModuleType], filename: str) -> Path:
+		from importlib.resources import files  # TODO: can be used as regular import > 3.8
+
+		# TODO: files() has wrong TypeHint Traversible vs. Path
+		resourcePath: Path = files(module) / filename
+		if not resourcePath.exists():
+			from pyTooling.Exceptions import ToolingException
+
+			raise ToolingException(f"Resource file '{filename}' not found in resource '{module}'.") from FileNotFoundError(str(resourcePath))
+
+		return resourcePath
+
+
+	@export
+	def readResourceFile(module: Union[str, ModuleType], filename: str) -> str:
+		from importlib.resources import files
 
-CurrentPlatform = Platform()     #: Gathered information for the current platform.
+		return files(module).joinpath(filename).read_text()
 
 
 @export
 def isnestedclass(cls: Type, scope: Type) -> bool:
 	"""
 	Returns true, if the given class ``cls`` is a member on an outer class ``scope``.
```

### Comparing `pyTooling-6.1.0/pyTooling/Configuration/JSON.py` & `pytooling-6.2.0/pyTooling/Configuration/JSON.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Configuration/YAML.py` & `pytooling-6.2.0/pyTooling/Configuration/YAML.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Configuration/__init__.py` & `pytooling-6.2.0/pyTooling/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Decorators/__init__.py` & `pytooling-6.2.0/pyTooling/Decorators/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,20 @@
 
 		func.__notImplemented__ = True
 		return func
 
 	return decorator
 
 
+# Further Reading:
+# * https://github.com/python/cpython/issues/89519#issuecomment-1397534245
+# * https://stackoverflow.com/questions/128573/using-property-on-classmethods/64738850#64738850
+# * https://stackoverflow.com/questions/128573/using-property-on-classmethods
+# * https://stackoverflow.com/questions/5189699/how-to-make-a-class-property
+
 @export
 def classproperty(method):
 
 	class Descriptor:
 		"""A decorator adding properties to classes."""
 		_getter: Callable
 		_setter: Callable
```

### Comparing `pyTooling-6.1.0/pyTooling/Exceptions/__init__.py` & `pytooling-6.2.0/pyTooling/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/GenericPath/URL.py` & `pytooling-6.2.0/pyTooling/GenericPath/URL.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/GenericPath/__init__.py` & `pytooling-6.2.0/pyTooling/GenericPath/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Graph/GraphML.py` & `pytooling-6.2.0/pyTooling/Graph/GraphML.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Graph/__init__.py` & `pytooling-6.2.0/pyTooling/Graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,32 @@
 			 I ---> E --> F --> D
 
 			 classDef node fill:#eee,stroke:#777,font-size:smaller;
 """
 import heapq
 from collections import deque
 from itertools   import chain
+from sys         import version_info           # needed for versions before Python 3.11
 from typing      import TypeVar, Generic, Optional as Nullable, Iterable, Hashable, Generator, Callable
 from typing      import List, Union, Dict, Iterator as typing_Iterator, Set, Deque, Tuple
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 	from pyTooling.Exceptions  import ToolingException
+	from pyTooling.Common      import getFullyQualifiedName
 	from pyTooling.Tree        import Node
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Graph] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators          import export, readonly
 		from MetaClasses         import ExtendedType, mixin
 		from Exceptions          import ToolingException
+		from Common              import getFullyQualifiedName
 		from Tree                import Node
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Graph] Could not import directly!")
 		raise ex
 
 
 DictKeyType = TypeVar("DictKeyType", bound=Hashable)
@@ -355,15 +358,18 @@
 
 	def __init__(self, name: Nullable[str] = None) -> None:
 		"""
 		.. todo:: GRAPH::BaseWithName::init Needs documentation.
 
 		"""
 		if name is not None and not isinstance(name, str):
-			raise TypeError("Parameter 'name' is not of type 'str'.")
+			ex = TypeError("Parameter 'name' is not of type 'str'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(name)}'.")
+			raise ex
 
 		super().__init__()
 
 		self._name = name
 
 	@property
 	def Name(self) -> Nullable[str]:
@@ -373,15 +379,18 @@
 		:returns: The value of a component.
 		"""
 		return self._name
 
 	@Name.setter
 	def Name(self, value: str) -> None:
 		if not isinstance(value, str):
-			raise TypeError("Name is not of type 'str'.")
+			ex = TypeError("Name is not of type 'str'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(value)}'.")
+			raise ex
 
 		self._name = value
 
 
 @export
 class BaseWithVertices(
 	BaseWithName[DictKeyType, DictValueType],
@@ -408,15 +417,18 @@
 		"""
 		.. todo:: GRAPH::Component::init Needs documentation.
 
 		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
 		if not isinstance(graph, Graph):
-			raise TypeError("Parameter 'graph' is not of type 'Graph'.")
+			ex = TypeError("Parameter 'graph' is not of type 'Graph'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(graph)}'.")
+			raise ex
 
 		super().__init__(name)
 
 		self._graph = graph
 		self._vertices = set() if vertices is None else {v for v in vertices}
 
 	def __del__(self):
@@ -484,15 +496,18 @@
 
 	def __init__(self, vertexID: Nullable[VertexIDType] = None, value: Nullable[VertexValueType] = None, weight: Nullable[VertexWeightType] = None, graph: Nullable['Graph'] = None, subgraph: Nullable['Subgraph'] = None) -> None:
 		"""
 		.. todo:: GRAPH::Vertex::init Needs documentation.
 
 		"""
 		if vertexID is not None and not isinstance(vertexID, Hashable):
-			raise TypeError("Parameter 'vertexID' is not of type 'VertexIDType'.")
+			ex = TypeError("Parameter 'vertexID' is not of type 'VertexIDType'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(vertexID)}'.")
+			raise ex
 
 		super().__init__(vertexID, value, weight)
 
 		if subgraph is None:
 			self._graph = graph if graph is not None else Graph()
 			self._subgraph = None
 			self._component = Component(self._graph, vertices=(self,))
@@ -1648,23 +1663,35 @@
 
 	def __init__(self, source: Vertex, destination: Vertex, edgeID: Nullable[EdgeIDType] = None, value: Nullable[EdgeValueType] = None, weight: Nullable[EdgeWeightType] = None) -> None:
 		"""
 		.. todo:: GRAPH::Edge::init Needs documentation.
 
 		"""
 		if not isinstance(source, Vertex):
-			raise TypeError("Parameter 'source' is not of type 'Vertex'.")
+			ex = TypeError("Parameter 'source' is not of type 'Vertex'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(source)}'.")
+			raise ex
 		if not isinstance(destination, Vertex):
-			raise TypeError("Parameter 'destination' is not of type 'Vertex'.")
+			ex = TypeError("Parameter 'destination' is not of type 'Vertex'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(destination)}'.")
+			raise ex
 		if edgeID is not None and not isinstance(edgeID, Hashable):
-			raise TypeError("Parameter 'edgeID' is not of type 'EdgeIDType'.")
+			ex = TypeError("Parameter 'edgeID' is not of type 'EdgeIDType'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(edgeID)}'.")
+			raise ex
 		# if value is not None and  not isinstance(value, Vertex):
 		# 	raise TypeError("Parameter 'value' is not of type 'EdgeValueType'.")
 		if weight is not None and not isinstance(weight, (int, float)):
-			raise TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
+			ex = TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(weight)}'.")
+			raise ex
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
 		super().__init__(source, destination, edgeID, value, weight)
 
 	def Delete(self) -> None:
 		# Remove from Source and Destination
@@ -1708,23 +1735,35 @@
 
 	def __init__(self, source: Vertex, destination: Vertex, linkID: LinkIDType = None, value: LinkValueType = None, weight: Nullable[LinkWeightType] = None) -> None:
 		"""
 		.. todo:: GRAPH::Edge::init Needs documentation.
 
 		"""
 		if not isinstance(source, Vertex):
-			raise TypeError("Parameter 'source' is not of type 'Vertex'.")
+			ex = TypeError("Parameter 'source' is not of type 'Vertex'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(source)}'.")
+			raise ex
 		if not isinstance(destination, Vertex):
-			raise TypeError("Parameter 'destination' is not of type 'Vertex'.")
+			ex = TypeError("Parameter 'destination' is not of type 'Vertex'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(destination)}'.")
+			raise ex
 		if linkID is not None and not isinstance(linkID, Hashable):
-			raise TypeError("Parameter 'edgeID' is not of type 'EdgeIDType'.")
+			ex = TypeError("Parameter 'linkID' is not of type 'LinkIDType'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(linkID)}'.")
+			raise ex
 		# if value is not None and  not isinstance(value, Vertex):
 		# 	raise TypeError("Parameter 'value' is not of type 'EdgeValueType'.")
 		if weight is not None and not isinstance(weight, (int, float)):
-			raise TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
+			ex = TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(weight)}'.")
+			raise ex
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
 		super().__init__(source, destination, linkID, value, weight)
 
 	def Delete(self) -> None:
 		self._source._outboundEdges.remove(self)
@@ -1933,23 +1972,21 @@
 		:returns:           A generator to iterate all vertices in topological order.
 		:except CycleError: Raised if graph is cyclic, thus topological sorting isn't possible.
 		"""
 		outboundEdgeCounts = {}
 		leafVertices = []
 
 		for vertex in self._verticesWithoutID:
-			count = len(vertex._outboundEdges)
-			if count == 0:
+			if (count := len(vertex._outboundEdges)) == 0:
 				leafVertices.append(vertex)
 			else:
 				outboundEdgeCounts[vertex] = count
 
 		for vertex in self._verticesWithID.values():
-			count = len(vertex._outboundEdges)
-			if count == 0:
+			if (count := len(vertex._outboundEdges)) == 0:
 				leafVertices.append(vertex)
 			else:
 				outboundEdgeCounts[vertex] = count
 
 		if not leafVertices:
 			raise CycleError(f"Graph has no leafs. Thus, no topological sorting exists.")
 
@@ -2199,23 +2236,21 @@
 		if len(self._verticesWithID) + len(self._verticesWithoutID) == 0:
 			return False
 
 		outboundEdgeCounts = {}
 		leafVertices = []
 
 		for vertex in self._verticesWithoutID:
-			count = len(vertex._outboundEdges)
-			if count == 0:
+			if (count := len(vertex._outboundEdges)) == 0:
 				leafVertices.append(vertex)
 			else:
 				outboundEdgeCounts[vertex] = count
 
 		for vertex in self._verticesWithID.values():
-			count = len(vertex._outboundEdges)
-			if count == 0:
+			if (count := len(vertex._outboundEdges)) == 0:
 				leafVertices.append(vertex)
 			else:
 				outboundEdgeCounts[vertex] = count
 
 		# If there are no leafs, then each vertex has at least one inbound and one outbound edges. Thus, there is a cycle.
 		if not leafVertices:
 			return True
@@ -2267,15 +2302,18 @@
 		"""
 		.. todo:: GRAPH::Subgraph::init Needs documentation.
 
 		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
 		if not isinstance(graph, Graph):
-			raise TypeError("Parameter 'graph' is not of type 'Graph'.")
+			ex = TypeError("Parameter 'graph' is not of type 'Graph'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(graph)}'.")
+			raise ex
 
 		super().__init__(name)
 
 		graph._subgraphs.add(self)
 
 		self._graph = graph
```

### Comparing `pyTooling-6.1.0/pyTooling/Licensing/__init__.py` & `pytooling-6.2.0/pyTooling/Licensing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
    * https://github.com/spdx/license-list-XML
 
    List of `Python classifiers <https://pypi.org/classifiers/>`__
 
 .. hint:: See :ref:`high-level help <LICENSING>` for explanations and usage examples.
 """
 from dataclasses  import dataclass
+from sys          import version_info           # needed for versions before Python 3.11
 from typing       import Any, Dict, Optional as Nullable
 
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
@@ -190,27 +191,33 @@
 
 		:returns:          ``True``, if both licenses are identical.
 		:raises TypeError: If second operand is not of type :class:`License` or :class:`str`.
 		"""
 		if isinstance(other, License):
 			return self._spdxIdentifier == other._spdxIdentifier
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by equal operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by equal operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: License, str")
+			raise ex
 
 	def __ne__(self, other: Any) -> bool:
 		"""
 		Returns true, if both licenses are not identical (comparison based on SPDX identifiers).
 
 		:returns:          ``True``, if both licenses are not identical.
 		:raises TypeError: If second operand is not of type :class:`License` or :class:`str`.
 		"""
 		if isinstance(other, License):
 			return self._spdxIdentifier != other._spdxIdentifier
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by unequal operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by unequal operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: License, str")
+			raise ex
 
 	def __le__(self, other: Any) -> bool:
 		"""Returns true, if both licenses are compatible."""
 		raise NotImplementedError("License compatibility check is not yet implemented.")
 
 	def __ge__(self, other: Any) -> bool:
 		"""Returns true, if both licenses are compatible."""
```

### Comparing `pyTooling-6.1.0/pyTooling/MetaClasses/__init__.py` & `pytooling-6.2.0/pyTooling/MetaClasses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,20 @@
 from types      import FunctionType  #, MethodType
 from typing     import Any, Tuple, List, Dict, Callable, Generator, Set, Iterator, Iterable, Union
 from typing     import Type, TypeVar, Generic, _GenericAlias, ClassVar, Optional as Nullable
 
 try:
 	from pyTooling.Exceptions import ToolingException
 	from pyTooling.Decorators import export
-	from pyTooling.Attributes import ATTRIBUTES_MEMBER_NAME, AttributeScope
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.MetaClasses] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Exceptions import ToolingException
 		from Decorators import export
-		from Attributes import ATTRIBUTES_MEMBER_NAME, AttributeScope
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.MetaClasses] Could not import directly!")
 		raise ex
 
 
 __all__ = ["M"]
 
@@ -405,14 +403,19 @@
 		                        If false, create slots if ``slots`` is true.
 		                        If none, preserve behavior of primary base-class.
 		:param singleton:       If true, make the class a :term:`Singleton`.
 		:returns:               The new class.
 		:raises AttributeError: If base-class has no '__slots__' attribute.
 		:raises AttributeError: If slot already exists in base-class.
 		"""
+		try:
+			from pyTooling.Attributes import ATTRIBUTES_MEMBER_NAME, AttributeScope
+		except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
+			from Attributes import ATTRIBUTES_MEMBER_NAME, AttributeScope
+
 		# Inherit 'slots' feature from primary base-class
 		if len(baseClasses) > 0:
 			primaryBaseClass = baseClasses[0]
 			if isinstance(primaryBaseClass, self):
 				slots = primaryBaseClass.__slotted__
 
 		# Compute slots and mixin-slots from annotated fields as well as class- and object-fields with initial values.
```

### Comparing `pyTooling-6.1.0/pyTooling/Packaging/__init__.py` & `pytooling-6.2.0/pyTooling/Packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Platform/__init__.py` & `pytooling-6.2.0/pyTooling/Platform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 		from MetaClasses         import ExtendedType, mixin
 		from Versioning          import SemanticVersion
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Platform] Could not import directly!")
 		raise ex
 
 
+__all__ = ["CurrentPlatform"]
+
+
 @export
 class PythonImplementation(Flag):
 	Unknown = 0
 
 	CPython = 1
 	PyPy = 2
 
@@ -511,7 +514,10 @@
 			architecture = "x86-64"
 		elif Platforms.ARCH_AArch64 in self._platform:
 			architecture = "amd64"
 		else:
 			architecture = "arch:dec-err"
 
 		return f"{platform}{environment} ({architecture}){runtime}"
+
+
+CurrentPlatform = Platform()     #: Gathered information for the current platform.
```

### Comparing `pyTooling-6.1.0/pyTooling/StateMachine/__init__.py` & `pytooling-6.2.0/pyTooling/StateMachine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/TerminalUI/__init__.py` & `pytooling-6.2.0/pyTooling/TerminalUI/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """A set of helpers to implement a text user interface (TUI) in a terminal."""
 from enum                    import Enum, unique
 from io                      import TextIOWrapper
-from sys                     import stdin, stdout, stderr
+from sys                     import stdin, stdout, stderr, version_info           # needed for versions before Python 3.11
 from textwrap                import dedent
 from typing                  import NoReturn, Tuple, Any, List, Optional as Nullable, Dict, Callable, ClassVar
 
 try:
 	from colorama import Fore as Foreground
 except ImportError as ex:  # pragma: no cover
 	raise Exception(f"Optional dependency 'colorama' not installed. Either install pyTooling with extra dependencies 'pyTooling[terminal]' or install 'colorama' directly.") from ex
@@ -502,80 +502,98 @@
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both severity levels are equal.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value == other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by == operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by == operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 	def __ne__(self, other: Any) -> bool:
 		"""
 		Compare two Severity instances (severity level) for inequality.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both severity levels are unequal.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value != other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by != operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by != operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 	def __lt__(self, other: Any) -> bool:
 		"""
 		Compare two Severity instances (severity level) for less-than.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if severity levels is less than other severity level.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value < other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by < operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by < operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 	def __le__(self, other: Any) -> bool:
 		"""
 		Compare two Severity instances (severity level) for less-than-or-equal.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if severity levels is less than or equal other severity level.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value <= other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by <= operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by <= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 	def __gt__(self, other: Any) -> bool:
 		"""
 		Compare two Severity instances (severity level) for greater-than.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if severity levels is greater than other severity level.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value >	other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by > operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by > operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 	def __ge__(self, other: Any) -> bool:
 		"""
 		Compare two Severity instances (severity level) for greater-than-or-equal.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if severity levels is greater than or equal other severity level.
 		:raises TypeError: If parameter ``other`` is not of type :class:`Severity`.
 		"""
 		if isinstance(other, Severity):
 			return self.value >= other.value
 		else:
-			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by >= operator.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by >= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: Severity")
+			raise ex
 
 
 @export
 @unique
 class Mode(Enum):
 	TextToStdOut_ErrorsToStdErr = 0
 	AllLinearToStdOut = 1
```

### Comparing `pyTooling-6.1.0/pyTooling/Timer/__init__.py` & `pytooling-6.2.0/pyTooling/Timer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyTooling/Tree/__init__.py` & `pytooling-6.2.0/pyTooling/Tree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,30 @@
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """A powerful tree data structure for Python."""
 from collections   import deque
+from sys           import version_info           # needed for versions before Python 3.11
 from typing        import List, Generator, Iterable, TypeVar, Generic, Dict, Optional as Nullable, Hashable, Tuple, Callable, Union, Deque, Iterator
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 	from pyTooling.Exceptions  import ToolingException
+	from pyTooling.Common      import getFullyQualifiedName
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Tree] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators          import export, readonly
 		from MetaClasses         import ExtendedType, mixin
 		from Exceptions          import ToolingException
+		from Common              import getFullyQualifiedName
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.Tree] Could not import directly!")
 		raise ex
 
 
 IDType = TypeVar("IDType", bound=Hashable)
 """A type variable for a tree's ID."""
@@ -165,15 +168,18 @@
 
 		"""
 		self._id = nodeID
 		self._value = value
 		self._dict = {}
 
 		if parent is not None and not isinstance(parent, Node):
-			raise TypeError(f"Parameter 'parent' is not of type 'Node'.")
+			ex = TypeError(f"Parameter 'parent' is not of type 'Node'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+			raise ex
 
 		if parent is None:
 			self._root = self
 			self._parent = None
 			self._level = 0
 
 			self._nodesWithID = {}
@@ -197,19 +203,25 @@
 
 			parent._children.append(self)
 
 		self._children = []
 
 		if children is not None:
 			if not isinstance(children, Iterable):
-				raise TypeError(f"Parameter 'children' is not iterable.")
+				ex = TypeError(f"Parameter 'children' is not iterable.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(children)}'.")
+				raise ex
 
 			for child in children:
 				if not isinstance(child, Node):
-					raise TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
+					ex = TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
+					if version_info >= (3, 11):  # pragma: no cover
+						ex.add_note(f"Got type '{getFullyQualifiedName(child)}'.")
+					raise ex
 
 				child.Parent = self
 
 	@readonly
 	def ID(self) -> Nullable[IDType]:
 		"""
 		Read-only property to access the unique ID of a node (:attr:`_id`).
@@ -327,15 +339,18 @@
 					del self._nodesWithID[sibling._id]
 
 			self._parent._children.remove(self)
 
 			self._root = self
 			self._parent = None
 		elif not isinstance(parent, Node):
-			raise TypeError(f"Parameter 'parent' is not of type 'Node'.")
+			ex = TypeError(f"Parameter 'parent' is not of type 'Node'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+			raise ex
 		else:
 			if parent._root is self._root:
 				raise AlreadyInTreeError(f"Parent '{parent}' is already a child node in this tree.")
 
 			self._root = parent._root
 			self._parent = parent
 			self._level = parent._level + 1
@@ -515,15 +530,18 @@
 
 		   :attr:`Parent` |br|
 		      |rarr| Set the parent of a node.
 		   :meth:`AddChildren` |br|
 		      |rarr| Add multiple children at once.
 		"""
 		if not isinstance(child, Node):
-			raise TypeError(f"Parameter 'child' is not of type 'Node'.")
+			ex = TypeError(f"Parameter 'child' is not of type 'Node'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(child)}'.")
+			raise ex
 
 		if child._root is self._root:
 			raise AlreadyInTreeError(f"Child '{child}' is already a node in this tree.")
 
 		child._root = self._root
 		child._parent = self
 		child._level = self._level + 1
@@ -546,15 +564,18 @@
 		   :attr:`Parent` |br|
 		      |rarr| Set the parent of a node.
 		   :meth:`AddChild` |br|
 		      |rarr| Add a child node to the tree.
 		"""
 		for child in children:
 			if not isinstance(child, Node):
-				raise TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
+				ex = TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(child)}'.")
+				raise ex
 
 			if child._root is self._root:
 				# TODO: create a more specific exception
 				raise AlreadyInTreeError(f"Child '{child}' is already a node in this tree.")
 
 			child._root = self._root
 			child._parent = self
```

### Comparing `pyTooling-6.1.0/pyTooling/Versioning/__init__.py` & `pytooling-6.2.0/pyTooling/Versioning/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 # ==================================================================================================================== #
 #
 """
 Implementation of semantic and date versioning version-numbers.
 
 .. hint:: See :ref:`high-level help <VERSIONING>` for explanations and usage examples.
 """
-from enum          import IntEnum
-from typing        import Optional as Nullable, Any
+from enum   import IntEnum
+from sys    import version_info           # needed for versions before Python 3.11
+from typing import Optional as Nullable, Any
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.Versioning] Could not import from 'pyTooling.*'!")
 
@@ -164,15 +165,18 @@
 		Compare two Version instances (version numbers) for equality.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both version numbers are equal.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by == operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		return (
 			(self._major == other._major) and
 			(self._minor == other._minor) and
 			(self._patch == other._patch) and
 			(self._build == other._build)
 		)
@@ -182,15 +186,18 @@
 		Compare two Version instances (version numbers) for inequality.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both version numbers are not equal.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by != operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		return not self.__eq__(other)
 
 	@staticmethod
 	def __compare(left: 'SemanticVersion', right: 'SemanticVersion') -> Nullable[bool]:
 		"""
 		Private helper method to compute the comparison of two :class:`SemanticVersion` instances.
@@ -228,56 +235,68 @@
 		Compare two Version instances (version numbers) if the version is less than the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is less than the second operand.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by < operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		result = self.__compare(self, other)
 		return result if result is not None else False
 
 	def __le__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is less than or equal to the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is less than or equal to the second operand.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by <= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		result = self.__compare(self, other)
 		return result if result is not None else True
 
 	def __gt__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is greater than the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is greater than the second operand.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by > operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		return not self.__le__(other)
 
 	def __ge__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is greater than or equal to the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is greater than or equal to the second operand.
 		:raises TypeError: If parameter ``other`` is not of type :class:`SemanticVersion`.
 		"""
 		if not isinstance(other, SemanticVersion):
-			raise TypeError(f"Parameter 'other' is not of type 'SemanticVersion'.")
+			ex = TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by >= operator.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Supported types for second operand: SemanticVersion")
+			raise ex
 
 		return not self.__lt__(other)
 
 	def __repr__(self) -> str:
 		"""
 		Return a string representation of this version number without prefix ``v``.
```

### Comparing `pyTooling-6.1.0/pyTooling.egg-info/PKG-INFO` & `pytooling-6.2.0/pyTooling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.1.0
+Version: 6.2.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,66 +21,65 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: docutils~=0.18.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: colorama>=0.4.6; extra == "test"
-Requires-Dist: lxml>=5.0; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: mypy>=1.8.0; extra == "test"
-Requires-Dist: ruamel.yaml>=0.18; extra == "test"
-Requires-Dist: Coverage>=7.4; extra == "test"
-Requires-Dist: typing_extensions>=4.9.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
+Requires-Dist: docutils~=0.18.0; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: Coverage>=7.4; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
 Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
-Requires-Dist: mypy>=1.8.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: lxml>=5.0; extra == "all"
-Requires-Dist: typing_extensions>=4.9.0; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pyTooling-6.1.0/pyTooling.egg-info/SOURCES.txt` & `pytooling-6.2.0/pyTooling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTooling-6.1.0/pyproject.toml` & `pytooling-6.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-  "setuptools >= 69.0.0",
-  "wheel >= 0.40.0",
-  "pyTooling ~= 6.0"
+  "setuptools ~= 69.5",
+  "wheel ~= 0.40.0",
+  "pyTooling ~= 6.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
```

### Comparing `pyTooling-6.1.0/setup.py` & `pytooling-6.2.0/setup.py`

 * *Files identical despite different names*

