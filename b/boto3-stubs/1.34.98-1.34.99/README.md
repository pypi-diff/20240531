# Comparing `tmp/boto3_stubs-1.34.98.tar.gz` & `tmp/boto3_stubs-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3_stubs-1.34.98.tar", last modified: Fri May  3 19:32:39 2024, max compression
+gzip compressed data, was "boto3_stubs-1.34.99.tar", last modified: Mon May  6 19:32:23 2024, max compression
```

## Comparing `boto3_stubs-1.34.98.tar` & `boto3_stubs-1.34.99.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.645256 boto3_stubs-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:31:37.000000 boto3_stubs-1.34.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-05-03 19:32:39.645256 boto3_stubs-1.34.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-05-03 19:31:37.000000 boto3_stubs-1.34.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   205730 2024-05-03 19:31:41.000000 boto3_stubs-1.34.98/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:41.000000 boto3_stubs-1.34.98/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.545255 boto3_stubs-1.34.98/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   232778 2024-05-03 19:31:45.000000 boto3_stubs-1.34.98/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:39.549255 boto3_stubs-1.34.98/boto3_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 19:32:39.000000 boto3_stubs-1.34.98/boto3_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:39.645256 boto3_stubs-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    50417 2024-05-03 19:31:36.000000 boto3_stubs-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.797556 boto3_stubs-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 19:31:55.000000 boto3_stubs-1.34.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-05-06 19:32:23.797556 boto3_stubs-1.34.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-05-06 19:31:55.000000 boto3_stubs-1.34.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.693554 boto3_stubs-1.34.99/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   205730 2024-05-06 19:31:59.000000 boto3_stubs-1.34.99/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.693554 boto3_stubs-1.34.99/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.693554 boto3_stubs-1.34.99/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.693554 boto3_stubs-1.34.99/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:31:59.000000 boto3_stubs-1.34.99/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.697554 boto3_stubs-1.34.99/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.697554 boto3_stubs-1.34.99/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   232778 2024-05-06 19:32:03.000000 boto3_stubs-1.34.99/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:23.697554 boto3_stubs-1.34.99/boto3_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 19:32:23.000000 boto3_stubs-1.34.99/boto3_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:32:23.797556 boto3_stubs-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    50417 2024-05-06 19:31:54.000000 boto3_stubs-1.34.99/setup.py
```

### Comparing `boto3_stubs-1.34.98/LICENSE` & `boto3_stubs-1.34.99/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/PKG-INFO` & `boto3_stubs-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.34.98
-Summary: Type annotations for boto3 1.34.98 generated with mypy-boto3-builder 7.24.0
+Version: 1.34.99
+Summary: Type annotations for boto3 1.34.99 generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -421,16 +421,16 @@
 Requires-Dist: mypy-boto3-dynamodb<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-ec2<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-lambda<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-rds<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-s3<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-sqs<1.35.0,>=1.34.0; extra == "essential"
 Provides-Extra: boto3
-Requires-Dist: boto3==1.34.98; extra == "boto3"
-Requires-Dist: botocore==1.34.98; extra == "boto3"
+Requires-Dist: boto3==1.34.99; extra == "boto3"
+Requires-Dist: botocore==1.34.99; extra == "boto3"
 Provides-Extra: accessanalyzer
 Requires-Dist: mypy-boto3-accessanalyzer<1.35.0,>=1.34.0; extra == "accessanalyzer"
 Provides-Extra: account
 Requires-Dist: mypy-boto3-account<1.35.0,>=1.34.0; extra == "account"
 Provides-Extra: acm
 Requires-Dist: mypy-boto3-acm<1.35.0,>=1.34.0; extra == "acm"
 Provides-Extra: acm-pca
@@ -1202,15 +1202,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/1.34.98/index.html)
+[boto3 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/1.34.99/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3_stubs-1.34.98/README.md` & `boto3_stubs-1.34.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/1.34.98/index.html)
+[boto3 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/1.34.99/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3_stubs-1.34.98/boto3-stubs/__init__.pyi` & `boto3_stubs-1.34.99/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/crt.pyi` & `boto3_stubs-1.34.99/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/docs/utils.pyi` & `boto3_stubs-1.34.99/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/dynamodb/conditions.pyi` & `boto3_stubs-1.34.99/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/dynamodb/table.pyi` & `boto3_stubs-1.34.99/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/dynamodb/transform.pyi` & `boto3_stubs-1.34.99/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/dynamodb/types.pyi` & `boto3_stubs-1.34.99/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/exceptions.pyi` & `boto3_stubs-1.34.99/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/action.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/base.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/collection.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/model.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/params.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/resources/response.pyi` & `boto3_stubs-1.34.99/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/s3/inject.pyi` & `boto3_stubs-1.34.99/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/s3/transfer.pyi` & `boto3_stubs-1.34.99/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/session.pyi` & `boto3_stubs-1.34.99/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3-stubs/utils.pyi` & `boto3_stubs-1.34.99/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3_stubs.egg-info/PKG-INFO` & `boto3_stubs-1.34.99/boto3_stubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.34.98
-Summary: Type annotations for boto3 1.34.98 generated with mypy-boto3-builder 7.24.0
+Version: 1.34.99
+Summary: Type annotations for boto3 1.34.99 generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -421,16 +421,16 @@
 Requires-Dist: mypy-boto3-dynamodb<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-ec2<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-lambda<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-rds<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-s3<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-sqs<1.35.0,>=1.34.0; extra == "essential"
 Provides-Extra: boto3
-Requires-Dist: boto3==1.34.98; extra == "boto3"
-Requires-Dist: botocore==1.34.98; extra == "boto3"
+Requires-Dist: boto3==1.34.99; extra == "boto3"
+Requires-Dist: botocore==1.34.99; extra == "boto3"
 Provides-Extra: accessanalyzer
 Requires-Dist: mypy-boto3-accessanalyzer<1.35.0,>=1.34.0; extra == "accessanalyzer"
 Provides-Extra: account
 Requires-Dist: mypy-boto3-account<1.35.0,>=1.34.0; extra == "account"
 Provides-Extra: acm
 Requires-Dist: mypy-boto3-acm<1.35.0,>=1.34.0; extra == "acm"
 Provides-Extra: acm-pca
@@ -1202,15 +1202,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/1.34.98/index.html)
+[boto3 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/1.34.99/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3_stubs-1.34.98/boto3_stubs.egg-info/SOURCES.txt` & `boto3_stubs-1.34.99/boto3_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.98/boto3_stubs.egg-info/requires.txt` & `boto3_stubs-1.34.99/boto3_stubs.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -509,16 +509,16 @@
 [bedrock-runtime]
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 
 [billingconductor]
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 
 [boto3]
-boto3==1.34.98
-botocore==1.34.98
+boto3==1.34.99
+botocore==1.34.99
 
 [braket]
 mypy-boto3-braket<1.35.0,>=1.34.0
 
 [budgets]
 mypy-boto3-budgets<1.35.0,>=1.34.0
```

### Comparing `boto3_stubs-1.34.98/setup.py` & `boto3_stubs-1.34.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs",
-    version="1.34.98",
+    version="1.34.99",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.98 generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3 1.34.99 generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -442,15 +442,15 @@
             "mypy-boto3-dynamodb>=1.34.0, <1.35.0",
             "mypy-boto3-ec2>=1.34.0, <1.35.0",
             "mypy-boto3-lambda>=1.34.0, <1.35.0",
             "mypy-boto3-rds>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-sqs>=1.34.0, <1.35.0",
         ],
-        "boto3": ["boto3==1.34.98", "botocore==1.34.98"],
+        "boto3": ["boto3==1.34.99", "botocore==1.34.99"],
         "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.34.0, <1.35.0"],
         "account": ["mypy-boto3-account>=1.34.0, <1.35.0"],
         "acm": ["mypy-boto3-acm>=1.34.0, <1.35.0"],
         "acm-pca": ["mypy-boto3-acm-pca>=1.34.0, <1.35.0"],
         "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.34.0, <1.35.0"],
         "amp": ["mypy-boto3-amp>=1.34.0, <1.35.0"],
         "amplify": ["mypy-boto3-amplify>=1.34.0, <1.35.0"],
```

