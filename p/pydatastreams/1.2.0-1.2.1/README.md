# Comparing `tmp/pydatastreams-1.2.0.tar.gz` & `tmp/pydatastreams-1.2.1.tar.gz`

## Comparing `pydatastreams-1.2.0.tar` & `pydatastreams-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/__about__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/__init__.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/base.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/deserializing.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/serializing.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/twoway.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/__about__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/__init__.py
+-rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/base.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/deserializing.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/serializing.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/twoway.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/PKG-INFO
```

### Comparing `pydatastreams-1.2.0/datastream/base.py` & `pydatastreams-1.2.1/datastream/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,30 @@
 
     Args:
         backing_stream (typing.IO[bytes]): The backing stream object.
         byteorder (int): The byte order of the stream.
     """
 
     def __init__(self, backing_stream: typing.IO[bytes], byteorder: int):
+        if backing_stream is None:
+            return
+        
         if not isinstance(backing_stream, io.BytesIO):
             raise ValueError("backing_stream must be a BytesIO object")
 
         self._backing_stream = backing_stream
         self._byteorder = _byteorder_map[byteorder]
 
     @property
-    def byteorder(self) -> str:
+    def byteorder(self) -> ByteOrder:
         """
         Returns the byte order of the datastream.
 
         Returns:
-            str: The byte order of the datastream.
+            ByteOrder: The byte order of the datastream.
         """
         return ByteOrder(_byteorder_map.index(self._byteorder))
 
     @byteorder.setter
     def byteorder(self, value: int):
         """
         Sets the byte order for the datastream.
@@ -67,14 +70,17 @@
 
         Args:
             size (int): The maximum number of bytes to read.
 
         Returns:
             bytes: The bytes read from the backing stream.
         """
+        if self._backing_stream is None:
+            raise ValueError("backing_stream has not been set.")
+
         return self._backing_stream.read(size)
 
     def size(self) -> int:
         """
         Returns the size of the backing stream.
 
         Returns:
@@ -120,14 +126,17 @@
     def write(self, data: bytes):
         """
         Writes the given data to the backing stream.
 
         Args:
             data (bytes): The data to be written.
         """
+        if self._backing_stream is None:
+            raise ValueError("backing_stream has not been set.")
+
         self._backing_stream.write(data)
 
     def clone(self) -> typing.Self:
         """
         Creates a clone of the current object.
 
         Returns:
@@ -244,14 +253,16 @@
             if chunk == data:
                 index = self.tell() - len(data)
                 self.seek(pos)
 
                 return index
 
             remaining -= len(data)
+        
+        return -1
 
     def clear(self):
         """
         Clears the backing stream by truncating it to 0 bytes and resetting the stream
         position to the beginning.
         """
         self._backing_stream.truncate(0)
```

### Comparing `pydatastreams-1.2.0/datastream/deserializing.py` & `pydatastreams-1.2.1/datastream/deserializing.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,35 @@
 from datastream.base import BaseStream, ByteOrder
 
 
 class DeserializingStream(BaseStream):
     def __init__(
         self, buffer: bytes | typing.IO[bytes], byteorder: int = ByteOrder.NATIVE_ENDIAN
     ):
+        if buffer is None:
+            super().__init__(buffer, byteorder)
+            
+            return
+        
         if not isinstance(buffer, io.BytesIO):
             if isinstance(buffer, io.IOBase):
                 buffer = io.BytesIO(buffer.getvalue()) # type: ignore
             else:
                 buffer = io.BytesIO(buffer) # type: ignore
 
         super().__init__(buffer, byteorder)
+    
+    def set(self, buffer: bytes | typing.IO[bytes]):
+        if not isinstance(buffer, io.BytesIO):
+            if isinstance(buffer, io.IOBase):
+                self._backing_stream = io.BytesIO(buffer.getvalue()) # type: ignore
+            else:
+                self._backing_stream = io.BytesIO(buffer) # type: ignore
+        else:
+            self._backing_stream = buffer
 
     def read_format(self, fmt: str) -> typing.Any:
         return struct.unpack(self._byteorder + fmt, self.read(struct.calcsize(fmt)))[0]
 
     def read_int64(self) -> int:
         return self.read_format("q")
```

### Comparing `pydatastreams-1.2.0/datastream/serializing.py` & `pydatastreams-1.2.1/datastream/serializing.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.0/datastream/twoway.py` & `pydatastreams-1.2.1/datastream/twoway.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     ):
         if buffer is None:
             buffer = io.BytesIO()
         elif isinstance(buffer, bytes):
             buffer = io.BytesIO(buffer)
 
         self.dstream = DeserializingStream(buffer, byteorder)
-        self.sstream = SerializingStream(buffer, byteorder)
+        self.sstream = SerializingStream(buffer, byteorder) # type: ignore
 
-        super().__init__(buffer, byteorder)
+        super().__init__(buffer, byteorder) # type: ignore
 
     def read_format(self, fmt: str) -> typing.Any:
         return self.dstream.read_format(fmt)
 
     def read_int64(self) -> int:
         return self.read_format("q")
```

### Comparing `pydatastreams-1.2.0/.gitignore` & `pydatastreams-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.0/LICENSE.txt` & `pydatastreams-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.0/README.md` & `pydatastreams-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 To install the library, use the following:
 ```console
 python -m pip install --user -U pydatastreams
 ```
 
 To import the library, use the following:
 ```python
-from datastream import SerializingStream, DeserializingStream, ByteOrder
+from datastream import SerializingStream, DeserializingStream, TwoWayStream, ByteOrder
 ```
 
 Retrieving serialized data from a SerializingStream:
 ```python
 stream = SerializingStream()
 stream.write_int32(42)
 
@@ -54,14 +54,15 @@
 | | | [`write_uleb128_safe(value: int, max_bytes: int = 16)`](datastream/serializing.py#L78) | [`read_uleb128_safe(max_bytes: int = 16) -> int`](datastream/deserializing.py#L68) |
 | `sleb128` | Variable sized signed 128-bit number | [`write_sleb128(value: int)`](datastream/serializing.py#L99) | [`read_sleb128() -> int`](datastream/deserializing.py#L95) |
 | | | [`write_sleb128_safe(value: int, max_bytes: int = 16)`](datastream/serializing.py#L110) | [`read_sleb128_safe(max_bytes: int = 16) -> int`](datastream/deserializing.py#L107) |
 
 Finally, the stream classes also provide the following utility functions:
 | Function | Description |
 | --- | --- |
+| [`set(buffer:  bytes \| typing.IO[bytes])`](datastream/deserializing.py#L25) | Sets the backing stream to the given buffer. DeserializingStream only. |
 | [`read(size: int) -> bytes`](datastream/base.py#L64) | Reads up to `size` bytes from the backing stream. |
 | [`write(data: bytes)`](datastream/base.py#L120) | Writes the given data to the backing stream. |
 | [`size() -> int`](datastream/base.py#L76) | Returns the size of the backing stream. |
 | [`seek(offset: int, whence: int = io.SEEK_SET)`](datastream/base.py#L94) | Change the stream position to the given offset. |
 | [`tell() -> int`](datastream/base.py#L105) | Returns the current position of the stream. |
 | [`close()`](datastream/base.py#L114) | Closes the backing stream. |
 | [`remaining() -> int`](datastream/base.py#L85) | Returns the number of bytes remaining in the backing stream. |
```

### Comparing `pydatastreams-1.2.0/pyproject.toml` & `pydatastreams-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.0/PKG-INFO` & `pydatastreams-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydatastreams
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple and easy to use library for reading and writing data streams.
 Project-URL: Homepage, https://github.com/yntha/datastream
 Project-URL: Repository, https://github.com/yntha/datastream.git
 Project-URL: Issues, https://github.com/yntha/datastream/issues
 Author-email: yntha <bguznvjk@gmail.com>
 License-File: LICENSE.txt
 Keywords: binary,data,file,io,stream
@@ -31,15 +31,15 @@
 To install the library, use the following:
 ```console
 python -m pip install --user -U pydatastreams
 ```
 
 To import the library, use the following:
 ```python
-from datastream import SerializingStream, DeserializingStream, ByteOrder
+from datastream import SerializingStream, DeserializingStream, TwoWayStream, ByteOrder
 ```
 
 Retrieving serialized data from a SerializingStream:
 ```python
 stream = SerializingStream()
 stream.write_int32(42)
 
@@ -73,14 +73,15 @@
 | | | [`write_uleb128_safe(value: int, max_bytes: int = 16)`](datastream/serializing.py#L78) | [`read_uleb128_safe(max_bytes: int = 16) -> int`](datastream/deserializing.py#L68) |
 | `sleb128` | Variable sized signed 128-bit number | [`write_sleb128(value: int)`](datastream/serializing.py#L99) | [`read_sleb128() -> int`](datastream/deserializing.py#L95) |
 | | | [`write_sleb128_safe(value: int, max_bytes: int = 16)`](datastream/serializing.py#L110) | [`read_sleb128_safe(max_bytes: int = 16) -> int`](datastream/deserializing.py#L107) |
 
 Finally, the stream classes also provide the following utility functions:
 | Function | Description |
 | --- | --- |
+| [`set(buffer:  bytes \| typing.IO[bytes])`](datastream/deserializing.py#L25) | Sets the backing stream to the given buffer. DeserializingStream only. |
 | [`read(size: int) -> bytes`](datastream/base.py#L64) | Reads up to `size` bytes from the backing stream. |
 | [`write(data: bytes)`](datastream/base.py#L120) | Writes the given data to the backing stream. |
 | [`size() -> int`](datastream/base.py#L76) | Returns the size of the backing stream. |
 | [`seek(offset: int, whence: int = io.SEEK_SET)`](datastream/base.py#L94) | Change the stream position to the given offset. |
 | [`tell() -> int`](datastream/base.py#L105) | Returns the current position of the stream. |
 | [`close()`](datastream/base.py#L114) | Closes the backing stream. |
 | [`remaining() -> int`](datastream/base.py#L85) | Returns the number of bytes remaining in the backing stream. |
```

