# Comparing `tmp/labcomm-0.0.2.tar.gz` & `tmp/labcomm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcomm-0.0.2.tar", last modified: Fri Aug 11 15:20:17 2023, max compression
+gzip compressed data, was "labcomm-0.0.3.tar", last modified: Fri May 31 14:56:24 2024, max compression
```

## Comparing `labcomm-0.0.2.tar` & `labcomm-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-11 15:20:17.996555 labcomm-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-08-04 21:12:38.000000 labcomm-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      780 2023-08-11 15:20:17.995550 labcomm-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-08-07 10:35:33.000000 labcomm-0.0.2/README.md
--rw-rw-rw-   0        0        0      664 2023-08-11 15:19:53.000000 labcomm-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-11 15:20:17.997553 labcomm-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-11 15:20:17.949329 labcomm-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-08-08 16:07:00.000000 labcomm-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-11 15:20:17.993548 labcomm-0.0.2/src/labcomm.egg-info/
--rw-rw-rw-   0        0        0      780 2023-08-11 15:20:17.000000 labcomm-0.0.2/src/labcomm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-08-11 15:20:17.000000 labcomm-0.0.2/src/labcomm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-11 15:20:17.000000 labcomm-0.0.2/src/labcomm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-11 15:20:17.000000 labcomm-0.0.2/src/labcomm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8200 2023-08-01 15:49:30.000000 labcomm-0.0.2/src/labcomm.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:56:24.874250 labcomm-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-08-04 21:12:38.000000 labcomm-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      780 2024-05-31 14:56:24.870265 labcomm-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-07 10:35:33.000000 labcomm-0.0.3/README.md
+-rw-rw-rw-   0        0        0      664 2024-05-31 14:32:01.000000 labcomm-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:56:24.874250 labcomm-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 14:56:24.846003 labcomm-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-08-08 16:07:00.000000 labcomm-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:56:24.866278 labcomm-0.0.3/src/labcomm.egg-info/
+-rw-rw-rw-   0        0        0      780 2024-05-31 14:56:24.000000 labcomm-0.0.3/src/labcomm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-31 14:56:24.000000 labcomm-0.0.3/src/labcomm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:56:24.000000 labcomm-0.0.3/src/labcomm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-31 14:56:24.000000 labcomm-0.0.3/src/labcomm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8139 2024-05-22 20:42:56.000000 labcomm-0.0.3/src/labcomm.py
```

### Comparing `labcomm-0.0.2/LICENSE` & `labcomm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `labcomm-0.0.2/PKG-INFO` & `labcomm-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcomm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fast binary protocol for interacting with integrated circuit demonstration boards.
 Author-email: Steve Martin <Steve.Martin@analog.com>
 Project-URL: Homepage, https://github.com/Xenomorphxx121/labcomm
 Project-URL: Bug Tracker, https://github.com/Xenomorphxx121/labcomm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labcomm-0.0.2/pyproject.toml` & `labcomm-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labcomm"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Steve Martin", email="Steve.Martin@analog.com" },
 ]
 description = "A fast binary protocol for interacting with integrated circuit demonstration boards."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `labcomm-0.0.2/src/labcomm.egg-info/PKG-INFO` & `labcomm-0.0.3/src/labcomm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcomm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fast binary protocol for interacting with integrated circuit demonstration boards.
 Author-email: Steve Martin <Steve.Martin@analog.com>
 Project-URL: Homepage, https://github.com/Xenomorphxx121/labcomm
 Project-URL: Bug Tracker, https://github.com/Xenomorphxx121/labcomm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labcomm-0.0.2/src/labcomm.py` & `labcomm-0.0.3/src/labcomm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
     def __init__(self):
         '''
         LABCOMM PACKET FRAME DEFINITION:
         ┌──────────┬─────────┬────────────────┬────────────────┬──────────────┬─────────────┬──────────┐
         │ PREAMBLE │ VERSION │ DESTINATION ID │    SOURCE ID   │ PAYLOAD SIZE │   PAYLOAD   │ ENDAMBLE │
         └──────────┴─────────┴────────────────┴────────────────┴──────────────┴─────────────┴──────────┘
         │◄───10B──►│◄──1B───►│◄──────2B──────►│◄──────2B──────►│◄─────4B─────►│◄─SIZE(P/L)─►│◄───4B───►│
-
-        See the document: "Labcomm Manual.docx"'''
+        '''
         self.PREAMBLE           = "L@BC0MmADI"
         self.ENDAMBLE           = "TeoM"
         self.VERSION            = "1"
         self.ENDAMBLE_LEN       = len(self.ENDAMBLE)
         self.ENDPOINT_LEN       = 2
         self.PAYLOAD_SIZE_LEN   = 4
+        self.META_SIZE          = len(self.PREAMBLE) + len(self.VERSION) + 2*self.ENDPOINT_LEN + self.PAYLOAD_SIZE_LEN
                 
     def assemble(self, source, destination, payload):        
         return  bytes(self.PREAMBLE, "latin-1")                                             + \
                 bytes(self.VERSION, "latin-1")                                              + \
                 int.to_bytes(destination, length=self.ENDPOINT_LEN, byteorder="big")        + \
                 int.to_bytes(source, length=self.ENDPOINT_LEN, byteorder="big")             + \
                 int.to_bytes(len(payload), length=self.PAYLOAD_SIZE_LEN, byteorder="big")   + \
@@ -71,15 +71,15 @@
         if len(self.source_id_buffer) == self.ENDPOINT_LEN:
             self.state = "get_payload_size"
 
     def get_payload_size(self, byte):
         if len(self.payload_size_buffer) < self.PAYLOAD_SIZE_LEN:
             self.payload_size_buffer += byte
         if len(self.payload_size_buffer) == self.PAYLOAD_SIZE_LEN:
-            self.payload_size = self._compute_payload_size(self.payload_size_buffer[0:4])
+            self._compute_payload_size(self.payload_size_buffer[0:4])
             self.state = "get_payload"
 
     def get_payload(self, byte):
         if len(self.payload_buffer_as_list) < self.payload_size:
             self.payload_buffer_as_list.append(ord(byte))
             self.payload_buffer_as_string += byte
         if len(self.payload_buffer_as_list) == self.payload_size:
@@ -106,25 +106,23 @@
             self.get_payload(byte)
         elif self.state == "get_endamble":
             self.get_endamble(byte)
         self.detect_preamble(byte) # Asynchronous start of packet detection
         
     def _compute_payload_size(self, string):
         try:
-            payload_size = ord(string[0])*256**3 + ord(string[1])*256**2 + ord(string[2])*256 + ord(string[3])
+            self.payload_size = ord(string[0])*256**3 + ord(string[1])*256**2 + ord(string[2])*256 + ord(string[3])
         except:
             print(f'\n\nLabcomm debug breakpoint in _compute_payload_size()...\nPayload_size came back as "{string}".\n\n')
-            payload_size = 0
-        return payload_size
+            self.payload_size = 0
 
     def read_message(self):
-        meta_size = len(self.PREAMBLE) + len(self.VERSION) + 2*self.ENDPOINT_LEN + self.PAYLOAD_SIZE_LEN
-        meta_data = self.interface.read(meta_size)
-        payload_size = self._compute_payload_size(meta_data[meta_size-self.PAYLOAD_SIZE_LEN:meta_size])
-        payload = self.interface.read(size=payload_size)
+        meta_data = self.interface.read(self.META_SIZE)
+        self._compute_payload_size(meta_data[self.META_SIZE-self.PAYLOAD_SIZE_LEN:self.META_SIZE])
+        payload = self.interface.read(size=self.payload_size)
         endamble = self.interface.read(size=self.ENDAMBLE_LEN)
         if endamble != self.ENDAMBLE:
             self.interface.reset_input_buffer()
             print('\n\n*** Labcomm Packet Error *******    Malformed Packet Received. READ ABORTED!!!')
             # print(f'Possible Labcomm Version:           {ord(meta_data[len(self.PREAMBLE)])}')
             # print(f'Possible Labcomm Preamble:          {meta_data[0:len(self.PREAMBLE)]}')
             # print(f'Possible Labcomm Target address:    {ord(meta_data[10])*256 + ord(meta_data[11])}')
```

