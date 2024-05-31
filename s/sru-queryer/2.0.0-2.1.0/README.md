# Comparing `tmp/sru_queryer-2.0.0.tar.gz` & `tmp/sru_queryer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sru_queryer-2.0.0.tar", last modified: Fri May  3 13:53:10 2024, max compression
+gzip compressed data, was "sru_queryer-2.1.0.tar", last modified: Fri May 31 16:46:51 2024, max compression
```

## Comparing `sru_queryer-2.0.0.tar` & `sru_queryer-2.1.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.428948 sru_queryer-2.0.0/
--rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-2.0.0/LICENSE
--rw-r--r--   0 ejones99   (505) staff       (20)    43463 2024-05-03 13:53:10.428667 sru_queryer-2.0.0/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-05-03 13:26:19.000000 sru_queryer-2.0.0/pyproject.toml
--rw-r--r--   0 ejones99   (505) staff       (20)    42967 2024-05-03 13:30:15.000000 sru_queryer-2.0.0/readme.md
--rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-05-03 13:53:10.429012 sru_queryer-2.0.0/setup.cfg
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.418255 sru_queryer-2.0.0/src/
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.420340 sru_queryer-2.0.0/src/sru_queryer/
--rw-r--r--   0 ejones99   (505) staff       (20)      131 2024-05-01 20:21:50.000000 sru_queryer-2.0.0/src/sru_queryer/__init__.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.425018 sru_queryer-2.0.0/src/sru_queryer/_base/
--rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-2.0.0/src/sru_queryer/_base/__init__.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5630 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4982 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1210 2024-05-01 15:58:54.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_exceptions.py
--rw-r--r--   0 ejones99   (505) staff       (20)      462 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_raw_cql.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3306 2024-05-02 17:17:10.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_search_clause.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3808 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_search_retrieve.py
--rw-r--r--   0 ejones99   (505) staff       (20)     2961 2024-04-22 13:47:27.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4368 2024-05-01 21:01:01.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1159 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_configuration.py
--rw-r--r--   0 ejones99   (505) staff       (20)    12230 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_explain_auto_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)    11729 2024-05-03 12:56:00.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_queryer.py
--rw-r--r--   0 ejones99   (505) staff       (20)    10887 2024-05-02 19:42:22.000000 sru_queryer-2.0.0/src/sru_queryer/_base/_sru_validator.py
--rw-r--r--   0 ejones99   (505) staff       (20)      433 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/src/sru_queryer/cql.py
--rw-r--r--   0 ejones99   (505) staff       (20)      241 2024-05-01 16:02:27.000000 sru_queryer-2.0.0/src/sru_queryer/exceptions.py
--rw-r--r--   0 ejones99   (505) staff       (20)      191 2024-05-01 20:21:50.000000 sru_queryer-2.0.0/src/sru_queryer/sru.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.428322 sru_queryer-2.0.0/src/sru_queryer.egg-info/
--rw-r--r--   0 ejones99   (505) staff       (20)    43463 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)     1147 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/SOURCES.txt
--rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/dependency_links.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/requires.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-05-03 13:53:10.000000 sru_queryer-2.0.0/src/sru_queryer.egg-info/top_level.txt
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-03 13:53:10.427891 sru_queryer-2.0.0/tests/
--rw-r--r--   0 ejones99   (505) staff       (20)    10310 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5670 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1087 2024-04-29 14:29:44.000000 sru_queryer-2.0.0/tests/test_raw_cql.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4852 2024-05-02 17:42:23.000000 sru_queryer-2.0.0/tests/test_search_clause.py
--rw-r--r--   0 ejones99   (505) staff       (20)    10206 2024-05-02 17:17:10.000000 sru_queryer-2.0.0/tests/test_search_retrieve.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3439 2024-04-17 17:20:07.000000 sru_queryer-2.0.0/tests/test_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     8096 2024-05-02 15:32:04.000000 sru_queryer-2.0.0/tests/test_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)    13475 2024-05-02 16:27:34.000000 sru_queryer-2.0.0/tests/test_sru_explain_auto_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)     9367 2024-05-02 18:07:43.000000 sru_queryer-2.0.0/tests/test_sru_queryer.py
--rw-r--r--   0 ejones99   (505) staff       (20)    11356 2024-05-02 19:38:45.000000 sru_queryer-2.0.0/tests/test_sru_validator.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.204867 sru_queryer-2.1.0/
+-rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-2.1.0/LICENSE
+-rw-r--r--   0 ejones99   (505) staff       (20)    53280 2024-05-31 16:46:51.204609 sru_queryer-2.1.0/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-05-31 14:06:45.000000 sru_queryer-2.1.0/pyproject.toml
+-rw-r--r--   0 ejones99   (505) staff       (20)    52784 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/readme.md
+-rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-05-31 16:46:51.204918 sru_queryer-2.1.0/setup.cfg
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.193878 sru_queryer-2.1.0/src/
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.196165 sru_queryer-2.1.0/src/sru_queryer/
+-rw-r--r--   0 ejones99   (505) staff       (20)      131 2024-05-01 20:21:50.000000 sru_queryer-2.1.0/src/sru_queryer/__init__.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.200937 sru_queryer-2.1.0/src/sru_queryer/_base/
+-rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-2.1.0/src/sru_queryer/_base/__init__.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     6606 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4982 2024-05-02 17:42:23.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1210 2024-05-01 15:58:54.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_exceptions.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1102 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_raw_cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4347 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_search_clause.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5925 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_search_retrieve.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4662 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4368 2024-05-01 21:01:01.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3059 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sru_configuration.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    12230 2024-05-02 16:27:34.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sru_explain_auto_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    12101 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sru_queryer.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    10887 2024-05-02 19:42:22.000000 sru_queryer-2.1.0/src/sru_queryer/_base/_sru_validator.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      433 2024-04-29 14:29:44.000000 sru_queryer-2.1.0/src/sru_queryer/cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      241 2024-05-01 16:02:27.000000 sru_queryer-2.1.0/src/sru_queryer/exceptions.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      191 2024-05-01 20:21:50.000000 sru_queryer-2.1.0/src/sru_queryer/sru.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.204287 sru_queryer-2.1.0/src/sru_queryer.egg-info/
+-rw-r--r--   0 ejones99   (505) staff       (20)    53280 2024-05-31 16:46:51.000000 sru_queryer-2.1.0/src/sru_queryer.egg-info/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)     1179 2024-05-31 16:46:51.000000 sru_queryer-2.1.0/src/sru_queryer.egg-info/SOURCES.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-05-31 16:46:51.000000 sru_queryer-2.1.0/src/sru_queryer.egg-info/dependency_links.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-05-31 16:46:51.000000 sru_queryer-2.1.0/src/sru_queryer.egg-info/requires.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-05-31 16:46:51.000000 sru_queryer-2.1.0/src/sru_queryer.egg-info/top_level.txt
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-05-31 16:46:51.203835 sru_queryer-2.1.0/tests/
+-rw-r--r--   0 ejones99   (505) staff       (20)    16129 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/tests/test_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5670 2024-05-02 17:42:23.000000 sru_queryer-2.1.0/tests/test_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     2412 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/tests/test_raw_cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     6206 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/tests/test_search_clause.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    15654 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/tests/test_search_retrieve.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     6049 2024-05-31 16:46:08.000000 sru_queryer-2.1.0/tests/test_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     8096 2024-05-02 15:32:04.000000 sru_queryer-2.1.0/tests/test_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3031 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/tests/test_sru_configuration.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    13475 2024-05-02 16:27:34.000000 sru_queryer-2.1.0/tests/test_sru_explain_auto_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    11729 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/tests/test_sru_queryer.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    11360 2024-05-31 14:02:22.000000 sru_queryer-2.1.0/tests/test_sru_validator.py
```

### Comparing `sru_queryer-2.0.0/LICENSE` & `sru_queryer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/PKG-INFO` & `sru_queryer-2.1.0/readme.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sru-queryer
-Version: 2.0.0
-Summary: A utility for integrating SRU queries into your applications.
-Author-email: Erik Jones <ejones99@umd.edu>
-Maintainer-email: USMAI <libclas@umd.edu>
-Keywords: sru,library,api
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7.17
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.27.1
-Requires-Dist: xmltodict>=0.13.0
-
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
 
 1. It handles validating much of the searchRetrieve request. This is particularly helpful because many SRU servers don't have good error messages.
@@ -36,15 +21,16 @@
    1. [SearchClause](#basic-query-component-searchclause-1)
    2. [SRUQueryer](#sruqueryer)
    3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
    4. [RawCQL](#custom-queries-rawcql)
    5. [Modifiers](#modifiying-operators---modifiers)
    6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
    7. [Sorting in v1.1](#sorting-in-11-SortKey)
-5. [Known Incompatibilities](#known-incompatibilities)
+5. [Integrating with APIs](#integrating-with-apis)
+6. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
 To install sru-queryer, just run `pip install sru-queryer`
 
 Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
 
@@ -194,14 +180,46 @@
 
 1. a search term,
 2. an index_name, relation, and search term,
 3. a context_set, index_name, relation, and search term.
 
 - RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SearchClause object. Keep in mind that these are validated the same as the SearchClause class.
+
+You MUST include 'type' for this to be recognized as a SearchClause. The same 'COMBINATIONS OF INITIALIZATION PROPERTIES' exist for this dict, and you don't need to include keys that you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
+In Python
+
+```python
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
 <br>
 <br>
 
 ### SRUQueryer
 
 `from sru_queryer import SRUQueryer`
 
@@ -275,17 +293,22 @@
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
+`from_dict`
+| Mandatory | Data Type | Description |
+| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
+| No | dict | A python dictionary representing an SRU Configuration, which will be used INSTEAD of the above options + contacting the SRU server. Do not create this dictionary yourself; it is meant to re-load a saved configuration which is created with the get_configuration() function.|
+
 #### AVAILABLE FUNCTIONS:
 
-There are three functions that the general user would want to use:
+There are four functions that the general user would want to use:
 
 ##### `search_retrieve`
 
 This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
 
 ##### USAGE
 
@@ -294,23 +317,24 @@
 
 There are additional options to you can set to modify the request. They will be discussed below.
 
 This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                                                          |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 <br>
 
 ##### `construct_search_retrieve_request`
 
 This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
 
@@ -319,30 +343,35 @@
 After initializing your SRUQueryer class: <br>
 `request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
 
 This will validate the request and return a requests.Request object.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                               |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 ##### `format_available_indexes`
 
 This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
 
 `format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
 
+##### `get_configuration`
+
+Gets a python dict representing the SRUQueryer. This allows saving the SRU queryer and allows you to re-create it without contacting the SRU server or setting the options again.
+
 <br>
 <br>
 
 ### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
@@ -384,14 +413,42 @@
 | Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
 Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a boolean operator object. Keep in mind that these are validated the same as the Boolean Operator class, so the requirements are all the same. This will NOT work with a custom boolean operator that extends the functionality of CQLBooleanOperatorBase.
+
+You MUST include 'type' and 'operator' for a dict to be recognized as a Boolean Operator. The 'conditions' array, just like above, is required and can contain SearchClause dicts, Boolean Operator dicts, or RawCQL dicts.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
+In Python
+
+```python
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
 <br>
 <br>
 
 ### Custom queries: RawCQL
 
 `from sru_queryer.cql import RawCQL`
 
@@ -426,14 +483,40 @@
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
 | -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
 | add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a RawCQL object. Keep in mind that this works the same as the above object EXCEPT that padding is automatically added.
+
+You MUST include 'type' for this dict to be recognized as RawCQL. Both keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "rawCQL",
+  "cql": "alma.title=Maryland"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "rawCQL",
+   "cql": "alma.title=Maryland"
+}
+```
+
 <br>
 <br>
 
 ### Modifiying operators - Modifiers
 
 Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
@@ -494,14 +577,44 @@
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
 You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a unique dict representation for use with the from_dict option for searches. It's the same as the above, but with the addition of a 'type' key which tells the library what this dict should be treated as.
+
+You MUST include 'type' for this dict to be recognized as a sortBy clause. As with the SortBy dict, all keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sort",
+  "index_set": "alma",
+  "index_name": "creator",
+  "sort_order": "ascending"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sort",
+   "index_set": "alma",
+   "index_name": "creator",
+   "sort_order": "ascending"
+}
+```
+
 <br>
 <br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
@@ -522,14 +635,138 @@
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SortKey object, so this dict will be used and validated in the same way as the SortKey object.
+
+You MUST include 'type' for this dict to be recognized as a SortKey. The other options are the same as the SortKey class (only xpath is required). You don't need to include the keys you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sortKey",
+   "xpath": "cql.author",
+   "schema": "marcxml",
+   "ascending": False,
+   "case_sensitive": True,
+   "missing_value": None
+}
+```
+
+<br>
+<br>
+
+---
+
+## Integrating with APIs
+
+New in version 2.1.0, this library has been significantly expanded to work with APIs. This includes:
+
+1. The capability to import/export SRU configurations from JSON.
+2. The ability for the queryer to accept a dictionary (parsed from JSON with json.loads() or created directly in Python) instead of the python objects mentioned above.
+
+### Importing/Exporting SRU Configurations
+
+This allows your application - particularly a web API - to easily save SRU configurations and use them between requests.
+
+Exporting an SRU Configuration: `sru_configuration_dict = queryer.get_configuration()`<br>
+Creating a queryer from a saved SRU configuration (Importing): `queryer = SRUQueryer(from_dict=sru_configuration_dict)`
+
+### Conducting a SearchRetrieve Request with JSON
+
+This makes creating dynamic queries a lot easier, particularly if you are using this library on a backend API. Just pass it the properly-formatted JSON dictionary, and it will validate the query just as if you have created it with the python objects mentioned above. Note that the required keys are the same for the dicts as the objects, so you can safely omit the ones you don't need.
+
+Note - Modifiers are not supported with this method of interaction at this time.
+
+#### Usage
+
+Say you have some JSON, either from a file or coming in from an API. This is an example of a properly-formatted JSON dictionary that can be used by the library (SRU version 1.2):
+
+```json
+{
+  "start_record": 4,
+  "maximum_records": 3,
+  "record_schema": "dc",
+  "record_packing": null,
+  "cql_query": {
+    "type": "booleanOperator",
+    "operator": "AND",
+    "conditions": [
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "title",
+        "relation": "=",
+        "search_term": "Maryland"
+      },
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "item_createDate",
+        "relation": ">",
+        "search_term": "1950"
+      }
+    ]
+  },
+  "sort_queries": [
+    {
+      "type": "sort",
+      "index_set": "alma",
+      "index_name": "creator",
+      "sort_order": "ascending"
+    }
+  ]
+}
+```
+
+Note that 'type' is the same for each instace of a 'type' of resource. For example, boolean operators will always have 'type' = 'booleanOperator'. Boolean Operators must also have an operator string, which should be 'AND', 'OR', 'NOT', or 'PROX'.
+
+First, if this JSON is not automatically converted into a python dictionary, use json.loads() to get it into a python dictionary.
+
+Next, simply pass this dictionary into either of the SearchRetrieve functions in your queryer!
+
+queryer.search_retrieve(from_dict=parsed_json_dict)<br>
+or <br>
+request = queryer.construct_search_retrieve_request(from_dict=parsed_json_dict)
+
+For version 1.1, the sort_queries will look different due to them being SortKeys instead. SortKey JSON format looks like:
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+Any of these values can be null except 'type' and 'xpath'
 <br>
 <br>
 
 ---
 
 ## Known Incompatibilities
```

### Comparing `sru_queryer-2.0.0/pyproject.toml` & `sru_queryer-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sru-queryer"
-version = "2.0.0"
+version = "2.1.0"
 description = "A utility for integrating SRU queries into your applications."
 readme = "readme.md"
 requires-python = ">=3.7.17"
 keywords = ["sru", "library", "api"]
 
 authors = [
     {name = "Erik Jones", email = "ejones99@umd.edu"},
```

### Comparing `sru_queryer-2.0.0/readme.md` & `sru_queryer-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: sru-queryer
+Version: 2.1.0
+Summary: A utility for integrating SRU queries into your applications.
+Author-email: Erik Jones <ejones99@umd.edu>
+Maintainer-email: USMAI <libclas@umd.edu>
+Keywords: sru,library,api
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7.17
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.27.1
+Requires-Dist: xmltodict>=0.13.0
+
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
 
 1. It handles validating much of the searchRetrieve request. This is particularly helpful because many SRU servers don't have good error messages.
@@ -21,15 +36,16 @@
    1. [SearchClause](#basic-query-component-searchclause-1)
    2. [SRUQueryer](#sruqueryer)
    3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
    4. [RawCQL](#custom-queries-rawcql)
    5. [Modifiers](#modifiying-operators---modifiers)
    6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
    7. [Sorting in v1.1](#sorting-in-11-SortKey)
-5. [Known Incompatibilities](#known-incompatibilities)
+5. [Integrating with APIs](#integrating-with-apis)
+6. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
 To install sru-queryer, just run `pip install sru-queryer`
 
 Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
 
@@ -179,14 +195,46 @@
 
 1. a search term,
 2. an index_name, relation, and search term,
 3. a context_set, index_name, relation, and search term.
 
 - RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SearchClause object. Keep in mind that these are validated the same as the SearchClause class.
+
+You MUST include 'type' for this to be recognized as a SearchClause. The same 'COMBINATIONS OF INITIALIZATION PROPERTIES' exist for this dict, and you don't need to include keys that you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
+In Python
+
+```python
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
 <br>
 <br>
 
 ### SRUQueryer
 
 `from sru_queryer import SRUQueryer`
 
@@ -260,17 +308,22 @@
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
+`from_dict`
+| Mandatory | Data Type | Description |
+| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
+| No | dict | A python dictionary representing an SRU Configuration, which will be used INSTEAD of the above options + contacting the SRU server. Do not create this dictionary yourself; it is meant to re-load a saved configuration which is created with the get_configuration() function.|
+
 #### AVAILABLE FUNCTIONS:
 
-There are three functions that the general user would want to use:
+There are four functions that the general user would want to use:
 
 ##### `search_retrieve`
 
 This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
 
 ##### USAGE
 
@@ -279,23 +332,24 @@
 
 There are additional options to you can set to modify the request. They will be discussed below.
 
 This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                                                          |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 <br>
 
 ##### `construct_search_retrieve_request`
 
 This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
 
@@ -304,30 +358,35 @@
 After initializing your SRUQueryer class: <br>
 `request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
 
 This will validate the request and return a requests.Request object.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                               |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 ##### `format_available_indexes`
 
 This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
 
 `format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
 
+##### `get_configuration`
+
+Gets a python dict representing the SRUQueryer. This allows saving the SRU queryer and allows you to re-create it without contacting the SRU server or setting the options again.
+
 <br>
 <br>
 
 ### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
@@ -369,14 +428,42 @@
 | Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
 Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a boolean operator object. Keep in mind that these are validated the same as the Boolean Operator class, so the requirements are all the same. This will NOT work with a custom boolean operator that extends the functionality of CQLBooleanOperatorBase.
+
+You MUST include 'type' and 'operator' for a dict to be recognized as a Boolean Operator. The 'conditions' array, just like above, is required and can contain SearchClause dicts, Boolean Operator dicts, or RawCQL dicts.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
+In Python
+
+```python
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
 <br>
 <br>
 
 ### Custom queries: RawCQL
 
 `from sru_queryer.cql import RawCQL`
 
@@ -411,14 +498,40 @@
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
 | -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
 | add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a RawCQL object. Keep in mind that this works the same as the above object EXCEPT that padding is automatically added.
+
+You MUST include 'type' for this dict to be recognized as RawCQL. Both keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "rawCQL",
+  "cql": "alma.title=Maryland"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "rawCQL",
+   "cql": "alma.title=Maryland"
+}
+```
+
 <br>
 <br>
 
 ### Modifiying operators - Modifiers
 
 Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
@@ -479,14 +592,44 @@
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
 You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a unique dict representation for use with the from_dict option for searches. It's the same as the above, but with the addition of a 'type' key which tells the library what this dict should be treated as.
+
+You MUST include 'type' for this dict to be recognized as a sortBy clause. As with the SortBy dict, all keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sort",
+  "index_set": "alma",
+  "index_name": "creator",
+  "sort_order": "ascending"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sort",
+   "index_set": "alma",
+   "index_name": "creator",
+   "sort_order": "ascending"
+}
+```
+
 <br>
 <br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
@@ -507,14 +650,138 @@
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SortKey object, so this dict will be used and validated in the same way as the SortKey object.
+
+You MUST include 'type' for this dict to be recognized as a SortKey. The other options are the same as the SortKey class (only xpath is required). You don't need to include the keys you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sortKey",
+   "xpath": "cql.author",
+   "schema": "marcxml",
+   "ascending": False,
+   "case_sensitive": True,
+   "missing_value": None
+}
+```
+
+<br>
+<br>
+
+---
+
+## Integrating with APIs
+
+New in version 2.1.0, this library has been significantly expanded to work with APIs. This includes:
+
+1. The capability to import/export SRU configurations from JSON.
+2. The ability for the queryer to accept a dictionary (parsed from JSON with json.loads() or created directly in Python) instead of the python objects mentioned above.
+
+### Importing/Exporting SRU Configurations
+
+This allows your application - particularly a web API - to easily save SRU configurations and use them between requests.
+
+Exporting an SRU Configuration: `sru_configuration_dict = queryer.get_configuration()`<br>
+Creating a queryer from a saved SRU configuration (Importing): `queryer = SRUQueryer(from_dict=sru_configuration_dict)`
+
+### Conducting a SearchRetrieve Request with JSON
+
+This makes creating dynamic queries a lot easier, particularly if you are using this library on a backend API. Just pass it the properly-formatted JSON dictionary, and it will validate the query just as if you have created it with the python objects mentioned above. Note that the required keys are the same for the dicts as the objects, so you can safely omit the ones you don't need.
+
+Note - Modifiers are not supported with this method of interaction at this time.
+
+#### Usage
+
+Say you have some JSON, either from a file or coming in from an API. This is an example of a properly-formatted JSON dictionary that can be used by the library (SRU version 1.2):
+
+```json
+{
+  "start_record": 4,
+  "maximum_records": 3,
+  "record_schema": "dc",
+  "record_packing": null,
+  "cql_query": {
+    "type": "booleanOperator",
+    "operator": "AND",
+    "conditions": [
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "title",
+        "relation": "=",
+        "search_term": "Maryland"
+      },
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "item_createDate",
+        "relation": ">",
+        "search_term": "1950"
+      }
+    ]
+  },
+  "sort_queries": [
+    {
+      "type": "sort",
+      "index_set": "alma",
+      "index_name": "creator",
+      "sort_order": "ascending"
+    }
+  ]
+}
+```
+
+Note that 'type' is the same for each instace of a 'type' of resource. For example, boolean operators will always have 'type' = 'booleanOperator'. Boolean Operators must also have an operator string, which should be 'AND', 'OR', 'NOT', or 'PROX'.
+
+First, if this JSON is not automatically converted into a python dictionary, use json.loads() to get it into a python dictionary.
+
+Next, simply pass this dictionary into either of the SearchRetrieve functions in your queryer!
+
+queryer.search_retrieve(from_dict=parsed_json_dict)<br>
+or <br>
+request = queryer.construct_search_retrieve_request(from_dict=parsed_json_dict)
+
+For version 1.1, the sort_queries will look different due to them being SortKeys instead. SortKey JSON format looks like:
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+Any of these values can be null except 'type' and 'xpath'
 <br>
 <br>
 
 ---
 
 ## Known Incompatibilities
```

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_cql_boolean_operators.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_cql_boolean_operators.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,39 @@
 from ._cql_modifiers import AndOrNotModifier, CQLModifierBase
 
 
 class CQLBooleanOperatorBase:
     operator = None
     unary_operator_error = "Error during formatting: Operator cannot have one argument AND the first condition of a parent operator (including if it's used by itself). No operators are unary, even NOT."
 
-    def __init__(self, *args, modifiers: list[AndOrNotModifier] = None):
+    def __init__(self, *args, modifiers: list[AndOrNotModifier] = None, from_dict: dict | None = None):
         self.conditions = []
 
-        for condition in args:
+        conditions_to_loop_through = []
+        if from_dict:
+            try:
+                self.operator = from_dict["operator"]
+            except KeyError:
+                ValueError(f"Operator dict is invalid: {from_dict.__str__()}")
+            for condition in from_dict["conditions"]:
+                try:
+                    if condition["type"] == "searchClause":
+                        conditions_to_loop_through.append(SearchClause(from_dict=condition))
+                    elif condition["type"] == "booleanOperator":
+                        conditions_to_loop_through.append(CQLBooleanOperatorBase(from_dict=condition))
+                    elif condition["type"] == "rawCQL":
+                        conditions_to_loop_through.append(RawCQL(from_dict=condition))
+                    else:
+                        raise KeyError()
+                except KeyError:
+                    ValueError(f"Condition is invalid: {condition.__str__()}")
+        else:
+            conditions_to_loop_through = args
+
+        for condition in conditions_to_loop_through:
             if isinstance(condition, SearchClause) or isinstance(condition, CQLBooleanOperatorBase) or isinstance(condition, RawCQL):
                 self.conditions.append(condition)
             else:
                 raise ValueError(
                     f"Condition '{condition.__str__()}' is not valid")
 
         if not self.conditions:
@@ -36,17 +57,16 @@
 
         formatted_conditional = ""
         is_first_condition_of_conditions = True
         for operator_is_index_or_raw_cql in self.conditions:
 
             parent_is_first_condition_of_parent = is_first_condition_of_parent
             # For clarity, I've set this variable name here. This means,
-            # "the parent of this condition (which is 'self', the object
-            # that this function is in) is the first condition in its
-            # parent operator (or, its the first level operator)"
+            # "the parent of this condition is the first condition in its
+            # parent operator."
 
             parent_is_unary_operator = is_unary_operator
             # Same deal as above. Now referring to the parent of this conditional in
             # the loop, which is 'self'
 
             condition_is_operator = isinstance(
                 operator_is_index_or_raw_cql, CQLBooleanOperatorBase)
@@ -105,14 +125,16 @@
         for condition in self.conditions:
             condition.validate(sru_configuration)
 
         if self.modifiers:
             for modifier in self.modifiers:
                 modifier.validate(sru_configuration)
 
+    
+
 
 class AND(CQLBooleanOperatorBase):
     operator = "and"
 
 
 class OR(CQLBooleanOperatorBase):
     operator = "or"
```

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_cql_modifiers.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_cql_modifiers.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_exceptions.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_exceptions.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_search_clause.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_search_clause.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,32 +14,50 @@
         a search_term,\n
         index_name + relation + search_term,\n
         OR context_set + index_name + relation + search_term.\n
 
     Modifiers will only be included if there's an relation.
         """
 
-    def __init__(self, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, search_term: str | None = None, modifiers: list[RelationModifier] | None = None):
-        self._context_set: str = context_set
-        self._index_name: str = index_name
-        self._relation: str = relation
-        self._search_term: str = search_term
-        self._modifiers = modifiers
+    def __init__(self, context_set: str | None = None, index_name: str | None = None, relation: str | None = None, search_term: str | None = None, modifiers: list[RelationModifier] | None = None, from_dict: dict | None = None):
+        self._context_set: str = context_set if not from_dict else None
+        self._index_name: str = index_name if not from_dict else None
+        self._relation: str = relation if not from_dict else None
+        self._search_term: str = search_term if not from_dict else None
+        self._modifiers = modifiers if not from_dict else None
+
+        if from_dict:
+            try:
+                if from_dict["type"] != "searchClause":
+                    raise ValueError(f"Search Clause type '{from_dict["type"]}' is not valid")
+                
+                if "context_set" in from_dict.keys():
+                    self._context_set: str = from_dict["context_set"]
+
+                if "index_name" in from_dict.keys():
+                    self._index_name: str = from_dict["index_name"]
+
+                if "relation" in from_dict.keys():
+                    self._relation: str = from_dict["relation"]
+                    
+                self._search_term: str = from_dict["search_term"]
+            except KeyError as ke:
+                raise ValueError(f"Invalid dictionary for creating a search clause: '{from_dict.__str__()}'. You're missing {ke.__str__()}.")
 
-        search_term_exists = search_term != None
+        search_term_exists = self._search_term != None
         if not search_term_exists:
             raise ValueError("You must provide a search term (search_term)")
 
-        if index_name and not relation:
+        if self._index_name and not self._relation:
             raise ValueError(
                 "If you include an index, you must include an relation")
-        if relation and not index_name:
+        if self._relation and not self._index_name:
             raise ValueError(
                 "If you include an relation, you must include an index")
-        if context_set and not index_name:
+        if self._context_set and not self._index_name:
             raise ValueError(
                 "If you have a context set, you must include an index.")
 
     def get_index_name(self):
         return self._index_name
 
     def get_relation(self):
@@ -87,8 +105,8 @@
 
     def validate(self, sru_configuration: SRUConfiguration):
         SRUValidator.validate_cql(sru_configuration, self._context_set,
             self._index_name, self._relation, self._search_term)
 
         if self._modifiers:
             for modifier in self._modifiers:
-                modifier.validate(sru_configuration)
+                modifier.validate(sru_configuration)
```

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_aux_formatter.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_sru_aux_formatter.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_explain_auto_parser.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_sru_explain_auto_parser.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_queryer.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_sru_queryer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import logging
 import xmltodict
 import requests
 from requests import Request
-from urllib3.exceptions import NewConnectionError
 
 from ._sru_aux_formatter import SRUAuxiliaryFormatter
 from ._exceptions import NoExplainResponseException, ExplainResponseContentTypeException, ExplainResponseParserException
 from ._sru_explain_auto_parser import SRUExplainAutoParser
 from ._sru_configuration import SRUConfiguration
 from ._search_clause import SearchClause
 from ._raw_cql import RawCQL
 from ._cql_boolean_operators import CQLBooleanOperatorBase
 from ._sort_key import SortKey
 from ._search_retrieve import SearchRetrieve
 
 class SRUQueryer():
     supported_sru_versions = ["1.2", "1.1"]
     
-    def __init__(self, server_url: str, sru_version: str = None, username: str | None = None, password: str | None = None, default_cql_context_set: str | None = None, default_cql_index: str | None = None, default_cql_relation: str | None = None, disable_validation_for_cql_defaults: bool = False, max_records_supported: int | None = None, default_records_returned: int | None = None , default_record_schema: str | None = None, default_sort_schema: str | None = None):
+    def __init__(self, server_url: str = None, sru_version: str = None, username: str | None = None, password: str | None = None, default_cql_context_set: str | None = None, default_cql_index: str | None = None, default_cql_relation: str | None = None, disable_validation_for_cql_defaults: bool = False, max_records_supported: int | None = None, default_records_returned: int | None = None , default_record_schema: str | None = None, default_sort_schema: str | None = None, from_dict: dict | None = None):
         """Raises ExplainResponseContentTypeException, NoExplainResponseException, ExplainResponseParserException, or PermissionError"""
+        # Ability to load from saved configuration. DO NOT CREATE MANUALLY.
+        if from_dict:
+            self.sru_configuration = SRUConfiguration(from_dict)
+            return
+        
         sru_version_to_use = sru_version
         if not sru_version_to_use:
             sru_version_to_use = "1.2"
         elif sru_version_to_use not in self.supported_sru_versions:
             logging.warning(f"SRU version {sru_version_to_use} is not supported. Defaulting to version 1.2...")
             sru_version_to_use = "1.2"
 
@@ -98,36 +102,36 @@
 
         if default_sort_schema:
             if configuration.default_sort_schema and (configuration.default_sort_schema != default_sort_schema): logging.warning(f"Overriding default sort schema (Using {default_sort_schema}, server specified {configuration.default_sort_schema}).")
             configuration.default_sort_schema = default_sort_schema
 
         self.sru_configuration = configuration
 
-    def search_retrieve(self, cql_query: SearchClause | CQLBooleanOperatorBase | RawCQL, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None, validate: bool = True) -> bytes:
+    def search_retrieve(self, cql_query: SearchClause | CQLBooleanOperatorBase | RawCQL | None = None, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None, validate: bool = True, from_dict: dict | None = None) -> bytes:
         """Conducts a searchRetrieve request and returns the response.
 
         This will throw ValueErrors for any incorrect portion of the query. 
         
         This function does not handle any errors in the searchRetrieveResponse."""
-        query = SearchRetrieve(self.sru_configuration, cql_query, start_record, maximum_records, record_schema, sort_queries, record_packing)
+        query = SearchRetrieve(self.sru_configuration, cql_query, start_record, maximum_records, record_schema, sort_queries, record_packing, from_dict)
         if validate:
             query.validate()
         request = query.construct_request()
         logging.info(f"Querying {request.url}")
         request = request.prepare()
         s = requests.Session()
         response = s.send(request)
         return response.content
     
-    def construct_search_retrieve_request(self, cql_query: SearchClause | CQLBooleanOperatorBase | RawCQL, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None, validate: bool = True) -> Request:
+    def construct_search_retrieve_request(self, cql_query: SearchClause | CQLBooleanOperatorBase | RawCQL | None = None, start_record: int | None = None, maximum_records: int | None = None, record_schema: str | None = None, sort_queries: list[dict] | list[SortKey] | None = None, record_packing: str | None = None, validate: bool = True, from_dict: dict | None = None) -> Request:
         """Construct a requests.Request object, which you can then prepare and use.
         
         This is helpful (as compared to search_retrieve) when you want to create a request, and perhaps modify it
         or use it with your own session mechanism."""
-        query = SearchRetrieve(self.sru_configuration, cql_query, start_record, maximum_records, record_schema, sort_queries, record_packing)
+        query = SearchRetrieve(self.sru_configuration, cql_query, start_record, maximum_records, record_schema, sort_queries, record_packing, from_dict)
         if validate:
             query.validate()
         return query.construct_request()
     
     def format_available_indexes(self, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None):
         """Formats available indexes, and prints to the console by default.
 
@@ -136,14 +140,17 @@
 
         if title_filter:
             available_context_sets_and_indexes = self._filter_available_context_sets_and_indexes(
                 available_context_sets_and_indexes, title_filter)
 
         SRUAuxiliaryFormatter.format_available_indexes(available_context_sets_and_indexes, filename, print_to_console)
 
+    def get_configuration(self):
+        return self.sru_configuration.__dict__
+
     @staticmethod
     def _filter_available_context_sets_and_indexes(available_context_sets_and_indexes: dict, title: str = None) -> dict:
         new_dict: dict = {}
 
         for context_set in available_context_sets_and_indexes:
             matched_contents = {}
             for index_code in available_context_sets_and_indexes[context_set]:
```

### Comparing `sru_queryer-2.0.0/src/sru_queryer/_base/_sru_validator.py` & `sru_queryer-2.1.0/src/sru_queryer/_base/_sru_validator.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/src/sru_queryer.egg-info/PKG-INFO` & `sru_queryer-2.1.0/src/sru_queryer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sru-queryer
-Version: 2.0.0
+Version: 2.1.0
 Summary: A utility for integrating SRU queries into your applications.
 Author-email: Erik Jones <ejones99@umd.edu>
 Maintainer-email: USMAI <libclas@umd.edu>
 Keywords: sru,library,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7.17
@@ -36,15 +36,16 @@
    1. [SearchClause](#basic-query-component-searchclause-1)
    2. [SRUQueryer](#sruqueryer)
    3. [Boolean Operators (AND, OR, NOT, PROX)](#boolean-operators)
    4. [RawCQL](#custom-queries-rawcql)
    5. [Modifiers](#modifiying-operators---modifiers)
    6. [Sorting in v1.2](#sorting-in-12-sortby-clauses)
    7. [Sorting in v1.1](#sorting-in-11-SortKey)
-5. [Known Incompatibilities](#known-incompatibilities)
+5. [Integrating with APIs](#integrating-with-apis)
+6. [Known Incompatibilities](#known-incompatibilities)
 
 ## Setting Up The Environment
 
 To install sru-queryer, just run `pip install sru-queryer`
 
 Note that you may have to specify pip3 if you have python2 installed. The install will fail if you try to use python2's PIP.
 
@@ -194,14 +195,46 @@
 
 1. a search term,
 2. an index_name, relation, and search term,
 3. a context_set, index_name, relation, and search term.
 
 - RelationModifiers can be set for all combinations, but will only added to the final query on combinations with an relation.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SearchClause object. Keep in mind that these are validated the same as the SearchClause class.
+
+You MUST include 'type' for this to be recognized as a SearchClause. The same 'COMBINATIONS OF INITIALIZATION PROPERTIES' exist for this dict, and you don't need to include keys that you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
+In Python
+
+```python
+{
+  "type": "searchClause",
+  "context_set": "alma",
+  "index_name": "title",
+  "relation": "=",
+  "search_term": "Maryland"
+}
+```
+
 <br>
 <br>
 
 ### SRUQueryer
 
 `from sru_queryer import SRUQueryer`
 
@@ -275,17 +308,22 @@
 | No | string | The default record schema that's returned by the searchRetrieve operation. If you don't specify what record schema you want in an individual query, the default record schema (if set) will be used in that query. If the explainResponse includes a default record schema and you don't specify one, the explainResponse's record schema will be included in all queries. |
 
 `default_sort_schema`
 | Mandatory | Data Type | Description |
 | ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
 | No | string | The default schema that sort operations are run on. I don't know too much about this. I use it for validating sortKeys, which are only for version 1.1. If the sort schema is not included in a sort key, this value will be used to validate the sort key (not all schemas can sort).|
 
+`from_dict`
+| Mandatory | Data Type | Description |
+| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------------------- |
+| No | dict | A python dictionary representing an SRU Configuration, which will be used INSTEAD of the above options + contacting the SRU server. Do not create this dictionary yourself; it is meant to re-load a saved configuration which is created with the get_configuration() function.|
+
 #### AVAILABLE FUNCTIONS:
 
-There are three functions that the general user would want to use:
+There are four functions that the general user would want to use:
 
 ##### `search_retrieve`
 
 This function sends a search retrieve request, using the values you provide and the information parsed from the SRU ExplainResponse.
 
 ##### USAGE
 
@@ -294,23 +332,24 @@
 
 There are additional options to you can set to modify the request. They will be discussed below.
 
 This will validate and send the request. You will receive whatever content the SRU server sends back - it may be a searchRetrieveResponse, or it might be an error. This library does not currently validate or parse the response.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                               |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before sending it. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                                                          |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 <br>
 
 ##### `construct_search_retrieve_request`
 
 This does the same thing as the previous function, however instead of running request.prepare() and sending the request, it returns the requests.Request object. This allows you to be more flexible by modifying the request - for instance, if you want to use a shared requests.Session between multiple requests, or add a custom authentication header.
 
@@ -319,30 +358,35 @@
 After initializing your SRUQueryer class: <br>
 `request = queryer.construct_search_retrieve_request(OR(SearchClause("alma", "title", "=", "Harry"), SearchClause("alma", "title", "=", "Potter")), record_schema="marcxml")`
 
 This will validate the request and return a requests.Request object.
 
 ##### INPUT PARAMETERS
 
-| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                           |
-| --------------- | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                    |
-| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                     |
-| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                     |
-| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse. |
-| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                              |
-| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                         |
-| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                    |
+| Option          | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                      |
+| --------------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cql_query       | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | The CQL query you wish to execute.                                                                                                                                                                                                                                                                                               |
+| start_record    | int                                                             | No        | An offset - Every search produces a set on the server, but not all will be returned. This determines the first record in that set that will be returned (offset).                                                                                                                                                                |
+| maximum_records | int                                                             | No        | Set maximum amount of records that will be returned. The default for this, if not included, can be set through SRUQueryer initialization.create_configuration_for_server, by the explainResponse, or is set to 5.                                                                                                                |
+| record_schema   | string                                                          | No        | The format in which the searchRetrieveRessponse will return records. Default is 'marcxml.' Any value set here will be validated against the available record schemas listed in the explainResponse. REQUIRED if the default is not returned with the explainResponse.                                                            |
+| sort_queries    | list[dict] or list[SortKey]                                     | No        | A list of sortBy dictionaries, which add sort clauses to the dictionary. See below for more information.                                                                                                                                                                                                                         |
+| record_packing  | string                                                          | No        | The record packing that the record will be returned in (either xml or string)                                                                                                                                                                                                                                                    |
+| validate        | boolean (default True)                                          | No        | Whether or not to validate the query before returning the requests.Request object. You can disable validation if you think the library is falsely failing a query.                                                                                                                                                               |
+| from_dict       | dict                                                            | No        | Use a dict representation of the query instead of the built-in CQL classes. This is useful for APIs in particular. See the 'Integrating with APIs' section for more info. You can still include any of the previous parameters aside from cql_query - they will apply but be overwritten by any values in the dict (if included) |
 
 ##### `format_available_indexes`
 
 This function nicely formats all the indexes availabe for an SRU server, as well as their information. It then prints this information to the console, to a text file, or both. It only prints to the console by default. You can filter the indexes based on their human-readable title.
 
 `format_available_indexes(sru_configuration, filename: str | None = None, print_to_console: bool = True, title_filter: str | None = None)`
 
+##### `get_configuration`
+
+Gets a python dict representing the SRUQueryer. This allows saving the SRU queryer and allows you to re-create it without contacting the SRU server or setting the options again.
+
 <br>
 <br>
 
 ### Boolean Operators
 
 `from sru_queryer.cql import AND, OR, NOT, PROX`
 
@@ -384,14 +428,42 @@
 | Option                   | Data Type                                                       | Mandatory | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | ------------------------ | --------------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Positional arguments 1-n | SearchClause, class extending CQLBooleanOperatorBase, or RawCQL | Yes       | Search clauses, which will be joined by the boolean operator. Must have at least one, or two if it is the outermost condition or first condition in a parent operator.                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | modifiers                | list[Class extending CQLModifierBase]                           | No        | A list of modifiers for the boolean operator, which will be tacked on to the end of the operator. Keep in mind that modifiers will be added to each instance of the formatted operator - if there's 3 conditions in the operator, leading to two 'and' conditions, this list will be included for both 'and's. To get around this, you may use a nested Boolean Operator with one condition and add the modifiers to that operator. In this case, it will replace the parent's operator with its own, which has the modifiers. The rest of the parent's operators will not be affected. |
 
 Note: RawCQL classes may work in place of modifiers, however, this has not been tested.
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a boolean operator object. Keep in mind that these are validated the same as the Boolean Operator class, so the requirements are all the same. This will NOT work with a custom boolean operator that extends the functionality of CQLBooleanOperatorBase.
+
+You MUST include 'type' and 'operator' for a dict to be recognized as a Boolean Operator. The 'conditions' array, just like above, is required and can contain SearchClause dicts, Boolean Operator dicts, or RawCQL dicts.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
+In Python
+
+```python
+{
+  "type": "booleanOperator",
+  "operator": "AND",
+  "conditions": []
+}
+```
+
 <br>
 <br>
 
 ### Custom queries: RawCQL
 
 `from sru_queryer.cql import RawCQL`
 
@@ -426,14 +498,40 @@
 #### INITIALIZATION OPTIONS
 
 | Option         | Data Type              | Mandatory | Description                                                                                                                                                                                                           |
 | -------------- | ---------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | raw_cql_string | string (should be CQL) | Yes       | A CQL query as a string. Again, you don't have to provide it in a url-exact format, spaces and other special characters will be replaced by their compability characters later on if you're using the provided tools. |
 | add_padding    | boolean                | No        | Whether or not to add a space (%20) before and after the string upon formatting. Set to false by default.                                                                                                             |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a RawCQL object. Keep in mind that this works the same as the above object EXCEPT that padding is automatically added.
+
+You MUST include 'type' for this dict to be recognized as RawCQL. Both keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "rawCQL",
+  "cql": "alma.title=Maryland"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "rawCQL",
+   "cql": "alma.title=Maryland"
+}
+```
+
 <br>
 <br>
 
 ### Modifiying operators - Modifiers
 
 Modifiers are conditions which modify the search query operators (AND, "all", OR, etc). As indicated above, in version 1.2, they can either modify SearchClause relations or Boolean Operators.
 
@@ -494,14 +592,44 @@
 Which will be formatted to:
 `sortBy%20alma.creator/sort.ascending`
 
 All values are required. The sort_order can either be "ascending" or "descending."
 
 You should add all desired sortBy clauses to the SRUQueryer.search_retrieve or SRUQueryer.construct_search_retrieve_request in an array with the keyword argument 'sort_queries='
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a unique dict representation for use with the from_dict option for searches. It's the same as the above, but with the addition of a 'type' key which tells the library what this dict should be treated as.
+
+You MUST include 'type' for this dict to be recognized as a sortBy clause. As with the SortBy dict, all keys are required.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sort",
+  "index_set": "alma",
+  "index_name": "creator",
+  "sort_order": "ascending"
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sort",
+   "index_set": "alma",
+   "index_name": "creator",
+   "sort_order": "ascending"
+}
+```
+
 <br>
 <br>
 
 ### Sorting in 1.1: SortKey
 
 `from sru_queryer.sru import SortKey`
 
@@ -522,14 +650,138 @@
 | Option         | Data Type | Mandatory | Description                                                                                            |
 | -------------- | --------- | --------- | ------------------------------------------------------------------------------------------------------ |
 | xpath          | string    | Yes       | The xpath of the index you want to sort by. It's just the index name prefixed by the context set.      |
 | schema         | string    | No        | The record schema you want to search by                                                                |
 | ascending      | boolean   | No        | Whether you want the results to be ascending. Default is True, False will set results to be descending |
 | case_sensitive | boolean   | No        | If case should be important during the search. Default is False.                                       |
 
+#### JSON / Dict representation
+
+As part of the 'Integrating with APIs' functionality (The second-to-last section), this class has a corresponding dict representation. Internally, the library will use this dict to create a SortKey object, so this dict will be used and validated in the same way as the SortKey object.
+
+You MUST include 'type' for this dict to be recognized as a SortKey. The other options are the same as the SortKey class (only xpath is required). You don't need to include the keys you aren't specifying.
+
+The format is as follows:
+
+In JSON
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+In Python
+
+```python
+{
+   "type": "sortKey",
+   "xpath": "cql.author",
+   "schema": "marcxml",
+   "ascending": False,
+   "case_sensitive": True,
+   "missing_value": None
+}
+```
+
+<br>
+<br>
+
+---
+
+## Integrating with APIs
+
+New in version 2.1.0, this library has been significantly expanded to work with APIs. This includes:
+
+1. The capability to import/export SRU configurations from JSON.
+2. The ability for the queryer to accept a dictionary (parsed from JSON with json.loads() or created directly in Python) instead of the python objects mentioned above.
+
+### Importing/Exporting SRU Configurations
+
+This allows your application - particularly a web API - to easily save SRU configurations and use them between requests.
+
+Exporting an SRU Configuration: `sru_configuration_dict = queryer.get_configuration()`<br>
+Creating a queryer from a saved SRU configuration (Importing): `queryer = SRUQueryer(from_dict=sru_configuration_dict)`
+
+### Conducting a SearchRetrieve Request with JSON
+
+This makes creating dynamic queries a lot easier, particularly if you are using this library on a backend API. Just pass it the properly-formatted JSON dictionary, and it will validate the query just as if you have created it with the python objects mentioned above. Note that the required keys are the same for the dicts as the objects, so you can safely omit the ones you don't need.
+
+Note - Modifiers are not supported with this method of interaction at this time.
+
+#### Usage
+
+Say you have some JSON, either from a file or coming in from an API. This is an example of a properly-formatted JSON dictionary that can be used by the library (SRU version 1.2):
+
+```json
+{
+  "start_record": 4,
+  "maximum_records": 3,
+  "record_schema": "dc",
+  "record_packing": null,
+  "cql_query": {
+    "type": "booleanOperator",
+    "operator": "AND",
+    "conditions": [
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "title",
+        "relation": "=",
+        "search_term": "Maryland"
+      },
+      {
+        "type": "searchClause",
+        "context_set": "alma",
+        "index_name": "item_createDate",
+        "relation": ">",
+        "search_term": "1950"
+      }
+    ]
+  },
+  "sort_queries": [
+    {
+      "type": "sort",
+      "index_set": "alma",
+      "index_name": "creator",
+      "sort_order": "ascending"
+    }
+  ]
+}
+```
+
+Note that 'type' is the same for each instace of a 'type' of resource. For example, boolean operators will always have 'type' = 'booleanOperator'. Boolean Operators must also have an operator string, which should be 'AND', 'OR', 'NOT', or 'PROX'.
+
+First, if this JSON is not automatically converted into a python dictionary, use json.loads() to get it into a python dictionary.
+
+Next, simply pass this dictionary into either of the SearchRetrieve functions in your queryer!
+
+queryer.search_retrieve(from_dict=parsed_json_dict)<br>
+or <br>
+request = queryer.construct_search_retrieve_request(from_dict=parsed_json_dict)
+
+For version 1.1, the sort_queries will look different due to them being SortKeys instead. SortKey JSON format looks like:
+
+```json
+{
+  "type": "sortKey",
+  "xpath": "cql.author",
+  "schema": "marcxml",
+  "ascending": false,
+  "case_sensitive": true,
+  "missing_value": null
+}
+```
+
+Any of these values can be null except 'type' and 'xpath'
 <br>
 <br>
 
 ---
 
 ## Known Incompatibilities
```

### Comparing `sru_queryer-2.0.0/src/sru_queryer.egg-info/SOURCES.txt` & `sru_queryer-2.1.0/src/sru_queryer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 tests/test_cql_boolean_operators.py
 tests/test_cql_modifiers.py
 tests/test_raw_cql.py
 tests/test_search_clause.py
 tests/test_search_retrieve.py
 tests/test_sort_key.py
 tests/test_sru_aux_formatter.py
+tests/test_sru_configuration.py
 tests/test_sru_explain_auto_parser.py
 tests/test_sru_queryer.py
 tests/test_sru_validator.py
```

### Comparing `sru_queryer-2.0.0/tests/test_cql_modifiers.py` & `sru_queryer-2.1.0/tests/test_cql_modifiers.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/tests/test_search_retrieve.py` & `sru_queryer-2.1.0/tests/test_sru_queryer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,198 +1,239 @@
-from unittest.mock import patch
 import unittest
+from unittest.mock import patch
+import json
 from requests import Request
 
-from src.sru_queryer._base._search_retrieve import SearchRetrieve
 from src.sru_queryer import SRUQueryer
+from src.sru_queryer._base._exceptions import ExplainResponseContentTypeException
 from src.sru_queryer.cql import SearchClause
-from src.sru_queryer.cql import AND, RawCQL
-from src.sru_queryer.sru import SortKey
-from tests.testData.test_data import TestFiles, get_alma_sru_configuration
-
-
-class TestSearchRetrieve(unittest.TestCase):
-
-    def test_construct_request(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-
-        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, SearchClause("alma", "bib_holding_count", "==", "10"), record_schema="marcxml").construct_request()
-
-        expected_request = Request(
-            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20==%20"10"')
-
-        self.assertEqual(
-            constructed_search_retrieve_request.method, expected_request.method)
-        self.assertEqual(
-            constructed_search_retrieve_request.url, expected_request.url)
-        self.assertEqual(
-            constructed_search_retrieve_request.headers, expected_request.headers)
-
-    def test_construct_request_complex(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-        sru_configuration.default_record_schema = "marcxml"
-
-        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, AND(
-            SearchClause("alma", "bib_holding_count", ">", "15"),
-            SearchClause("rec", "mms_id",  "==", "112233")
-        )).construct_request()
-
-        expected_request = Request(
-            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20>%20"15"%20and%20rec.mms_id%20==%20"112233"')
-
-        self.assertEqual(
-            constructed_search_retrieve_request.method, expected_request.method)
-        self.assertEqual(
-            constructed_search_retrieve_request.url, expected_request.url)
-        self.assertEqual(
-            constructed_search_retrieve_request.headers, expected_request.headers)
-
-    def test_construct_request_with_credentials(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-        sru_configuration.username = "test_user"
-        sru_configuration.password = "test_password"
-
-        constructed_search_retrieve_request = SearchRetrieve(sru_configuration, AND(
-            SearchClause("alma", "bib_holding_count", ">", "15"),
-            SearchClause("rec", "mms_id",  "==", "112233")
-        ), record_schema="marcxml").construct_request()
-
-        credentials_encoded = "dGVzdF91c2VyOnRlc3RfcGFzc3dvcmQ="
-        expected_request = Request(
-            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20>%20"15"%20and%20rec.mms_id%20==%20"112233"', headers={
-                "Authorization": f'Basic {credentials_encoded}'
-            })
-
-        self.assertEqual(
-            constructed_search_retrieve_request.method, expected_request.method)
-        self.assertEqual(
-            constructed_search_retrieve_request.url, expected_request.url)
-        self.assertEqual(
-            constructed_search_retrieve_request.headers, expected_request.headers)
-
-    def test_construct_request_with_sort_by(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-
-        constructed_search_retrieve_request = SearchRetrieve(sru_configuration,
-                                                    SearchClause("alma", "bib_holding_count", "==", '10'), record_schema="marcxml", sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}, {"index_set": "alma", "index_name": "title", "sort_order": "descending"}]).construct_request()
-
-        expected_request = Request(
-            "GET", f'https://example.com?version=1.2&operation=searchRetrieve&recordSchema=marcxml&query=alma.bib_holding_count%20==%20"10"%20sortBy%20alma.bib_holding_count/sort.ascending%20alma.title/sort.descending')
-
-        self.assertEqual(
-            constructed_search_retrieve_request.method, expected_request.method)
-        self.assertEqual(
-            constructed_search_retrieve_request.url, expected_request.url)
-        self.assertEqual(
-            constructed_search_retrieve_request.headers, expected_request.headers)
-
-    def test_validate_query_with_bad_record_schema_raises_error(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-
-        with self.assertRaises(ValueError) as ve:
-            SearchRetrieve(sru_configuration, SearchClause("alma", "action_note_note", "==", "10"), record_schema='fakefake').validate()
-
-        self.assertIn("'fakefake'", ve.exception.__str__())
-        self.assertIn("not available", ve.exception.__str__())
-
-    def test_validate_query_with_bad_default_record_schema_raises_error(self):
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-        sru_configuration.default_record_schema = "fakefake"
-
-        with self.assertRaises(ValueError) as ve:
-            SearchRetrieve(sru_configuration, SearchClause("alma", "action_note_note", "==", "10")).validate()
-
-        self.assertIn("'fakefake'", ve.exception.__str__())
-        self.assertIn("not available", ve.exception.__str__())
-
-    def test_validate_query_with_index_error_raises_error_query(self):
-        """Integration Test"""
-        sru_configuration = get_alma_sru_configuration()
-        sru_configuration.server_url = "https://example.com"
-        sru_configuration.sru_version = "1.2"
-        sru_configuration.default_records_returned = None
-
-        with self.assertRaises(ValueError) as ve:
-            SearchRetrieve(sru_configuration, SearchClause(
-                "alma", "fake_index", "==", "10"), record_schema="marcxml").validate()
-
-        self.assertIn("'fake_index'", ve.exception.__str__())
-                
-class TestQueryWithXMLData(unittest.TestCase):
-    @patch("src.sru_queryer._base._sru_queryer.requests.get")
-    def test_construct_request_gapines_data_default_schema_returned_by_explain(self, mock_get):
-        """Integration"""
-        with open(TestFiles.explain_response_gapines, "rb") as f:
-            mock_get.return_value.content = f.read()
-
-            # Initialize the gapines configuration
-            sru_configuration = SRUQueryer("https://example.com").sru_configuration
-
-            constructed_search_retrieve_request = SearchRetrieve(sru_configuration, SearchClause("alma", "bib_holding_count", "==", "10")).construct_request()
-
-            expected_request = Request(
-                "GET", f'https://example.com?version=1.1&operation=searchRetrieve&recordSchema=marcxml&maximumRecords=10&query=alma.bib_holding_count%20==%20"10"')
-            
-            self.assertEqual(
-                constructed_search_retrieve_request.url, expected_request.url)
-            
-    @patch("src.sru_queryer._base._sru_queryer.requests.get")
-    def test_initialize_1_2_query_with_invalid_sort_type_raises_error(self, mock_get):
-         with open(TestFiles.explain_response_alma, "rb") as f:
-            mock_get.return_value.content = f.read()
-
-            with self.assertRaises(ValueError) as ve:
-                sru_configuration = SRUQueryer("https://example.com").sru_configuration
-                SearchRetrieve(sru_configuration, SearchClause(search_term="dummyval"), record_schema="marcxml", sort_queries=[SortKey("example_xpath")])
-
-            self.assertIn("SortKeys", ve.exception.__str__())
-            self.assertIn("1.2", ve.exception.__str__())
-
-    @patch("src.sru_queryer._base._sru_queryer.requests.get")
-    def test_initialize_1_1_query_with_invalid_sort_type_raises_error(self, mock_get):
-        with open(TestFiles.explain_response_gapines, "rb") as f:
-            mock_get.return_value.content = f.read()
-
-            with self.assertRaises(ValueError) as ve:
-                sru_configuration = SRUQueryer("https://example.com").sru_configuration
-                SearchRetrieve(sru_configuration, SearchClause(search_term="dummyval"), sort_queries=[{"index_set": "alma", "index_name": "bib_holding_count", "sort_order": "ascending"}])
-            
-            self.assertIn("SortKeys", ve.exception.__str__())
-            self.assertIn("1.1", ve.exception.__str__())
-
-    @patch('src.sru_queryer._base._sru_queryer.requests.get')
-    def test_initialize_and_format_base_query_no_schema_no_error(self, mock_get):
-        """Integration"""
-        with open(TestFiles.explain_response_loc, "rb") as f:
-            mock_get.return_value.content = f.read()
-
-            sru_configuration = SRUQueryer("https://example.com").sru_configuration
-
-            SearchRetrieve(sru_configuration, RawCQL("pass")).validate()
-    
-    @patch('src.sru_queryer._base._sru_queryer.requests.get')
-    def test_initialize_query_default_schema_raises_no_error(self, mock_get):
-        """Integration"""
-        with open(TestFiles.explain_response_gapines, "rb") as f:
-            mock_get.return_value.content = f.read() 
-
-            sru_configuration = SRUQueryer("https://example.com").sru_configuration
+from tests.testData.test_data import get_alma_sru_configuration, get_gapines_sru_configuration, mock_searchable_indexes_and_descriptions, TestFiles, get_test_gapines_saved_sru_configuration
 
-            SearchRetrieve(sru_configuration, RawCQL("pass"))
+@patch("src.sru_queryer.SRUQueryer._retrieve_explain_response_xml")
+@patch("src.sru_queryer.SRUQueryer._parse_explain_response_configuration")
+class TestSRUQueryerInitialization(unittest.TestCase):
+
+    def test_merge_config_and_user_settings_urls_set_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com").sru_configuration
+
+        self.assertEqual(updated_config.server_url, "testurl2.com")
+
+    def test_merge_config_and_user_settings_version_updates_based_on_explain(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", sru_version="1.1").sru_configuration
+
+        self.assertEqual(updated_config.sru_version, "1.2")
+
+    def test_merge_config_and_user_settings_set_record_numbers_returned_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", default_records_returned=15, max_records_supported=40).sru_configuration
+
+        self.assertEqual(updated_config.default_records_returned, 15)
+        self.assertEqual(updated_config.max_records_supported, 40)
+
+    def test_merge_config_and_user_settings_set_username_password_returned_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", username="testusername", password="testpassword").sru_configuration
+
+        self.assertEqual(updated_config.username, "testusername")
+        self.assertEqual(updated_config.password, "testpassword")
+
+    def test_merge_config_and_user_settings_set_cql_defaults_returned_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", default_cql_context_set="alma", default_cql_index="all_for_ui", default_cql_relation="all").sru_configuration
+
+        self.assertEqual(updated_config.default_context_set, "alma")
+        self.assertEqual(updated_config.default_index, "all_for_ui")
+        self.assertEqual(updated_config.default_relation, "all")
+
+    def test_merge_config_and_user_settings_set_default_schemas_returned_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", default_record_schema="marcxml", default_sort_schema="marcxml").sru_configuration
+
+        self.assertEqual(updated_config.default_record_schema, "marcxml")
+        self.assertEqual(updated_config.default_sort_schema, "marcxml")
+
+    def test_merge_config_and_user_settings_set_disable_validation_for_cql_defaults_returned_correctly(self, mock_parse_explain_response, *args):
+        mock_parse_explain_response.return_value = get_alma_sru_configuration()
+
+        updated_config = SRUQueryer("testurl2.com", disable_validation_for_cql_defaults=True).sru_configuration
+
+        self.assertEqual(updated_config.disable_validation_for_cql_defaults, True)
+
+    def test_merge_config_and_user_settings_full_configuration_no_user_changes_stays_original(self, mock_parse_explain_response, *args):
+        configuration_parsed_from_explain_response = get_gapines_sru_configuration()
+        mock_parse_explain_response.return_value = configuration_parsed_from_explain_response
+
+        updated_config = SRUQueryer("testurl2.com").sru_configuration
+
+        self.assertEqual(updated_config.disable_validation_for_cql_defaults, False)
+        self.assertEqual(updated_config.default_context_set, "eg")
+        self.assertEqual(updated_config.default_index, "keyword")
+        self.assertEqual(updated_config.default_relation, "all")
+        self.assertEqual(updated_config.default_record_schema, "marcxml")
+        self.assertEqual(updated_config.default_sort_schema, "marcxml")
+        self.assertEqual(updated_config.default_records_returned, 10)
+        self.assertEqual(updated_config.max_records_supported, 50)
+        self.assertEqual(updated_config.sru_version, "1.1")
+
+    def test_initialize_from_dict(self, *args):
+        saved_dict = get_test_gapines_saved_sru_configuration()
+
+        sru_queryer = SRUQueryer(from_dict=saved_dict)
+
+        self.assertDictEqual(saved_dict, sru_queryer.sru_configuration.__dict__)
+
+    def test_get_configuration_information(self, *args):
+        saved_dict = get_test_gapines_saved_sru_configuration()
+
+        sru_queryer = SRUQueryer(from_dict=saved_dict)
+
+        self.assertDictEqual(saved_dict, sru_queryer.get_configuration())
+
+    @staticmethod
+    def create_index_info(title, id, sort, supported_relations, empty_term_supported) -> dict:
+        return {
+                "id": id,
+                "title": title,
+                "sort": sort,
+                "supported_relations": supported_relations,
+                "empty_term_supported": empty_term_supported
+    }
+
+    def verify_index_config_info(self, index, expected_index):
+        self.assertEqual(index["title"], expected_index["title"], "Title Incorrect!")
+        self.assertEqual(index["id"], expected_index["id"], "ID Incorrect! ")
+        self.assertEqual(index["sort"], expected_index["sort"], "Sort Incorrect!")
+        self.assertListEqual(index["supported_relations"], expected_index["supported_relations"], "Supported Operations incorrect!")
+        self.assertEqual(index["empty_term_supported"], expected_index["empty_term_supported"], "Empty Term Supported Incorrect!")
+
+
+    def test_filter_available_context_sets_and_indexes_different_capitalization(self, *args):
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
+            mock_searchable_indexes_and_descriptions, title="library")
+
+        self.assertDictEqual(filtered_dict, {
+            "alma": {
+                "library": {
+                    "id": None,
+                    "title": "Library Code",
+                    "sort": False,
+                    "supported_relations": ["==", "all"],
+                    "empty_term_supported": True
+                },
+                "library_status": {
+                    "id": None,
+                    "title": "Library Status",
+                    "sort": False,
+                    "supported_relations": ["==", "all"],
+                    "empty_term_supported": True
+                },
+            },
+        })
+
+    def test_filter_available_context_sets_and_indexes_different_set(self, *args):
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
+            mock_searchable_indexes_and_descriptions, title="mms")
+        
+        expected_index = self.create_index_info("Bib MMS ID", None, False, ["==", "all"], True)
+
+        self.verify_index_config_info(filtered_dict["rec"]["mms_id"], expected_index)
+
+
+    def test_filter_available_context_sets_and_indexes_two_sets(self, *args):
+        filtered_dict = SRUQueryer._filter_available_context_sets_and_indexes(
+            mock_searchable_indexes_and_descriptions, title="bib")
+
+        self.assertDictEqual(filtered_dict, {
+            "alma": {
+                "bib_holding_count": {
+                    "id": None,
+                    "title": "Bib Holding Count (Alma)",
+                    "sort": True,
+                    "supported_relations": [">", ">=", "==", "<", "<="],
+                    "empty_term_supported": True
+                },
+            },
+            "rec": {
+                "mms_id": {
+                    "id": None,
+                    "title": "Bib MMS ID",
+                    "sort": False,
+                    "supported_relations": ["==", "all"],
+                    "empty_term_supported": True
+                },
+            },
+        })
+
+class TestSRUQUeryerExplainResponseXMLParse(unittest.TestCase):
+
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_parse_html_raises_parser_failure_exception(self, mock_request_contents):
+        with open(TestFiles.gapines_html_response, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        with self.assertRaises(ExplainResponseContentTypeException) as pe:
+            SRUQueryer._retrieve_explain_response_xml("blahblah", None, None)
+        
+
+class TestInitializeSRUQueryerIntegration(unittest.TestCase):
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_construct_search_retrieve_request_not_validated_no_error(self, mock_request_contents):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        sc = SRUQueryer("https://server.com")
+        request = sc.construct_search_retrieve_request(SearchClause("fakecontextset", "bib", "=", "Radeon"), validate=False)
+
+    @patch("src.sru_queryer._base._sru_queryer.requests.Session.send")
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_search_retrieve_not_validated_no_error(self, mock_request_contents, *args):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        sc = SRUQueryer("https://server.com")
+        content = sc.search_retrieve(SearchClause("fakecontextset", "bib", "=", "Radeon"), validate=False)
+
+    @patch("src.sru_queryer._base._sru_queryer.requests.Session.send")
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_search_retrieve_with_dict(self, mock_request_contents, *args):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        with open("tests/testData/1_2_query_dict.json", "r") as f:
+            query_dict = json.loads(f.read()) 
+
+        sc = SRUQueryer("https://server.com")
+        content = sc.search_retrieve(from_dict=query_dict)
+
+    @patch("src.sru_queryer._base._sru_queryer.requests.Session.send")
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_search_retrieve_with_dict_invalid_value_fails(self, mock_request_contents, *args):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        with open("tests/testData/1_2_query_dict.json", "r") as f:
+            query_dict = json.loads(f.read()) 
+            query_dict["cql_query"]["conditions"][0]["index_name"] = "fake"
+
+        sc = SRUQueryer("https://server.com")
+        with self.assertRaises(ValueError):
+            sc.search_retrieve(from_dict=query_dict)
+
+    @patch("src.sru_queryer.SRUQueryer._get_request_contents")
+    def test_construct_search_retrieve_request_with_dict(self, mock_request_contents):
+        with open(TestFiles.explain_response_alma, "rb") as f:
+            mock_request_contents.return_value = f.read()
+
+        with open("tests/testData/1_2_query_dict.json", "r") as f:
+            query_dict = json.loads(f.read()) 
+
+        sc = SRUQueryer("https://server.com")
+        request: Request = sc.construct_search_retrieve_request(from_dict=query_dict)
+        self.assertIn("Frog", request.url)
```

### Comparing `sru_queryer-2.0.0/tests/test_sort_key.py` & `sru_queryer-2.1.0/tests/test_sort_key.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+import json
 
 from src.sru_queryer.sru import SortKey
 from tests.testData.test_data import MockSortKeyOne, MockSortKeyTwo
 
 class TestSortKey(unittest.TestCase):
 
     def test_initialize_sort_key(self):
@@ -85,7 +86,74 @@
     def test_format_array_of_sort_keys(self):
         sort_keys = [MockSortKeyOne("title", "dc", False), MockSortKeyTwo("name", "bath", missing_value="abort")]
 
         formatted_sort_keys = SortKey.format_array(sort_keys)
 
         self.assertEqual(formatted_sort_keys, "title,dc,0%20name,bath,,,abort")
 
+    def test_sort_key_from_dict(self):
+        sort_key = SortKey(from_dict = {
+            "type": "sortKey",
+            "xpath": "World",
+            "schema": "marcxml",
+            "ascending": "true",
+            "case_sensitive": "false",
+            "missing_value": "abort"
+        })
+
+        self.assertEqual(sort_key._xpath, "World")
+        self.assertEqual(sort_key._schema, "marcxml")
+        self.assertEqual(sort_key._ascending, True)
+        self.assertEqual(sort_key._case_sensitive, False)
+        self.assertEqual(sort_key._missing_value, "abort")
+
+    def test_sort_key_from_json(self):
+        with open("tests/testData/1_1_query_dict.json", "r") as f:
+            sort_key_dict = json.loads(f.read())["sort_queries"][1]
+
+        sort_key = SortKey(from_dict=sort_key_dict)
+
+        self.assertEqual(sort_key._xpath, "cql.author")
+        self.assertEqual(sort_key._schema, "marcxml")
+        self.assertEqual(sort_key._ascending, False)
+        self.assertEqual(sort_key._case_sensitive, True)
+        self.assertEqual(sort_key._missing_value, None)
+
+    def test_sort_key_from_json_string_bool_values(self):
+        with open("tests/testData/1_1_query_dict.json", "r") as f:
+            sort_key_dict = json.loads(f.read())["sort_queries"][0]
+
+        sort_key = SortKey(from_dict=sort_key_dict)
+
+        self.assertEqual(sort_key._xpath, "World")
+        self.assertEqual(sort_key._schema, "marcxml")
+        self.assertEqual(sort_key._ascending, True)
+        self.assertEqual(sort_key._case_sensitive, False)
+        self.assertEqual(sort_key._missing_value, "abort")
+
+    def test_sort_key_from_dict_minimal_values(self):
+        sort_key = SortKey(from_dict = {
+            "type": "sortKey",
+            "xpath": "World",
+            "schema": None,
+            "ascending": None,
+            "case_sensitive": None,
+            "missing_value": None
+        })
+
+        self.assertEqual(sort_key._xpath, "World")
+        self.assertEqual(sort_key._schema, None)
+        self.assertEqual(sort_key._ascending, None)
+        self.assertEqual(sort_key._case_sensitive, None)
+        self.assertEqual(sort_key._missing_value, None)
+
+    def test_sort_key_from_dict_required_values_only(self):
+        sort_key = SortKey(from_dict = {
+            "type": "sortKey",
+            "xpath": "World",
+        })
+
+        self.assertEqual(sort_key._xpath, "World")
+        self.assertEqual(sort_key._schema, None)
+        self.assertEqual(sort_key._ascending, None)
+        self.assertEqual(sort_key._case_sensitive, None)
+        self.assertEqual(sort_key._missing_value, None)
```

### Comparing `sru_queryer-2.0.0/tests/test_sru_aux_formatter.py` & `sru_queryer-2.1.0/tests/test_sru_aux_formatter.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/tests/test_sru_explain_auto_parser.py` & `sru_queryer-2.1.0/tests/test_sru_explain_auto_parser.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-2.0.0/tests/test_sru_validator.py` & `sru_queryer-2.1.0/tests/test_sru_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         self.assertIn("invalid", e.exception.__str__())
                 
     def test_validate_sort_key_schema_no_sort_raises_error(self):
         sru_configuration = get_alma_sru_configuration()
         sru_configuration.available_record_schemas = test_available_record_schemas_one_false
 
         with self.assertRaises(ValueError) as ve:
-            SRUValidator.validate_sort(sru_configuration, [SortKey("", schema="cnmarcxml")])
+            SRUValidator.validate_sort(sru_configuration, [SortKey("Moop", schema="cnmarcxml")])
 
         self.assertIn("'cnmarcxml'", ve.exception.__str__())
         self.assertIn("not available", ve.exception.__str__())
 
     def test_validate_sort_base_title_repeated_throws_error(self):
         sru_configuration = get_alma_sru_configuration()
         with self.assertRaises(ValueError) as ve:
```

