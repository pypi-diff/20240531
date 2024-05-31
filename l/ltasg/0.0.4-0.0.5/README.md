# Comparing `tmp/ltasg-0.0.4.tar.gz` & `tmp/ltasg-0.0.5.tar.gz`

## Comparing `ltasg-0.0.4.tar` & `ltasg-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ltasg-0.0.4/main.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.4/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/__init__.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/api.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/constants.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/traffic.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/helpers/helpers.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/__init__.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/bus.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/taxi.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/train.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.4/src/ltasg/transport/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.4/test/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.4/test/test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.4/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.4/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ltasg-0.0.5/main.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/__init__.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/api.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/constants.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/traffic.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/helpers/helpers.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/transport/__init__.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/transport/bus.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/transport/taxi.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/transport/train.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.5/src/ltasg/transport/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.5/test/test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.5/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.5/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.5/PKG-INFO
```

### Comparing `ltasg-0.0.4/src/ltasg/api.py` & `ltasg-0.0.5/src/ltasg/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,19 @@
         async with ClientSession() as session:
             while True:
                 try:
                     url_with_skip = url + f"{"" if query_params else "?"}$skip={skip_count}"
                     async with session.get(url_with_skip, headers=self.HEADERS) as response:
                         if response.ok:
                             curr_data = await response.json()
+                            if "Services" in curr_data or isinstance(curr_data['value'], dict):
+                                return curr_data
+                            if len(curr_data['value']) < 500:
+                                data.append(curr_data)
+                                break
                             if len(curr_data['value']) == 0:
                                 break
                             data.append(curr_data)
                             skip_count += 500
                         else:
                             raise Exception("Error calling api for {} with status code: {}".format(
                                 service_endpoint, response.status)) from None
```

### Comparing `ltasg-0.0.4/src/ltasg/constants.py` & `ltasg-0.0.5/src/ltasg/constants.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.4/src/ltasg/transport/bus.py` & `ltasg-0.0.5/src/ltasg/transport/bus.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.4/src/ltasg/transport/taxi.py` & `ltasg-0.0.5/src/ltasg/transport/taxi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..transport.transport import Transport
 from ..constants import TransportType
-
+from ..helpers.helpers import transform_data
 
 class Taxi(Transport):
     def __init__(self, base_url, api_key) -> None:
         super().__init__(base_url=base_url,api_key= api_key)
         self.taxi_services = self.transport_services[TransportType.TAXI]
 
     async def availability(self):
         data = await self.lta_api.fetch(self.taxi_services["AVAILABILITY"])
-        return data['value']
+        return transform_data(data)
     
     async def stands(self):
         data = await self.lta_api.fetch(self.taxi_services["STANDS"])
-        return data['value']
+        return transform_data(data)
```

### Comparing `ltasg-0.0.4/src/ltasg/transport/train.py` & `ltasg-0.0.5/src/ltasg/transport/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ..transport.transport import Transport
 from ..constants import TransportType
-from typing import Literal
 
 class Train(Transport):
     def __init__(self, base_url, api_key) -> None:
         super().__init__(base_url=base_url,api_key= api_key)
         self.train_services = self.transport_services[TransportType.TRAIN]
 
     async def service_alerts(self):
```

### Comparing `ltasg-0.0.4/test/test.py` & `ltasg-0.0.5/test/test.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.4/.gitignore` & `ltasg-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.4/LICENSE` & `ltasg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.4/pyproject.toml` & `ltasg-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ltasg"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Aw Sheng Xiang", email="awshengxiang@hotmail.com" },
 ]
 description = "A LTA Datamall API Wrapper Library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ltasg-0.0.4/PKG-INFO` & `ltasg-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ltasg
-Version: 0.0.4
+Version: 0.0.5
 Summary: A LTA Datamall API Wrapper Library for Python
 Project-URL: Homepage, https://github.com/ashe/ltasg
 Project-URL: Issues, https://github.com/ashe/ltasg/issues
 Author-email: Aw Sheng Xiang <awshengxiang@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

