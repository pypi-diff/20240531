# Comparing `tmp/dagster-airbyte-0.23.7.tar.gz` & `tmp/dagster-airbyte-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.23.7.tar", last modified: Thu May 23 20:55:51 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.8.tar", last modified: Thu May 30 22:27:30 2024, max compression
```

## Comparing `dagster-airbyte-0.23.7.tar` & `dagster-airbyte-0.23.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48304 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282772 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34862 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 20:55:51.000000 dagster-airbyte-0.23.7/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-23 20:55:51.768871 dagster-airbyte-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1636 2024-05-23 20:50:32.000000 dagster-airbyte-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:30.462882 dagster-airbyte-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-30 22:27:30.462882 dagster-airbyte-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:30.458882 dagster-airbyte-0.23.8/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48293 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:30.458882 dagster-airbyte-0.23.8/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:30.462882 dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119692 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282709 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14596 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:30.458882 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 22:27:30.000000 dagster-airbyte-0.23.8/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-30 22:27:30.462882 dagster-airbyte-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-05-30 22:22:14.000000 dagster-airbyte-0.23.8/setup.py
```

### Comparing `dagster-airbyte-0.23.7/LICENSE` & `dagster-airbyte-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/PKG-INFO` & `dagster-airbyte-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.8/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.8/dagster_airbyte/asset_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,15 +948,15 @@
     connection_to_auto_materialize_policy_fn: Optional[
         Callable[[AirbyteConnectionMetadata], Optional[AutoMaterializePolicy]]
     ] = None,
 ) -> CacheableAssetsDefinition:
     """Loads an Airbyte project into a set of Dagster assets.
 
     Point to the root folder of an Airbyte project synced using the Octavia CLI. For
-    more information, see https://github.com/airbytehq/airbyte/tree/master/octavia-cli#octavia-import-all.
+    more information, see https://airbyte.com/tutorials/version-control-airbyte-configurations.
 
     Args:
         project_dir (str): The path to the root of your Airbyte project, containing sources, destinations,
             and connections folders.
         workspace_id (Optional[str]): The ID of the Airbyte workspace to load connections from. Only
             required if multiple workspace state YAMLfiles exist in the project.
         key_prefix (Optional[CoercibleToAssetKeyPrefix]): A prefix for the asset keys created.
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/destinations.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         ],
         azure_blob_storage_endpoint_domain_name: Optional[str] = None,
         azure_blob_storage_container_name: Optional[str] = None,
         azure_blob_storage_output_buffer_size: Optional[int] = None,
     ):
         """Airbyte Destination for Azure Blob Storage.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/destinations/azureblobstorage
+        Documentation can be found at https://docs.airbyte.com/integrations/destinations/azure-blob-storage
 
         Args:
             name (str): The name of the destination.
             azure_blob_storage_endpoint_domain_name (Optional[str]): This is Azure Blob Storage endpoint domain name. Leave default value (or leave it empty if run container from command line) to use Microsoft native from example.
             azure_blob_storage_container_name (Optional[str]): The name of the Azure blob storage container. If not exists - will be created automatically. May be empty, then will be created automatically airbytecontainer+timestamp
             azure_blob_storage_account_name (str): The account's name of the Azure Blob Storage.
             azure_blob_storage_account_key (str): The Azure blob storage account key.
@@ -1290,15 +1290,15 @@
 
 
 class CsvDestination(GeneratedAirbyteDestination):
     @public
     def __init__(self, name: str, destination_path: str):
         """Airbyte Destination for Csv.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/destinations/local-csv
+        Documentation can be found at https://docs.airbyte.com/integrations/destinations/csv
 
         Args:
             name (str): The name of the destination.
             destination_path (str): Path to the directory where csv files will be written. The destination uses the local mount "/local" and any data files will be placed inside that local mount. For more information check out our docs
         """
         self.destination_path = check.str_param(destination_path, "destination_path")
         super().__init__("Csv", name)
@@ -2465,15 +2465,15 @@
 
 
 class ScaffoldDestinationPythonDestination(GeneratedAirbyteDestination):
     @public
     def __init__(self, name: str, TODO: Optional[str] = None):
         """Airbyte Destination for Scaffold Destination Python.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/destinations/scaffold-destination-python
+        Documentation for this source is no longer available.
 
         Args:
             name (str): The name of the destination.
             TODO (Optional[str]): FIX ME
         """
         self.TODO = check.opt_str_param(TODO, "TODO")
         super().__init__("Scaffold Destination Python", name)
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.8/dagster_airbyte/managed/generated/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         password: str,
         auth_source: str,
         replica_set: Optional[str] = None,
         ssl: Optional[bool] = None,
     ):
         """Airbyte Source for Mongodb.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/mongodb
+        Documentation for this source is no longer available (see MongodbV2Source)
 
         Args:
             name (str): The name of the destination.
             host (str): Host of a Mongo database to be replicated.
             port (int): Port of a Mongo database to be replicated.
             database (str): Database to be replicated.
             user (str): User
@@ -955,15 +955,15 @@
 
 
 class KustomerSingerSource(GeneratedAirbyteSource):
     @public
     def __init__(self, name: str, api_token: str, start_date: str):
         """Airbyte Source for Kustomer Singer.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/kustomer
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/kustomer-singer
 
         Args:
             name (str): The name of the destination.
             api_token (str): Kustomer API Token. See the docs on how to obtain this
             start_date (str): The date from which you'd like to replicate the data
         """
         self.api_token = check.str_param(api_token, "api_token")
@@ -1007,15 +1007,15 @@
         username: str,
         replication_method: str,
         password: Optional[str] = None,
         jdbc_url_params: Optional[str] = None,
     ):
         """Airbyte Source for Scaffold Java Jdbc.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/scaffold_java_jdbc
+        Documentation for this source is no longer available.
 
         Args:
             name (str): The name of the destination.
             host (str): Hostname of the database.
             port (int): Port of the database.
             database (str): Name of the database.
             username (str): Username to use to access the database.
@@ -1151,15 +1151,15 @@
         start_date: str,
         view_id: str,
         custom_reports: Optional[str] = None,
         window_in_days: Optional[int] = None,
     ):
         """Airbyte Source for Google Analytics V4.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/google-analytics-universal-analytics
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/google-analytics-v4
 
         Args:
             name (str): The name of the destination.
             credentials (Union[GoogleAnalyticsV4Source.AuthenticateViaGoogleOauth, GoogleAnalyticsV4Source.ServiceAccountKeyAuthentication]): Credentials for the service
             start_date (str): The date in the format YYYY-MM-DD. Any data before this date will not be replicated.
             view_id (str): The ID for the Google Analytics View you want to fetch data from. This can be found from the Google Analytics Account Explorer.
             custom_reports (Optional[str]): A JSON array describing the custom reports you want to sync from Google Analytics. See the docs for more information about the exact format you can use to fill out this field.
@@ -1753,15 +1753,15 @@
         start_date: str,
         access_key: str,
         base: Optional[str] = None,
         ignore_weekends: Optional[bool] = None,
     ):
         """Airbyte Source for Exchange Rates.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/exchangeratesapi
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/exchange-rates
 
         Args:
             name (str): The name of the destination.
             start_date (str): Start getting data from that date.
             access_key (str): Your API Key. See here. The key is case sensitive.
             base (Optional[str]): ISO reference currency. See here. Free plan doesn't support Source Currency Switching, default base currency is EUR
             ignore_weekends (Optional[bool]): Ignore weekends? (Exchanges don't run on weekends)
@@ -2090,15 +2090,15 @@
             "ElasticsearchSource.None_",
             "ElasticsearchSource.ApiKeySecret",
             "ElasticsearchSource.UsernamePassword",
         ],
     ):
         r"""Airbyte Source for Elasticsearch.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/source/elasticsearch
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/elasticsearch
 
         Args:
             name (str): The name of the destination.
             endpoint (str): The full url of the Elasticsearch server
             authenticationMethod (Union[ElasticsearchSource.None\\_, ElasticsearchSource.ApiKeySecret, ElasticsearchSource.UsernamePassword]): The type of authentication to be used
         """
         self.endpoint = check.str_param(endpoint, "endpoint")
@@ -2171,15 +2171,15 @@
 class SearchMetricsSource(GeneratedAirbyteSource):
     @public
     def __init__(
         self, name: str, api_key: str, client_secret: str, country_code: str, start_date: str
     ):
         """Airbyte Source for Search Metrics.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/seacrh-metrics
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/search-metrics
 
         Args:
             name (str): The name of the destination.
             country_code (str): The region of the S3 staging bucket to use if utilising a copy strategy.
             start_date (str): Data generated in SearchMetrics after this date will be replicated. This date must be specified in the format YYYY-MM-DDT00:00:00Z.
         """
         self.api_key = check.str_param(api_key, "api_key")
@@ -3930,15 +3930,15 @@
         is_sandbox: bool,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         refresh_token: Optional[str] = None,
     ):
         """Airbyte Source for Paypal Transaction.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/paypal-transactions
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/paypal-transaction
 
         Args:
             name (str): The name of the destination.
             client_id (Optional[str]): The Client ID of your Paypal developer application.
             client_secret (Optional[str]): The Client Secret of your Paypal developer application.
             refresh_token (Optional[str]): The key to refresh the expired access token.
             start_date (str): Start Date for data extraction in ISO format. Date must be in range from 3 years till 12 hrs before present time.
@@ -4297,15 +4297,15 @@
 
 
 class PythonHttpTutorialSource(GeneratedAirbyteSource):
     @public
     def __init__(self, name: str, start_date: str, base: str, access_key: Optional[str] = None):
         """Airbyte Source for Python Http Tutorial.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/exchangeratesapi
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/exchange-rates
 
         Args:
             name (str): The name of the destination.
             access_key (Optional[str]): API access key used to retrieve data from the Exchange Rates API.
             start_date (str): UTC date and time in the format 2017-01-25. Any data before this date will not be replicated.
             base (str): ISO reference currency. See here.
         """
@@ -4894,15 +4894,15 @@
         credentials: Union["SftpSource.PasswordAuthentication", "SftpSource.SSHKeyAuthentication"],
         file_types: Optional[str] = None,
         folder_path: Optional[str] = None,
         file_pattern: Optional[str] = None,
     ):
         """Airbyte Source for Sftp.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/source/sftp
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/sftp
 
         Args:
             name (str): The name of the destination.
             user (str): The server user
             host (str): The server host address
             port (int): The server port
             credentials (Union[SftpSource.PasswordAuthentication, SftpSource.SSHKeyAuthentication]): The server authentication method
@@ -5272,15 +5272,15 @@
         name: str,
         subdomain: str,
         start_date: str,
         credentials: Union["ZendeskSunshineSource.OAuth20", "ZendeskSunshineSource.APIToken"],
     ):
         """Airbyte Source for Zendesk Sunshine.
 
-        Documentation can be found at https://docs.airbyte.com/integrations/sources/zendesk_sunshine
+        Documentation can be found at https://docs.airbyte.com/integrations/sources/zendesk-sunshine
 
         Args:
             name (str): The name of the destination.
             subdomain (str): The subdomain for your Zendesk Account.
             start_date (str): The date from which you'd like to replicate data for Zendesk Sunshine API, in the format YYYY-MM-DDT00:00:00Z.
         """
         self.subdomain = check.str_param(subdomain, "subdomain")
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.8/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.8/dagster_airbyte/managed/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     ) -> "AirbyteSyncMode":
         """Syncs new records from the source, appending to an append-only history
         table in the destination. Also generates a deduplicated view mirroring the
         source table. May optionally specify the cursor field used to determine
         which records are new, and the primary key used to determine which records
         are duplicates.
 
-        https://docs.airbyte.com/understanding-airbyte/connections/incremental-append-dedup/
+        https://docs.airbyte.com/using-airbyte/core-concepts/sync-modes/incremental-append-deduped
         """
         cursor_field = check.opt_str_param(cursor_field, "cursor_field")
         if isinstance(primary_key, str):
             primary_key = [primary_key]
         primary_key = check.opt_list_param(primary_key, "primary_key", of_type=str)
 
         return cls(
@@ -113,15 +113,15 @@
 
 class AirbyteSource:
     """Represents a user-defined Airbyte source.
 
     Args:
         name (str): The display name of the source.
         source_type (str): The type of the source, from Airbyte's list
-            of sources https://airbytehq.github.io/category/sources/.
+            of sources https://docs.airbyte.com/integrations/sources/.
         source_configuration (Mapping[str, Any]): The configuration for the
             source, as defined by Airbyte's API.
     """
 
     @public
     def __init__(self, name: str, source_type: str, source_configuration: Mapping[str, Any]):
         self.name = check.str_param(name, "name")
@@ -157,15 +157,15 @@
 
 class AirbyteDestination:
     """Represents a user-defined Airbyte destination.
 
     Args:
         name (str): The display name of the destination.
         destination_type (str): The type of the destination, from Airbyte's list
-            of destinations https://airbytehq.github.io/category/destinations/.
+            of destinations https://docs.airbyte.com/integrations/destinations/.
         destination_configuration (Mapping[str, Any]): The configuration for the
             destination, as defined by Airbyte's API.
     """
 
     @public
     def __init__(
         self, name: str, destination_type: str, destination_configuration: Mapping[str, Any]
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.8/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.8/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/types.py` & `dagster-airbyte-0.23.8/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.8/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.8/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.7/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.8/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.7/setup.py` & `dagster-airbyte-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
+        "dagster==1.7.8",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.23.7",
+            "dagster-managed-elements==0.23.8",
         ],
     },
 )
```

