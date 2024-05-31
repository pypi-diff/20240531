# Comparing `tmp/dwh_oppfolging-0.0.93.tar.gz` & `tmp/dwh_oppfolging-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.93.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.94.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.93.tar` & `dwh_oppfolging-0.0.94.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/LICENSE
--rw-r--r--   0        0        0      325 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/README.md
--rw-r--r--   0        0        0       22 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0       14 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/airflow_api_v1.py
--rw-r--r--   0        0        0     8543 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     4051 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1_types.py
--rw-r--r--   0        0        0    17798 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v2.py
--rw-r--r--   0        0        0     2297 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/dbt_oracle_api_v1.py
--rw-r--r--   0        0        0      422 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/generic_api_v1.py
--rw-r--r--   0        0        0      741 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0    24608 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1_types.py
--rw-r--r--   0        0        0    11838 2024-05-27 07:29:30.951534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      125 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1_types.py
--rw-r--r--   0        0        0     2371 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     6831 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0    11843 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1_types.py
--rw-r--r--   0        0        0        0 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/__init__.py
--rw-r--r--   0        0        0     9224 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/datatypes.py
--rw-r--r--   0        0        0     9521 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/functions.py
--rw-r--r--   0        0        0     1644 2024-05-27 07:29:30.955534 dwh_oppfolging-0.0.93/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/LICENSE
+-rw-r--r--   0        0        0      325 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/README.md
+-rw-r--r--   0        0        0       22 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/airflow_api_v1.py
+-rw-r--r--   0        0        0     8543 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     4051 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v1_types.py
+-rw-r--r--   0        0        0    17798 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v2.py
+-rw-r--r--   0        0        0     2297 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/dbt_oracle_api_v1.py
+-rw-r--r--   0        0        0      422 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/generic_api_v1.py
+-rw-r--r--   0        0        0      741 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0    24608 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/kafka_api_v1_types.py
+-rw-r--r--   0        0        0    11838 2024-05-31 06:33:11.030558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      125 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/oracle_api_v1_types.py
+-rw-r--r--   0        0        0     2371 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     6831 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0    11873 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/apis/ssb_api_v1_types.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/transforms/__init__.py
+-rw-r--r--   0        0        0     9224 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/transforms/datatypes.py
+-rw-r--r--   0        0        0     9521 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/dwh_oppfolging/transforms/functions.py
+-rw-r--r--   0        0        0     1644 2024-05-31 06:33:11.034558 dwh_oppfolging-0.0.94/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.94/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.93/LICENSE` & `dwh_oppfolging-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v1_types.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/brreg_api_v2.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/brreg_api_v2.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/dbt_oracle_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/dbt_oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/kafka_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/kafka_api_v1_types.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/kafka_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/oracle_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/secrets_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/secrets_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/ssb_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/apis/ssb_api_v1_types.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/apis/ssb_api_v1_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
     """Link to source version"""
     target_url: str
     """Link to target version"""
 
     @classmethod
     def from_json(cls, data: dict):
         """Constructs CorrespondenceHeader from an entry in the json-version's correspondenceTables"""
-        self_url = data["_links"]["self"]["href"].replace("http", "https")
-        source_url = data["_links"]["source"]["href"].replace("http", "https")
-        target_url = data["_links"]["target"]["href"].replace("http", "https")
+        self_url = data["_links"]["self"]["href"].replace("http:", "https:", 1)
+        source_url = data["_links"]["source"]["href"].replace("http:", "https:", 1)
+        target_url = data["_links"]["target"]["href"].replace("http:", "https:", 1)
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
         return CorrespondenceHeader(
             data["name"], data["owningSection"], data["source"], data["sourceId"], data["target"],
             data["targetId"], data["changeTable"], last_modified, self_url, source_url, target_url
         )
 
 
@@ -137,15 +137,15 @@
     """URL to full version data"""
     version_id: int
     """Version identifier"""
 
     @classmethod
     def from_json(cls, data: dict) -> Self:
         """Constructs VersionHeader from an entry in the json-classification's versions list"""
-        url: str = data["_links"]["self"]["href"].replace("http", "https")
+        url: str = data["_links"]["self"]["href"].replace("http:", "https:", 1)
         version_id: int = int(url[url.rfind("/")+1:])
         #valid_from = string_to_naive_norwegian_datetime(data["validFrom"])
         #valid_to = string_to_naive_norwegian_datetime(data["validTo"]) if "validTo" in data else None
         # trunc valid dates, these are in form yyyy-mm-dd, and should not have time of day
         valid_from = datetime.strptime(data["validFrom"], _VALID_DATE_FMT)
         valid_to = datetime.strptime(data["validTo"], _VALID_DATE_FMT) if "validTo" in data else None
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
@@ -174,15 +174,15 @@
     """Classification identifier"""
 
     @classmethod
     def from_json(cls, data: dict) -> Self:
         """Constructs Classification from json-classification"""
         versions = [VersionHeader.from_json(version) for version in data["versions"]]
         last_modified =  string_to_naive_norwegian_datetime(data["lastModified"])
-        url = data["_links"]["self"]["href"].replace("http", "https")
+        url = data["_links"]["self"]["href"].replace("http:", "https:", 1)
         classification_id = int(url[url.rindex("/") + 1 :])
         return cls(
             data["name"], last_modified, data["description"],
             data["includeShortName"], data["includeNotes"], data["statisticalUnits"],
             data["owningSection"], versions, classification_id
         )
     
@@ -226,15 +226,15 @@
         last_modified = string_to_naive_norwegian_datetime(data["lastModified"])
         #valid_from = string_to_naive_norwegian_datetime(data["validFrom"])
         #valid_to = string_to_naive_norwegian_datetime(data["validTo"]) if "validTo" in data else None
         # trunc valid dates, these are in form yyyy-mm-dd, and should not have time of day
         valid_from = datetime.strptime(data["validFrom"], _VALID_DATE_FMT)
         valid_to = datetime.strptime(data["validTo"], _VALID_DATE_FMT) if "validTo" in data else None
         corr_tables = [CorrespondenceHeader.from_json(corr) for corr in data["correspondenceTables"]]
-        url = data["_links"]["self"]["href"].replace("http", "https")
+        url = data["_links"]["self"]["href"].replace("http:", "https:", 1)
         version_id = int(url[url.rindex("/") + 1 :])
         return cls(
             data["name"], valid_from, valid_to, last_modified, data["introduction"], classification_id,
             version_id, data["owningSection"], data.get("derivedFrom"), data.get("changelogs"), data["levels"],
             data["classificationItems"], corr_tables
             )
```

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/datatypes.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/transforms/datatypes.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/dwh_oppfolging/transforms/functions.py` & `dwh_oppfolging-0.0.94/dwh_oppfolging/transforms/functions.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.93/pyproject.toml` & `dwh_oppfolging-0.0.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwh-oppfolging"
-version = "0.0.93"
+version = "0.0.94"
 description = "Oppfolging python package for DWH ETL"
 authors = ["Team Oppfølging"]
 packages = [{include = "dwh_oppfolging"}]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `dwh_oppfolging-0.0.93/PKG-INFO` & `dwh_oppfolging-0.0.94/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwh-oppfolging
-Version: 0.0.93
+Version: 0.0.94
 Summary: Oppfolging python package for DWH ETL
 Author: Team Oppfølging
 Requires-Python: ==3.11.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confluent-kafka (==2.4.0)
 Requires-Dist: dbt-oracle (==1.7.5)
```

