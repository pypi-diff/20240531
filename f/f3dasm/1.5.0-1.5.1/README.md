# Comparing `tmp/f3dasm-1.5.0.tar.gz` & `tmp/f3dasm-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-1.5.0.tar", last modified: Wed May 29 13:44:57 2024, max compression
+gzip compressed data, was "f3dasm-1.5.1.tar", last modified: Fri May 31 12:53:48 2024, max compression
```

## Comparing `f3dasm-1.5.0.tar` & `f3dasm-1.5.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2024-05-24 09:01:59.000000 f3dasm-1.5.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2024-05-24 09:01:59.000000 f3dasm-1.5.0/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     4991 2024-05-29 13:44:56.992264 f3dasm-1.5.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     3329 2024-05-29 13:42:22.000000 f3dasm-1.5.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-29 13:42:22.000000 f3dasm-1.5.0/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2024-05-24 09:01:59.000000 f3dasm-1.5.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       85 2024-05-24 09:01:59.000000 f3dasm-1.5.0/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1435 2024-05-29 13:44:56.992264 f3dasm-1.5.0/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.984264 f3dasm-1.5.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1481 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       27 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/__version__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/_argparser.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1309 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5153 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/datagenerator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)      125 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9056 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    21530 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/design/domain.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10505 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/design/parameter.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_columns.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17943 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10131 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_io.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_jobqueue.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_newdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    68077 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12635 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentsample.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12662 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/samplers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/hydra_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3478 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/logger.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/_src/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1549 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2534 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1765 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/numpy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7538 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2116 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2336 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/scipy_implementations.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)      755 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/datageneration/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      906 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/datageneration/functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      903 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/hydra_tools.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      823 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     4991 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1967 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      132 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2024-05-24 09:01:59.000000 f3dasm-1.5.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2024-05-24 09:01:59.000000 f3dasm-1.5.1/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     5331 2024-05-31 12:53:48.956451 f3dasm-1.5.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3670 2024-05-31 12:46:05.000000 f3dasm-1.5.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-31 12:46:05.000000 f3dasm-1.5.1/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2024-05-24 09:01:59.000000 f3dasm-1.5.1/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       85 2024-05-24 09:01:59.000000 f3dasm-1.5.1/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1435 2024-05-31 12:53:48.956451 f3dasm-1.5.1/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.948451 f3dasm-1.5.1/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1481 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       27 2024-05-31 12:46:05.000000 f3dasm-1.5.1/src/f3dasm/__version__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/_argparser.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/_src/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1309 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5153 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/datagenerator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      125 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9056 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/function_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.952451 f3dasm-1.5.1/src/f3dasm/_src/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    21530 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/design/domain.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10505 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/design/parameter.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_columns.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17943 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10131 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_io.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_newdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    68077 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12635 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/experimentsample.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12662 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/samplers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/experimentdata/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/hydra_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3478 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/logger.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/src/f3dasm/_src/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1549 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/src/f3dasm/_src/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2534 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1765 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/numpy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7538 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2116 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/optimizer_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2336 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/_src/optimization/scipy_implementations.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/src/f3dasm/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      755 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      906 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/datageneration/functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      903 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-05-24 09:01:59.000000 f3dasm-1.5.1/src/f3dasm/hydra_tools.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      823 2024-05-29 13:42:22.000000 f3dasm-1.5.1/src/f3dasm/optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 12:53:48.956451 f3dasm-1.5.1/src/f3dasm.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     5331 2024-05-31 12:53:48.000000 f3dasm-1.5.1/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1967 2024-05-31 12:53:48.000000 f3dasm-1.5.1/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-31 12:53:48.000000 f3dasm-1.5.1/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      132 2024-05-31 12:53:48.000000 f3dasm-1.5.1/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-05-31 12:53:48.000000 f3dasm-1.5.1/src/f3dasm.egg-info/top_level.txt
```

### Comparing `f3dasm-1.5.0/LICENSE` & `f3dasm-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/PKG-INFO` & `f3dasm-1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.5.0
+Version: 1.5.1
 Summary: f3dasm - Framework for Data-driven Development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -39,25 +39,25 @@
 Provides-Extra: benchmark
 Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
 Requires-Dist: f3dasm_optimize; extra == "benchmark"
 
 f3dasm
 ------
 
-<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/pr/1.5/paper/f3dasm_logo_long.png" width="800"/></div>
+<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/main/paper/f3dasm_logo_long.png" width="800"/></div>
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
 
 [**Docs**](https://f3dasm.readthedocs.io/)
-| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html)
+| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 
 ## Summary
 
 Welcome to `f3dasm`, a **f**ramework for **d**ata-**d**riven **d**esign and **a**nalysis of **s**tructures and **m**aterials.
 
@@ -76,15 +76,17 @@
     - The framework includes a collection of benchmark functions, optimization algorithms and sampling strategies to get you started right away!
 
 - **Hydra integration**
     - The framework is supports the [hydra](https://hydra.cc/) configuration manager, to easily manage and run experiments.
 
 ## Getting started
 
-The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
+* Read the [overview](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) section, containing a brief introduction to the framework and a statement of need.
+* Follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) to get going!
+* Check out the [tutorials](https://f3dasm.readthedocs.io/en/latest/auto_examples/index.html) section, containing a collection of examples to get you familiar with the framework.
 
 ## Illustrative benchmarks
 
 This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies/` folder, and include the following studies:
 
 - Benchmarking optimization algorithms against well-known benchmark functions
 - 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
```

### Comparing `f3dasm-1.5.0/README.md` & `f3dasm-1.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 f3dasm
 ------
 
-<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/pr/1.5/paper/f3dasm_logo_long.png" width="800"/></div>
+<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/main/paper/f3dasm_logo_long.png" width="800"/></div>
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
 
 [**Docs**](https://f3dasm.readthedocs.io/)
-| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html)
+| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 
 ## Summary
 
 Welcome to `f3dasm`, a **f**ramework for **d**ata-**d**riven **d**esign and **a**nalysis of **s**tructures and **m**aterials.
 
@@ -34,15 +34,17 @@
     - The framework includes a collection of benchmark functions, optimization algorithms and sampling strategies to get you started right away!
 
 - **Hydra integration**
     - The framework is supports the [hydra](https://hydra.cc/) configuration manager, to easily manage and run experiments.
 
 ## Getting started
 
-The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
+* Read the [overview](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) section, containing a brief introduction to the framework and a statement of need.
+* Follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) to get going!
+* Check out the [tutorials](https://f3dasm.readthedocs.io/en/latest/auto_examples/index.html) section, containing a collection of examples to get you familiar with the framework.
 
 ## Illustrative benchmarks
 
 This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies/` folder, and include the following studies:
 
 - Benchmarking optimization algorithms against well-known benchmark functions
 - 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
@@ -59,8 +61,8 @@
 
 ## License
 
 Copyright 2024, Martin van der Schelling
 
 All rights reserved.
 
-This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
+This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
```

### Comparing `f3dasm-1.5.0/setup.cfg` & `f3dasm-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/__init__.py` & `f3dasm-1.5.1/src/f3dasm/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/_argparser.py` & `f3dasm-1.5.1/src/f3dasm/_src/_argparser.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/__init__.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/datagenerator.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/datagenerator.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/__init__.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/function.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function_factory.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/function_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/pybenchfunction.py` & `f3dasm-1.5.1/src/f3dasm/_src/datageneration/functions/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/design/domain.py` & `f3dasm-1.5.1/src/f3dasm/_src/design/domain.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/design/parameter.py` & `f3dasm-1.5.1/src/f3dasm/_src/design/parameter.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_columns.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_columns.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_data.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_data.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_io.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_io.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_jobqueue.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_jobqueue.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_newdata.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/_newdata.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentdata.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/experimentdata.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentsample.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/experimentsample.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/samplers.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/samplers.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/utils.py` & `f3dasm-1.5.1/src/f3dasm/_src/experimentdata/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/hydra_utils.py` & `f3dasm-1.5.1/src/f3dasm/_src/hydra_utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/logger.py` & `f3dasm-1.5.1/src/f3dasm/_src/logger.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/__init__.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/scipy_implementations.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/adapters/scipy_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/numpy_implementations.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/numpy_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer_factory.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/_src/optimization/scipy_implementations.py` & `f3dasm-1.5.1/src/f3dasm/_src/optimization/scipy_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/datageneration/__init__.py` & `f3dasm-1.5.1/src/f3dasm/datageneration/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/datageneration/functions.py` & `f3dasm-1.5.1/src/f3dasm/datageneration/functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/design.py` & `f3dasm-1.5.1/src/f3dasm/design.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/hydra_tools.py` & `f3dasm-1.5.1/src/f3dasm/hydra_tools.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm/optimization.py` & `f3dasm-1.5.1/src/f3dasm/optimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.5.0/src/f3dasm.egg-info/PKG-INFO` & `f3dasm-1.5.1/src/f3dasm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.5.0
+Version: 1.5.1
 Summary: f3dasm - Framework for Data-driven Development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -39,25 +39,25 @@
 Provides-Extra: benchmark
 Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
 Requires-Dist: f3dasm_optimize; extra == "benchmark"
 
 f3dasm
 ------
 
-<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/pr/1.5/paper/f3dasm_logo_long.png" width="800"/></div>
+<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/main/paper/f3dasm_logo_long.png" width="800"/></div>
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
 
 [**Docs**](https://f3dasm.readthedocs.io/)
-| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html)
+| [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 
 ## Summary
 
 Welcome to `f3dasm`, a **f**ramework for **d**ata-**d**riven **d**esign and **a**nalysis of **s**tructures and **m**aterials.
 
@@ -76,15 +76,17 @@
     - The framework includes a collection of benchmark functions, optimization algorithms and sampling strategies to get you started right away!
 
 - **Hydra integration**
     - The framework is supports the [hydra](https://hydra.cc/) configuration manager, to easily manage and run experiments.
 
 ## Getting started
 
-The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
+* Read the [overview](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) section, containing a brief introduction to the framework and a statement of need.
+* Follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/installation.html) to get going!
+* Check out the [tutorials](https://f3dasm.readthedocs.io/en/latest/auto_examples/index.html) section, containing a collection of examples to get you familiar with the framework.
 
 ## Illustrative benchmarks
 
 This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies/` folder, and include the following studies:
 
 - Benchmarking optimization algorithms against well-known benchmark functions
 - 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
```

### Comparing `f3dasm-1.5.0/src/f3dasm.egg-info/SOURCES.txt` & `f3dasm-1.5.1/src/f3dasm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

