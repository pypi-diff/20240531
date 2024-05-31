# Comparing `tmp/mypy-boto3-launch-wizard-1.34.0.tar.gz` & `tmp/mypy_boto3_launch_wizard-1.34.117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-launch-wizard-1.34.0.tar", last modified: Wed Dec 13 21:23:04 2023, max compression
+gzip compressed data, was "mypy_boto3_launch_wizard-1.34.117.tar", last modified: Fri May 31 19:47:09 2024, max compression
```

## Comparing `mypy-boto3-launch-wizard-1.34.0.tar` & `mypy_boto3_launch_wizard-1.34.117.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:04.539265 mypy-boto3-launch-wizard-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2023-12-13 21:23:04.539265 mypy-boto3-launch-wizard-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:04.535265 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9822 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9447 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-12-13 21:12:48.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:04.539265 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 21:23:04.000000 mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:04.539265 mypy-boto3-launch-wizard-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-12-13 21:12:47.000000 mypy-boto3-launch-wizard-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.865631 mypy_boto3_launch_wizard-1.34.117/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-31 19:47:09.865631 mypy_boto3_launch_wizard-1.34.117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.865631 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12071 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.865631 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 19:47:09.000000 mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:47:09.865631 mypy_boto3_launch_wizard-1.34.117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-31 19:46:58.000000 mypy_boto3_launch_wizard-1.34.117/setup.py
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/LICENSE` & `mypy_boto3_launch_wizard-1.34.117/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/PKG-INFO` & `mypy_boto3_launch_wizard-1.34.117/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-launch-wizard
-Version: 1.34.0
-Summary: Type annotations for boto3.LaunchWizard 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.117
+Summary: Type annotations for boto3.LaunchWizard 1.34.117 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-launch-wizard"></a>
 
 # mypy-boto3-launch-wizard
 
 [![PyPI - mypy-boto3-launch-wizard](https://img.shields.io/pypi/v/mypy-boto3-launch-wizard.svg?color=blue)](https://pypi.org/project/mypy-boto3-launch-wizard)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-launch-wizard.svg?color=blue)](https://pypi.org/project/mypy-boto3-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-launch-wizard)](https://pepy.tech/project/mypy-boto3-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LaunchWizard 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[boto3.LaunchWizard 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-launch-wizard docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/README.md` & `mypy_boto3_launch_wizard-1.34.117/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-launch-wizard.svg?color=blue)](https://pypi.org/project/mypy-boto3-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-launch-wizard)](https://pepy.tech/project/mypy-boto3-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LaunchWizard 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[boto3.LaunchWizard 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-launch-wizard docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__init__.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListDeploymentsPaginator,
     ListWorkloadDeploymentPatternsPaginator,
     ListWorkloadsPaginator,
 )
 
 Client = LaunchWizardClient
 
-
 __all__ = (
     "Client",
     "LaunchWizardClient",
     "ListDeploymentEventsPaginator",
     "ListDeploymentsPaginator",
     "ListWorkloadDeploymentPatternsPaginator",
     "ListWorkloadsPaginator",
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__init__.pyi` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/__main__.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LaunchWizard 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.LaunchWizard 1.34.117\n"
+        "Version:         1.34.117\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.117")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/client.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,27 +26,28 @@
     ListWorkloadsPaginator,
 )
 from .type_defs import (
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentOutputTypeDef,
     DeploymentFilterTypeDef,
     GetDeploymentOutputTypeDef,
+    GetWorkloadDeploymentPatternOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ListDeploymentEventsOutputTypeDef,
     ListDeploymentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListWorkloadDeploymentPatternsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LaunchWizardClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -98,15 +99,16 @@
     def create_deployment(
         self,
         *,
         deploymentPatternName: str,
         name: str,
         specifications: Mapping[str, str],
         workloadName: str,
-        dryRun: bool = ...
+        dryRun: bool = ...,
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Creates a deployment for the given workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#create_deployment)
         """
@@ -145,14 +147,26 @@
         """
         Returns information about a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_workload)
         """
 
+    def get_workload_deployment_pattern(
+        self, *, deploymentPatternName: str, workloadName: str
+    ) -> GetWorkloadDeploymentPatternOutputTypeDef:
+        """
+        Returns details for a given workload and deployment pattern, including the
+        available
+        specifications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_workload_deployment_pattern)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_workload_deployment_pattern)
+        """
+
     def list_deployment_events(
         self, *, deploymentId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDeploymentEventsOutputTypeDef:
         """
         Lists the events of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployment_events)
@@ -160,43 +174,67 @@
         """
 
     def list_deployments(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_deployments)
         """
 
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
+        """
+        Lists the tags associated with a specified resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_tags_for_resource)
+        """
+
     def list_workload_deployment_patterns(
         self, *, workloadName: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkloadDeploymentPatternsOutputTypeDef:
         """
-        Lists the workload deployment patterns.
+        Lists the workload deployment patterns for a given workload name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workload_deployment_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_workload_deployment_patterns)
         """
 
     def list_workloads(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Lists the workloads.
+        Lists the available workload names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_workloads)
         """
 
+    def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Adds the specified tags to the given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes the specified tags from the given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#untag_resource)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_deployment_events"]
     ) -> ListDeploymentEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_paginator)
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/client.pyi` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -26,17 +26,19 @@
     ListWorkloadsPaginator,
 )
 from .type_defs import (
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentOutputTypeDef,
     DeploymentFilterTypeDef,
     GetDeploymentOutputTypeDef,
+    GetWorkloadDeploymentPatternOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ListDeploymentEventsOutputTypeDef,
     ListDeploymentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListWorkloadDeploymentPatternsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -94,15 +96,16 @@
     def create_deployment(
         self,
         *,
         deploymentPatternName: str,
         name: str,
         specifications: Mapping[str, str],
         workloadName: str,
-        dryRun: bool = ...
+        dryRun: bool = ...,
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Creates a deployment for the given workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#create_deployment)
         """
@@ -141,14 +144,26 @@
         """
         Returns information about a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_workload)
         """
 
+    def get_workload_deployment_pattern(
+        self, *, deploymentPatternName: str, workloadName: str
+    ) -> GetWorkloadDeploymentPatternOutputTypeDef:
+        """
+        Returns details for a given workload and deployment pattern, including the
+        available
+        specifications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_workload_deployment_pattern)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_workload_deployment_pattern)
+        """
+
     def list_deployment_events(
         self, *, deploymentId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDeploymentEventsOutputTypeDef:
         """
         Lists the events of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployment_events)
@@ -156,43 +171,67 @@
         """
 
     def list_deployments(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_deployments)
         """
 
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
+        """
+        Lists the tags associated with a specified resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_tags_for_resource)
+        """
+
     def list_workload_deployment_patterns(
         self, *, workloadName: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkloadDeploymentPatternsOutputTypeDef:
         """
-        Lists the workload deployment patterns.
+        Lists the workload deployment patterns for a given workload name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workload_deployment_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_workload_deployment_patterns)
         """
 
     def list_workloads(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Lists the workloads.
+        Lists the available workload names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#list_workloads)
         """
 
+    def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Adds the specified tags to the given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes the specified tags from the given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#untag_resource)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_deployment_events"]
     ) -> ListDeploymentEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/client/#get_paginator)
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/literals.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DeploymentFilterKeyType",
     "DeploymentStatusType",
     "EventStatusType",
     "ListDeploymentEventsPaginatorName",
     "ListDeploymentsPaginatorName",
     "ListWorkloadDeploymentPatternsPaginatorName",
@@ -32,15 +31,14 @@
     "WorkloadStatusType",
     "LaunchWizardServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DeploymentFilterKeyType = Literal["DEPLOYMENT_STATUS", "WORKLOAD_NAME"]
 DeploymentStatusType = Literal[
     "COMPLETED",
     "CREATING",
     "DELETED",
     "DELETE_FAILED",
     "DELETE_INITIATING",
@@ -81,14 +79,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -99,14 +98,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -124,14 +124,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -144,24 +145,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -222,15 +225,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -272,14 +274,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -302,17 +305,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -357,14 +362,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -402,19 +408,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/literals.pyi` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -97,14 +98,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -122,14 +124,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -142,24 +145,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -220,15 +225,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -270,14 +274,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -300,17 +305,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -355,14 +362,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -400,19 +408,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/paginator.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 __all__ = (
     "ListDeploymentEventsPaginator",
     "ListDeploymentsPaginator",
     "ListWorkloadDeploymentPatternsPaginator",
     "ListWorkloadsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -78,15 +77,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/paginators/#listdeploymentspaginator)
         """
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/paginator.pyi` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/paginators/#listdeploymentspaginator)
         """
 
 class ListWorkloadDeploymentPatternsPaginator(Paginator):
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/type_defs.py` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,73 +29,90 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateDeploymentInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
+    "DeploymentConditionalFieldTypeDef",
     "DeploymentDataSummaryTypeDef",
     "DeploymentDataTypeDef",
     "DeploymentEventDataSummaryTypeDef",
     "DeploymentFilterTypeDef",
     "GetDeploymentInputRequestTypeDef",
+    "GetWorkloadDeploymentPatternInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "WorkloadDataTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeploymentEventsInputRequestTypeDef",
+    "ListTagsForResourceInputRequestTypeDef",
     "ListWorkloadDeploymentPatternsInputRequestTypeDef",
     "WorkloadDeploymentPatternDataSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "WorkloadDataSummaryTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "DeploymentSpecificationsFieldTypeDef",
     "ListDeploymentsOutputTypeDef",
     "GetDeploymentOutputTypeDef",
     "ListDeploymentEventsOutputTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "GetWorkloadOutputTypeDef",
     "ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef",
     "ListWorkloadsInputListWorkloadsPaginateTypeDef",
     "ListWorkloadDeploymentPatternsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
+    "WorkloadDeploymentPatternDataTypeDef",
+    "GetWorkloadDeploymentPatternOutputTypeDef",
 )
 
 CreateDeploymentInputRequestTypeDef = TypedDict(
     "CreateDeploymentInputRequestTypeDef",
     {
         "deploymentPatternName": str,
         "name": str,
         "specifications": Mapping[str, str],
         "workloadName": str,
         "dryRun": NotRequired[bool],
+        "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteDeploymentInputRequestTypeDef = TypedDict(
     "DeleteDeploymentInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
+DeploymentConditionalFieldTypeDef = TypedDict(
+    "DeploymentConditionalFieldTypeDef",
+    {
+        "comparator": NotRequired[str],
+        "name": NotRequired[str],
+        "value": NotRequired[str],
+    },
+)
 DeploymentDataSummaryTypeDef = TypedDict(
     "DeploymentDataSummaryTypeDef",
     {
         "createdAt": NotRequired[datetime],
         "id": NotRequired[str],
         "name": NotRequired[str],
         "patternName": NotRequired[str],
@@ -104,20 +121,22 @@
     },
 )
 DeploymentDataTypeDef = TypedDict(
     "DeploymentDataTypeDef",
     {
         "createdAt": NotRequired[datetime],
         "deletedAt": NotRequired[datetime],
+        "deploymentArn": NotRequired[str],
         "id": NotRequired[str],
         "name": NotRequired[str],
         "patternName": NotRequired[str],
         "resourceGroup": NotRequired[str],
         "specifications": NotRequired[Dict[str, str]],
         "status": NotRequired[DeploymentStatusType],
+        "tags": NotRequired[Dict[str, str]],
         "workloadName": NotRequired[str],
     },
 )
 DeploymentEventDataSummaryTypeDef = TypedDict(
     "DeploymentEventDataSummaryTypeDef",
     {
         "description": NotRequired[str],
@@ -136,14 +155,21 @@
 )
 GetDeploymentInputRequestTypeDef = TypedDict(
     "GetDeploymentInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
+GetWorkloadDeploymentPatternInputRequestTypeDef = TypedDict(
+    "GetWorkloadDeploymentPatternInputRequestTypeDef",
+    {
+        "deploymentPatternName": str,
+        "workloadName": str,
+    },
+)
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "workloadName": str,
     },
 )
 WorkloadDataTypeDef = TypedDict(
@@ -170,14 +196,20 @@
     "ListDeploymentEventsInputRequestTypeDef",
     {
         "deploymentId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListTagsForResourceInputRequestTypeDef = TypedDict(
+    "ListTagsForResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
 ListWorkloadDeploymentPatternsInputRequestTypeDef = TypedDict(
     "ListWorkloadDeploymentPatternsInputRequestTypeDef",
     {
         "workloadName": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -204,14 +236,28 @@
 WorkloadDataSummaryTypeDef = TypedDict(
     "WorkloadDataSummaryTypeDef",
     {
         "displayName": NotRequired[str],
         "workloadName": NotRequired[str],
     },
 )
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Mapping[str, str],
+    },
+)
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
 CreateDeploymentOutputTypeDef = TypedDict(
     "CreateDeploymentOutputTypeDef",
     {
         "deploymentId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -219,14 +265,31 @@
     "DeleteDeploymentOutputTypeDef",
     {
         "status": DeploymentStatusType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DeploymentSpecificationsFieldTypeDef = TypedDict(
+    "DeploymentSpecificationsFieldTypeDef",
+    {
+        "allowedValues": NotRequired[List[str]],
+        "conditionals": NotRequired[List[DeploymentConditionalFieldTypeDef]],
+        "description": NotRequired[str],
+        "name": NotRequired[str],
+        "required": NotRequired[str],
+    },
+)
 ListDeploymentsOutputTypeDef = TypedDict(
     "ListDeploymentsOutputTypeDef",
     {
         "deployments": List[DeploymentDataSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -300,7 +363,27 @@
     "ListWorkloadsOutputTypeDef",
     {
         "nextToken": str,
         "workloads": List[WorkloadDataSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+WorkloadDeploymentPatternDataTypeDef = TypedDict(
+    "WorkloadDeploymentPatternDataTypeDef",
+    {
+        "deploymentPatternName": NotRequired[str],
+        "description": NotRequired[str],
+        "displayName": NotRequired[str],
+        "specifications": NotRequired[List[DeploymentSpecificationsFieldTypeDef]],
+        "status": NotRequired[WorkloadDeploymentPatternStatusType],
+        "statusMessage": NotRequired[str],
+        "workloadName": NotRequired[str],
+        "workloadVersionName": NotRequired[str],
+    },
+)
+GetWorkloadDeploymentPatternOutputTypeDef = TypedDict(
+    "GetWorkloadDeploymentPatternOutputTypeDef",
+    {
+        "workloadDeploymentPattern": WorkloadDeploymentPatternDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard/type_defs.pyi` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -33,68 +33,86 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateDeploymentInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
+    "DeploymentConditionalFieldTypeDef",
     "DeploymentDataSummaryTypeDef",
     "DeploymentDataTypeDef",
     "DeploymentEventDataSummaryTypeDef",
     "DeploymentFilterTypeDef",
     "GetDeploymentInputRequestTypeDef",
+    "GetWorkloadDeploymentPatternInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "WorkloadDataTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeploymentEventsInputRequestTypeDef",
+    "ListTagsForResourceInputRequestTypeDef",
     "ListWorkloadDeploymentPatternsInputRequestTypeDef",
     "WorkloadDeploymentPatternDataSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "WorkloadDataSummaryTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "DeploymentSpecificationsFieldTypeDef",
     "ListDeploymentsOutputTypeDef",
     "GetDeploymentOutputTypeDef",
     "ListDeploymentEventsOutputTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "GetWorkloadOutputTypeDef",
     "ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef",
     "ListWorkloadsInputListWorkloadsPaginateTypeDef",
     "ListWorkloadDeploymentPatternsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
+    "WorkloadDeploymentPatternDataTypeDef",
+    "GetWorkloadDeploymentPatternOutputTypeDef",
 )
 
 CreateDeploymentInputRequestTypeDef = TypedDict(
     "CreateDeploymentInputRequestTypeDef",
     {
         "deploymentPatternName": str,
         "name": str,
         "specifications": Mapping[str, str],
         "workloadName": str,
         "dryRun": NotRequired[bool],
+        "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteDeploymentInputRequestTypeDef = TypedDict(
     "DeleteDeploymentInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
+DeploymentConditionalFieldTypeDef = TypedDict(
+    "DeploymentConditionalFieldTypeDef",
+    {
+        "comparator": NotRequired[str],
+        "name": NotRequired[str],
+        "value": NotRequired[str],
+    },
+)
 DeploymentDataSummaryTypeDef = TypedDict(
     "DeploymentDataSummaryTypeDef",
     {
         "createdAt": NotRequired[datetime],
         "id": NotRequired[str],
         "name": NotRequired[str],
         "patternName": NotRequired[str],
@@ -103,20 +121,22 @@
     },
 )
 DeploymentDataTypeDef = TypedDict(
     "DeploymentDataTypeDef",
     {
         "createdAt": NotRequired[datetime],
         "deletedAt": NotRequired[datetime],
+        "deploymentArn": NotRequired[str],
         "id": NotRequired[str],
         "name": NotRequired[str],
         "patternName": NotRequired[str],
         "resourceGroup": NotRequired[str],
         "specifications": NotRequired[Dict[str, str]],
         "status": NotRequired[DeploymentStatusType],
+        "tags": NotRequired[Dict[str, str]],
         "workloadName": NotRequired[str],
     },
 )
 DeploymentEventDataSummaryTypeDef = TypedDict(
     "DeploymentEventDataSummaryTypeDef",
     {
         "description": NotRequired[str],
@@ -135,14 +155,21 @@
 )
 GetDeploymentInputRequestTypeDef = TypedDict(
     "GetDeploymentInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
+GetWorkloadDeploymentPatternInputRequestTypeDef = TypedDict(
+    "GetWorkloadDeploymentPatternInputRequestTypeDef",
+    {
+        "deploymentPatternName": str,
+        "workloadName": str,
+    },
+)
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "workloadName": str,
     },
 )
 WorkloadDataTypeDef = TypedDict(
@@ -169,14 +196,20 @@
     "ListDeploymentEventsInputRequestTypeDef",
     {
         "deploymentId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListTagsForResourceInputRequestTypeDef = TypedDict(
+    "ListTagsForResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
 ListWorkloadDeploymentPatternsInputRequestTypeDef = TypedDict(
     "ListWorkloadDeploymentPatternsInputRequestTypeDef",
     {
         "workloadName": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -203,14 +236,28 @@
 WorkloadDataSummaryTypeDef = TypedDict(
     "WorkloadDataSummaryTypeDef",
     {
         "displayName": NotRequired[str],
         "workloadName": NotRequired[str],
     },
 )
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Mapping[str, str],
+    },
+)
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
 CreateDeploymentOutputTypeDef = TypedDict(
     "CreateDeploymentOutputTypeDef",
     {
         "deploymentId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -218,14 +265,31 @@
     "DeleteDeploymentOutputTypeDef",
     {
         "status": DeploymentStatusType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DeploymentSpecificationsFieldTypeDef = TypedDict(
+    "DeploymentSpecificationsFieldTypeDef",
+    {
+        "allowedValues": NotRequired[List[str]],
+        "conditionals": NotRequired[List[DeploymentConditionalFieldTypeDef]],
+        "description": NotRequired[str],
+        "name": NotRequired[str],
+        "required": NotRequired[str],
+    },
+)
 ListDeploymentsOutputTypeDef = TypedDict(
     "ListDeploymentsOutputTypeDef",
     {
         "deployments": List[DeploymentDataSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -299,7 +363,27 @@
     "ListWorkloadsOutputTypeDef",
     {
         "nextToken": str,
         "workloads": List[WorkloadDataSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+WorkloadDeploymentPatternDataTypeDef = TypedDict(
+    "WorkloadDeploymentPatternDataTypeDef",
+    {
+        "deploymentPatternName": NotRequired[str],
+        "description": NotRequired[str],
+        "displayName": NotRequired[str],
+        "specifications": NotRequired[List[DeploymentSpecificationsFieldTypeDef]],
+        "status": NotRequired[WorkloadDeploymentPatternStatusType],
+        "statusMessage": NotRequired[str],
+        "workloadName": NotRequired[str],
+        "workloadVersionName": NotRequired[str],
+    },
+)
+GetWorkloadDeploymentPatternOutputTypeDef = TypedDict(
+    "GetWorkloadDeploymentPatternOutputTypeDef",
+    {
+        "workloadDeploymentPattern": WorkloadDeploymentPatternDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/PKG-INFO` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-launch-wizard
-Version: 1.34.0
-Summary: Type annotations for boto3.LaunchWizard 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.117
+Summary: Type annotations for boto3.LaunchWizard 1.34.117 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-launch-wizard"></a>
 
 # mypy-boto3-launch-wizard
 
 [![PyPI - mypy-boto3-launch-wizard](https://img.shields.io/pypi/v/mypy-boto3-launch-wizard.svg?color=blue)](https://pypi.org/project/mypy-boto3-launch-wizard)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-launch-wizard.svg?color=blue)](https://pypi.org/project/mypy-boto3-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-launch-wizard)](https://pepy.tech/project/mypy-boto3-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LaunchWizard 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[boto3.LaunchWizard 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-launch-wizard docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-launch-wizard-1.34.0/mypy_boto3_launch_wizard.egg-info/SOURCES.txt` & `mypy_boto3_launch_wizard-1.34.117/mypy_boto3_launch_wizard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-launch-wizard-1.34.0/setup.py` & `mypy_boto3_launch_wizard-1.34.117/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-launch-wizard",
-    version="1.34.0",
+    version="1.34.117",
     packages=["mypy_boto3_launch_wizard"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.LaunchWizard 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.LaunchWizard 1.34.117 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 launch-wizard type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_launch_wizard": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_launch_wizard/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

