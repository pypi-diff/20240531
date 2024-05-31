# Comparing `tmp/ecmind_blue_client-0.6.1.tar.gz` & `tmp/ecmind_blue_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecmind_blue_client-0.6.1.tar", last modified: Thu Feb 22 07:20:01 2024, max compression
+gzip compressed data, was "ecmind_blue_client-0.7.0.tar", last modified: Fri May 31 06:58:30 2024, max compression
```

## Comparing `ecmind_blue_client-0.6.1.tar` & `ecmind_blue_client-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-02-22 07:20:00.990513 ecmind_blue_client-0.6.1/
--rw-r--r--   0 rk        (1000) rk        (1000)     1069 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/LICENSE
--rw-r--r--   0 rk        (1000) rk        (1000)     3723 2024-02-22 07:20:00.990513 ecmind_blue_client-0.6.1/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)     3028 2024-01-29 15:02:54.000000 ecmind_blue_client-0.6.1/README.md
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-02-22 07:20:00.977180 ecmind_blue_client-0.6.1/ecmind_blue_client/
--rw-r--r--   0 rk        (1000) rk        (1000)      421 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/__init__.py
--rw-r--r--   0 rk        (1000) rk        (1000)      303 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/blue_exception.py
--rw-r--r--   0 rk        (1000) rk        (1000)    25250 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/client.py
--rw-r--r--   0 rk        (1000) rk        (1000)     3471 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/com_client.py
--rw-r--r--   0 rk        (1000) rk        (1000)    21895 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/const.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1006 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/dms_result.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2280 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/job.py
--rw-r--r--   0 rk        (1000) rk        (1000)     7352 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/options.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1890 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/param.py
--rw-r--r--   0 rk        (1000) rk        (1000)     3953 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/query_condition_field.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2234 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/query_condition_group.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1958 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/query_result_field.py
--rw-r--r--   0 rk        (1000) rk        (1000)      998 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/result.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2758 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/result_file.py
--rw-r--r--   0 rk        (1000) rk        (1000)     4696 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/soap_client.py
--rw-r--r--   0 rk        (1000) rk        (1000)     5910 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client.py
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-02-22 07:20:00.990513 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/
--rw-r--r--   0 rk        (1000) rk        (1000)        0 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/__init__.py
--rw-r--r--   0 rk        (1000) rk        (1000)      322 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/call_job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)      263 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/file_footer.py
--rw-r--r--   0 rk        (1000) rk        (1000)      688 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/file_header.py
--rw-r--r--   0 rk        (1000) rk        (1000)    17844 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_caller.py
--rw-r--r--   0 rk        (1000) rk        (1000)      616 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_header.py
--rw-r--r--   0 rk        (1000) rk        (1000)      254 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_parameter_data.py
--rw-r--r--   0 rk        (1000) rk        (1000)      207 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_parameter_description.py
--rw-r--r--   0 rk        (1000) rk        (1000)      552 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)      177 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/response_job_error_data.py
--rw-r--r--   0 rk        (1000) rk        (1000)      301 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/response_job_error_description.py
--rw-r--r--   0 rk        (1000) rk        (1000)      427 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/response_job_errors.py
--rw-r--r--   0 rk        (1000) rk        (1000)      373 2023-10-16 15:36:37.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/response_job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)     5137 2024-02-22 07:18:11.000000 ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_pool_client.py
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-02-22 07:20:00.980513 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/
--rw-r--r--   0 rk        (1000) rk        (1000)     3723 2024-02-22 07:20:00.000000 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)     1574 2024-02-22 07:20:00.000000 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/SOURCES.txt
--rw-r--r--   0 rk        (1000) rk        (1000)        1 2024-02-22 07:20:00.000000 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/dependency_links.txt
--rw-r--r--   0 rk        (1000) rk        (1000)      314 2024-02-22 07:20:00.000000 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/requires.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       19 2024-02-22 07:20:00.000000 ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/top_level.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       38 2024-02-22 07:20:00.990513 ecmind_blue_client-0.6.1/setup.cfg
--rw-r--r--   0 rk        (1000) rk        (1000)     1370 2024-02-22 07:18:11.000000 ecmind_blue_client-0.6.1/setup.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-05-31 06:58:30.170757 ecmind_blue_client-0.7.0/
+-rw-r--r--   0 rk        (1000) rk        (1000)     1069 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/LICENSE
+-rw-r--r--   0 rk        (1000) rk        (1000)     4486 2024-05-31 06:58:30.167424 ecmind_blue_client-0.7.0/PKG-INFO
+-rw-r--r--   0 rk        (1000) rk        (1000)     3222 2024-05-30 14:19:56.000000 ecmind_blue_client-0.7.0/README.md
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-05-31 06:58:30.150756 ecmind_blue_client-0.7.0/ecmind_blue_client/
+-rw-r--r--   0 rk        (1000) rk        (1000)      532 2024-05-31 06:56:52.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/__init__.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      303 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/blue_exception.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    25331 2024-05-31 06:56:52.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     3710 2024-05-30 14:19:56.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/com_client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    21895 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/const.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1006 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/dms_result.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2600 2024-05-31 06:56:52.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/job.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     7352 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/options.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1890 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/param.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     3953 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/query_condition_field.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2234 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/query_condition_group.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1958 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/query_result_field.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2198 2024-05-31 06:56:52.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/request_file.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      998 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/result.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2758 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/result_file.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     4935 2024-05-30 14:19:56.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/soap_client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     5910 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-05-31 06:58:30.160757 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/
+-rw-r--r--   0 rk        (1000) rk        (1000)        0 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/__init__.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      322 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/call_job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      263 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/file_footer.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      688 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/file_header.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    17664 2024-05-31 06:56:52.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_caller.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      616 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_header.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      254 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_parameter_data.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      207 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_parameter_description.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      552 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      177 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/response_job_error_data.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      301 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/response_job_error_description.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      427 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/response_job_errors.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      373 2023-10-16 15:36:37.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/response_job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     5137 2024-02-22 07:18:11.000000 ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_pool_client.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2024-05-31 06:58:30.164090 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/
+-rw-r--r--   0 rk        (1000) rk        (1000)     4486 2024-05-31 06:58:29.000000 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/PKG-INFO
+-rw-r--r--   0 rk        (1000) rk        (1000)     1609 2024-05-31 06:58:30.000000 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/SOURCES.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)        1 2024-05-31 06:58:29.000000 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/dependency_links.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)      314 2024-05-31 06:58:29.000000 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/requires.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)       19 2024-05-31 06:58:29.000000 ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/top_level.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)       38 2024-05-31 06:58:30.170757 ecmind_blue_client-0.7.0/setup.cfg
+-rw-r--r--   0 rk        (1000) rk        (1000)     1370 2024-05-31 06:45:44.000000 ecmind_blue_client-0.7.0/setup.py
```

### Comparing `ecmind_blue_client-0.6.1/LICENSE` & `ecmind_blue_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/PKG-INFO` & `ecmind_blue_client-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,16 @@
-Metadata-Version: 2.1
-Name: ecmind_blue_client
-Version: 0.6.1
-Summary: A client wrapper for blue
-Home-page: https://gitlab.ecmind.ch/open/ecmind_blue_client
-Author: Ulrich Wohlfeil, Roland Koller
-Author-email: info@ecmind.ch
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: SoapClient
-Provides-Extra: ComClient
-Provides-Extra: TcpClient
-Provides-Extra: soap
-Provides-Extra: com
-Provides-Extra: tcp
-Provides-Extra: manage
-Provides-Extra: objdef
-Provides-Extra: portfolio
-Provides-Extra: workflow
-License-File: LICENSE
-
 # ECMind blue client
 
 A client wrapper for blue.
 
+## Deprecation warning
+
+- From Mai 2024, `ecmind_blue_client.com_client` is no longer supported nor tested.
+- From Mai 2024, `ecmind_blue_client.soap_client` is no longer supported nor tested.
+
 ## Installation
 
 `pip install ecmind_blue_client`
 
 ## Usage
 
 The workflow consists roughly of the following:
@@ -103,8 +84,8 @@
     },
     files = ["invoice.pdf"]
 )
 
 # Check if the import was successful and output OSID
 assert import_result, import_result.error_message
 print(import_result.import_action, import_result.object_id)
-```
+```
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/client.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .dms_result import DmsResult
 from .job import Job
 from .param import Param, ParamTypes
 from .query_condition_group import QueryConditionGroup
 from .query_result_field import QueryResultField
 from .result import Result
 from .result_file import ResultFile
+from .request_file import RequestFile
 
 log = logging.getLogger(__name__)
 
 
 class Client(ABC):
     @abstractmethod
     def execute(self, job: Job) -> Result:
@@ -105,15 +106,15 @@
         folder_id: int = None,
         register_id: int = None,
         object_id: int = None,
         options: Union[Options, str] = "",
         action0: ImportActions = ImportActions.INSERT,
         action1: ImportActions = ImportActions.UPDATE,
         actionM: ImportActions = ImportActions.ERROR,
-        files: List[str] = None,
+        files: List[Union[RequestFile, str]] = None,
         main_type: Union[MainTypeId, int, None] = None,
         variant_parent_id: int = None,
     ) -> DmsResult:
         """Helper function: Execute the dms.XMLImport job.
 
         ### Keyword arguments
 
@@ -128,15 +129,15 @@
         - `options` -- (Optional) Semicolon separated string of import options.
         - `action0` -- (Optional) `ImportActions` Enum element defining how to handle
         imports when the search_fields do not match any pre-existing objects.
         - `action1` -- (Optional) `ImportActions` Enum element defining how to handle
         imports when the search_fields do match exactly one pre-existing object.
         - `actionM` -- (Optional) `ImportActions` Enum element defining how to handle
         imports when the search_fields do match more then one pre-existing object.
-        - `files` -- (Optional) List of strings containing file path to import into a document object.
+        - `files` -- (Optional) List of strings containing file path to import into a document object or RequestFile objects.
         - `main_type` -- (Optional) Set the main type id for document imports or leave empty for default value.
         Valid ids are `DOC_GRAYSCALE`/`1`, `DOC_BW`/`2`, DOC_COLOR`3`, `DOC_WINDOWS`/`4`,
         `DOC_MULTIMEDIA`/`5`, `DOC_MAIL`/`6`, `DOC_XML`/`7`, `DOC_CONTAINER`/`8`.
         - `variant_parent_id` -- (Optional) Set the parent id for document variant imports.
         `search_fields` must be empty when `variant_parent_id` is set.
         """
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/com_client.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/com_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import os
+from warnings import warn
 
 from comtypes import COMError
 from comtypes.client import CreateObject
 
 from .blue_exception import BlueException
 from .client import Client
 from .const import ParamTypes
 from .job import Job
 from .result import Result
 from .result_file import ResultFile, ResultFileType
 
 
 class ComClient(Client):
     def __init__(self, hostname: str, port: int, username: str, password: str):
+        warn(
+            f"{self.__class__.__name__} is deprecated and will be removed in a future version."
+            "Please use TcpClient or TcpPoolClient instead.",
+            DeprecationWarning
+        )
         self.hostname = hostname
         self.port = port
         self.username = username
         self.server = CreateObject("OxSvrSpt.Server")
         self.session = self.server.Login(username, password, hostname, str(port))
 
     def execute(self, job: Job) -> Result:
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/const.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/const.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/dms_result.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/dms_result.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/job.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from typing import List, Union
 
 from .const import Jobs, ParamTypes
 from .param import Param
+from .request_file import RequestFile, RequestFileFromPath
 
 
 class Job:
     def __init__(
         self,
         jobname: Union[str, Jobs],
-        files: Union[List[str], None] = None,
+        files: Union[List[Union[RequestFile, str]], None] = None,
         context_user: Union[str, None] = None,
         raise_exception:bool = False,
         **params,
     ):
         """Create a new Job() object.
 
         Keyword arguments:
         jobname -- String with the a blue jobname, i. e. 'dms.GetResultList'
-        files -- (Optional) List of strings with file paths to add to the job.
+        files -- (Optional) List of strings with file paths to add to the job or RequestFile objects.
         context_user -- (Optional) Set the magical parameter `$$$SwitchContextUserName$$$` to a username.
         raise_exception -- (Optional) Set to true to raise BlueException() on non-zero results.
         **params -- Add arbitrary job input parameters. Uses Param.infer_type() to guess the blue parameter type.
         """
         self.name = jobname.value if isinstance(jobname, Jobs) else jobname
         self.params: List[Param] = []
-        self.files = files if files is not None else []
+        
+        self.files:List[RequestFile] = []
+        if files:
+            for file in files:
+                self.append_file(file)
+
         self.raise_exception = raise_exception
         for name, value in params.items():
             self.append(Param.infer_type(name, value))
         if context_user:
             self.append(Param("$$$SwitchContextUserName$$$", ParamTypes.STRING, context_user))
 
     def append(self, param: Param):
@@ -46,16 +52,19 @@
         for current_param in self.params:
             if current_param.name == param.name:
                 current_param.value = param.value
                 current_param.type = param.type
                 return True
         self.append(param)
 
-    def append_file(self, filepath: str):
+    def append_file(self, file: Union[str, RequestFile]):
         """Appends a job input file parameter.
         Keyword arguments:
         filepath -- String with file path to append.
         """
-        self.files.append(filepath)
+        if isinstance(file, RequestFile):
+            self.files.append(file)
+        else:
+            self.files.append(RequestFileFromPath(str(file)))
 
     def __repr__(self) -> str:
         return f'Job "{self.name}" ({len(self.files)} files): {self.params}'
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/options.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/options.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/param.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/param.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/query_condition_field.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/query_condition_field.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/query_condition_group.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/query_condition_group.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/query_result_field.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/query_result_field.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/result.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/result.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/result_file.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/result_file.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/soap_client.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/soap_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import uuid
 from typing import List
+from warnings import warn
 
 import zeep
 import zeep.exceptions
 
 from .blue_exception import BlueException
 from .client import Client
 from .const import ParamTypes
@@ -12,14 +13,19 @@
 from .param import Param
 from .result import Result
 from .result_file import ResultFile, ResultFileType
 
 
 class SoapClient(Client):
     def __init__(self, endpoint: str, appname: str, username: str, password: str):
+        warn(
+            f"{self.__class__.__name__} is deprecated and will be removed in a future version."
+            "Please use TcpClient or TcpPoolClient instead.",
+            DeprecationWarning
+        )
         self.endpoint = endpoint
         self.wsdlUri = endpoint + "/EcmWsMtom?wsdl"
         self.client = zeep.Client(wsdl=self.wsdlUri)
         self.enaioWsTypesFactory = self.client.type_factory("ns0")
         self.enaioWsFactory = self.client.type_factory("ns1")
         self.sessionId = str(uuid.uuid4())
         self.auth = self.enaioWsTypesFactory.Authentication(
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/file_header.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/file_header.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_caller.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_caller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from struct import unpack
 from tempfile import gettempdir
 from typing import List, Optional
 from uuid import uuid4
 
 from ecmind_blue_client.blue_exception import BlueException
 
+from ..job import Job
 from ..const import ParamTypes
 from ..param import Param
 from ..result import Result
 from ..result_file import ResultFile, ResultFileType
 from .call_job_parameters import CallJobParameters
 from .file_footer import FileFooter
 from .file_header import FileHeader
@@ -85,15 +86,15 @@
         else:
             self.socket = plain_text_socket
         self.socket.connect((hostname, port))
 
     def close(self):
         self.socket.close()
 
-    def execute(self, job):
+    def execute(self, job:Job):
         # Create internal parameter
         intern_params: List[Param] = []
         intern_params.append(Param("streams", ParamTypes.INTEGER, len(job.files)))
         internal_parameters = self.build_parameters(intern_params)
 
         # create parameter
         parameters = self.build_parameters(job.params)
@@ -117,43 +118,38 @@
 
         # send request
         self.socket.send(request_header_binary)
         self.socket.send(request_parameters_binary)
 
         # for each file
         for file in job.files:
-            # read file info
-            with pathlib.Path(file) as path:
-                size = path.stat().st_size
-                extension = path.suffix[1:]
-
-                # write file header
-                request_file_header = FileHeader()
-                request_file_header.set_file_length(size)
-                request_file_header.extension = extension
-                request_file_header_binary = request_file_header.serialize()
+            # write file header
+            request_file_header = FileHeader()
+            request_file_header.set_file_length(file.size)
+            request_file_header.extension = file.extension
+            request_file_header_binary = request_file_header.serialize()
 
-                self.socket.send(request_file_header_binary)
-                request_digest.update(request_file_header_binary)
+            self.socket.send(request_file_header_binary)
+            request_digest.update(request_file_header_binary)
 
-                # stream file
-                file_stream = open(file, "rb")
+            # stream file
+            with file.open() as file_stream:
                 data = file_stream.read(1024)
                 while data:
                     self.socket.send(data)
                     request_digest.update(data)
                     data = file_stream.read(1024)
                 file_stream.close()
 
-                # write fix file footer @0000000000@MAERTSSA
-                request_file_footer = FileFooter()
-                request_file_footer_binary = request_file_footer.serialize()
-                self.socket.send(request_file_footer_binary)
+            # write fix file footer @0000000000@MAERTSSA
+            request_file_footer = FileFooter()
+            request_file_footer_binary = request_file_footer.serialize()
+            self.socket.send(request_file_footer_binary)
 
-                request_digest.update(request_file_footer_binary)
+            request_digest.update(request_file_footer_binary)
 
         # send request digest
         self.socket.send(request_digest.digest())
 
         # ----------------------------------------------------------------------
         # Start read response
         # ----------------------------------------------------------------------
```

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_header.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_header.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_client_classes/job_parameters.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_client_classes/job_parameters.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client/tcp_pool_client.py` & `ecmind_blue_client-0.7.0/ecmind_blue_client/tcp_pool_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.6.1/ecmind_blue_client.egg-info/SOURCES.txt` & `ecmind_blue_client-0.7.0/ecmind_blue_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ecmind_blue_client/dms_result.py
 ecmind_blue_client/job.py
 ecmind_blue_client/options.py
 ecmind_blue_client/param.py
 ecmind_blue_client/query_condition_field.py
 ecmind_blue_client/query_condition_group.py
 ecmind_blue_client/query_result_field.py
+ecmind_blue_client/request_file.py
 ecmind_blue_client/result.py
 ecmind_blue_client/result_file.py
 ecmind_blue_client/soap_client.py
 ecmind_blue_client/tcp_client.py
 ecmind_blue_client/tcp_pool_client.py
 ecmind_blue_client.egg-info/PKG-INFO
 ecmind_blue_client.egg-info/SOURCES.txt
```

### Comparing `ecmind_blue_client-0.6.1/setup.py` & `ecmind_blue_client-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ecmind_blue_client",
-    version="0.6.1",
+    version="0.7.0",
     author="Ulrich Wohlfeil, Roland Koller",
     author_email="info@ecmind.ch",
     description="A client wrapper for blue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.ecmind.ch/open/ecmind_blue_client",
     packages=setuptools.find_packages(),
```

