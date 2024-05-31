# Comparing `tmp/WrenchCL-2.2.0.tar.gz` & `tmp/WrenchCL-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.2.0.tar", last modified: Mon May 20 20:01:34 2024, max compression
+gzip compressed data, was "WrenchCL-2.3.0.tar", last modified: Fri May 31 21:26:57 2024, max compression
```

## Comparing `WrenchCL-2.2.0.tar` & `WrenchCL-2.3.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.408168 WrenchCL-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-20 20:01:34.408168 WrenchCL-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Connect/AwsClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/DataFlow/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/DataFlow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/DataFlow/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/DataFlow/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/Models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL/Models/OpenAI/
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Models/OpenAI/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Models/OpenAI/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Models/OpenAI/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Models/OpenAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.408168 WrenchCL-2.2.0/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/JsonSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.408168 WrenchCL-2.2.0/WrenchCL/_Internal/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/_Internal/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/_Internal/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/_Internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 20:01:12.000000 WrenchCL-2.2.0/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:34.404168 WrenchCL-2.2.0/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-20 20:01:34.000000 WrenchCL-2.2.0/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-20 20:01:34.000000 WrenchCL-2.2.0/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:01:34.000000 WrenchCL-2.2.0/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 20:01:34.000000 WrenchCL-2.2.0/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 20:01:34.000000 WrenchCL-2.2.0/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:01:34.408168 WrenchCL-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-20 20:01:33.000000 WrenchCL-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24362 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23716 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Decorators/MultiThreaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/JsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/TypeChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31886 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 21:26:34.000000 WrenchCL-2.3.0/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:26:57.815675 WrenchCL-2.3.0/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24362 2024-05-31 21:26:57.000000 WrenchCL-2.3.0/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-31 21:26:57.000000 WrenchCL-2.3.0/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:26:57.000000 WrenchCL-2.3.0/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 21:26:57.000000 WrenchCL-2.3.0/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 21:26:57.000000 WrenchCL-2.3.0/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:26:57.819675 WrenchCL-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-31 21:26:56.000000 WrenchCL-2.3.0/setup.py
```

### Comparing `WrenchCL-2.2.0/LICENSE` & `WrenchCL-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/PKG-INFO` & `WrenchCL-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.2.0
+Version: 2.3.0
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; width: 90%; max-width: 800px;">
+    <br><br>
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
         <img alt="GitHub Workflow Status (with event)" src="https://img.shields.io/github/actions/workflow/status/WrenchAI/WrenchCL/publish-to-pypi.yml?event=push&logo=Github&label=Test%20%26%20Publish%20%F0%9F%90%8D%20to%20PyPI%20%F0%9F%93%A6">
     </a>
 </p>
 
+
 ## Description
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
 - **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
 - **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
 - **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
+
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
-Upon recieving the below error: 
+
+## Development
+
+To locally develop the plugin, clone the repository locally and make your changes.
+
+Open the console in your working directory; the building command is
 
 ```bash
-ImportError: failed to find libmagic.  Check your installation
+python setup.py sdist bdist_wheel
 ```
 
-Install the package with the optional libmagic dependency, users can using the following command:
+You can then install the package with 
 
 ```bash
-1. pip uninstall python-magic -y
-2. pip install WrenchCL[libmagic]
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall
 ```
 
+Use the `--no-dependencies flag` to reinstall quickly if there are no dependency changes
 
-# User Guides
+```bash
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies
+```
 
-Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
+<h1 align="center">Package Documentation</h1>
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AwsClientHub
+   from WrenchCL.Connect import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
-   aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
+   aws_client_hub = AwsClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
-   # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
+   # aws_client_hub = AwsClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
+   **Keyword Arguments for `AwsClientHub`**:
+   - `AWS_PROFILE` (str): AWS profile name for creating sessions.
+   - `REGION_NAME` (str): AWS region name.
+   - `SECRET_ARN` (str): ARN of the AWS Secrets Manager secret.
+   - `OPENAI_API_KEY` (str): API key for OpenAI.
+   - `SSH_SERVER` (str): SSH server address.
+   - `SSH_PORT` (int): SSH server port.
+   - `SSH_USER` (str): SSH username.
+   - `SSH_PASSWORD` (str): SSH user password.
+   - `PEM_PATH` (str): Path to the PEM file for SSH authentication.
+   - `DB_BATCH_OVERRIDE` (int): Batch size for database operations.
+   - `AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH tunnel configuration.
+
 2. **Using `RdsServiceGateway`**:
    ```python
-   from WrenchCL.Connections import RdsServiceGateway
+   from WrenchCL.Connect import RdsServiceGateway
 
    # Initialize RdsServiceGateway with the AWSClientHub instance
    rds_service = RdsServiceGateway(aws_client_hub)
 
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
@@ -155,15 +178,17 @@
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
    - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
    - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 
+
+1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
    - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
    - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
@@ -191,18 +216,14 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
-Got it! Here is the section about the custom JSON serializer in the specified format:
-
-### Custom JSON Serializer
-
 - **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
 
     ```python
     # Usage with json_dumps
     from datetime import datetime
     import json
     from WrenchCL.Tools import robust_serializer
@@ -262,15 +283,15 @@
   maybe_value = Maybe(None).len().end_maybe()
   print(result)  # Output: None
   # Does not raise an exception
   ```
 
 - **WrenchLogger**: A custom logger for advanced logging.
   ```python
-  from WrenchCL.Tools import logger
+  from WrenchCL import logger
 
   logger.info("This is an info log message", "with additional info")
   logger.error("This is an error log message", "with error details")
   ```
 
   **Non-hidden Methods in `WrenchLogger`**:
   
@@ -358,15 +379,17 @@
   
 ### Decorators
 
 WrenchCL includes several decorators for common patterns:
 
 - **Retryable**: Retries a function call if specified exceptions occur.
   ```python
-  from WrenchCL.Decorators import Retryable
+  from
+
+ WrenchCL.Decorators import Retryable
 
   @Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2)
   def might_fail():
       if random.random() < 0.5:
           raise ValueError("Random failure")
       return "Success"
 
@@ -533,7 +556,10 @@
 
 trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
     lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
     message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
+```
+
+This README includes comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as utility tools and decorators provided by the WrenchCL library. It also specifies the keyword arguments that can be passed to `AwsClientHub` and `_ConfigurationManager`.
```

#### html2text {}

```diff
@@ -1,77 +1,87 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.2.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.3.0 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
 markdown License-File: LICENSE
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
-    [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
+                                    [Logo]
+
+       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
 WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-Upon recieving the below error: ```bash ImportError: failed to find libmagic.
-Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash 1. pip uninstall
-python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
-Here's an updated and more detailed README that provides extensive instructions
-on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
-`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
-practical examples for the `Maybe` monad and other utility tools. ###
-Connecting to AWS Services To interact with AWS RDS and S3 services, follow
-these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+## Development To locally develop the plugin, clone the repository locally and
+make your changes. Open the console in your working directory; the building
+command is ```bash python setup.py sdist bdist_wheel ``` You can then install
+the package with ```bash pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-
+any.whl --force-reinstall ``` Use the `--no-dependencies flag` to reinstall
+quickly if there are no dependency changes ```bash pip install ./dist/WrenchCL-
+0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies ```
+                      ************ PPaacckkaaggee DDooccuummeennttaattiioonn ************
+### Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connect
 import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
-arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+arguments aws_client_hub = AwsClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
-= AWSClientHub(aws_profile='your_profile', region_name='your_region',
-secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
-```python from WrenchCL.Connections import RdsServiceGateway # Initialize
-RdsServiceGateway with the AWSClientHub instance rds_service =
-RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
-query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
-(data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
-accepted_type: Optional[Type] = None, none_is_ok: bool = False,
-accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
-> Optional[Any]` - Fetches data from the database based on the input query and
-parameters. - `update_database(query: str, payload: Union[dict,
-'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
-the database by executing the given query with the provided payload. 3. **Using
-`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
-Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
-S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
-bucket_name = "your-bucket-name" object_key = "path/to/your/object"
-s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
-**Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
-str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
-(bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
-object from S3 to the local file system. - `get_object_headers(bucket_name:
-str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
-`upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
-Uploads a local file to S3. - `delete_object(bucket_name: str, object_key: str)
--> None` - Deletes an object from S3. - `move_object(src_bucket_name: str,
-src_object_key: str, dst_bucket_name: str, dst_object_key: str) -> None` -
-Moves an object from one S3 location to another. - `copy_object
-(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
-dst_object_key: str) -> None` - Copies an object from one S3 location to
-another. - `rename_object(bucket_name: str, src_object_key: str,
+= AwsClientHub(aws_profile='your_profile', region_name='your_region',
+secret_arn='your_secret_arn', ...) ``` **Keyword Arguments for
+`AwsClientHub`**: - `AWS_PROFILE` (str): AWS profile name for creating
+sessions. - `REGION_NAME` (str): AWS region name. - `SECRET_ARN` (str): ARN of
+the AWS Secrets Manager secret. - `OPENAI_API_KEY` (str): API key for OpenAI. -
+`SSH_SERVER` (str): SSH server address. - `SSH_PORT` (int): SSH server port. -
+`SSH_USER` (str): SSH username. - `SSH_PASSWORD` (str): SSH user password. -
+`PEM_PATH` (str): Path to the PEM file for SSH authentication. -
+`DB_BATCH_OVERRIDE` (int): Batch size for database operations. -
+`AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH
+tunnel configuration. 2. **Using `RdsServiceGateway`**: ```python from
+WrenchCL.Connect import RdsServiceGateway # Initialize RdsServiceGateway with
+the AWSClientHub instance rds_service = RdsServiceGateway(aws_client_hub) #
+Example: Fetching data from the database query = "SELECT * FROM your_table"
+data = rds_service.get_data(query) print(data) ``` **Methods in
+`RdsServiceGateway`**: - `get_data(query: str, payload: Optional[dict] = None,
+fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type]
+= None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int],
+Optional[int]] = (None, None)) -> Optional[Any]` - Fetches data from the
+database based on the input query and parameters. - `update_database(query:
+str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] =
+None) -> None` - Updates the database by executing the given query with the
+provided payload. 3. **Using `S3ServiceGateway`**: ```python from
+WrenchCL.Connect import S3ServiceGateway # Initialize S3ServiceGateway with the
+AWSClientHub instance s3_service = S3ServiceGateway(aws_client_hub) # Example:
+Downloading an object from S3 bucket_name = "your-bucket-name" object_key =
+"path/to/your/object" s3_service.download_object(bucket_name, object_key,
+"local/path/to/save") ``` **Methods in `S3ServiceGateway`**: - `get_object
+(bucket_name: str, object_key: str) -> io.BytesIO` - Retrieves an object from
+S3. - `download_object(bucket_name: str, object_key: str, local_path: str) -
+> None` - Downloads an object from S3 to the local file system. -
+`get_object_headers(bucket_name: str, object_key: str) -> dict` - Retrieves the
+headers of an object in S3. - `upload_object(file_path: str, bucket_name: str,
+object_key: str) -> None` - Uploads a local file to S3. - `delete_object
+(bucket_name: str, object_key: str) -> None` - Deletes an object from S3. -
+`move_object(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
+dst_object_key: str) -> None` - Moves an object from one S3 location to
+another. - `copy_object(src_bucket_name: str, src_object_key: str,
+dst_bucket_name: str, dst_object_key: str) -> None` - Copies an object from one
+S3 location to another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
@@ -108,115 +118,112 @@
 to text and then generates embeddings for the text. -
 `image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
 str = "text-embedding-3-small") -> list` - Performs a vision query to
 understand an image and then generates embeddings for the response. -
 `validate_response_with_gpt(initial_response: str, validation_prompt: str) -
 > str` - Uses an initial response and validates or expands upon it with a
 secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
-for various purposes: Got it! Here is the section about the custom JSON
-serializer in the specified format: ### Custom JSON Serializer -
-**robust_serializer**: Serializes objects not natively serializable by JSON,
-including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
-with json_dumps from datetime import datetime import json from WrenchCL.Tools
-import robust_serializer print(json.dumps({"timestamp": datetime.now()},
-default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
-56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
-against expected types. ```python from WrenchCL.Tools import
-validate_input_dict params = { 'event': 'event_data', 'context':
-'context_data', 'start_time': 1625256000, 'lambda_client':
+for various purposes: - **robust_serializer**: Serializes objects not natively
+serializable by JSON, including `datetime`, `date`, `Decimal`, and custom
+objects. ```python # Usage with json_dumps from datetime import datetime import
+json from WrenchCL.Tools import robust_serializer print(json.dumps(
+{"timestamp": datetime.now()}, default=robust_serializer)) # Output:
+{"timestamp": "2024-05-17T12:34:56.789012"} ``` - **validate_input_dict**:
+Validates the input dictionary against expected types. ```python from
+WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
+'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
 file") print(file_type) ``` - **Image2B64**: A utility for encoding images to
 base64. ```python from WrenchCL.Tools import image_to_base64 image_b64 =
 image_to_base64("path/to/your/image.jpg") print(image_b64) ``` -
 **MaybeMonad**: A utility for handling nullable values with method chaining.
 ```python from WrenchCL.Tools import Maybe maybe_value = Maybe(None).len
 ().end_maybe() print(result) # Output: None # Does not raise an exception ``` -
-**WrenchLogger**: A custom logger for advanced logging. ```python from
-WrenchCL.Tools import logger logger.info("This is an info log message", "with
-additional info") logger.error("This is an error log message", "with error
-details") ``` **Non-hidden Methods in `WrenchLogger`**: #### Logging Methods -
-`info(*args: str, stack_info: Optional[bool] = False) -> None` - `context
-(*args: str, stack_info: Optional[bool] = False) -> None` - `warning(*args:
-str, stack_info: Optional[bool] = False) -> None` - `HDL_WARN(*args: str,
-stack_info: Optional[bool] = False) -> None` - `error(*args: str, stack_info:
-Optional[bool] = False) -> None` - `data(data: Any, wrap_length: Optional[int]
-= None, max_rows: Optional[int] = None, stack_info: Optional[bool] = False) -
-> None` - `HDL_ERR(*args: str, stack_info: Optional[bool] = False) -> None` -
-`RECV_ERR(*args: str, stack_info: Optional[bool] = False) -> None` - `critical
-(*args: str, stack_info: Optional[bool] = False) -> None` - `debug(*args: str,
-stack_info: Optional[bool] = False) -> None` - `start_time() -> None` -
-`log_time(message: str = "Elapsed time", format: str = "seconds", stack_info:
-Optional[bool] = False) -> None` - `header(text: str, size: int = 80, newline:
-bool = True) -> None` - `compact_header(text: str, size: int = 40) -> None`
-**Note**: The logging methods support chaining multiple string arguments. ####
-Configuration Methods - `setLevel(level: str) -> None` - Changes the reporting
-level of the logger. - `revertLoggingLevel() -> None` - Reverts the logging
-level to the previous level. - `set_file_logging(file_logging: bool) -> None` -
-Enables or disables file logging. - `set_log_file_location(new_append_mode:
-Optional[str] = None) -> None` - Changes the file append mode and optionally
-deletes the old file. #### Utility Methods - `initiate_new_run() -> None` -
-Initiates a new run with a unique run ID. - `overwrite_lambda_mode(setting:
-bool) -> None` - Sets whether the logger is running on AWS Lambda. -
-`set_global_traceback(setting: bool) -> None` - Sets whether to always include
-stack traces for errors. - `release_resources() -> None` - Releases file
-handler resources. ```python # Example usage of logger methods logger.info
-("This is an info log message", "with additional info") logger.context("This is
-a contextual log message", "with more context") logger.warning("This is a
-warning log message") logger.HDL_WARN("This is a handled warning log message")
-logger.error("This is an error log message", str(Exception("Example
-exception")), stack_info=True) data_dict = {"key": "value", "another_key": 123}
-logger.data(data_dict, wrap_length=40, max_rows=10) logger.HDL_ERR("This is a
-handled error log message") logger.RECV_ERR("This is a recoverable error log
-message", "with additional recoverable error details") logger.critical("This is
-a critical log message", "with critical details", stack_info=True) logger.debug
-("This is a debug log message", str(data_dict), stack_info=True)
-logger.start_time() # ... some operations ... logger.log_time("Processing
-time", format="formatted") logger.initiate_new_run()
-logger.overwrite_lambda_mode(setting=True) logger.set_global_traceback
-(setting=True) logger.setLevel("DEBUG") logger.header("Header Text")
-logger.compact_header("Compact Header Text") ``` - **FetchMetaData**: A utility
-to retrieve metadata from a URL or local file path. ```python from
-WrenchCL.Tools import get_metadata # Get metadata from a URL url_metadata =
-get_metadata("https://example.com/file.txt") print(url_metadata) # Output:
-{'content_type': 'text/plain', 'content_length': '1234', 'last_modified':
-datetime.datetime(2023, 5, 17, 12, 34, 56), 'url': 'https://example.com/
-file.txt'} # Get metadata from a local file file_metadata = get_metadata("/
-path/to/file.txt", is_url=False) print(file_metadata) # Output: {'file_path':
-'/path/to/file.txt', 'file_size': 1234, 'creation_time': '2023-05-17T12:34:56',
-'mime_type': 'text/plain'} ``` ### Decorators WrenchCL includes several
-decorators for common patterns: - **Retryable**: Retries a function call if
-specified exceptions occur. ```python from WrenchCL.Decorators import Retryable
-@Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2) def
-might_fail(): if random.random() < 0.5: raise ValueError("Random failure")
-return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
-Ensures a class only has one instance. ```python from WrenchCL.Decorators
-import SingletonClass @SingletonClass class MySingleton: def __init__(self):
-self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
-(instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
-taken to execute a method. ```python from WrenchCL.Decorators import
-TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
-WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `DataFlow` module. #### build_return_json Constructs
-a JSON response with a given status code and message. ```python from
-WrenchCL.DataFlow import build_return_json response = build_return_json
-(code=200, message="Success") print(response) # Output: {'statusCode': 200,
-'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
-Lambda function responses, including logging and error handling. It stops the
-Lambda function execution and returns a specified response when a
-`GuardedResponseTrigger` exception is raised. This is particularly useful for
-ensuring that the Lambda function exits immediately and returns the correct
-response, even if the exception occurs deep within nested function calls.
-Hereâs a comprehensive example demonstrating how to use
+**WrenchLogger**: A custom logger for advanced logging. ```python from WrenchCL
+import logger logger.info("This is an info log message", "with additional
+info") logger.error("This is an error log message", "with error details") ```
+**Non-hidden Methods in `WrenchLogger`**: #### Logging Methods - `info(*args:
+str, stack_info: Optional[bool] = False) -> None` - `context(*args: str,
+stack_info: Optional[bool] = False) -> None` - `warning(*args: str, stack_info:
+Optional[bool] = False) -> None` - `HDL_WARN(*args: str, stack_info: Optional
+[bool] = False) -> None` - `error(*args: str, stack_info: Optional[bool] =
+False) -> None` - `data(data: Any, wrap_length: Optional[int] = None, max_rows:
+Optional[int] = None, stack_info: Optional[bool] = False) -> None` - `HDL_ERR
+(*args: str, stack_info: Optional[bool] = False) -> None` - `RECV_ERR(*args:
+str, stack_info: Optional[bool] = False) -> None` - `critical(*args: str,
+stack_info: Optional[bool] = False) -> None` - `debug(*args: str, stack_info:
+Optional[bool] = False) -> None` - `start_time() -> None` - `log_time(message:
+str = "Elapsed time", format: str = "seconds", stack_info: Optional[bool] =
+False) -> None` - `header(text: str, size: int = 80, newline: bool = True) -
+> None` - `compact_header(text: str, size: int = 40) -> None` **Note**: The
+logging methods support chaining multiple string arguments. #### Configuration
+Methods - `setLevel(level: str) -> None` - Changes the reporting level of the
+logger. - `revertLoggingLevel() -> None` - Reverts the logging level to the
+previous level. - `set_file_logging(file_logging: bool) -> None` - Enables or
+disables file logging. - `set_log_file_location(new_append_mode: Optional[str]
+= None) -> None` - Changes the file append mode and optionally deletes the old
+file. #### Utility Methods - `initiate_new_run() -> None` - Initiates a new run
+with a unique run ID. - `overwrite_lambda_mode(setting: bool) -> None` - Sets
+whether the logger is running on AWS Lambda. - `set_global_traceback(setting:
+bool) -> None` - Sets whether to always include stack traces for errors. -
+`release_resources() -> None` - Releases file handler resources. ```python #
+Example usage of logger methods logger.info("This is an info log message",
+"with additional info") logger.context("This is a contextual log message",
+"with more context") logger.warning("This is a warning log message")
+logger.HDL_WARN("This is a handled warning log message") logger.error("This is
+an error log message", str(Exception("Example exception")), stack_info=True)
+data_dict = {"key": "value", "another_key": 123} logger.data(data_dict,
+wrap_length=40, max_rows=10) logger.HDL_ERR("This is a handled error log
+message") logger.RECV_ERR("This is a recoverable error log message", "with
+additional recoverable error details") logger.critical("This is a critical log
+message", "with critical details", stack_info=True) logger.debug("This is a
+debug log message", str(data_dict), stack_info=True) logger.start_time() # ...
+some operations ... logger.log_time("Processing time", format="formatted")
+logger.initiate_new_run() logger.overwrite_lambda_mode(setting=True)
+logger.set_global_traceback(setting=True) logger.setLevel("DEBUG")
+logger.header("Header Text") logger.compact_header("Compact Header Text") ``` -
+**FetchMetaData**: A utility to retrieve metadata from a URL or local file
+path. ```python from WrenchCL.Tools import get_metadata # Get metadata from a
+URL url_metadata = get_metadata("https://example.com/file.txt") print
+(url_metadata) # Output: {'content_type': 'text/plain', 'content_length':
+'1234', 'last_modified': datetime.datetime(2023, 5, 17, 12, 34, 56), 'url':
+'https://example.com/file.txt'} # Get metadata from a local file file_metadata
+= get_metadata("/path/to/file.txt", is_url=False) print(file_metadata) #
+Output: {'file_path': '/path/to/file.txt', 'file_size': 1234, 'creation_time':
+'2023-05-17T12:34:56', 'mime_type': 'text/plain'} ``` ### Decorators WrenchCL
+includes several decorators for common patterns: - **Retryable**: Retries a
+function call if specified exceptions occur. ```python from WrenchCL.Decorators
+import Retryable @Retryable(retry_on_exceptions=(ValueError,), max_retries=3,
+delay=2) def might_fail(): if random.random() < 0.5: raise ValueError("Random
+failure") return "Success" result = might_fail() print(result) ``` -
+**SingletonClass**: Ensures a class only has one instance. ```python from
+WrenchCL.Decorators import SingletonClass @SingletonClass class MySingleton:
+def __init__(self): self.value = 42 instance1 = MySingleton() instance2 =
+MySingleton() print(instance1 is instance2) # Output: True ``` -
+**TimedMethod**: Logs the time taken to execute a method. ```python from
+WrenchCL.Decorators import TimedMethod @TimedMethod def slow_function():
+time.sleep(2) return "Done" result = slow_function() print(result) # Output:
+"Done" ``` ### DataFlow WrenchCL includes various helper functions to assist
+with common tasks. These helpers are located in the `DataFlow` module. ####
+build_return_json Constructs a JSON response with a given status code and
+message. ```python from WrenchCL.DataFlow import build_return_json response =
+build_return_json(code=200, message="Success") print(response) # Output:
+{'statusCode': 200, 'body': '{"message": "Success"}'} ``` ####
+handle_lambda_response Handles Lambda function responses, including logging and
+error handling. It stops the Lambda function execution and returns a specified
+response when a `GuardedResponseTrigger` exception is raised. This is
+particularly useful for ensuring that the Lambda function exits immediately and
+returns the correct response, even if the exception occurs deep within nested
+function calls. Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
 import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
@@ -277,8 +284,13 @@
 purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
 trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
 additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
-refer to the documentation or contact the maintainers.
+refer to the documentation or contact the maintainers. ``` This README includes
+comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`,
+`S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as
+utility tools and decorators provided by the WrenchCL library. It also
+specifies the keyword arguments that can be passed to `AwsClientHub` and
+`_ConfigurationManager`.
```

### Comparing `WrenchCL-2.2.0/README.md` & `WrenchCL-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,78 +1,101 @@
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; width: 90%; max-width: 800px;">
+    <br><br>
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
         <img alt="GitHub Workflow Status (with event)" src="https://img.shields.io/github/actions/workflow/status/WrenchAI/WrenchCL/publish-to-pypi.yml?event=push&logo=Github&label=Test%20%26%20Publish%20%F0%9F%90%8D%20to%20PyPI%20%F0%9F%93%A6">
     </a>
 </p>
 
+
 ## Description
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
 - **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
 - **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
 - **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
+
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
-Upon recieving the below error: 
+
+## Development
+
+To locally develop the plugin, clone the repository locally and make your changes.
+
+Open the console in your working directory; the building command is
 
 ```bash
-ImportError: failed to find libmagic.  Check your installation
+python setup.py sdist bdist_wheel
 ```
 
-Install the package with the optional libmagic dependency, users can using the following command:
+You can then install the package with 
 
 ```bash
-1. pip uninstall python-magic -y
-2. pip install WrenchCL[libmagic]
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall
 ```
 
+Use the `--no-dependencies flag` to reinstall quickly if there are no dependency changes
 
-# User Guides
+```bash
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies
+```
 
-Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
+<h1 align="center">Package Documentation</h1>
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AwsClientHub
+   from WrenchCL.Connect import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
-   aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
+   aws_client_hub = AwsClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
-   # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
+   # aws_client_hub = AwsClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
+   **Keyword Arguments for `AwsClientHub`**:
+   - `AWS_PROFILE` (str): AWS profile name for creating sessions.
+   - `REGION_NAME` (str): AWS region name.
+   - `SECRET_ARN` (str): ARN of the AWS Secrets Manager secret.
+   - `OPENAI_API_KEY` (str): API key for OpenAI.
+   - `SSH_SERVER` (str): SSH server address.
+   - `SSH_PORT` (int): SSH server port.
+   - `SSH_USER` (str): SSH username.
+   - `SSH_PASSWORD` (str): SSH user password.
+   - `PEM_PATH` (str): Path to the PEM file for SSH authentication.
+   - `DB_BATCH_OVERRIDE` (int): Batch size for database operations.
+   - `AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH tunnel configuration.
+
 2. **Using `RdsServiceGateway`**:
    ```python
-   from WrenchCL.Connections import RdsServiceGateway
+   from WrenchCL.Connect import RdsServiceGateway
 
    # Initialize RdsServiceGateway with the AWSClientHub instance
    rds_service = RdsServiceGateway(aws_client_hub)
 
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
@@ -143,15 +166,17 @@
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
    - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
    - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 
+
+1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
    - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
    - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
@@ -179,18 +204,14 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
-Got it! Here is the section about the custom JSON serializer in the specified format:
-
-### Custom JSON Serializer
-
 - **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
 
     ```python
     # Usage with json_dumps
     from datetime import datetime
     import json
     from WrenchCL.Tools import robust_serializer
@@ -250,15 +271,15 @@
   maybe_value = Maybe(None).len().end_maybe()
   print(result)  # Output: None
   # Does not raise an exception
   ```
 
 - **WrenchLogger**: A custom logger for advanced logging.
   ```python
-  from WrenchCL.Tools import logger
+  from WrenchCL import logger
 
   logger.info("This is an info log message", "with additional info")
   logger.error("This is an error log message", "with error details")
   ```
 
   **Non-hidden Methods in `WrenchLogger`**:
   
@@ -346,15 +367,17 @@
   
 ### Decorators
 
 WrenchCL includes several decorators for common patterns:
 
 - **Retryable**: Retries a function call if specified exceptions occur.
   ```python
-  from WrenchCL.Decorators import Retryable
+  from
+
+ WrenchCL.Decorators import Retryable
 
   @Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2)
   def might_fail():
       if random.random() < 0.5:
           raise ValueError("Random failure")
       return "Success"
 
@@ -521,7 +544,10 @@
 
 trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
     lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
     message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
+```
+
+This README includes comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as utility tools and decorators provided by the WrenchCL library. It also specifies the keyword arguments that can be passed to `AwsClientHub` and `_ConfigurationManager`.
```

#### html2text {}

```diff
@@ -1,68 +1,78 @@
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
-    [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
+                                    [Logo]
+
+       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
 WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-Upon recieving the below error: ```bash ImportError: failed to find libmagic.
-Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash 1. pip uninstall
-python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
-Here's an updated and more detailed README that provides extensive instructions
-on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
-`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
-practical examples for the `Maybe` monad and other utility tools. ###
-Connecting to AWS Services To interact with AWS RDS and S3 services, follow
-these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+## Development To locally develop the plugin, clone the repository locally and
+make your changes. Open the console in your working directory; the building
+command is ```bash python setup.py sdist bdist_wheel ``` You can then install
+the package with ```bash pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-
+any.whl --force-reinstall ``` Use the `--no-dependencies flag` to reinstall
+quickly if there are no dependency changes ```bash pip install ./dist/WrenchCL-
+0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies ```
+                      ************ PPaacckkaaggee DDooccuummeennttaattiioonn ************
+### Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connect
 import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
-arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+arguments aws_client_hub = AwsClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
-= AWSClientHub(aws_profile='your_profile', region_name='your_region',
-secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
-```python from WrenchCL.Connections import RdsServiceGateway # Initialize
-RdsServiceGateway with the AWSClientHub instance rds_service =
-RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
-query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
-(data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
-accepted_type: Optional[Type] = None, none_is_ok: bool = False,
-accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
-> Optional[Any]` - Fetches data from the database based on the input query and
-parameters. - `update_database(query: str, payload: Union[dict,
-'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
-the database by executing the given query with the provided payload. 3. **Using
-`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
-Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
-S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
-bucket_name = "your-bucket-name" object_key = "path/to/your/object"
-s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
-**Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
-str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
-(bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
-object from S3 to the local file system. - `get_object_headers(bucket_name:
-str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
-`upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
-Uploads a local file to S3. - `delete_object(bucket_name: str, object_key: str)
--> None` - Deletes an object from S3. - `move_object(src_bucket_name: str,
-src_object_key: str, dst_bucket_name: str, dst_object_key: str) -> None` -
-Moves an object from one S3 location to another. - `copy_object
-(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
-dst_object_key: str) -> None` - Copies an object from one S3 location to
-another. - `rename_object(bucket_name: str, src_object_key: str,
+= AwsClientHub(aws_profile='your_profile', region_name='your_region',
+secret_arn='your_secret_arn', ...) ``` **Keyword Arguments for
+`AwsClientHub`**: - `AWS_PROFILE` (str): AWS profile name for creating
+sessions. - `REGION_NAME` (str): AWS region name. - `SECRET_ARN` (str): ARN of
+the AWS Secrets Manager secret. - `OPENAI_API_KEY` (str): API key for OpenAI. -
+`SSH_SERVER` (str): SSH server address. - `SSH_PORT` (int): SSH server port. -
+`SSH_USER` (str): SSH username. - `SSH_PASSWORD` (str): SSH user password. -
+`PEM_PATH` (str): Path to the PEM file for SSH authentication. -
+`DB_BATCH_OVERRIDE` (int): Batch size for database operations. -
+`AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH
+tunnel configuration. 2. **Using `RdsServiceGateway`**: ```python from
+WrenchCL.Connect import RdsServiceGateway # Initialize RdsServiceGateway with
+the AWSClientHub instance rds_service = RdsServiceGateway(aws_client_hub) #
+Example: Fetching data from the database query = "SELECT * FROM your_table"
+data = rds_service.get_data(query) print(data) ``` **Methods in
+`RdsServiceGateway`**: - `get_data(query: str, payload: Optional[dict] = None,
+fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type]
+= None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int],
+Optional[int]] = (None, None)) -> Optional[Any]` - Fetches data from the
+database based on the input query and parameters. - `update_database(query:
+str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] =
+None) -> None` - Updates the database by executing the given query with the
+provided payload. 3. **Using `S3ServiceGateway`**: ```python from
+WrenchCL.Connect import S3ServiceGateway # Initialize S3ServiceGateway with the
+AWSClientHub instance s3_service = S3ServiceGateway(aws_client_hub) # Example:
+Downloading an object from S3 bucket_name = "your-bucket-name" object_key =
+"path/to/your/object" s3_service.download_object(bucket_name, object_key,
+"local/path/to/save") ``` **Methods in `S3ServiceGateway`**: - `get_object
+(bucket_name: str, object_key: str) -> io.BytesIO` - Retrieves an object from
+S3. - `download_object(bucket_name: str, object_key: str, local_path: str) -
+> None` - Downloads an object from S3 to the local file system. -
+`get_object_headers(bucket_name: str, object_key: str) -> dict` - Retrieves the
+headers of an object in S3. - `upload_object(file_path: str, bucket_name: str,
+object_key: str) -> None` - Uploads a local file to S3. - `delete_object
+(bucket_name: str, object_key: str) -> None` - Deletes an object from S3. -
+`move_object(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
+dst_object_key: str) -> None` - Moves an object from one S3 location to
+another. - `copy_object(src_bucket_name: str, src_object_key: str,
+dst_bucket_name: str, dst_object_key: str) -> None` - Copies an object from one
+S3 location to another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
@@ -99,115 +109,112 @@
 to text and then generates embeddings for the text. -
 `image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
 str = "text-embedding-3-small") -> list` - Performs a vision query to
 understand an image and then generates embeddings for the response. -
 `validate_response_with_gpt(initial_response: str, validation_prompt: str) -
 > str` - Uses an initial response and validates or expands upon it with a
 secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
-for various purposes: Got it! Here is the section about the custom JSON
-serializer in the specified format: ### Custom JSON Serializer -
-**robust_serializer**: Serializes objects not natively serializable by JSON,
-including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
-with json_dumps from datetime import datetime import json from WrenchCL.Tools
-import robust_serializer print(json.dumps({"timestamp": datetime.now()},
-default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
-56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
-against expected types. ```python from WrenchCL.Tools import
-validate_input_dict params = { 'event': 'event_data', 'context':
-'context_data', 'start_time': 1625256000, 'lambda_client':
+for various purposes: - **robust_serializer**: Serializes objects not natively
+serializable by JSON, including `datetime`, `date`, `Decimal`, and custom
+objects. ```python # Usage with json_dumps from datetime import datetime import
+json from WrenchCL.Tools import robust_serializer print(json.dumps(
+{"timestamp": datetime.now()}, default=robust_serializer)) # Output:
+{"timestamp": "2024-05-17T12:34:56.789012"} ``` - **validate_input_dict**:
+Validates the input dictionary against expected types. ```python from
+WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
+'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
 file") print(file_type) ``` - **Image2B64**: A utility for encoding images to
 base64. ```python from WrenchCL.Tools import image_to_base64 image_b64 =
 image_to_base64("path/to/your/image.jpg") print(image_b64) ``` -
 **MaybeMonad**: A utility for handling nullable values with method chaining.
 ```python from WrenchCL.Tools import Maybe maybe_value = Maybe(None).len
 ().end_maybe() print(result) # Output: None # Does not raise an exception ``` -
-**WrenchLogger**: A custom logger for advanced logging. ```python from
-WrenchCL.Tools import logger logger.info("This is an info log message", "with
-additional info") logger.error("This is an error log message", "with error
-details") ``` **Non-hidden Methods in `WrenchLogger`**: #### Logging Methods -
-`info(*args: str, stack_info: Optional[bool] = False) -> None` - `context
-(*args: str, stack_info: Optional[bool] = False) -> None` - `warning(*args:
-str, stack_info: Optional[bool] = False) -> None` - `HDL_WARN(*args: str,
-stack_info: Optional[bool] = False) -> None` - `error(*args: str, stack_info:
-Optional[bool] = False) -> None` - `data(data: Any, wrap_length: Optional[int]
-= None, max_rows: Optional[int] = None, stack_info: Optional[bool] = False) -
-> None` - `HDL_ERR(*args: str, stack_info: Optional[bool] = False) -> None` -
-`RECV_ERR(*args: str, stack_info: Optional[bool] = False) -> None` - `critical
-(*args: str, stack_info: Optional[bool] = False) -> None` - `debug(*args: str,
-stack_info: Optional[bool] = False) -> None` - `start_time() -> None` -
-`log_time(message: str = "Elapsed time", format: str = "seconds", stack_info:
-Optional[bool] = False) -> None` - `header(text: str, size: int = 80, newline:
-bool = True) -> None` - `compact_header(text: str, size: int = 40) -> None`
-**Note**: The logging methods support chaining multiple string arguments. ####
-Configuration Methods - `setLevel(level: str) -> None` - Changes the reporting
-level of the logger. - `revertLoggingLevel() -> None` - Reverts the logging
-level to the previous level. - `set_file_logging(file_logging: bool) -> None` -
-Enables or disables file logging. - `set_log_file_location(new_append_mode:
-Optional[str] = None) -> None` - Changes the file append mode and optionally
-deletes the old file. #### Utility Methods - `initiate_new_run() -> None` -
-Initiates a new run with a unique run ID. - `overwrite_lambda_mode(setting:
-bool) -> None` - Sets whether the logger is running on AWS Lambda. -
-`set_global_traceback(setting: bool) -> None` - Sets whether to always include
-stack traces for errors. - `release_resources() -> None` - Releases file
-handler resources. ```python # Example usage of logger methods logger.info
-("This is an info log message", "with additional info") logger.context("This is
-a contextual log message", "with more context") logger.warning("This is a
-warning log message") logger.HDL_WARN("This is a handled warning log message")
-logger.error("This is an error log message", str(Exception("Example
-exception")), stack_info=True) data_dict = {"key": "value", "another_key": 123}
-logger.data(data_dict, wrap_length=40, max_rows=10) logger.HDL_ERR("This is a
-handled error log message") logger.RECV_ERR("This is a recoverable error log
-message", "with additional recoverable error details") logger.critical("This is
-a critical log message", "with critical details", stack_info=True) logger.debug
-("This is a debug log message", str(data_dict), stack_info=True)
-logger.start_time() # ... some operations ... logger.log_time("Processing
-time", format="formatted") logger.initiate_new_run()
-logger.overwrite_lambda_mode(setting=True) logger.set_global_traceback
-(setting=True) logger.setLevel("DEBUG") logger.header("Header Text")
-logger.compact_header("Compact Header Text") ``` - **FetchMetaData**: A utility
-to retrieve metadata from a URL or local file path. ```python from
-WrenchCL.Tools import get_metadata # Get metadata from a URL url_metadata =
-get_metadata("https://example.com/file.txt") print(url_metadata) # Output:
-{'content_type': 'text/plain', 'content_length': '1234', 'last_modified':
-datetime.datetime(2023, 5, 17, 12, 34, 56), 'url': 'https://example.com/
-file.txt'} # Get metadata from a local file file_metadata = get_metadata("/
-path/to/file.txt", is_url=False) print(file_metadata) # Output: {'file_path':
-'/path/to/file.txt', 'file_size': 1234, 'creation_time': '2023-05-17T12:34:56',
-'mime_type': 'text/plain'} ``` ### Decorators WrenchCL includes several
-decorators for common patterns: - **Retryable**: Retries a function call if
-specified exceptions occur. ```python from WrenchCL.Decorators import Retryable
-@Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2) def
-might_fail(): if random.random() < 0.5: raise ValueError("Random failure")
-return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
-Ensures a class only has one instance. ```python from WrenchCL.Decorators
-import SingletonClass @SingletonClass class MySingleton: def __init__(self):
-self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
-(instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
-taken to execute a method. ```python from WrenchCL.Decorators import
-TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
-WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `DataFlow` module. #### build_return_json Constructs
-a JSON response with a given status code and message. ```python from
-WrenchCL.DataFlow import build_return_json response = build_return_json
-(code=200, message="Success") print(response) # Output: {'statusCode': 200,
-'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
-Lambda function responses, including logging and error handling. It stops the
-Lambda function execution and returns a specified response when a
-`GuardedResponseTrigger` exception is raised. This is particularly useful for
-ensuring that the Lambda function exits immediately and returns the correct
-response, even if the exception occurs deep within nested function calls.
-Hereâs a comprehensive example demonstrating how to use
+**WrenchLogger**: A custom logger for advanced logging. ```python from WrenchCL
+import logger logger.info("This is an info log message", "with additional
+info") logger.error("This is an error log message", "with error details") ```
+**Non-hidden Methods in `WrenchLogger`**: #### Logging Methods - `info(*args:
+str, stack_info: Optional[bool] = False) -> None` - `context(*args: str,
+stack_info: Optional[bool] = False) -> None` - `warning(*args: str, stack_info:
+Optional[bool] = False) -> None` - `HDL_WARN(*args: str, stack_info: Optional
+[bool] = False) -> None` - `error(*args: str, stack_info: Optional[bool] =
+False) -> None` - `data(data: Any, wrap_length: Optional[int] = None, max_rows:
+Optional[int] = None, stack_info: Optional[bool] = False) -> None` - `HDL_ERR
+(*args: str, stack_info: Optional[bool] = False) -> None` - `RECV_ERR(*args:
+str, stack_info: Optional[bool] = False) -> None` - `critical(*args: str,
+stack_info: Optional[bool] = False) -> None` - `debug(*args: str, stack_info:
+Optional[bool] = False) -> None` - `start_time() -> None` - `log_time(message:
+str = "Elapsed time", format: str = "seconds", stack_info: Optional[bool] =
+False) -> None` - `header(text: str, size: int = 80, newline: bool = True) -
+> None` - `compact_header(text: str, size: int = 40) -> None` **Note**: The
+logging methods support chaining multiple string arguments. #### Configuration
+Methods - `setLevel(level: str) -> None` - Changes the reporting level of the
+logger. - `revertLoggingLevel() -> None` - Reverts the logging level to the
+previous level. - `set_file_logging(file_logging: bool) -> None` - Enables or
+disables file logging. - `set_log_file_location(new_append_mode: Optional[str]
+= None) -> None` - Changes the file append mode and optionally deletes the old
+file. #### Utility Methods - `initiate_new_run() -> None` - Initiates a new run
+with a unique run ID. - `overwrite_lambda_mode(setting: bool) -> None` - Sets
+whether the logger is running on AWS Lambda. - `set_global_traceback(setting:
+bool) -> None` - Sets whether to always include stack traces for errors. -
+`release_resources() -> None` - Releases file handler resources. ```python #
+Example usage of logger methods logger.info("This is an info log message",
+"with additional info") logger.context("This is a contextual log message",
+"with more context") logger.warning("This is a warning log message")
+logger.HDL_WARN("This is a handled warning log message") logger.error("This is
+an error log message", str(Exception("Example exception")), stack_info=True)
+data_dict = {"key": "value", "another_key": 123} logger.data(data_dict,
+wrap_length=40, max_rows=10) logger.HDL_ERR("This is a handled error log
+message") logger.RECV_ERR("This is a recoverable error log message", "with
+additional recoverable error details") logger.critical("This is a critical log
+message", "with critical details", stack_info=True) logger.debug("This is a
+debug log message", str(data_dict), stack_info=True) logger.start_time() # ...
+some operations ... logger.log_time("Processing time", format="formatted")
+logger.initiate_new_run() logger.overwrite_lambda_mode(setting=True)
+logger.set_global_traceback(setting=True) logger.setLevel("DEBUG")
+logger.header("Header Text") logger.compact_header("Compact Header Text") ``` -
+**FetchMetaData**: A utility to retrieve metadata from a URL or local file
+path. ```python from WrenchCL.Tools import get_metadata # Get metadata from a
+URL url_metadata = get_metadata("https://example.com/file.txt") print
+(url_metadata) # Output: {'content_type': 'text/plain', 'content_length':
+'1234', 'last_modified': datetime.datetime(2023, 5, 17, 12, 34, 56), 'url':
+'https://example.com/file.txt'} # Get metadata from a local file file_metadata
+= get_metadata("/path/to/file.txt", is_url=False) print(file_metadata) #
+Output: {'file_path': '/path/to/file.txt', 'file_size': 1234, 'creation_time':
+'2023-05-17T12:34:56', 'mime_type': 'text/plain'} ``` ### Decorators WrenchCL
+includes several decorators for common patterns: - **Retryable**: Retries a
+function call if specified exceptions occur. ```python from WrenchCL.Decorators
+import Retryable @Retryable(retry_on_exceptions=(ValueError,), max_retries=3,
+delay=2) def might_fail(): if random.random() < 0.5: raise ValueError("Random
+failure") return "Success" result = might_fail() print(result) ``` -
+**SingletonClass**: Ensures a class only has one instance. ```python from
+WrenchCL.Decorators import SingletonClass @SingletonClass class MySingleton:
+def __init__(self): self.value = 42 instance1 = MySingleton() instance2 =
+MySingleton() print(instance1 is instance2) # Output: True ``` -
+**TimedMethod**: Logs the time taken to execute a method. ```python from
+WrenchCL.Decorators import TimedMethod @TimedMethod def slow_function():
+time.sleep(2) return "Done" result = slow_function() print(result) # Output:
+"Done" ``` ### DataFlow WrenchCL includes various helper functions to assist
+with common tasks. These helpers are located in the `DataFlow` module. ####
+build_return_json Constructs a JSON response with a given status code and
+message. ```python from WrenchCL.DataFlow import build_return_json response =
+build_return_json(code=200, message="Success") print(response) # Output:
+{'statusCode': 200, 'body': '{"message": "Success"}'} ``` ####
+handle_lambda_response Handles Lambda function responses, including logging and
+error handling. It stops the Lambda function execution and returns a specified
+response when a `GuardedResponseTrigger` exception is raised. This is
+particularly useful for ensuring that the Lambda function exits immediately and
+returns the correct response, even if the exception occurs deep within nested
+function calls. Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
 import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
@@ -268,8 +275,13 @@
 purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
 trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
 additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
-refer to the documentation or contact the maintainers.
+refer to the documentation or contact the maintainers. ``` This README includes
+comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`,
+`S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as
+utility tools and decorators provided by the WrenchCL library. It also
+specifies the keyword arguments that can be passed to `AwsClientHub` and
+`_ConfigurationManager`.
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Connect/AwsClientHub.py` & `WrenchCL-2.3.0/WrenchCL/Connect/AwsClientHub.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,61 +31,75 @@
 @SingletonClass
 class AwsClientHub:
     """
     Manages AWS client services including RDS and S3. Ensures that client instances are created as singletons to
     maintain efficient use of resources and consistency across operations.
 
     Attributes:
-        self.config (str): _ConfigurationManager instance
+        config (_ConfigurationManager): Instance of the configuration manager.
         aws_session_client (boto3.session.Session): The AWS session client for accessing various AWS services.
         db_client (object): Client for interacting with AWS RDS databases.
         s3_client (object): Client for interacting with AWS S3 storage.
         need_ssh_tunnel (bool): Indicates if an SSH tunnel is required for database connections, based on secret data.
     """
 
-    def __init__(self, env_path=None):
+    def __init__(self, env_path=None, **kwargs):
         """
         Initializes the AwsClientHub by setting up the AWS profile and fetching necessary secrets for other
         AWS service configurations.
 
         :param env_path: The path to the environment configuration file.
         :type env_path: str, optional
+        :param kwargs: Additional keyword arguments to pass to the configuration manager.
+            - AWS_PROFILE (str): AWS profile name for creating sessions.
+            - REGION_NAME (str): AWS region name.
+            - SECRET_ARN (str): ARN of the AWS Secrets Manager secret.
+            - OPENAI_API_KEY (str): API key for OpenAI.
+            - SSH_SERVER (str): SSH server address.
+            - SSH_PORT (int): SSH server port.
+            - SSH_USER (str): SSH username.
+            - SSH_PASSWORD (str): SSH user password.
+            - PEM_PATH (str): Path to the PEM file for SSH authentication.
+            - DB_BATCH_OVERRIDE (int): Batch size for database operations.
+            - AWS_DEPLOYMENT (bool): Indicates if the deployment is on AWS, affecting SSH tunnel configuration.
         """
         self.lambda_client = None
         self.config = None
         self.aws_session_client = None
         self.db_client = None
         self.s3_client = None
         self.secret_client = None
         self.need_ssh_tunnel = False
-        self.reload_config(env_path=env_path)
+        self._kwargs = kwargs  # Store kwargs as an instance variable
+        self.reload_config(env_path=env_path, **kwargs)
         self._get_secret()
         self._initialized = True
 
-    def reload_config(self, env_path=None):
+    def reload_config(self, env_path=None, **kwargs):
         """
         Reloads the configuration from the specified environment path.
 
         :param env_path: The path to the environment configuration file.
         :type env_path: str, optional
+        :param kwargs: Additional keyword arguments to pass to the configuration manager.
         """
-        self.config = _ConfigurationManager(env_path=env_path)
+        self.config = _ConfigurationManager(env_path=env_path, **kwargs)
 
     def get_config(self):
         """
         Retrieves and returns the ConfigurationManager instance, initializing it if not already done.
 
         :returns: The initialized ConfigurationManager instance.
         :rtype: _ConfigurationManager
 
         :Usage:
             config = client_manager.get_config()
         """
         if self.config is None:
-            self.reload_config()
+            self.reload_config(**self._kwargs)  # Use stored kwargs when reloading the config
         return self.config
 
     def get_db_uri(self) -> str:
         """
         Constructs and returns the database URI from the secret configuration.
 
         :returns: The database URI.
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.3.0/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         """
         logger.debug(f"Getting headers for object: {object_key} in bucket: {bucket_name}")
         obj = self.s3_client.head_object(Bucket=bucket_name, Key=object_key)
         logger.debug(f"Headers retrieved for object: {object_key}")
         return obj
 
     @Retryable()
-    def upload_object(self, file_path, bucket_name, object_key):
+    def upload_file(self, file_path, bucket_name, object_key):
         """
         Uploads a file to S3.
 
         :param file_path: The local path of the file to be uploaded.
         :type file_path: str
         :param bucket_name: The name of the S3 bucket.
         :type bucket_name: str
@@ -106,14 +106,30 @@
         """
         logger.debug(f"Uploading file: {file_path} to bucket: {bucket_name} as object: {object_key}")
         with open(file_path, 'rb') as f:
             self.s3_client.upload_fileobj(f, bucket_name, object_key)
         logger.debug(f"File uploaded: {file_path} as object: {object_key} in bucket: {bucket_name}")
 
     @Retryable()
+    def upload_object(self, obj, bucket_name, object_key):
+        """
+        Uploads an object to S3.
+
+        :param obj: The bytes of the object to be uploaded
+        :type obj: str | bytes | IO | StreamingBody
+        :param bucket_name: The name of the S3 bucket.
+        :type bucket_name: str
+        :param object_key: The key of the object in the S3 bucket.
+        :type object_key: str
+        """
+        logger.debug(f"Uploading object to bucket: {bucket_name} as object: {object_key}")
+        self.s3_client.put_object(Body=obj, Bucket=bucket_name, Key=object_key)
+        logger.debug(f"Object uploaded as object: {object_key} in bucket: {bucket_name}")
+
+    @Retryable()
     def delete_object(self, bucket_name, object_key):
         """
         Deletes an object from S3.
 
         :param bucket_name: The name of the S3 bucket.
         :type bucket_name: str
         :param object_key: The key of the object in the S3 bucket.
```

### Comparing `WrenchCL-2.2.0/WrenchCL/DataFlow/build_return_json.py` & `WrenchCL-2.3.0/WrenchCL/DataFlow/build_return_json.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/DataFlow/handle_lambda_response.py` & `WrenchCL-2.3.0/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
-
 from boto3 import client as boto3client
 
-from ..Tools.DictValidator import validate_input_dict
+from ..Tools.TypeChecker import typechecker  # Update this to the correct import path
 from ..Tools.WrenchLogger import logger
 from .build_return_json import build_return_json
 from .trigger_dataflow_metrics import trigger_minimum_dataflow_metrics
 
 lambda_response = None
 
 
@@ -29,109 +28,122 @@
     def __init__(self, response):
         self.response = response
 
     def get_response(self):
         """
         Retrieves the response associated with this exception.
 
-        Returns:
-            dict: The response dictionary associated with this exception.
+        :returns: The response dictionary associated with this exception.
+        :rtype: dict
         """
         return self.response
 
 
 def handle_lambda_response(code, message, params, response_body=None, client_id=None, entity_id=None):
     """
     Handles the Lambda function response generation and logging based on the provided status code and message.
 
-    Args:
-        code (int): The HTTP status code to be included in the response.
-        message (str): The message to be included in the response body.
-        params (dict): A dictionary containing parameters required for further processing.
-        response_body (dict, optional): The json response body
-        client_id (str, optional): The client ID. Defaults to None.
-        entity_id (str, optional): The entity ID. Defaults to None.
-
-    Raises:
-        GuardedResponseTrigger: Custom exception to signal early exit from the Lambda function. If raised and not handled
-                                at the Lambda handler level, this exception will cause an immediate return with the
-                                generated response. If caught within nested calls, ensure to re-raise it as follows:
-                                `except GuardedResponseTrigger as e: raise e`
+    :param int code: The HTTP status code to be included in the response.
+    :param str message: The message to be included in the response body.
+    :param dict params: A dictionary containing parameters required for further processing.
+    :param dict response_body: The json response body (optional).
+    :param str client_id: The client ID (optional).
+    :param str entity_id: The entity ID (optional).
+
+    :raises GuardedResponseTrigger: Custom exception to signal early exit from the Lambda function. If raised and not handled
+        at the Lambda handler level, this exception will cause an immediate return with the generated response. If caught
+        within nested calls, ensure to re-raise it as follows:
+        ``except GuardedResponseTrigger as e: raise e``
     """
     code = int(code)
-    expected_types = {'event': str, 'context': str, 'start_time': (int, float), 'lambda_client': boto3client, }
+    expected_types = {
+        'event': str,
+        'context': str,
+        'start_time': (int, float),
+        'lambda_client': boto3client,
+    }
 
     try:
-        validate_input_dict(params, expected_types)
-        trigger_minimum_dataflow_metrics(event=params.get('event'), context=params.get('context'),
-                                         start_time=params.get('start_time'), lambda_client=params.get('lambda_client'),
-                                         job_name='Model Inference Service', job_type='Lambda', status_code=str(code),
-                                         message=str(message))
+        typechecker(params, expected_types, none_is_ok=True)
+        trigger_minimum_dataflow_metrics(
+            event=params.get('event', {}),
+            context=params.get('context', {}),
+            lambda_client=params.get('lambda_client', boto3client),
+            job_name='Model Inference Service',
+            job_type='Lambda',
+            status_code=str(code),
+            message=str(message)
+        )
     except Exception as e:
         logger.error(f"Failed to invoke dataflow metrics with error {e}")
 
-    custom_error_messages = {700: "Generic Custom Error: A fallback error for unspecified issues.",
-                             701: "Invalid Request Format: The request body does not match the expected schema.",
-                             702: "Authentication Failed: Credentials provided are invalid or expired.",
-                             703: "Authorization Denied: The authenticated user does not have permission to access the requested resource.",
-                             704: "Resource Not Found: The requested resource does not exist or is not available.",
-                             705: "Resource Locked: The resource is currently locked or in use and cannot be modified.",
-                             706: "Rate Limit Exceeded: The request has exceeded the rate limit. Try again later.",
-                             707: "Data Validation Failed: The provided data does not meet validation criteria.",
-                             708: "Dependency Error: A failure occurred in an external service or dependency.",
-                             709: "Feature Deprecated: The requested feature is no longer supported.",
-                             710: "Uncaught Expected Exit Path: The Lambda has been exited in an expected manner without successfully ending.",
-
-                             730: "Model Training Error: An error occurred during the training process of a machine learning model.",
-                             731: "Model Not Found: The specified machine learning model could not be found.",
-                             732: "Prediction Error: An Internal error occurred while making a prediction with the model.",
-                             733: "Model Update Failure: Failed to update the machine learning model.",
-                             734: "Invalid Model Input: The input data for the model is invalid or malformed.",
-                             735: "Model Deployment Error: An error occurred while deploying the machine learning model.",
-                             736: "Model Version Conflict: There is a version conflict with the machine learning model.",
-                             737: "Prediction Error: Invalid prediction provided by model.",
-                             738: "Data Value Error: Returned score does not satisfy constraints or expected range.",
-                             740: "Lambda Invocation Error: An error occurred while invoking an AWS Lambda function.",
-                             741: "Lambda Timeout: The AWS Lambda function timed out before completion.",
-                             742: "Insufficient Permissions: The AWS Lambda function does not have the necessary permissions.",
-                             743: "Cold Start Delay: Delay due to AWS Lambda cold start.",
-                             744: "API Gateway Integration Error: An error occurred in the integration between Lambda and API Gateway.",
-                             745: "Lambda Resource Limit Exceeded: The AWS Lambda function exceeded its allocated resources.",
-
-                             750: "Data Retrieval Failure: Failed to retrieve data from the database or storage.",
-                             751: "Data Save Failure: Failed to save data to the database or storage.",
-                             752: "Data Integrity Error: The data integrity check failed.",
-                             753: "Data Serialization Error: An error occurred during data serialization or deserialization.",
-                             754: "Data Version Mismatch: The version of the data does not match the expected version.",
-                             755: "Data Expiry Error: Attempted to access data that has expired or is no longer valid.",
-                             756: "Data Encryption Error: An error occurred during data encryption or decryption.",
-                             757: "Data Typing Error: An error occurred during data type coercion.",
-                             758: "Data Retrieval Rejection: The requested data already exists.",
-
-                             800: "Payment Required: The request cannot be processed without payment.",
-                             801: "Quota Exceeded: The usage quota for the service or resource has been exceeded.",
-                             802: "Duplicate Request: The same request has been received more than once.",
-                             803: "Resource Conflict: The request could not be completed due to a conflict with the current state of the resource.",
-                             804: "Precondition Failed: One or more conditions in the request header fields evaluated to false.",
-                             805: "Validation Timeout: The validation process for the request has timed out.",
-                             806: "Operation Not Allowed: The requested operation is not allowed.",
-                             807: "Data Mismatch Error: The provided data does not match the expected data.",
-                             808: "Partial Success: The operation was partially successful.",
-                             809: "Dependent Resource Unavailable: A resource that the request depends on is not available."}
+    custom_error_messages = {
+        700: "Generic Custom Error: A fallback error for unspecified issues.",
+        701: "Invalid Request Format: The request body does not match the expected schema.",
+        702: "Authentication Failed: Credentials provided are invalid or expired.",
+        703: "Authorization Denied: The authenticated user does not have permission to access the requested resource.",
+        704: "Resource Not Found: The requested resource does not exist or is not available.",
+        705: "Resource Locked: The resource is currently locked or in use and cannot be modified.",
+        706: "Rate Limit Exceeded: The request has exceeded the rate limit. Try again later.",
+        707: "Data Validation Failed: The provided data does not meet validation criteria.",
+        708: "Dependency Error: A failure occurred in an external service or dependency.",
+        709: "Feature Deprecated: The requested feature is no longer supported.",
+        710: "Uncaught Expected Exit Path: The Lambda has been exited in an expected manner without successfully ending.",
+        730: "Model Training Error: An error occurred during the training process of a machine learning model.",
+        731: "Model Not Found: The specified machine learning model could not be found.",
+        732: "Prediction Error: An Internal error occurred while making a prediction with the model.",
+        733: "Model Update Failure: Failed to update the machine learning model.",
+        734: "Invalid Model Input: The input data for the model is invalid or malformed.",
+        735: "Model Deployment Error: An error occurred while deploying the machine learning model.",
+        736: "Model Version Conflict: There is a version conflict with the machine learning model.",
+        737: "Prediction Error: Invalid prediction provided by model.",
+        738: "Data Value Error: Returned score does not satisfy constraints or expected range.",
+        740: "Lambda Invocation Error: An error occurred while invoking an AWS Lambda function.",
+        741: "Lambda Timeout: The AWS Lambda function timed out before completion.",
+        742: "Insufficient Permissions: The AWS Lambda function does not have the necessary permissions.",
+        743: "Cold Start Delay: Delay due to AWS Lambda cold start.",
+        744: "API Gateway Integration Error: An error occurred in the integration between Lambda and API Gateway.",
+        745: "Lambda Resource Limit Exceeded: The AWS Lambda function exceeded its allocated resources.",
+        750: "Data Retrieval Failure: Failed to retrieve data from the database or storage.",
+        751: "Data Save Failure: Failed to save data to the database or storage.",
+        752: "Data Integrity Error: The data integrity check failed.",
+        753: "Data Serialization Error: An error occurred during data serialization or deserialization.",
+        754: "Data Version Mismatch: The version of the data does not match the expected version.",
+        755: "Data Expiry Error: Attempted to access data that has expired or is no longer valid.",
+        756: "Data Encryption Error: An error occurred during data encryption or decryption.",
+        757: "Data Typing Error: An error occurred during data type coercion.",
+        758: "Data Retrieval Rejection: The requested data already exists.",
+        800: "Payment Required: The request cannot be processed without payment.",
+        801: "Quota Exceeded: The usage quota for the service or resource has been exceeded.",
+        802: "Duplicate Request: The same request has been received more than once.",
+        803: "Resource Conflict: The request could not be completed due to a conflict with the current state of the resource.",
+        804: "Precondition Failed: One or more conditions in the request header fields evaluated to false.",
+        805: "Validation Timeout: The validation process for the request has timed out.",
+        806: "Operation Not Allowed: The requested operation is not allowed.",
+        807: "Data Mismatch Error: The provided data does not match the expected data.",
+        808: "Partial Success: The operation was partially successful.",
+        809: "Dependent Resource Unavailable: A resource that the request depends on is not available."
+    }
 
     if code in custom_error_messages:
         logger.warning(
-            f"status code = {code} | {custom_error_messages[code]} | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
+            f"status code = {code} | {custom_error_messages[code]} | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
+        )
     elif 400 <= code < 500:
         logger.error(
-            f"status code = {code} | Un-Handled Exception Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
+            f"status code = {code} | Un-Handled Exception Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
+        )
     elif code != 200:
         logger.error(
-            f"status code = {code} | Unexpected Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
+            f"status code = {code} | Unexpected Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
+        )
     elif code == 200:
         logger.info(
-            f"status code = {code} | Success Status | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
+            f"status code = {code} | Success Status | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
+        )
 
-    response = build_return_json(code=code,
-                                 response_body=dict(Message=message) if response_body is None else response_body)
+    response = build_return_json(
+        code=code,
+        response_body=dict(Message=message) if response_body is None else response_body
+    )
     logger.context(f"Built Lambda Response: {response}")
     raise GuardedResponseTrigger(response)
```

### Comparing `WrenchCL-2.2.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py` & `WrenchCL-2.3.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,237 +9,165 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
+# Created by Jeong Kim
+# Github: https://github.com/dalmad2
+# Annotated and refactored by Willem van der Schans
+# Github: https://github.com/Kydoimos97
 
 import time
 import json
 import uuid
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 from ..Tools.WrenchLogger import logger
 
-# Created by Jeong Kim
-# Github: https://github.com/dalmad2
-# Annotated by Willem van der Schans
-# Github: https://github.com/Kydoimos97
-
-
-def trigger_minimum_dataflow_metrics(
-        event: Dict[str, Any],
-        context: Any,
-        lambda_client: Any,
-        **kwargs: Any
-) -> None:
-    """
-    Triggers the minimum dataflow metrics for a given job.
-
-    This function triggers the minimum set of dataflow metrics, capturing essential
-    information about the job execution.
-
-    Args:
-        event: Dict[str, Any]
-            The event input received by the Lambda function.
-        context: Any
-            The context object provided by AWS Lambda.
-        lambda_client: Any
-            The AWS Lambda client object.
-        kwargs: Any
-            'job_type': str
-                The type of job being executed (e.g., glue, batch, lambda, fargate).
-            'job_name': str
-                The name of the job being executed.
-            'status_code': int
-                The status code indicating the result of the job execution.
-            'client_id': str, optional
-                The client ID associated with the job.
-            'action': str, optional
-                The action performed by the job.
-            'exception_msg': str, optional
-                The exception message encountered during the job execution.
-            Additional keyword arguments can be passed to provide more detailed metrics.
-    """
-    trigger_dataflow_metrics(event=event, context=context, lambda_client=lambda_client, **kwargs)
-
 
 def trigger_dataflow_metrics(
         event: Dict[str, Any],
         context: Any,
         lambda_client: Any,
         **kwargs: Any
 ) -> None:
     """
     Triggers comprehensive dataflow metrics for a given job.
 
     This function captures comprehensive dataflow metrics related to a job execution,
     including details about resource usage, input/output counts, exception messages,
     and other relevant information.
 
-    Args:
-        event: Dict[str, Any]
-            The event input received by the Lambda function.
-        context: Any
-            The context object provided by AWS Lambda.
-        lambda_client: Any
-            The AWS Lambda client object.
-        kwargs: Any
-            Additional keyword arguments can be passed to provide more detailed metrics:
-            'job_type': str
-                The type of job being executed (e.g., glue, batch, lambda, fargate).
-            'job_name': str
-                The name of the job being executed.
-            'status_code': int
-                The status code indicating the result of the job execution.
-            'client_id': str, optional
-                The client ID associated with the job.
-            'action': str, optional
-                The action performed by the job.
-            'exception_msg': str, optional
-                The exception message encountered during the job execution.
-            'trigger': str
-                The type of job being executed (e.g., glue, batch, lambda, fargate).
-            'job_name': str
-                The name of the job being executed.
-            'state_machine_name': str
-                The name of the state machine associated with the job.
-            'state_name': str
-                The name of the state under which the job is run.
-            'workflow_id': str
-                The ID of the workflow associated with the job.
-            'job_type': str
-                The type of job being executed (e.g., glue, batch, lambda, fargate).
-            'job_run_state': str
-                The state of the job execution (e.g., 'Success', 'Failure').
-            'client_id': str
-                The client ID associated with the job.
-            'client_job_processing_datetime': str
-                The processing datetime associated with the job.
-            'job_run_started_on': str
-                The start time of the job run.
-            'duration': None
-                The duration of the job execution.
-            'bootstrap_duration': float
-                The duration of the bootstrap process.
-            'lifecycle_duration': None
-                The duration of the job lifecycle.
-            'max_memory_used': None
-                The maximum memory used during the job execution.
-            'rows_input': Any
-                The number of input rows for the job.
-            'rows_input_detail': Any
-                Additional details about the input rows.
-            'rows_output': Any
-                The number of output rows for the job.
-            'rows_output_detail': Any
-                Additional details about the output rows.
-            'uuids_input_detail': Any
-                Details about the UUIDs of input rows.
-            'uuids_output': Any
-                Details about the UUIDs of output rows.
-            'exception_msg': str
-                The exception message encountered during the job execution.
-            's3_output_path': str
-                The S3 output path for the job.
-            'rds_target_table': str
-                The target RDS table for the job.
-            'rds_input_table': str
-                The input RDS table for the job.
-            'job_id': str
-                The ID of the job.
-            'memory_limit_in_mb': int
-                The memory limit in megabytes.
-            'time_remaining_in_ms': int
-                The time remaining in milliseconds.
-            'source_id': str
-                The ID of the source service.
-            'log_stream_name': str
-                The name of the log stream.
-            'log_group_name': str
-                The name of the log group.
-            'state_entered_time': str
-                The time when the state was entered.
-            'status_code': int
-                The status code indicating the result of the job execution.
-            'message': str
-                Additional message related to the job execution.
-            'action': str
-                The action performed by the job.
+    :param event: The event input received by the Lambda function.
+    :type event: dict
+    :param context: The context object provided by AWS Lambda.
+    :type context: Any
+    :param lambda_client: The AWS Lambda client object.
+    :type lambda_client: Any
+    :param kwargs: Additional keyword arguments to provide more detailed metrics:
+        - job_type (str): The type of job being executed (e.g., glue, batch, lambda, fargate).
+        - job_name (str): The name of the job being executed.
+        - status_code (int): The status code indicating the result of the job execution.
+        - client_id (str, optional): The client ID associated with the job.
+        - action (str, optional): The action performed by the job.
+        - exception_msg (str, optional): The exception message encountered during the job execution.
+        - trigger (str): The type of job being executed (e.g., glue, batch, lambda, fargate).
+        - state_machine_name (str): The name of the state machine associated with the job.
+        - state_name (str): The name of the state under which the job is run.
+        - workflow_id (str): The ID of the workflow associated with the job.
+        - job_run_state (str): The state of the job execution (e.g., 'Success', 'Failure').
+        - client_job_processing_datetime (str): The processing datetime associated with the job.
+        - job_run_started_on (str): The start time of the job run.
+        - duration (None): The duration of the job execution.
+        - bootstrap_duration (float): The duration of the bootstrap process.
+        - lifecycle_duration (None): The duration of the job lifecycle.
+        - max_memory_used (None): The maximum memory used during the job execution.
+        - rows_input (Any): The number of input rows for the job.
+        - rows_input_detail (Any): Additional details about the input rows.
+        - rows_output (Any): The number of output rows for the job.
+        - rows_output_detail (Any): Additional details about the output rows.
+        - uuids_input_detail (Any): Details about the UUIDs of input rows.
+        - uuids_output (Any): Details about the UUIDs of output rows.
+        - s3_output_path (str): The S3 output path for the job.
+        - rds_target_table (str): The target RDS table for the job.
+        - rds_input_table (str): The input RDS table for the job.
+        - job_id (str): The ID of the job.
+        - memory_limit_in_mb (int): The memory limit in megabytes.
+        - time_remaining_in_ms (int): The time remaining in milliseconds.
+        - source_id (str): The ID of the source service.
+        - log_stream_name (str): The name of the log stream.
+        - log_group_name (str): The name of the log group.
+        - state_entered_time (str): The time when the state was entered.
+        - status_code (int): The status code indicating the result of the job execution.
+        - message (str): Additional message related to the job execution.
+        - action (str): The action performed by the job.
     """
     try:
         end_time = time.time()
-        bootstrap_duration = end_time - kwargs.get('start_time', time.time())
-
-        '''
-        Input From Lambda
-        '''
-        memory_limit_in_mb = context.memory_limit_in_mb
-        time_remaining_in_ms = context.get_remaining_time_in_millis()
-        source_id = context.aws_request_id
-        log_stream_name = context.log_stream_name
-        log_group_name = context.log_group_name
-
-        '''
-        Input From Step Function
-        '''
-        job_run_started_on = event.get('execution_starttime')
-        state_entered_time = event.get('state_enteredtime')
-        state_name = event.get('state_name')
-        workflow_id = event.get('statemachine_id')
-        state_machine_name = event.get('state_machine_name')
-
-        '''
-        Input From User Input
-        '''
-        job_id = event.get('job_id')
-        processing_datetime = event.get('processing_datetime')
-
-        job_run_state = 'Success' if kwargs.get('status_code') == 200 else None
+        bootstrap_duration = end_time - kwargs.get('start_time', end_time)
 
         performance_metrics = {
             'trigger': kwargs.get('job_type'),
             'job_name': kwargs.get('job_name'),
-            'state_machine_name': state_machine_name,
-            'state_name': state_name,
-            'workflow_id': workflow_id,
+            'state_machine_name': event.get('state_machine_name'),
+            'state_name': event.get('state_name'),
+            'workflow_id': event.get('statemachine_id'),
             'job_type': kwargs.get('job_type'),
-            'job_run_state': job_run_state,
-            'client_id': str(kwargs.get('client_id')) if isinstance(kwargs.get('client_id'), uuid.UUID) else kwargs.get(
-                'client_id'),
-            'client_job_processing_datetime': processing_datetime,
-            'job_run_started_on': job_run_started_on,
+            'job_run_state': 'Success' if kwargs.get('status_code') == 200 else 'Failure',
+            'client_id': str(kwargs.get('client_id')) if isinstance(kwargs.get('client_id'), uuid.UUID) else kwargs.get('client_id'),
+            'client_job_processing_datetime': event.get('processing_datetime'),
+            'job_run_started_on': event.get('execution_starttime'),
             'duration': None,
             'bootstrap_duration': bootstrap_duration,
             'lifecycle_duration': None,
             'max_memory_used': None,
             'rows_input': kwargs.get('rows_input'),
-            'rows_input_detail': kwargs.get('rows_input_details'),
+            'rows_input_detail': kwargs.get('rows_input_detail'),
             'rows_output': kwargs.get('rows_output'),
-            'rows_output_detail': kwargs.get('rows_output_details'),
-            'uuids_input_detail': kwargs.get('uuids_input_details'),
+            'rows_output_detail': kwargs.get('rows_output_detail'),
+            'uuids_input_detail': kwargs.get('uuids_input_detail'),
             'uuids_output': kwargs.get('uuids_output'),
             'exception_msg': kwargs.get('exception_msg'),
             's3_output_path': kwargs.get('s3_output_path'),
             'rds_target_table': kwargs.get('rds_target_table'),
             'rds_input_table': kwargs.get('rds_input_table'),
-            'job_id': job_id,
-            'memory_limit_in_mb': memory_limit_in_mb,
-            'time_remaining_in_ms': time_remaining_in_ms,
-            'source_id': source_id,
-            'log_stream_name': log_stream_name,
-            'log_group_name': log_group_name,
-            'state_entered_time': state_entered_time,
+            'job_id': event.get('job_id'),
+            'memory_limit_in_mb': getattr(context, 'memory_limit_in_mb', None),
+            'time_remaining_in_ms': getattr(context, 'get_remaining_time_in_millis', lambda: None)(),
+            'source_id': getattr(context, 'aws_request_id', None),
+            'log_stream_name': getattr(context, 'log_stream_name', None),
+            'log_group_name': getattr(context, 'log_group_name', None),
+            'state_entered_time': event.get('state_enteredtime'),
             'status_code': kwargs.get('status_code'),
             'message': kwargs.get('message'),
             'action': kwargs.get('action')
         }
 
-        performance_lambda_response = lambda_client.invoke(
+        lambda_client.invoke(
             FunctionName='dataflow-metrics',
             InvocationType='Event',
             Payload=json.dumps(performance_metrics, default=str)
         )
         logger.info('Invoked dataflow-metrics lambda')
     except Exception as e:
         logger.warning('Failed to invoke dataflow-metrics lambda')
         logger.warning(e)
+
+
+def trigger_minimum_dataflow_metrics(event: Dict[str, Any], context: Any, lambda_client: Any, job_type: str,
+        job_name: str, status_code: int, client_id: Optional[str] = None, action: Optional[str] = None,
+        exception_msg: Optional[str] = None) -> None:
+    """
+    Triggers the minimum dataflow metrics for a given job.
+
+    This function triggers the minimum set of dataflow metrics, capturing essential
+    information about the job execution.
+
+    :param event: The event input received by the Lambda function.
+    :type event: dict
+    :param context: The context object provided by AWS Lambda.
+    :type context: Any
+    :param lambda_client: The AWS Lambda client object.
+    :type lambda_client: Any
+    :param job_type: The type of job being executed (e.g., glue, batch, lambda, fargate).
+    :type job_type: str
+    :param job_name: The name of the job being executed.
+    :type job_name: str
+    :param status_code: The status code indicating the result of the job execution.
+    :type status_code: int
+    :param client_id: The client ID associated with the job (optional).
+    :type client_id: str, optional
+    :param action: The action performed by the job (optional).
+    :type action: str, optional
+    :param exception_msg: The exception message encountered during the job execution (optional).
+    :type exception_msg: str, optional
+    """
+    trigger_dataflow_metrics(event=event,
+                             context=context,
+                             lambda_client=lambda_client,
+                             job_type=job_type,
+                             job_name=job_name,
+                             status_code=status_code,
+                             client_id=client_id,
+                             action=action,
+                             exception_msg=exception_msg)
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.3.0/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.3.0/WrenchCL/Decorators/TimedMethod.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,40 +13,51 @@
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 import time
 
 from ..Tools.WrenchLogger import logger
 
-def TimedMethod(func):
+
+def TimedMethod(func, level='DEBUG'):
     """
     Decorator that logs the execution time of the decorated function. This can be useful for monitoring performance
     and identifying bottlenecks in the code.
 
     :param func: The function to be decorated.
     :type func: function
+    :param level: The logging level of the decorator
+    :type level: String ['DEBUG', 'INFO', 'CONTEXT']
     :returns: The decorated function that logs its execution time.
     :rtype: function
 
     **Example**::
 
         >>> @TimedMethod
         ... def example_function():
         ...     time.sleep(2)
         ...
         >>> example_function()  # Logs: example_function took 2.00 seconds
     """
+
     def wrapper(*args, **kwargs):
         """
         Wraps the function call to log its execution time.
 
         :param args: Positional arguments for the function.
         :param kwargs: Keyword arguments for the function.
         :returns: The result of the function call.
         """
         start = time.time()
         result = func(*args, **kwargs)
         elapsed = time.time() - start
-        logger.context(f"{func.__name__} took {elapsed:.2f} seconds")
+        log_string = f"{func.__name__} took {elapsed:.2f} seconds"
+        if level.lower() == "info":
+            logger.info(log_string)
+        elif level.lower() == "context":
+            logger.context(log_string)
+        else:
+            logger.debug(log_string)
+
         return result
 
     return wrapper
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Models/OpenAI/OpenAIFactory.py` & `WrenchCL-2.3.0/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,54 +41,58 @@
 
         :param api_key: The OpenAI API key.
         :type api_key: str
         """
         super().__init__(api_key)
 
     @TimedMethod
-    def audio_to_text_to_embeddings(self, audio_path, embedding_model="text-embedding-3-small"):
+    def audio_to_text_to_embeddings(self, audio_source, dimensions = None, embedding_model="text-embedding-3-small"):
         """
         Transcribes audio to text and then generates embeddings for the text.
 
-        :param audio_path: The path to the audio file.
-        :type audio_path: str
+        :param audio_source: The path to the audio file.
+        :type audio_source: str
+        :param dimensions: The dimension of the return vector.
+        :type dimensions: int, optional
         :param embedding_model: The model to use for generating embeddings.
         :type embedding_model: str, optional
         :returns: The generated embeddings for the transcribed text.
         :rtype: list
         """
-        transcription = self.audio_to_text(audio_path, model="whisper-1")
-        embeddings = self.get_embeddings(transcription, model=embedding_model)
+        transcription = self.audio_to_text(audio_source, model="whisper-1")
+        embeddings = self.get_embeddings(transcription, model=embedding_model, dimensions = dimensions)
         return embeddings
 
     @TimedMethod
-    def image_to_text_to_embeddings(self, image_path, question, embedding_model="text-embedding-3-small"):
+    def image_to_text_to_embeddings(self, image_source, prompt, dimensions = None, embedding_model="text-embedding-3-small", **kwargs):
         """
         Performs a vision query to understand an image and then generates embeddings for the response.
 
-        :param image_path: The path to the image file.
-        :type image_path: str
-        :param question: The question to ask about the image.
-        :type question: str
+        :param image_source: The path to the image file.
+        :type image_source: str
+        :param prompt: The question to ask about the image.
+        :type prompt: str
+        :param dimensions: The dimension of the return vector.
+        :type dimensions: int, optional
         :param embedding_model: The model to use for generating embeddings.
         :type embedding_model: str, optional
-        :returns: The generated embeddings for the vision query response.
-        :rtype: list
+        :returns: The generated embeddings for the vision query response. and the text content response
+        :rtype: tuple(list, str)
         """
-        vision_response = self.image_to_text(question, image_path)
-        embeddings = self.get_embeddings(vision_response, model=embedding_model)
-        return embeddings
+        vision_response = self.image_to_text(prompt, image_source, **kwargs)
+        embeddings = self.get_embeddings(vision_response, dimensions = dimensions, model=embedding_model)
+        return embeddings, vision_response
 
     @TimedMethod
     def validate_response_with_gpt(self, initial_response, validation_prompt):
         """
         Uses an initial response and validates or expands upon it with a secondary GPT call.
 
         :param initial_response: The initial response to validate or expand.
         :type initial_response: str
         :param validation_prompt: The prompt to use for validation or expansion.
         :type validation_prompt: str
         :returns: The validated or expanded response.
         :rtype: str
         """
-        validated_response = self.text_response(validation_prompt + initial_response)
+        validated_response = self.text_response(validation_prompt + " :  " + initial_response)
         return validated_response
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Models/OpenAI/OpenAIGateway.py` & `WrenchCL-2.3.0/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 import json
 import base64
 import os
+
+import requests
 from openai import OpenAI
 
+from ...Tools import image_to_base64,get_file_type, validate_base64
 from ...Decorators.TimedMethod import TimedMethod
 from ._ConversationManager import ConversationManager
 from ...Tools.WrenchLogger import logger
 
 
 class OpenAIGateway:
     """
@@ -96,26 +99,28 @@
             return self.generate_image_variations(image_path, **kwargs)
         elif operation == "vision" and text and image_path:
             return self.image_to_text(text, image_path, **kwargs)
         else:
             raise ValueError("Invalid or insufficient parameters for requested operation.")
 
     @TimedMethod
-    def text_response(self, text, model="gpt-3.5-turbo", system_prompt=None, image_url=None, json_mode=False, stream=False, **kwargs):
+    def text_response(self, text, model="gpt-3.5-turbo", assistant_id = None, response_format = None, system_prompt=None, json_mode=False, stream=False, **kwargs):
         """
         Processes text input using the specified model and returns the response.
 
         :param text: The text input.
         :type text: str
         :param model: The model to use for text processing.
         :type model: str, optional
+        :param response_format: (Optional) The assistant to use, will internally switch to threads (Streaming not supported)
+        :type response_format: str
+        :param response_format: (Optional) The format of the response. Possible values: { "type": "json_object" }
+        :type response_format: dict
         :param system_prompt: A system prompt to include in the request.
         :type system_prompt: str, optional
-        :param image_url: An image URL to include in the request.
-        :type image_url: str, optional
         :param json_mode: If True, expects the response to be in JSON format.
         :type json_mode: bool, optional
         :param stream: If True, stream the response as it's generated.
         :type stream: bool, optional
         :returns: The processed text or JSON response.
         :raises ValueError: If the JSON response cannot be decoded.
         :raises InterruptedError: If the response cannot be completed due to content filters or other issues.
@@ -124,34 +129,50 @@
         try:
             messages = []
 
             if system_prompt:
                 messages.append({"role": "system", "content": [{"type": "text", "text": system_prompt}]})
 
             user_content = [{"type": "text", "text": text}]
-            if image_url:
-                user_content.append({"type": "image_url", "image_url": image_url})
 
             messages.append({"role": "user", "content": user_content})
 
+            if assistant_id is not None:
+                logger.info(f"Using threads as assistant_id has been passed: {assistant_id}")
+                logger.setLevel('WARNING')
+                thread = self.client.beta.threads.create(messages = messages)
+                run = self.client.beta.threads.runs.create_and_poll(thread_id = thread.id,
+                                                                    assistant_id = assistant_id,
+                                                                    response_format = response_format,
+                                                                    model=model,
+                                                                    max_completion_tokens = kwargs.get('max_tokens', 2500))
+                messages = self.client.beta.threads.messages.list(
+                  thread_id=thread.id
+                )
+                response = messages.data[0].content[0].text.value
+                logger.revertLoggingLevel()
+                return response
             if stream:
+                logger.setLevel('WARNING')
                 response = self.client.chat.completions.create(
                     model=model,
                     messages=messages,
                     stream=True,
                     max_tokens=kwargs.get('max_tokens', 2500)
                 )
+                logger.revertLoggingLevel()
                 return response
             else:
+                logger.setLevel('WARNING')
                 response = self.client.chat.completions.create(
                     model=model,
                     messages=messages,
                     max_tokens=kwargs.get('max_tokens', 2500)
                 )
-
+                logger.revertLoggingLevel()
                 finish_reason = response.choices[0].finish_reason
                 if finish_reason == 'stop':
                     response_content = response.choices[0].message.content
                 elif finish_reason == 'length':
                     logger.warning(f"Not enough tokens available to complete message. Please increase max tokens | current setting = {kwargs.get('max_tokens', 2500)}")
                     response_content = response.choices[0].message.content
                 elif finish_reason == 'content_filter':
@@ -174,27 +195,29 @@
 
         except Exception as e:
             logger.error(f"Error processing text: {str(e)}")
             raise
 
 
     @TimedMethod
-    def get_embeddings(self, text, model="text-embedding-3-small"):
+    def get_embeddings(self, text, dimensions = 512, model="text-embedding-3-small"):
         """
         Retrieves embeddings for the given text using the specified model.
 
         :param text: The text input.
         :type text: str
         :param model: The model to use for generating embeddings.
         :type model: str, optional
+        :param dimensions: The dimension of the return vector.
+        :type dimensions: int, optional
         :returns: The generated embeddings.
         :raises Exception: If an error occurs while retrieving embeddings.
         """
         try:
-            response = self.client.embeddings.create(input=text, model=model)
+            response = self.client.embeddings.create(input=text, model=model, dimensions=dimensions)
             embeddings = response.data[0].embedding
             return embeddings
         except Exception as e:
             logger.error(f"Error getting embeddings: {str(e)}")
             raise
 
     @TimedMethod
@@ -289,58 +312,79 @@
                 response = self.client.images.edit(model="dall-e-2", image=image, mask=mask, prompt=prompt, n=n, size=size)
             return response.data[0].url
         except Exception as e:
             logger.error(f"Error editing image: {str(e)}")
             raise
 
     @TimedMethod
-    def image_to_text(self, question, image_path, **kwargs):
+    def image_to_text(self, prompt, image_source, model = 'gpt-4-turbo', max_tokens = 300, system_prompt = None, response_format = None, **kwargs):
         """
-        Processes a vision query based on the provided question and image.
+            Processes a vision query based on the provided question and image.
 
-        :param question: The question to ask.
-        :type question: str
-        :param image_path: The path to the image file.
-        :type image_path: str
-        :returns: The response to the vision query.
-        :raises Exception: If an error occurs while processing the vision query.
+            :param prompt: The question to ask.
+            :type prompt: str
+            :param image_source: The path to the image file, a URL, or a Base64-encoded string.
+            :type image_source: str
+            :param model: The name of the model to use for the vision query. Default is 'gpt-4-turbo'.
+            :type model: str
+            :param max_tokens: The maximum number of tokens to generate in the response. Default is 300.
+            :type max_tokens: int
+            :param system_prompt: (Optional) The system prompt to use for the request
+            :type system_prompt: str
+            :param response_format: (Optional) The format of the response. Possible values: { "type": "json_object" }
+            :type response_format: dict
+            :returns: The response to the vision query.
+            :rtype: str
+            :raises ValueError: If an invalid image path, URL, or Base64 string is provided.
+            :raises Exception: If an error occurs while processing the vision query.
         """
         try:
-            image_content = self.convert_image_to_url_or_base64(image_path)
-            messages = [{"role": "user", "content": [{"type": "text", "text": question},
-                                                     {"type": "image_url", "image_url": {"url": image_content}}]}]
-            response = self.client.chat.completions.create(model="gpt-4-turbo", messages=messages, max_tokens=300,
-                                                           **kwargs)
-            return response.choices[0]
+            if os.path.isfile(image_source):
+                base64_image = image_to_base64(image_source, is_url=False)
+                _, mime_type = get_file_type(image_source, is_url=False)
+                image_url = f"data:{mime_type};base64,{base64_image}"
+            elif validate_base64(image_source):
+                _, mime_type = get_file_type(image_source, is_url=False)
+                image_url = f"data:{mime_type};base64,{image_source}"
+            elif requests.get(image_source).status_code == 200:
+                base64_image = image_to_base64(image_source, is_url=True)
+                _, mime_type = get_file_type(image_source, is_url=True)
+                image_url = f"data:{mime_type};base64,{base64_image}"
+            else:
+                raise ValueError("Invalid image path, URL, or Base64 string")
+            messages = []
+            if system_prompt:
+                messages.append({"role": "system", "content": [{"type": "text", "text": system_prompt}]})
+            messages.append({
+                "role": "user",
+                "content": [
+                    {"type": "text", "text": prompt},
+                    {
+                        "type": "image_url",
+                        "image_url": {
+                            "url": image_url
+                        }
+                    }
+                ]
+            })
+            response = self.client.chat.completions.create(model=model, messages=messages, max_tokens=max_tokens, response_format=kwargs.get('response_format'))
+            return response.choices[0].message.content
         except Exception as e:
             logger.error(f"Error in vision query: {str(e)}")
             raise
 
     @TimedMethod
-    def convert_image_to_url_or_base64(self, image_path):
-        """
-        Converts an image to a URL or base64 encoded string.
-
-        :param image_path: The path to the image file.
-        :type image_path: str
-        :returns: The image URL or base64 encoded string.
-        :raises ValueError: If the image path or data is invalid.
-        :raises Exception: If an error occurs while processing the image.
-        """
-        if image_path.startswith("http://") or image_path.startswith("https://"):
-            return image_path
-        try:
-            with open(image_path, "rb") as image_file:
-                return f"data:image/jpeg;base64,{base64.b64encode(image_file.read()).decode('utf-8')}"
-        except Exception as e:
-            logger.error("Failed to process image for vision query")
-            raise ValueError("Invalid image path or data.")
-
-    @TimedMethod
     def start_conversation(self, **kwargs):
         """
         Initiates a conversation using the provided initial text.
 
         :raises Exception: If an error occurs while initiating the conversation.
         """
         conversation_manager = ConversationManager(self.client, kwargs.get("assistant_id"))
         conversation_manager.initiate_conversation()
+
+    @TimedMethod
+    def get_assistant_response(self):
+        thread_id = self.client.beta.threads.create()
+        print(thread_id)
+
+
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Models/OpenAI/_ConversationManager.py` & `WrenchCL-2.3.0/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Models/OpenAI/__init__.py` & `WrenchCL-2.3.0/WrenchCL/Models/OpenAI/__init__.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.3.0/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.3.0/WrenchCL/Tools/TypeChecker.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,59 +36,87 @@
 #
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
-from typing import Any, Dict, Type, Literal
+from typing import Any, Dict, List, Type, Union, Iterable
 from .WrenchLogger import logger
 
 
-def validate_input_dict(
-    params: Dict[str, Any],
-    expected_types: Dict[str, Type],
-    errors: Literal['raise', 'coerce'] = 'raise'
-) -> None:
+def typechecker(
+    data: Union[Dict[str, Any], List[Dict[str, Any]]],
+    expected_types: Dict[str, Union[Type, List[Type]]],
+    none_is_ok: bool = False,
+    errors: str = 'raise'
+) -> bool:
     """
-    Validates that each entry in a dictionary matches the expected type.
-
-    This function iterates through a dictionary of parameters (params) and checks
-    each value against a corresponding expected type defined in expected_types. If
-    the type does not match, the function will either raise a TypeError or attempt
-    to coerce the value to the correct type based on the 'errors' argument.
+    Validates that each entry in a dictionary or a list of dictionaries matches the expected type.
 
     Args:
-        params: A dictionary of parameters to validate, where the key is a string
-                representing the name of the parameter, and the value is the value
-                of the parameter.
-        expected_types: A dictionary mapping parameter names to the expected types.
-                        The keys should correspond to keys in 'params'.
-        errors: A string that determines the error handling strategy. If set to
-                'raise', the function will raise a TypeError when a mismatch is found.
-                If set to 'coerce', the function will attempt to coerce the value
-                to the expected type.
+        data: A dictionary or a list of dictionaries to validate.
+        expected_types: A dictionary mapping parameter names to the expected types. Each type can be a single type or a list of types.
+        none_is_ok: If True, allows None as a valid value.
+        errors: A string that determines the error handling strategy. If set to 'raise', the function will raise a TypeError when a mismatch is found.
+                If set to 'coerce', the function will attempt to coerce the value to the expected type.
 
     Raises:
-        TypeError: If any parameter does not match the expected type and 'errors'
-                   is set to 'raise'.
+        TypeError: If any parameter does not match the expected type and 'errors' is set to 'raise'.
+        ValueError: If any required parameter is missing.
+
+    Returns:
+        bool: True if the data is valid, False otherwise.
+
+    Usage example:
+        >>> from WrenchCL.Tools import typechecker
+
+        >>> data = [
+        >>>     {"name": "John", "age": 30},
+        >>>     {"name": "Jane", "age": "twenty"}
+        >>> ]
+        >>> expected_types = {"name": str, "age": int}
+
+        >>> try:
+        >>>     result = typechecker(data, expected_types, none_is_ok=False, errors='raise')
+        >>>     print("Data is valid:", result)
+        >>> except (TypeError, ValueError) as e:
+        >>>     print(f"Validation failed: {e}")
+
+        # This will raise a TypeError because the age of "Jane" is not an int
     """
-    # Check for missing parameters
-    missing_params = [param for param in expected_types if param not in params]
-    if missing_params:
-        raise ValueError(f"Missing required params: {', '.join(missing_params)}")
-
-    # Check for incorrect types
-    incorrect_types = {
-        param: type(params[param])
-        for param, expected in expected_types.items()
-        if not isinstance(params[param], expected)
-    }
-    if incorrect_types:
-        error_messages = [
-            f"'{param}' is {actual.__name__}, expected {expected_types[param].__name__}"
-            for param, actual in incorrect_types.items()
-        ]
-        if errors == 'raise':
-            raise TypeError(f"Incorrect param types: {', '.join(error_messages)}")
-        elif errors == 'coerce':
-            logger.warning(f"Invalid input found when checking input dictionary {error_messages}")
+
+    # Ensure data is iterable
+    if not isinstance(data, Iterable) or isinstance(data, (str, bytes)):
+        data = [data] if data is not None else []
+
+    for item in data:
+        # Check for incorrect types
+        for param, expected in expected_types.items():
+            logger.debug(f"Checking param: {param}, expected type(s): {expected}")
+
+            if not isinstance(item, dict):
+                item = {param: item}
+                logger.debug(f"Converted item to dict: {item}")
+
+            if none_is_ok and item.get(param) is None:
+                continue
+
+            actual_type = type(item.get(param))
+            if isinstance(expected, list):
+                if not any(isinstance(item.get(param), exp) for exp in expected):
+                    error_message = f"'{param}' is {actual_type.__name__}, expected one of {[t.__name__ for t in expected]}"
+                    if errors == 'raise':
+                        raise TypeError(f"Incorrect param types: {error_message}")
+                    elif errors == 'coerce':
+                        logger.warning(f"Invalid input found when checking input dictionary: {error_message}")
+                        return False
+            else:
+                if not isinstance(item.get(param), expected):
+                    error_message = f"'{param}' is {actual_type.__name__}, expected {expected.__name__}"
+                    if errors == 'raise':
+                        raise TypeError(f"Incorrect param types: {error_message}")
+                    elif errors == 'coerce':
+                        logger.warning(f"Invalid input found when checking input dictionary: {error_message}")
+                        return False
+
+    return True
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.3.0/WrenchCL/Tools/FetchMetaData.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.3.0/WrenchCL/Tools/FileTyper.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,45 @@
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
+import base64
 import mimetypes
+from io import BytesIO
 import requests
+from PIL import Image
+
+from .Image2B64 import validate_base64
 
 
 def get_file_type(file_source, is_url=True):
     """
-    Determine the file type of a file from a URL or file path.
+    Determine the file type of file from a URL, file path, or Base64 string.
 
-    :param file_source: URL or file path of the file
+    :param file_source: URL, file path, or Base64 string of the file
     :type file_source: str
     :param is_url: Flag indicating if the file_source is a URL, defaults to True
     :type is_url: bool, optional
     :return: File type based on extension or MIME type
     :rtype: str
     """
-    if is_url:
+    if validate_base64(file_source):
+        # Decode the Base64 string momentarily to determine the file type
+        base64_data = base64.b64decode(file_source)
+        image = Image.open(BytesIO(base64_data))
+        mime_type = Image.MIME[image.format]
+    elif is_url:
         response = requests.head(file_source)
         response.raise_for_status()
         mime_type = response.headers.get('Content-Type')
     else:
         mime_type, _ = mimetypes.guess_type(file_source)
 
     file_extension = mimetypes.guess_extension(mime_type)
-
     return file_extension, mime_type
 
 # Example usage:
 # file_type = determine_file_type("https://example.com/file.txt")
 # file_type = determine_file_type("/path/to/file.txt", is_url=False)
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.3.0/WrenchCL/Tools/Image2B64.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,42 +8,78 @@
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
-
 import base64
 import requests
+import hashlib
 from io import BytesIO
 
 
-def image_to_base64(image_source, is_url=True):
+def get_hash(data):
+    """
+    Generate SHA-1 hash for the given data.
+
+    :param data: Data in bytes
+    :return: SHA-1 hash of the data
+    :rtype: str
     """
-    Convert an image from a URL or file path to a Base64 string.
+    if isinstance(data, str):
+        data = data.encode('utf-8')
+
+
+    sha1 = hashlib.sha1()
+    sha1.update(data)
+    return sha1.hexdigest()
+
+
+def image_to_base64(image_source, is_url=True, return_hash=False):
+    """
+    Convert an image from a URL or file path to a Base64 string, optionally returning its SHA-1 hash.
 
     :param image_source: URL or file path of the image
     :type image_source: str
     :param is_url: Flag indicating if the image_source is a URL, defaults to True
     :type is_url: bool, optional
-    :return: Base64 encoded string of the image
-    :rtype: str
+    :param return_hash: Flag indicating if the SHA-1 hash of the image should be returned, defaults to False
+    :type return_hash: bool, optional
+    :return: Base64 encoded string of the image and optionally the SHA-1 hash in order
+    :rtype: str | tuple(str, str)
     """
     if is_url:
         # Handle the URL case
         response = requests.get(image_source)
         response.raise_for_status()
-        image_data = BytesIO(response.content)
+        image_data = BytesIO(response.content).getvalue()
     else:
         # Handle the file path case
         with open(image_source, "rb") as image_file:
-            image_data = BytesIO(image_file.read())
+            image_data = BytesIO(image_file.read()).getvalue()
 
     # Encode the image data to Base64
-    base64_string = base64.b64encode(image_data.getvalue()).decode('utf-8')
+    base64_string = base64.b64encode(image_data).decode('utf-8')
+
+    if return_hash:
+        image_hash = get_hash(image_data)
+        return base64_string, image_hash
 
     return base64_string
 
-# Example usage:
-# base64_str = image_to_base64("https://example.com/image.jpg")
-# base64_str = image_to_base64("/path/to/image.jpg", is_url=False)
+
+def validate_base64(b64_string):
+    """
+    Validate a Base64 encoded string.
+
+    :param b64_string: Base64 encoded string
+    :type b64_string: str
+    :return: True if the string is a valid Base64 encoded string, False otherwise
+    :rtype: bool
+    """
+    try:
+        # Decode the base64 string
+        base64.b64decode(b64_string, validate=True)
+        return True
+    except (base64.binascii.Error, ValueError):
+        return False
```

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.3.0/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.3.0/WrenchCL/Tools/WrenchLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,26 +252,28 @@
         record = self.logger.makeRecord(name=self.logger.name, level=level, fn=filepath_out, lno=line_no_out, msg=msg,
             args=None, exc_info=None, func=func_name_out, sinfo=sinfo)
         self.logger.handle(record)
 
     def _log_with_color(self, level: int, text: str, color: Optional[str] = None,
                         stack_info: Optional[bool] = False) -> None:
         indent_prefix = '  -->    '  # Custom indent prefix for new lines
-        if level <= 15:
+        if level <= 25:
             text_col = ColoramaFore.LIGHTWHITE_EX
+            text_style = ColoramaStyle.NORMAL
         else:
-            text_col = ColoramaFore.WHITE
+            text_col = ColoramaFore.RESET
+            text_style = ColoramaStyle.BRIGHT
 
         if colorama_imported and color and not self.running_on_lambda:
             # Apply color to each line and indent new lines
             lines = text.splitlines()
             colored_lines = [f"{lines[0]}"]
-            colored_lines += [f"{text_col}{indent_prefix}{line}{ColoramaStyle.RESET_ALL}" for line in lines[1:]]
+            colored_lines += [f"{text_col}{text_style}{indent_prefix}{line}{ColoramaStyle.RESET_ALL}" for line in lines[1:]]
             text = '\n'.join(colored_lines)
-            self._handlerFormat(color)
+            self._handlerFormat(color, start_empty=True)
 
         elif self.running_on_lambda:
 
             # Join lines with a separator for AWS Lambda
             text = " ".join(text.split())
             self._handlerFormat()  # Use default handler format
         else:
@@ -396,14 +398,17 @@
         elif pd and isinstance(data, pd.DataFrame):
             prefix_str = f"DataType: {type(data).__name__} | Shape: {data.shape[0]} rows | {data.shape[1]} columns"
             with pd.option_context('display.max_rows', max_rows, 'display.max_columns', None):
                 formatted_text = str(data)
         elif isinstance(data, (list, tuple, set)):
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
             formatted_text = json.dumps(serialize(data), indent=indent, default=self._custom_serializer)
+        elif isinstance(data, str):
+            prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
+            formatted_text = data
         else:
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
             formatted_text = json.dumps(serialize(data), indent=indent, default=self._custom_serializer)
 
         if not content:
             formatted_text = ""
             wrapped_text = formatted_text
@@ -417,14 +422,16 @@
         else:
             wrapped_text = formatted_text
 
         # Add color and whitespace for visual distinction
         if colorama_imported and color and not self.running_on_lambda:
             if not stack_trace:
                 final_text = f"\n{ColoramaFore.LIGHTBLUE_EX}{prefix_str}\n{ColoramaFore.LIGHTBLACK_EX}{wrapped_text}{ColoramaFore.RESET}\n"
+            if isinstance(data, str):
+                final_text = f"\n{wrapped_text}\n"
             else:
                 final_text = f"\n{ColoramaFore.LIGHTBLACK_EX}{wrapped_text}{ColoramaFore.RESET}\n"
         elif not self.running_on_lambda:
             final_text = f"\n\n{wrapped_text}\n"
         else:
             # In environments like AWS Lambda, where color might not be supported or desired
             final_text = wrapped_text
@@ -455,40 +462,40 @@
         Logs a header text, centered and separated by dashes.
 
         Parameters:
             text (str): The header text.
             size (int, optional): The width of the header. Default is 80.
             newline (bool, optional): Whether to prepend a newline before the header. Default is True.
         """
-        header = text
+        header = text if not colorama_imported else f"{ColoramaFore.CYAN}{ColoramaStyle.BRIGHT}{text}{ColoramaStyle.RESET_ALL}"
         if self.file_handler:
             self.file_handler.setFormatter(logging.Formatter(f'%(message)s'))
         self.console_handler.setFormatter(logging.Formatter(f'%(message)s'))
         if newline:
             logging.info("\n")
         logging.info(header.center(size, "-"))  # Print header centered in 80 characters
         if self.file_handler:
             self.file_handler.setFormatter(self.base_format)
         self._handlerFormat()
 
-    def _handlerFormat(self, color: Optional[str] = None) -> None:
+    def _handlerFormat(self, color: Optional[str] = None, start_empty = False) -> None:
         """
         Configures the console handler's formatter with optional color.
 
         Parameters:
             color (str, optional): The color code for colorama. Default is None.
         """
         if colorama_imported and color:
             if 'hex_color_palette' not in locals() and color != ColoramaFore.LIGHTWHITE_EX:
                 reset_var = ColoramaStyle.RESET_ALL
                 white_col = ColoramaFore.LIGHTWHITE_EX
                 format_str = f"{color}%(levelname)-8s:  [{self.run_id}] %(filename)s:%(funcName)s:%(lineno)-4d | %(asctime)s | {white_col}%(message)s {reset_var}"
             elif 'hex_color_palette' not in locals() and color == ColoramaFore.LIGHTWHITE_EX:
                 reset_var = ColoramaStyle.RESET_ALL
-                format_str = f"{color}-----%(levelname)s----- %(message)s{reset_var}"
+                format_str = f"{color}-----%(levelname)s----- %(message)s{reset_var}" if not start_empty else ''
             else:
                 reset_var = ColoramaStyle.RESET_ALL
                 white_col = ColoramaFore.RESET
                 format_str = f"{color}%(levelname)-8s: [{self.run_id}] %(filename)s:%(funcName)s:%(lineno)-4d | %(asctime)s |{reset_var} \x1b[38;20m %(message)s \x1b[0m"
         else:
             format_str = f"%(levelname)-8s: [{self.run_id}] %(filename)s:%(funcName)s:%(lineno)-4d | %(asctime)s | %(message)s"
 
@@ -688,15 +695,15 @@
                 # Convert seconds to a timedelta object, then format as days, hours, minutes, and seconds
                 td = timedelta(seconds=elapsed_time)
                 time_str = str(td)
             else:
                 self.warning("Invalid format specified for log_time(). Defaulting to seconds.")
                 time_str = f"{elapsed_time:.2f} seconds"
 
-            self.info(f"{message}: {time_str}", stack_info)
+            self.info(f"{message}: {time_str}", stack_info = stack_info)
         else:
             self.warning("Timer was not started with start_time() before calling log_time().")
 
     # Alias for log_time
     Time = log_time
```

### Comparing `WrenchCL-2.2.0/WrenchCL/_Internal/_ConfigurationManager.py` & `WrenchCL-2.3.0/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,18 @@
                           Path(os.getcwd()).joinpath('resources', 'secrets'),
                           Path(os.getcwd()).parent.joinpath('Resources', 'Secrets'),
                           Path(os.getcwd()).parent.joinpath('resources', 'secrets'),
                           Path(os.getcwd()).parent.parent.joinpath('Resources', 'Secrets'),
                           Path(os.getcwd()).parent.parent.joinpath('resources', 'secrets')]
 
         for base_path in possible_paths:
-            env_path = base_path.joinpath('.env')
+            if not str(base_path).endswith('.env'):
+                env_path = base_path.joinpath('.env')
+            else:
+                env_path = base_path
             logger.debug('Checking Path', str(env_path))
             if env_path.exists():
                 return str(env_path)
         raise FileNotFoundError("No .env file found in expected locations.")
 
     def _init_from_kwargs(self, kwargs):
         """
@@ -138,15 +141,15 @@
         :type kwargs: dict
         """
         self.aws_profile = kwargs.get('AWS_PROFILE', self.aws_profile)
         self.region_name = kwargs.get('REGION_NAME', self.region_name)
         self.secret_arn = kwargs.get('SECRET_ARN', self.secret_arn)
         self.openai_api_key = kwargs.get('OPENAI_API_KEY', self.openai_api_key)
         self.ssh_server = kwargs.get('SSH_SERVER', self.ssh_server)
-        self.ssh_port = int(kwargs.get('SSH_PORT', self.ssh_port or 0))
+        self.ssh_port = int(kwargs.get('SSH_PORT', self.ssh_port or 22))
         self.ssh_user = kwargs.get('SSH_USER', self.ssh_user)
         self.ssh_password = kwargs.get('SSH_PASSWORD', self.ssh_password)
         self.pem_path = kwargs.get('PEM_PATH', self.pem_path)
         self.db_batch_size = int(kwargs.get('DB_BATCH_OVERRIDE', self.db_batch_size or 10000))
         self.aws_deployment = str(kwargs.get('AWS_DEPLOYMENT', self.aws_deployment)).lower() == 'true'
 
     def _init_from_env(self):
@@ -154,13 +157,13 @@
         Initializes configuration values from environment variables.
         """
         self.aws_profile = os.getenv('AWS_PROFILE', self.aws_profile)
         self.region_name = os.getenv('REGION_NAME', self.region_name)
         self.secret_arn = os.getenv('SECRET_ARN', self.secret_arn)
         self.openai_api_key = os.getenv('OPENAI_API_KEY', self.openai_api_key)
         self.ssh_server = os.getenv('SSH_SERVER', self.ssh_server)
-        self.ssh_port = int(os.getenv('SSH_PORT', self.ssh_port or 0))
+        self.ssh_port = int(os.getenv('SSH_PORT', self.ssh_port or 22))
         self.ssh_user = os.getenv('SSH_USER', self.ssh_user)
         self.ssh_password = os.getenv('SSH_PASSWORD', self.ssh_password)
         self.pem_path = os.getenv('PEM_PATH', self.pem_path)
         self.db_batch_size = int(os.getenv('DB_BATCH_OVERRIDE', self.db_batch_size or 10000))
         self.aws_deployment = str(os.getenv('AWS_DEPLOYMENT', None)).lower() == 'true'
```

### Comparing `WrenchCL-2.2.0/WrenchCL/_Internal/_SshTunnelManager.py` & `WrenchCL-2.3.0/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.2.0/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.3.0/WrenchCL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.2.0
+Version: 2.3.0
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; width: 90%; max-width: 800px;">
+    <br><br>
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
         <img alt="GitHub Workflow Status (with event)" src="https://img.shields.io/github/actions/workflow/status/WrenchAI/WrenchCL/publish-to-pypi.yml?event=push&logo=Github&label=Test%20%26%20Publish%20%F0%9F%90%8D%20to%20PyPI%20%F0%9F%93%A6">
     </a>
 </p>
 
+
 ## Description
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
 - **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
 - **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
 - **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
+
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
-Upon recieving the below error: 
+
+## Development
+
+To locally develop the plugin, clone the repository locally and make your changes.
+
+Open the console in your working directory; the building command is
 
 ```bash
-ImportError: failed to find libmagic.  Check your installation
+python setup.py sdist bdist_wheel
 ```
 
-Install the package with the optional libmagic dependency, users can using the following command:
+You can then install the package with 
 
 ```bash
-1. pip uninstall python-magic -y
-2. pip install WrenchCL[libmagic]
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall
 ```
 
+Use the `--no-dependencies flag` to reinstall quickly if there are no dependency changes
 
-# User Guides
+```bash
+pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies
+```
 
-Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
+<h1 align="center">Package Documentation</h1>
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AwsClientHub
+   from WrenchCL.Connect import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
-   aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
+   aws_client_hub = AwsClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
-   # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
+   # aws_client_hub = AwsClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
+   **Keyword Arguments for `AwsClientHub`**:
+   - `AWS_PROFILE` (str): AWS profile name for creating sessions.
+   - `REGION_NAME` (str): AWS region name.
+   - `SECRET_ARN` (str): ARN of the AWS Secrets Manager secret.
+   - `OPENAI_API_KEY` (str): API key for OpenAI.
+   - `SSH_SERVER` (str): SSH server address.
+   - `SSH_PORT` (int): SSH server port.
+   - `SSH_USER` (str): SSH username.
+   - `SSH_PASSWORD` (str): SSH user password.
+   - `PEM_PATH` (str): Path to the PEM file for SSH authentication.
+   - `DB_BATCH_OVERRIDE` (int): Batch size for database operations.
+   - `AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH tunnel configuration.
+
 2. **Using `RdsServiceGateway`**:
    ```python
-   from WrenchCL.Connections import RdsServiceGateway
+   from WrenchCL.Connect import RdsServiceGateway
 
    # Initialize RdsServiceGateway with the AWSClientHub instance
    rds_service = RdsServiceGateway(aws_client_hub)
 
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
@@ -155,15 +178,17 @@
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
    - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
    - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 
+
+1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
    - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
    - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
@@ -191,18 +216,14 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
-Got it! Here is the section about the custom JSON serializer in the specified format:
-
-### Custom JSON Serializer
-
 - **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
 
     ```python
     # Usage with json_dumps
     from datetime import datetime
     import json
     from WrenchCL.Tools import robust_serializer
@@ -262,15 +283,15 @@
   maybe_value = Maybe(None).len().end_maybe()
   print(result)  # Output: None
   # Does not raise an exception
   ```
 
 - **WrenchLogger**: A custom logger for advanced logging.
   ```python
-  from WrenchCL.Tools import logger
+  from WrenchCL import logger
 
   logger.info("This is an info log message", "with additional info")
   logger.error("This is an error log message", "with error details")
   ```
 
   **Non-hidden Methods in `WrenchLogger`**:
   
@@ -358,15 +379,17 @@
   
 ### Decorators
 
 WrenchCL includes several decorators for common patterns:
 
 - **Retryable**: Retries a function call if specified exceptions occur.
   ```python
-  from WrenchCL.Decorators import Retryable
+  from
+
+ WrenchCL.Decorators import Retryable
 
   @Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2)
   def might_fail():
       if random.random() < 0.5:
           raise ValueError("Random failure")
       return "Success"
 
@@ -533,7 +556,10 @@
 
 trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
     lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
     message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
+```
+
+This README includes comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as utility tools and decorators provided by the WrenchCL library. It also specifies the keyword arguments that can be passed to `AwsClientHub` and `_ConfigurationManager`.
```

#### html2text {}

```diff
@@ -1,77 +1,87 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.2.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.3.0 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
 markdown License-File: LICENSE
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
-    [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
+                                    [Logo]
+
+       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
 WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-Upon recieving the below error: ```bash ImportError: failed to find libmagic.
-Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash 1. pip uninstall
-python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
-Here's an updated and more detailed README that provides extensive instructions
-on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
-`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
-practical examples for the `Maybe` monad and other utility tools. ###
-Connecting to AWS Services To interact with AWS RDS and S3 services, follow
-these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+## Development To locally develop the plugin, clone the repository locally and
+make your changes. Open the console in your working directory; the building
+command is ```bash python setup.py sdist bdist_wheel ``` You can then install
+the package with ```bash pip install ./dist/WrenchCL-0.0.1.dev0-py3-none-
+any.whl --force-reinstall ``` Use the `--no-dependencies flag` to reinstall
+quickly if there are no dependency changes ```bash pip install ./dist/WrenchCL-
+0.0.1.dev0-py3-none-any.whl --force-reinstall --no-dependencies ```
+                      ************ PPaacckkaaggee DDooccuummeennttaattiioonn ************
+### Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connect
 import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
-arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+arguments aws_client_hub = AwsClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
-= AWSClientHub(aws_profile='your_profile', region_name='your_region',
-secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
-```python from WrenchCL.Connections import RdsServiceGateway # Initialize
-RdsServiceGateway with the AWSClientHub instance rds_service =
-RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
-query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
-(data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
-accepted_type: Optional[Type] = None, none_is_ok: bool = False,
-accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
-> Optional[Any]` - Fetches data from the database based on the input query and
-parameters. - `update_database(query: str, payload: Union[dict,
-'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
-the database by executing the given query with the provided payload. 3. **Using
-`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
-Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
-S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
-bucket_name = "your-bucket-name" object_key = "path/to/your/object"
-s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
-**Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
-str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
-(bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
-object from S3 to the local file system. - `get_object_headers(bucket_name:
-str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
-`upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
-Uploads a local file to S3. - `delete_object(bucket_name: str, object_key: str)
--> None` - Deletes an object from S3. - `move_object(src_bucket_name: str,
-src_object_key: str, dst_bucket_name: str, dst_object_key: str) -> None` -
-Moves an object from one S3 location to another. - `copy_object
-(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
-dst_object_key: str) -> None` - Copies an object from one S3 location to
-another. - `rename_object(bucket_name: str, src_object_key: str,
+= AwsClientHub(aws_profile='your_profile', region_name='your_region',
+secret_arn='your_secret_arn', ...) ``` **Keyword Arguments for
+`AwsClientHub`**: - `AWS_PROFILE` (str): AWS profile name for creating
+sessions. - `REGION_NAME` (str): AWS region name. - `SECRET_ARN` (str): ARN of
+the AWS Secrets Manager secret. - `OPENAI_API_KEY` (str): API key for OpenAI. -
+`SSH_SERVER` (str): SSH server address. - `SSH_PORT` (int): SSH server port. -
+`SSH_USER` (str): SSH username. - `SSH_PASSWORD` (str): SSH user password. -
+`PEM_PATH` (str): Path to the PEM file for SSH authentication. -
+`DB_BATCH_OVERRIDE` (int): Batch size for database operations. -
+`AWS_DEPLOYMENT` (bool): Indicates if the deployment is on AWS, affecting SSH
+tunnel configuration. 2. **Using `RdsServiceGateway`**: ```python from
+WrenchCL.Connect import RdsServiceGateway # Initialize RdsServiceGateway with
+the AWSClientHub instance rds_service = RdsServiceGateway(aws_client_hub) #
+Example: Fetching data from the database query = "SELECT * FROM your_table"
+data = rds_service.get_data(query) print(data) ``` **Methods in
+`RdsServiceGateway`**: - `get_data(query: str, payload: Optional[dict] = None,
+fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type]
+= None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int],
+Optional[int]] = (None, None)) -> Optional[Any]` - Fetches data from the
+database based on the input query and parameters. - `update_database(query:
+str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] =
+None) -> None` - Updates the database by executing the given query with the
+provided payload. 3. **Using `S3ServiceGateway`**: ```python from
+WrenchCL.Connect import S3ServiceGateway # Initialize S3ServiceGateway with the
+AWSClientHub instance s3_service = S3ServiceGateway(aws_client_hub) # Example:
+Downloading an object from S3 bucket_name = "your-bucket-name" object_key =
+"path/to/your/object" s3_service.download_object(bucket_name, object_key,
+"local/path/to/save") ``` **Methods in `S3ServiceGateway`**: - `get_object
+(bucket_name: str, object_key: str) -> io.BytesIO` - Retrieves an object from
+S3. - `download_object(bucket_name: str, object_key: str, local_path: str) -
+> None` - Downloads an object from S3 to the local file system. -
+`get_object_headers(bucket_name: str, object_key: str) -> dict` - Retrieves the
+headers of an object in S3. - `upload_object(file_path: str, bucket_name: str,
+object_key: str) -> None` - Uploads a local file to S3. - `delete_object
+(bucket_name: str, object_key: str) -> None` - Deletes an object from S3. -
+`move_object(src_bucket_name: str, src_object_key: str, dst_bucket_name: str,
+dst_object_key: str) -> None` - Moves an object from one S3 location to
+another. - `copy_object(src_bucket_name: str, src_object_key: str,
+dst_bucket_name: str, dst_object_key: str) -> None` - Copies an object from one
+S3 location to another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
@@ -108,115 +118,112 @@
 to text and then generates embeddings for the text. -
 `image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
 str = "text-embedding-3-small") -> list` - Performs a vision query to
 understand an image and then generates embeddings for the response. -
 `validate_response_with_gpt(initial_response: str, validation_prompt: str) -
 > str` - Uses an initial response and validates or expands upon it with a
 secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
-for various purposes: Got it! Here is the section about the custom JSON
-serializer in the specified format: ### Custom JSON Serializer -
-**robust_serializer**: Serializes objects not natively serializable by JSON,
-including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
-with json_dumps from datetime import datetime import json from WrenchCL.Tools
-import robust_serializer print(json.dumps({"timestamp": datetime.now()},
-default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
-56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
-against expected types. ```python from WrenchCL.Tools import
-validate_input_dict params = { 'event': 'event_data', 'context':
-'context_data', 'start_time': 1625256000, 'lambda_client':
+for various purposes: - **robust_serializer**: Serializes objects not natively
+serializable by JSON, including `datetime`, `date`, `Decimal`, and custom
+objects. ```python # Usage with json_dumps from datetime import datetime import
+json from WrenchCL.Tools import robust_serializer print(json.dumps(
+{"timestamp": datetime.now()}, default=robust_serializer)) # Output:
+{"timestamp": "2024-05-17T12:34:56.789012"} ``` - **validate_input_dict**:
+Validates the input dictionary against expected types. ```python from
+WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
+'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
 file") print(file_type) ``` - **Image2B64**: A utility for encoding images to
 base64. ```python from WrenchCL.Tools import image_to_base64 image_b64 =
 image_to_base64("path/to/your/image.jpg") print(image_b64) ``` -
 **MaybeMonad**: A utility for handling nullable values with method chaining.
 ```python from WrenchCL.Tools import Maybe maybe_value = Maybe(None).len
 ().end_maybe() print(result) # Output: None # Does not raise an exception ``` -
-**WrenchLogger**: A custom logger for advanced logging. ```python from
-WrenchCL.Tools import logger logger.info("This is an info log message", "with
-additional info") logger.error("This is an error log message", "with error
-details") ``` **Non-hidden Methods in `WrenchLogger`**: #### Logging Methods -
-`info(*args: str, stack_info: Optional[bool] = False) -> None` - `context
-(*args: str, stack_info: Optional[bool] = False) -> None` - `warning(*args:
-str, stack_info: Optional[bool] = False) -> None` - `HDL_WARN(*args: str,
-stack_info: Optional[bool] = False) -> None` - `error(*args: str, stack_info:
-Optional[bool] = False) -> None` - `data(data: Any, wrap_length: Optional[int]
-= None, max_rows: Optional[int] = None, stack_info: Optional[bool] = False) -
-> None` - `HDL_ERR(*args: str, stack_info: Optional[bool] = False) -> None` -
-`RECV_ERR(*args: str, stack_info: Optional[bool] = False) -> None` - `critical
-(*args: str, stack_info: Optional[bool] = False) -> None` - `debug(*args: str,
-stack_info: Optional[bool] = False) -> None` - `start_time() -> None` -
-`log_time(message: str = "Elapsed time", format: str = "seconds", stack_info:
-Optional[bool] = False) -> None` - `header(text: str, size: int = 80, newline:
-bool = True) -> None` - `compact_header(text: str, size: int = 40) -> None`
-**Note**: The logging methods support chaining multiple string arguments. ####
-Configuration Methods - `setLevel(level: str) -> None` - Changes the reporting
-level of the logger. - `revertLoggingLevel() -> None` - Reverts the logging
-level to the previous level. - `set_file_logging(file_logging: bool) -> None` -
-Enables or disables file logging. - `set_log_file_location(new_append_mode:
-Optional[str] = None) -> None` - Changes the file append mode and optionally
-deletes the old file. #### Utility Methods - `initiate_new_run() -> None` -
-Initiates a new run with a unique run ID. - `overwrite_lambda_mode(setting:
-bool) -> None` - Sets whether the logger is running on AWS Lambda. -
-`set_global_traceback(setting: bool) -> None` - Sets whether to always include
-stack traces for errors. - `release_resources() -> None` - Releases file
-handler resources. ```python # Example usage of logger methods logger.info
-("This is an info log message", "with additional info") logger.context("This is
-a contextual log message", "with more context") logger.warning("This is a
-warning log message") logger.HDL_WARN("This is a handled warning log message")
-logger.error("This is an error log message", str(Exception("Example
-exception")), stack_info=True) data_dict = {"key": "value", "another_key": 123}
-logger.data(data_dict, wrap_length=40, max_rows=10) logger.HDL_ERR("This is a
-handled error log message") logger.RECV_ERR("This is a recoverable error log
-message", "with additional recoverable error details") logger.critical("This is
-a critical log message", "with critical details", stack_info=True) logger.debug
-("This is a debug log message", str(data_dict), stack_info=True)
-logger.start_time() # ... some operations ... logger.log_time("Processing
-time", format="formatted") logger.initiate_new_run()
-logger.overwrite_lambda_mode(setting=True) logger.set_global_traceback
-(setting=True) logger.setLevel("DEBUG") logger.header("Header Text")
-logger.compact_header("Compact Header Text") ``` - **FetchMetaData**: A utility
-to retrieve metadata from a URL or local file path. ```python from
-WrenchCL.Tools import get_metadata # Get metadata from a URL url_metadata =
-get_metadata("https://example.com/file.txt") print(url_metadata) # Output:
-{'content_type': 'text/plain', 'content_length': '1234', 'last_modified':
-datetime.datetime(2023, 5, 17, 12, 34, 56), 'url': 'https://example.com/
-file.txt'} # Get metadata from a local file file_metadata = get_metadata("/
-path/to/file.txt", is_url=False) print(file_metadata) # Output: {'file_path':
-'/path/to/file.txt', 'file_size': 1234, 'creation_time': '2023-05-17T12:34:56',
-'mime_type': 'text/plain'} ``` ### Decorators WrenchCL includes several
-decorators for common patterns: - **Retryable**: Retries a function call if
-specified exceptions occur. ```python from WrenchCL.Decorators import Retryable
-@Retryable(retry_on_exceptions=(ValueError,), max_retries=3, delay=2) def
-might_fail(): if random.random() < 0.5: raise ValueError("Random failure")
-return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
-Ensures a class only has one instance. ```python from WrenchCL.Decorators
-import SingletonClass @SingletonClass class MySingleton: def __init__(self):
-self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
-(instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
-taken to execute a method. ```python from WrenchCL.Decorators import
-TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
-WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `DataFlow` module. #### build_return_json Constructs
-a JSON response with a given status code and message. ```python from
-WrenchCL.DataFlow import build_return_json response = build_return_json
-(code=200, message="Success") print(response) # Output: {'statusCode': 200,
-'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
-Lambda function responses, including logging and error handling. It stops the
-Lambda function execution and returns a specified response when a
-`GuardedResponseTrigger` exception is raised. This is particularly useful for
-ensuring that the Lambda function exits immediately and returns the correct
-response, even if the exception occurs deep within nested function calls.
-Hereâs a comprehensive example demonstrating how to use
+**WrenchLogger**: A custom logger for advanced logging. ```python from WrenchCL
+import logger logger.info("This is an info log message", "with additional
+info") logger.error("This is an error log message", "with error details") ```
+**Non-hidden Methods in `WrenchLogger`**: #### Logging Methods - `info(*args:
+str, stack_info: Optional[bool] = False) -> None` - `context(*args: str,
+stack_info: Optional[bool] = False) -> None` - `warning(*args: str, stack_info:
+Optional[bool] = False) -> None` - `HDL_WARN(*args: str, stack_info: Optional
+[bool] = False) -> None` - `error(*args: str, stack_info: Optional[bool] =
+False) -> None` - `data(data: Any, wrap_length: Optional[int] = None, max_rows:
+Optional[int] = None, stack_info: Optional[bool] = False) -> None` - `HDL_ERR
+(*args: str, stack_info: Optional[bool] = False) -> None` - `RECV_ERR(*args:
+str, stack_info: Optional[bool] = False) -> None` - `critical(*args: str,
+stack_info: Optional[bool] = False) -> None` - `debug(*args: str, stack_info:
+Optional[bool] = False) -> None` - `start_time() -> None` - `log_time(message:
+str = "Elapsed time", format: str = "seconds", stack_info: Optional[bool] =
+False) -> None` - `header(text: str, size: int = 80, newline: bool = True) -
+> None` - `compact_header(text: str, size: int = 40) -> None` **Note**: The
+logging methods support chaining multiple string arguments. #### Configuration
+Methods - `setLevel(level: str) -> None` - Changes the reporting level of the
+logger. - `revertLoggingLevel() -> None` - Reverts the logging level to the
+previous level. - `set_file_logging(file_logging: bool) -> None` - Enables or
+disables file logging. - `set_log_file_location(new_append_mode: Optional[str]
+= None) -> None` - Changes the file append mode and optionally deletes the old
+file. #### Utility Methods - `initiate_new_run() -> None` - Initiates a new run
+with a unique run ID. - `overwrite_lambda_mode(setting: bool) -> None` - Sets
+whether the logger is running on AWS Lambda. - `set_global_traceback(setting:
+bool) -> None` - Sets whether to always include stack traces for errors. -
+`release_resources() -> None` - Releases file handler resources. ```python #
+Example usage of logger methods logger.info("This is an info log message",
+"with additional info") logger.context("This is a contextual log message",
+"with more context") logger.warning("This is a warning log message")
+logger.HDL_WARN("This is a handled warning log message") logger.error("This is
+an error log message", str(Exception("Example exception")), stack_info=True)
+data_dict = {"key": "value", "another_key": 123} logger.data(data_dict,
+wrap_length=40, max_rows=10) logger.HDL_ERR("This is a handled error log
+message") logger.RECV_ERR("This is a recoverable error log message", "with
+additional recoverable error details") logger.critical("This is a critical log
+message", "with critical details", stack_info=True) logger.debug("This is a
+debug log message", str(data_dict), stack_info=True) logger.start_time() # ...
+some operations ... logger.log_time("Processing time", format="formatted")
+logger.initiate_new_run() logger.overwrite_lambda_mode(setting=True)
+logger.set_global_traceback(setting=True) logger.setLevel("DEBUG")
+logger.header("Header Text") logger.compact_header("Compact Header Text") ``` -
+**FetchMetaData**: A utility to retrieve metadata from a URL or local file
+path. ```python from WrenchCL.Tools import get_metadata # Get metadata from a
+URL url_metadata = get_metadata("https://example.com/file.txt") print
+(url_metadata) # Output: {'content_type': 'text/plain', 'content_length':
+'1234', 'last_modified': datetime.datetime(2023, 5, 17, 12, 34, 56), 'url':
+'https://example.com/file.txt'} # Get metadata from a local file file_metadata
+= get_metadata("/path/to/file.txt", is_url=False) print(file_metadata) #
+Output: {'file_path': '/path/to/file.txt', 'file_size': 1234, 'creation_time':
+'2023-05-17T12:34:56', 'mime_type': 'text/plain'} ``` ### Decorators WrenchCL
+includes several decorators for common patterns: - **Retryable**: Retries a
+function call if specified exceptions occur. ```python from WrenchCL.Decorators
+import Retryable @Retryable(retry_on_exceptions=(ValueError,), max_retries=3,
+delay=2) def might_fail(): if random.random() < 0.5: raise ValueError("Random
+failure") return "Success" result = might_fail() print(result) ``` -
+**SingletonClass**: Ensures a class only has one instance. ```python from
+WrenchCL.Decorators import SingletonClass @SingletonClass class MySingleton:
+def __init__(self): self.value = 42 instance1 = MySingleton() instance2 =
+MySingleton() print(instance1 is instance2) # Output: True ``` -
+**TimedMethod**: Logs the time taken to execute a method. ```python from
+WrenchCL.Decorators import TimedMethod @TimedMethod def slow_function():
+time.sleep(2) return "Done" result = slow_function() print(result) # Output:
+"Done" ``` ### DataFlow WrenchCL includes various helper functions to assist
+with common tasks. These helpers are located in the `DataFlow` module. ####
+build_return_json Constructs a JSON response with a given status code and
+message. ```python from WrenchCL.DataFlow import build_return_json response =
+build_return_json(code=200, message="Success") print(response) # Output:
+{'statusCode': 200, 'body': '{"message": "Success"}'} ``` ####
+handle_lambda_response Handles Lambda function responses, including logging and
+error handling. It stops the Lambda function execution and returns a specified
+response when a `GuardedResponseTrigger` exception is raised. This is
+particularly useful for ensuring that the Lambda function exits immediately and
+returns the correct response, even if the exception occurs deep within nested
+function calls. Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
 import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
@@ -277,8 +284,13 @@
 purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
 trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
 additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
-refer to the documentation or contact the maintainers.
+refer to the documentation or contact the maintainers. ``` This README includes
+comprehensive details on how to use the `AwsClientHub`, `RdsServiceGateway`,
+`S3ServiceGateway`, `OpenAIFactory`, and `OpenAIGateway` classes, as well as
+utility tools and decorators provided by the WrenchCL library. It also
+specifies the keyword arguments that can be passed to `AwsClientHub` and
+`_ConfigurationManager`.
```

### Comparing `WrenchCL-2.2.0/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.3.0/WrenchCL.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 WrenchCL/Connect/RdsServiceGateway.py
 WrenchCL/Connect/S3ServiceGateway.py
 WrenchCL/Connect/__init__.py
 WrenchCL/DataFlow/__init__.py
 WrenchCL/DataFlow/build_return_json.py
 WrenchCL/DataFlow/handle_lambda_response.py
 WrenchCL/DataFlow/trigger_dataflow_metrics.py
+WrenchCL/Decorators/MultiThreaded.py
 WrenchCL/Decorators/Retryable.py
 WrenchCL/Decorators/SingletonClass.py
 WrenchCL/Decorators/TimedMethod.py
 WrenchCL/Decorators/__init__.py
 WrenchCL/Models/__init__.py
 WrenchCL/Models/OpenAI/OpenAIFactory.py
 WrenchCL/Models/OpenAI/OpenAIGateway.py
 WrenchCL/Models/OpenAI/_ConversationManager.py
 WrenchCL/Models/OpenAI/__init__.py
 WrenchCL/Tools/Coalesce.py
-WrenchCL/Tools/DictValidator.py
 WrenchCL/Tools/FetchMetaData.py
 WrenchCL/Tools/FileTyper.py
 WrenchCL/Tools/Image2B64.py
 WrenchCL/Tools/JsonSerializer.py
 WrenchCL/Tools/MaybeMonad.py
+WrenchCL/Tools/TypeChecker.py
 WrenchCL/Tools/WrenchLogger.py
 WrenchCL/Tools/__init__.py
 WrenchCL/_Internal/_ConfigurationManager.py
 WrenchCL/_Internal/_SshTunnelManager.py
 WrenchCL/_Internal/__init__.py
```

### Comparing `WrenchCL-2.2.0/setup.py` & `WrenchCL-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     egg_info_folder = find_egg_info_folder()
     if egg_info_folder:
         requires_path = os.path.join(egg_info_folder, 'requires.txt')
         if os.path.exists(requires_path):
             with open(requires_path, "r", encoding="utf-8") as f:
                 required = f.read().splitlines()
 
-setup(name='WrenchCL', version='v2.2.0',
+setup(name='WrenchCL', version='v2.3.0',
       description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
       long_description=long_description, long_description_content_type="text/markdown",
       url='https://github.com/WrenchAI/WrenchCL', packages=find_packages(), install_requires=required, python_requires='>=3.11',
       classifiers=['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent', ], )
```

