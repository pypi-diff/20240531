# Comparing `tmp/price2bq_zfullio-1.2.1.tar.gz` & `tmp/price2bq_zfullio-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "price2bq_zfullio-1.2.1.tar", max compression
+gzip compressed data, was "price2bq_zfullio-1.3.0.tar", max compression
```

## Comparing `price2bq_zfullio-1.2.1.tar` & `price2bq_zfullio-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-03-04 12:54:10.867735 price2bq_zfullio-1.2.1/LICENSE
--rw-r--r--   0        0        0      160 2024-03-04 12:54:10.867735 price2bq_zfullio-1.2.1/README.md
--rw-r--r--   0        0        0     1327 2024-03-04 13:44:33.241168 price2bq_zfullio-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      150 2024-03-04 12:54:10.867735 price2bq_zfullio-1.2.1/src/price2bq_zfullio/__init__.py
--rw-r--r--   0        0        0    11602 2024-03-04 12:54:10.867735 price2bq_zfullio-1.2.1/src/price2bq_zfullio/main.py
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 price2bq_zfullio-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-04 12:54:10.867735 price2bq_zfullio-1.3.0/LICENSE
+-rw-r--r--   0        0        0      160 2024-03-04 12:54:10.867735 price2bq_zfullio-1.3.0/README.md
+-rw-r--r--   0        0        0     1327 2024-05-31 00:31:46.752113 price2bq_zfullio-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-03-04 12:54:10.867735 price2bq_zfullio-1.3.0/src/price2bq_zfullio/__init__.py
+-rw-r--r--   0        0        0    11711 2024-05-31 00:25:36.058326 price2bq_zfullio-1.3.0/src/price2bq_zfullio/main.py
+-rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 price2bq_zfullio-1.3.0/PKG-INFO
```

### Comparing `price2bq_zfullio-1.2.1/LICENSE` & `price2bq_zfullio-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `price2bq_zfullio-1.2.1/pyproject.toml` & `price2bq_zfullio-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "price2bq-zfullio"
-version = "1.2.1"
+version = "1.3.0"
 description = "Экспорт файлов c площадок 'Яндекс Недвижимость', 'Авито' 'Циан' в BigQuery"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 pandas = "^2"
```

### Comparing `price2bq_zfullio-1.2.1/src/price2bq_zfullio/main.py` & `price2bq_zfullio-1.3.0/src/price2bq_zfullio/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,19 @@
               SchemaField("date_upload", "DATETIME")]
     bq = Client(bq_path_token, bq_project_id)
     bq.upload_table(df, bq_table, schema)
     return start_date, finish_date
 
 
 def prepare_novostroy_m(path_file: str) -> pd.DataFrame:
-    df = pd.read_excel(path_file, sheet_name="Make-Connect.ru")
+    df = pd.DataFrame
+    if path_file.endswith(".xls"):
+        df = pd.read_excel(path_file, sheet_name="Make-Connect.ru")
+    else:
+        df = pd.read_excel(path_file)
     df = df.rename(columns={"Дата": "date",
                             "Время": "time",
                             "Название РК": "campaign",
                             "Телефон абонента": "incoming_number",
                             "Длительность звонка": "call_duration",
                             "Спор": "dispute",
                             "Итоговый статус": "status",
```

### Comparing `price2bq_zfullio-1.2.1/PKG-INFO` & `price2bq_zfullio-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: price2bq-zfullio
-Version: 1.2.1
+Version: 1.3.0
 Summary: Экспорт файлов c площадок 'Яндекс Недвижимость', 'Авито' 'Циан' в BigQuery
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

