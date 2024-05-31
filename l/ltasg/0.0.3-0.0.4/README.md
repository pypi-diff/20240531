# Comparing `tmp/ltasg-0.0.3.tar.gz` & `tmp/ltasg-0.0.4.tar.gz`

## Comparing `ltasg-0.0.3.tar` & `ltasg-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.3/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/__init__.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/api.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/constants.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/traffic.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/transport/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/transport/bus.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/transport/taxi.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/transport/train.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.3/src/ltasg/transport/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.3/test/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.3/test/test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.3/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.3/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ltasg-0.0.4/main.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/__init__.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/api.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/constants.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/traffic.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/helpers/helpers.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/__init__.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/bus.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/taxi.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/train.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.4/test/test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.4/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.4/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.4/PKG-INFO
```

### Comparing `ltasg-0.0.3/src/ltasg/api.py` & `ltasg-0.0.4/src/ltasg/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from aiohttp import ClientSession, ClientConnectionError
-import traceback
+
+
 class LTADataMall:
     def __init__(self, base_url, api_key) -> None:
         self.BASE_URL = base_url
         self.API_KEY = api_key
         self.HEADERS = {
             "Accept": "application/json",
             "AccountKey": self.API_KEY
         }
 
-    async def fetch(self, service_endpoint: str, query_params: dict=None, data:dict=None):
+    async def fetch(self, service_endpoint: str, query_params: dict = None, data: dict = None):
         url = f"{self.BASE_URL}{service_endpoint}"
+        skip_count = 0
+        data = []
         if query_params:
             url += "?"
             for param, value in query_params.items():
-                url += f"{param}={value}"
-                if param != list(query_params.keys())[-1]:
-                    url += "&"
+                url += f"{param}={value}&"
+                # if param != list(query_params.keys())[-1]:
+                #     url += "&"
         async with ClientSession() as session:
-            try:
-                async with session.get(url, headers=self.HEADERS) as response:
-                    if response.status == 200:
-                        return await response.json()
-                    else:
-                        raise Exception("Error calling api for {} with status code: {}".format(
-                            service_endpoint, response.status)) from None
-            except ClientConnectionError as e:
-                raise e
+            while True:
+                try:
+                    url_with_skip = url + f"{"" if query_params else "?"}$skip={skip_count}"
+                    async with session.get(url_with_skip, headers=self.HEADERS) as response:
+                        if response.ok:
+                            curr_data = await response.json()
+                            if len(curr_data['value']) == 0:
+                                break
+                            data.append(curr_data)
+                            skip_count += 500
+                        else:
+                            raise Exception("Error calling api for {} with status code: {}".format(
+                                service_endpoint, response.status)) from None
+                except ClientConnectionError as e:
+                    raise e
+            return data
+
```

### Comparing `ltasg-0.0.3/src/ltasg/constants.py` & `ltasg-0.0.4/src/ltasg/constants.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/src/ltasg/transport/bus.py` & `ltasg-0.0.4/src/ltasg/transport/bus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from ..transport.transport import Transport
 from ..constants import TransportType
+from ..helpers.helpers import transform_data
+
 
 class Bus(Transport):
     def __init__(self, base_url, api_key) -> None:
         super().__init__(base_url=base_url,api_key= api_key)
         self.bus_services = self.transport_services[TransportType.BUS]
-
+    
     async def arrival(self, bus_stop_code: int, bus_no: int):
         data = await self.lta_api.fetch(self.bus_services['ARRIVAL'], query_params={
             "BusStopCode": bus_stop_code,
             "ServiceNo": bus_no
         })
         return data["Services"]
     
     async def services(self):
         data = await self.lta_api.fetch(self.bus_services['SERVICES'])
-        return data["value"]
+        return transform_data(data)
     async def stop_services(self, bus_stop_code):
         data = await self.lta_api.fetch(self.bus_services['ARRIVAL'], query_params={
             "BusStopCode": bus_stop_code
         })
         services = [ service["ServiceNo"] for service in data["Services"]]
         return services
     async def routes(self):
         data = await self.lta_api.fetch(self.bus_services['ROUTES'])
-        return data["value"]
+        return transform_data(data)
 
     async def stops(self):
         data = await self.lta_api.fetch(self.bus_services['STOPS'])
-        return data["value"]
-
-    
-# BusArrivalv2?BusStopCode=71111&ServiceNo=137
+        return transform_data(data)
```

### Comparing `ltasg-0.0.3/src/ltasg/transport/taxi.py` & `ltasg-0.0.4/src/ltasg/transport/taxi.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/src/ltasg/transport/train.py` & `ltasg-0.0.4/src/ltasg/transport/train.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/test/test.py` & `ltasg-0.0.4/test/test.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/.gitignore` & `ltasg-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/LICENSE` & `ltasg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.3/pyproject.toml` & `ltasg-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ltasg"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Aw Sheng Xiang", email="awshengxiang@hotmail.com" },
 ]
 description = "A LTA Datamall API Wrapper Library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ltasg-0.0.3/PKG-INFO` & `ltasg-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ltasg
-Version: 0.0.3
+Version: 0.0.4
 Summary: A LTA Datamall API Wrapper Library for Python
 Project-URL: Homepage, https://github.com/ashe/ltasg
 Project-URL: Issues, https://github.com/ashe/ltasg/issues
 Author-email: Aw Sheng Xiang <awshengxiang@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

