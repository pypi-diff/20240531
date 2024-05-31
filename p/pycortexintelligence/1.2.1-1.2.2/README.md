# Comparing `tmp/pycortexintelligence-1.2.1-py3-none-any.whl.zip` & `tmp/pycortexintelligence-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15732 bytes, number of entries: 14
+Zip file size: 15982 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jul-08 22:55 pycortexintelligence/__init__.py
--rw-rw-r--  2.0 unx    16421 b- defN 24-Jan-02 20:44 pycortexintelligence/functions.py
+-rw-rw-r--  2.0 unx    17584 b- defN 24-May-31 20:23 pycortexintelligence/functions.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jul-08 22:55 pycortexintelligence/core/__init__.py
 -rw-rw-r--  2.0 unx      487 b- defN 22-Jul-08 22:55 pycortexintelligence/core/config.py
 -rw-rw-r--  2.0 unx     2211 b- defN 23-May-22 18:36 pycortexintelligence/core/funcs_env.py
 -rw-rw-r--  2.0 unx     1818 b- defN 23-May-22 18:36 pycortexintelligence/core/funcs_mail.py
 -rw-rw-r--  2.0 unx     7189 b- defN 23-May-22 18:36 pycortexintelligence/core/funcs_startproject.py
 -rw-rw-r--  2.0 unx      884 b- defN 23-Aug-24 14:28 pycortexintelligence/core/messages.py
--rwxrwxr-x  2.0 unx     1461 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.data/scripts/cortex.py
--rw-rw-r--  2.0 unx     1073 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5194 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1304 b- defN 24-Jan-04 13:17 pycortexintelligence-1.2.1.dist-info/RECORD
-14 files, 38155 bytes uncompressed, 13504 bytes compressed:  64.6%
+-rwxrwxr-x  2.0 unx     1461 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.data/scripts/cortex.py
+-rw-rw-r--  2.0 unx     1073 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5194 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1304 b- defN 24-May-31 20:24 pycortexintelligence-1.2.2.dist-info/RECORD
+14 files, 39318 bytes uncompressed, 13754 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: pycortexintelligence/core/funcs_startproject.py
 Comment: 
 
 Filename: pycortexintelligence/core/messages.py
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.data/scripts/cortex.py
+Filename: pycortexintelligence-1.2.2.data/scripts/cortex.py
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.dist-info/LICENSE
+Filename: pycortexintelligence-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.dist-info/METADATA
+Filename: pycortexintelligence-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.dist-info/WHEEL
+Filename: pycortexintelligence-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.dist-info/top_level.txt
+Filename: pycortexintelligence-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pycortexintelligence-1.2.1.dist-info/RECORD
+Filename: pycortexintelligence-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycortexintelligence/functions.py

```diff
@@ -295,15 +295,15 @@
         username: str,
         password: str,
         file_object: BytesIO or str,
         cube_id: Optional[str] = None,
         cube_name: Optional[str] = None,
         filters: Optional[List] = None,
         columns: Union[List, str] = "*",
-        **kwargs
+        **kwargs,
     ) -> Any:
         if not isinstance(file_object, BytesIO):
             file_object = open(file_object, "wb")  # type: ignore
 
         if cube_id and cube_name:
             raise ValueError(DOWNLOAD_ERROR_JUST_ID_OR_NAME)
 
@@ -383,29 +383,54 @@
         password: str,
         filters: Optional[List] = None,
     ):
         auth_header = cls.platform_auth(platform_url, username, password, return_user_id=True)
         payload = {"cube": f'{{"id": "{cube_id}"}}', "filters": list()}
 
         if filters is None:
-            payload["filters"] = [{"name": "# Records", "type": "SIMPLE", "value": 1}]
+            payload["filters"] = json.dumps([{"name": "# Records", "type": "SIMPLE", "value": 1}])
 
         if filters is not None:
             payload["filters"] = cls.make_filter(filters)
 
         delete_url = f"https://{platform_url}/service/integration-cube-service.delete"
 
         response = requests.get(delete_url, params=payload, headers=auth_header)
-
         if response.status_code == HTTPStatus.OK:
             return response.status_code
 
         if response.status_code != HTTPStatus.OK:
             raise ValueError(f"O status code recebido, foi: {response.status_code}\n {response.content}")
 
+    @classmethod
+    def cube_creation(
+        cls, platform_url: str, username: str, password: str, table_name: str, dimensions: list, **kwargs
+    ):
+        auth_header = cls.platform_auth(platform_url, username, password, return_user_id=True)
+        url = f"https://{platform_url}/controller/cube/create?"
+        data = {
+            "name": table_name,
+            "creditControlEnabled": kwargs.get("credit_control_enabled", False),
+            "pendingPublish": kwargs.get("pending_publish", False),
+            "dimensions": dimensions,
+            "permissions": [{"editor": True, "groupId": auth_header["x-authorization-user-id"]}],
+        }
+        if kwargs.get("cloud_storage_path", False):
+            data["cloud_storage_path"] = kwargs["cloud_storage_path"]
+
+        params = {"async": kwargs.get("async", "true")}
+
+        resp = requests.post(url, headers=auth_header, json=data, params=params)
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(
+                "Não foi possível criar o cubo.\n" f"O status retornado foi: {resp.status_code}\n" f"{resp.text}"
+            )
+
+        return resp.json()
+
     @staticmethod
     def _make_download_url(platform_url: str):
         return f"https://{platform_url}/service/integration-cube-service.download?"
 
 
 def download_from_cortex(**kwargs) -> Any:
     import warnings
```

## Comparing `pycortexintelligence-1.2.1.data/scripts/cortex.py` & `pycortexintelligence-1.2.2.data/scripts/cortex.py`

 * *Files identical despite different names*

## Comparing `pycortexintelligence-1.2.1.dist-info/LICENSE` & `pycortexintelligence-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycortexintelligence-1.2.1.dist-info/METADATA` & `pycortexintelligence-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycortexintelligence
-Version: 1.2.1
+Version: 1.2.2
 Summary: Cortex Intelligence Platform Python SDK
 Home-page: https://github.com/cortex-intelligence/pycortexintelligence
 Author: Enderson Menezes
 Author-email: data.integrations@cortex-intelligence.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pycortexintelligence-1.2.1.dist-info/RECORD` & `pycortexintelligence-1.2.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pycortexintelligence/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pycortexintelligence/functions.py,sha256=GzCqoA0C1ptwVt38B0AphKdj5XFesTSu23xV8ul1QAo,16421
+pycortexintelligence/functions.py,sha256=qdw_kktwPCzQQLPdx246SoAvIgqExp50f2N_zkmgLbs,17584
 pycortexintelligence/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pycortexintelligence/core/config.py,sha256=CAKTpp_r7dP5cIHzltZmqQZzwzqo9U__xzHjdHtdAXs,487
 pycortexintelligence/core/funcs_env.py,sha256=I5r3kiYC9wwVWiz25NTqf2rJsqeB0_ROc__7gzm8iZ0,2211
 pycortexintelligence/core/funcs_mail.py,sha256=FFz_uxNe-etPXPB2QhmH8s18i6z3i2CXyPc-b40q2u4,1818
 pycortexintelligence/core/funcs_startproject.py,sha256=wU_RUQj8rp-2fwKcdttuFqD95-kWWErOa8GYJf9fGyo,7189
 pycortexintelligence/core/messages.py,sha256=v05j48pcjtSSdXUttSzJ3X4y-ZfASnanGtuJSqgeHoY,884
-pycortexintelligence-1.2.1.data/scripts/cortex.py,sha256=4JnCrwLKqLTdoqBiPJHRyQtq6V3iRO9M1UeCWQKqi7k,1461
-pycortexintelligence-1.2.1.dist-info/LICENSE,sha256=2bFR2oxY5CiDtRqM6078TnDiRti_ZBECF7zvqZWcRWM,1073
-pycortexintelligence-1.2.1.dist-info/METADATA,sha256=SXSgseRQh01TsZ1MAXSyHBVpWhY5axeKdAb4bFmqnyE,5194
-pycortexintelligence-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pycortexintelligence-1.2.1.dist-info/top_level.txt,sha256=7yAXb7mVR9f1GBrXUCSQ7rhgv71IVQrjI7X6dYrLCIM,21
-pycortexintelligence-1.2.1.dist-info/RECORD,,
+pycortexintelligence-1.2.2.data/scripts/cortex.py,sha256=4JnCrwLKqLTdoqBiPJHRyQtq6V3iRO9M1UeCWQKqi7k,1461
+pycortexintelligence-1.2.2.dist-info/LICENSE,sha256=2bFR2oxY5CiDtRqM6078TnDiRti_ZBECF7zvqZWcRWM,1073
+pycortexintelligence-1.2.2.dist-info/METADATA,sha256=a72k6M46n3VGeOoWfPtXQgKCVgUn2Ccf-_ghSzXz2gc,5194
+pycortexintelligence-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pycortexintelligence-1.2.2.dist-info/top_level.txt,sha256=7yAXb7mVR9f1GBrXUCSQ7rhgv71IVQrjI7X6dYrLCIM,21
+pycortexintelligence-1.2.2.dist-info/RECORD,,
```

