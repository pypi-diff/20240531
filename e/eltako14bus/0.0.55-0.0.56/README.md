# Comparing `tmp/eltako14bus-0.0.55.tar.gz` & `tmp/eltako14bus-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.55.tar", last modified: Wed May 29 20:35:39 2024, max compression
+gzip compressed data, was "eltako14bus-0.0.56.tar", last modified: Fri May 31 09:40:51 2024, max compression
```

## Comparing `eltako14bus-0.0.55.tar` & `eltako14bus-0.0.56.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/eltako14bus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-29 20:35:39.000000 eltako14bus-0.0.55/eltako14bus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-29 20:35:39.000000 eltako14bus-0.0.55/eltako14bus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:35:39.000000 eltako14bus-0.0.55/eltako14bus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 20:35:39.000000 eltako14bus-0.0.55/eltako14bus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 20:35:39.000000 eltako14bus-0.0.55/eltako14bus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/eltakobus/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    46007 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/eep.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/eltakobus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:35:39.124260 eltako14bus-0.0.55/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 20:35:26.000000 eltako14bus-0.0.55/tests/generic_eep_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/eltako14bus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-31 09:40:51.000000 eltako14bus-0.0.56/eltako14bus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 09:40:51.000000 eltako14bus-0.0.56/eltako14bus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:40:51.000000 eltako14bus-0.0.56/eltako14bus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 09:40:51.000000 eltako14bus-0.0.56/eltako14bus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 09:40:51.000000 eltako14bus-0.0.56/eltako14bus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/eltakobus/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46930 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/eep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/eltakobus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:40:51.380032 eltako14bus-0.0.56/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-31 09:40:43.000000 eltako14bus-0.0.56/tests/generic_eep_test.py
```

### Comparing `eltako14bus-0.0.55/LICENSE` & `eltako14bus-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/PKG-INFO` & `eltako14bus-0.0.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.55
+Version: 0.0.56
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.55/README.md` & `eltako14bus-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.56/eltako14bus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.55
+Version: 0.0.56
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.55/eltakobus/bus.py` & `eltako14bus-0.0.56/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/coap.py` & `eltako14bus-0.0.56/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/device.py` & `eltako14bus-0.0.56/eltakobus/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,32 +275,46 @@
             key = int(mem_line[4])
             func = int(mem_line[5])
             ch = int(mem_line[6])
 
             address_off_set = 0
 
             if int.from_bytes(s_adr, "big") > 0:
-                while ch > 0:
-                    if ch & 0x1 == 1:
-                        dev_adr:int = self.address + address_off_set
-
-                        result.append(
-                            SensorInfo(
-                                dev_type = self.__class__.__name__,
-                                sensor_id = s_adr,
-                                dev_adr = dev_adr.to_bytes(4, byteorder = 'big'),
-                                key = key,
-                                dev_id = int(self.address),
-                                key_func = func,
-                                channel = address_off_set+1,
-                                in_func_group=in_func_group,
-                                memory_line=i
-                                ))
-                    ch = ch >> 1
-                    address_off_set += 1
+                if ch == 0:
+                    result.append(
+                        SensorInfo(
+                            dev_type = self.__class__.__name__,
+                            sensor_id = s_adr,
+                            dev_adr = self.address.to_bytes(4, byteorder = 'big'),
+                            key = key,
+                            dev_id = int(self.address),
+                            key_func = func,
+                            channel = ch,
+                            in_func_group=in_func_group,
+                            memory_line=i
+                            ))
+                else:
+                    while ch > 0:
+                        if ch & 0x1 == 1:
+                            dev_adr:int = self.address + address_off_set
+
+                            result.append(
+                                SensorInfo(
+                                    dev_type = self.__class__.__name__,
+                                    sensor_id = s_adr,
+                                    dev_adr = dev_adr.to_bytes(4, byteorder = 'big'),
+                                    key = key,
+                                    dev_id = int(self.address),
+                                    key_func = func,
+                                    channel = address_off_set+1,
+                                    in_func_group=in_func_group,
+                                    memory_line=i
+                                    ))
+                        ch = ch >> 1
+                        address_off_set += 1
 
         return result
     
     async def get_all_sensors(self) -> list[SensorInfo]:
         return []
         # return await self.get_registered_sensors(self.sensor_address_range)
 
@@ -982,14 +996,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class FTD14(BusObject):
     size=1
     discovery_names = [ bytes((0x04, 0xa0)) ]
+    sensor_address_range = range(8, 127)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     async def get_base_id(self) -> str:
         """Gets base id from memory."""
         mem_line = await self.read_mem_line(1)
@@ -1001,15 +1016,18 @@
         return mem_line[0:4]
 
     async def get_base_id_in_int(self) -> int:
         """Gets base id from memory."""
         mem_line = await self.read_mem_line(1)
         return int.from_bytes(mem_line[0:4], "big") 
     
-
+    async def get_all_sensors(self) -> list[SensorInfo]:
+        result = []
+        result.extend( await self.get_registered_sensors(self.sensor_address_range, 1) )
+        return result
 
 
 
 known_objects = [FAM14, FUD14, FUD14_800W, FSB14, FSR14_1x, FSR14_2x, FSR14_4x, F4SR14_LED, F3Z14D, FMZ14, FWG14MS, FSU14, FMSR14, FWZ14_65A, FSG14_1_10V, FGW14_USB, FDG14, FHK14, F4HK14, FAE14SSR, FTD14]
 # sorted so the first match of (discovery name is a prefix, size matches) can be used
 sorted_known_objects = sorted(known_objects, key=lambda o: len(o.discovery_names[0]) + 0.5 * (o.size is not None), reverse=True)
```

### Comparing `eltako14bus-0.0.55/eltakobus/eep.py` & `eltako14bus-0.0.56/eltakobus/eep.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/error.py` & `eltako14bus-0.0.56/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/locking.py` & `eltako14bus-0.0.56/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/message.py` & `eltako14bus-0.0.56/eltakobus/message.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/serial.py` & `eltako14bus-0.0.56/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/eltakobus/util.py` & `eltako14bus-0.0.56/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.55/setup.py` & `eltako14bus-0.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.55",
+    version="0.0.56",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

### Comparing `eltako14bus-0.0.55/tests/generic_eep_test.py` & `eltako14bus-0.0.56/tests/generic_eep_test.py`

 * *Files identical despite different names*

