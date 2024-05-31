# Comparing `tmp/data_serialize-0.2.2-py3-none-any.whl.zip` & `tmp/data_serialize-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,21 @@
-Zip file size: 12518 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      498 b- defN 23-Jul-31 05:09 data_serialize/__init__.py
--rw-rw-rw-  2.0 fat     1833 b- defN 22-Nov-07 07:50 data_serialize/demo.py
--rw-rw-rw-  2.0 fat     1067 b- defN 23-Jul-31 05:06 data_serialize/setup.py
--rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-31 04:45 data_serialize/pb/__init__.py
--rw-rw-rw-  2.0 fat     4003 b- defN 23-Jul-31 04:53 data_serialize/pb/example_pb2.py
--rw-rw-rw-  2.0 fat    14902 b- defN 22-Nov-07 01:57 data_serialize/pb/feature_pb2.py
--rw-rw-rw-  2.0 fat     9345 b- defN 22-Nov-07 06:14 data_serialize/pb/numpyobject_pb2.py
--rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-31 04:45 data_serialize/pb4/__init__.py
--rw-rw-rw-  2.0 fat     1836 b- defN 23-Jul-31 04:56 data_serialize/pb4/example_pb2.py
--rw-rw-rw-  2.0 fat     6063 b- defN 23-Jul-31 04:40 data_serialize/pb4/feature_pb2.py
--rw-rw-rw-  2.0 fat     3832 b- defN 23-Jul-31 04:40 data_serialize/pb4/numpyobject_pb2.py
--rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1282 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/RECORD
-15 files, 47173 bytes uncompressed, 10378 bytes compressed:  78.0%
+Zip file size: 16010 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat      642 b- defN 24-May-31 11:56 data_serialize/__init__.py
+-rw-rw-rw-  2.0 fat     1833 b- defN 22-Nov-07 10:41 data_serialize/demo.py
+-rw-rw-rw-  2.0 fat     1067 b- defN 24-May-31 11:52 data_serialize/setup.py
+-rw-rw-rw-  2.0 fat       77 b- defN 23-Sep-16 08:45 data_serialize/pb/__init__.py
+-rw-rw-rw-  2.0 fat     4003 b- defN 23-Sep-16 08:45 data_serialize/pb/example_pb2.py
+-rw-rw-rw-  2.0 fat    14902 b- defN 23-Sep-16 08:45 data_serialize/pb/feature_pb2.py
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Sep-16 08:45 data_serialize/pb/numpyobject_pb2.py
+-rw-rw-rw-  2.0 fat       77 b- defN 23-Sep-16 08:45 data_serialize/pb4/__init__.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 24-May-31 11:55 data_serialize/pb4/example_pb2.py
+-rw-rw-rw-  2.0 fat     6063 b- defN 23-Sep-16 08:45 data_serialize/pb4/feature_pb2.py
+-rw-rw-rw-  2.0 fat     3832 b- defN 23-Sep-16 08:45 data_serialize/pb4/numpyobject_pb2.py
+-rw-rw-rw-  2.0 fat       80 b- defN 24-May-31 10:39 data_serialize/pb5/__init__.py
+-rw-rw-rw-  2.0 fat     1649 b- defN 24-May-31 11:55 data_serialize/pb5/example_pb2.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 24-May-31 11:27 data_serialize/pb5/feature_pb2.py
+-rw-rw-rw-  2.0 fat     2935 b- defN 24-May-31 11:27 data_serialize/pb5/numpyobject_pb2.py
+-rw-rw-rw-  2.0 fat     2331 b- defN 24-May-31 11:56 data_serialize-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 11:56 data_serialize-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-31 11:56 data_serialize-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1641 b- defN 24-May-31 11:56 data_serialize-0.3.0.dist-info/RECORD
+19 files, 56198 bytes uncompressed, 13300 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -27,20 +27,32 @@
 
 Filename: data_serialize/pb4/feature_pb2.py
 Comment: 
 
 Filename: data_serialize/pb4/numpyobject_pb2.py
 Comment: 
 
-Filename: data_serialize-0.2.2.dist-info/METADATA
+Filename: data_serialize/pb5/__init__.py
 Comment: 
 
-Filename: data_serialize-0.2.2.dist-info/WHEEL
+Filename: data_serialize/pb5/example_pb2.py
 Comment: 
 
-Filename: data_serialize-0.2.2.dist-info/top_level.txt
+Filename: data_serialize/pb5/feature_pb2.py
 Comment: 
 
-Filename: data_serialize-0.2.2.dist-info/RECORD
+Filename: data_serialize/pb5/numpyobject_pb2.py
+Comment: 
+
+Filename: data_serialize-0.3.0.dist-info/METADATA
+Comment: 
+
+Filename: data_serialize-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: data_serialize-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: data_serialize-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_serialize/__init__.py

```diff
@@ -5,15 +5,20 @@
 
 try:
     from google.protobuf import __version__ as pb_ver
 
 except:
     pb_ver = '3'
 
-if pb_ver.startswith('4') or pb_ver.startswith('3.20') or pb_ver.startswith('3.21') :
+if pb_ver.startswith('5'):
+    from .pb5.feature_pb2 import *
+    from .pb5.example_pb2 import *
+    from .pb5.numpyobject_pb2 import *
+
+elif pb_ver.startswith('4') or pb_ver.startswith('3.20') or pb_ver.startswith('3.21') :
     from .pb4.feature_pb2 import *
     from .pb4.example_pb2 import *
     from .pb4.numpyobject_pb2 import *
 else:
     from .pb.feature_pb2 import *
     from .pb.example_pb2 import *
     from .pb.numpyobject_pb2 import *
```

## data_serialize/setup.py

```diff
@@ -17,15 +17,15 @@
 # read the contents of README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'),mode='r',encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='data_serialize',
-    version='0.2.2',
+    version='0.3.0',
     description='data serialize',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='ssbuild',
     author_email='9727464@qq.com',
     url='https://github.com/ssbuild/fastdatasets',
     packages=find_packages(),
```

## data_serialize/pb4/example_pb2.py

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
-
+from . import feature_pb2 as feature__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rexample.proto\x12\x0e\x64\x61ta_serialize\x1a\rfeature.proto\"5\n\x07\x45xample\x12*\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x18.data_serialize.Features\"q\n\x0fSequenceExample\x12)\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x18.data_serialize.Features\x12\x33\n\rfeature_lists\x18\x02 \x01(\x0b\x32\x1c.data_serialize.FeatureListsb\x06proto3')
 
 
 
 _EXAMPLE = DESCRIPTOR.message_types_by_name['Example']
 _SEQUENCEEXAMPLE = DESCRIPTOR.message_types_by_name['SequenceExample']
```

## Comparing `data_serialize-0.2.2.dist-info/METADATA` & `data_serialize-0.3.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,100 @@
-Metadata-Version: 2.1
-Name: data-serialize
-Version: 0.2.2
-Summary: data serialize
-Home-page: https://github.com/ssbuild/fastdatasets
-Author: ssbuild
-Author-email: 9727464@qq.com
-License: MIT
-Keywords: data_serialize,serialize,deserialize
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: protobuf
-
-# data_serialize
-
-This library allows reading and writing binary to string 
-
-## Installation
-
-```pip3 install data_serialize```
-
-
-## serialize and deserialize
-
-```python
-#
-import data_serialize
-import numpy as np
-
-
-def test_feature():
-    val1 = data_serialize.Int64List(value=[1, 2, 3] * 20)
-    val2 = data_serialize.FloatList(value=[1, 2, 3] * 20)
-    val3 = data_serialize.BytesList(value=[b'The china', b'boy'])
-
-    featrue = data_serialize.Features(feature=
-    {
-        "item_0": data_serialize.Feature(int64_list=val1),
-        "item_1": data_serialize.Feature(float_list=val2),
-        "item_2": data_serialize.Feature(bytes_list=val3)
-    }
-    )
-
-    example = data_serialize.Example(features=featrue)
-
-    # 序列化
-    serialize = example.SerializeToString()
-    print(serialize)
-
-    # 反序列化
-    example = data_serialize.Example()
-    example.ParseFromString(serialize)
-    print(example)
-
-
-def test_numpyobject():
-    a = np.random.randint(0, 21128, size=(10,), dtype=np.int64)
-    b = np.random.rand(3, 4)
-    c = np.asarray(b'The china')
-
-    val1 = data_serialize.NumpyObject(
-        header='',
-        dtype=str(a.dtype),
-        shape=list(a.shape),
-        int64=a.reshape((-1,)).tolist(),
-    )
-    val2 = data_serialize.NumpyObject(
-        header='',
-        dtype=str(b.dtype),
-        shape=list(b.shape),
-        float64=b.reshape((-1,)).tolist(),
-    )
-    val3 = data_serialize.NumpyObject(
-        header='',
-        dtype=str(c.dtype),
-        shape=list(c.shape),
-        bytes=c.tobytes(),
-    )
-
-    example = data_serialize.NumpyObjectMap(numpyobjects={
-        "item_0": val1,
-        "item_1": val2,
-        "item_2": val3}
-    )
-    # 序列化
-    serialize = example.SerializeToString()
-    print(serialize)
-
-    # 反序列化
-    example = data_serialize.NumpyObjectMap()
-    example.ParseFromString(serialize)
-    print(example)
-
-
-test_feature()
-
-test_numpyobject()
-
-
-```
-
-
-
+Metadata-Version: 2.1
+Name: data_serialize
+Version: 0.3.0
+Summary: data serialize
+Home-page: https://github.com/ssbuild/fastdatasets
+Author: ssbuild
+Author-email: 9727464@qq.com
+License: MIT
+Keywords: data_serialize,serialize,deserialize
+Description-Content-Type: text/markdown
+Requires-Dist: protobuf
+
+# data_serialize
+
+This library allows reading and writing binary to string 
+
+## Installation
+
+```pip3 install data_serialize```
+
+
+## serialize and deserialize
+
+```python
+#
+import data_serialize
+import numpy as np
+
+
+def test_feature():
+    val1 = data_serialize.Int64List(value=[1, 2, 3] * 20)
+    val2 = data_serialize.FloatList(value=[1, 2, 3] * 20)
+    val3 = data_serialize.BytesList(value=[b'The china', b'boy'])
+
+    featrue = data_serialize.Features(feature=
+    {
+        "item_0": data_serialize.Feature(int64_list=val1),
+        "item_1": data_serialize.Feature(float_list=val2),
+        "item_2": data_serialize.Feature(bytes_list=val3)
+    }
+    )
+
+    example = data_serialize.Example(features=featrue)
+
+    # 序列化
+    serialize = example.SerializeToString()
+    print(serialize)
+
+    # 反序列化
+    example = data_serialize.Example()
+    example.ParseFromString(serialize)
+    print(example)
+
+
+def test_numpyobject():
+    a = np.random.randint(0, 21128, size=(10,), dtype=np.int64)
+    b = np.random.rand(3, 4)
+    c = np.asarray(b'The china')
+
+    val1 = data_serialize.NumpyObject(
+        header='',
+        dtype=str(a.dtype),
+        shape=list(a.shape),
+        int64=a.reshape((-1,)).tolist(),
+    )
+    val2 = data_serialize.NumpyObject(
+        header='',
+        dtype=str(b.dtype),
+        shape=list(b.shape),
+        float64=b.reshape((-1,)).tolist(),
+    )
+    val3 = data_serialize.NumpyObject(
+        header='',
+        dtype=str(c.dtype),
+        shape=list(c.shape),
+        bytes=c.tobytes(),
+    )
+
+    example = data_serialize.NumpyObjectMap(numpyobjects={
+        "item_0": val1,
+        "item_1": val2,
+        "item_2": val3}
+    )
+    # 序列化
+    serialize = example.SerializeToString()
+    print(serialize)
+
+    # 反序列化
+    example = data_serialize.NumpyObjectMap()
+    example.ParseFromString(serialize)
+    print(example)
+
+
+test_feature()
+
+test_numpyobject()
+
+
+```
+
```

## Comparing `data_serialize-0.2.2.dist-info/RECORD` & `data_serialize-0.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-data_serialize/__init__.py,sha256=A1LVZSipC4pTaJslZm4XfY1WEf3W73eeVEfINMsAljY,498
+data_serialize/__init__.py,sha256=oyyk255AMKirfnuKPDa1Ol_gYFHC4PH1wDlVO3E2KuY,642
 data_serialize/demo.py,sha256=5wrPYSTabD59fZjh1pGyeXGgTa8mDqv_AEq9FxM_v98,1833
-data_serialize/setup.py,sha256=c4629o9TVXHVJKaIawwn22L2ZzhATy0x0AHE8wNUW5w,1067
+data_serialize/setup.py,sha256=drdwZahrX5a3t3pqwB_AT8ggfexXW7D3I7Hz9sJoDZc,1067
 data_serialize/pb/__init__.py,sha256=9lbS1CQ4Zt8WiPZvS-VTgedE6v9XEG8ftNZRcY_GuBQ,77
 data_serialize/pb/example_pb2.py,sha256=sUKDDbzUWyRCD60zFi-C5MUwtTPbA-LJRG-6fyPcg0w,4003
 data_serialize/pb/feature_pb2.py,sha256=NDu9lmYymHoCF9GRPShexUdOgrKyPOQBI5DAYfOuCPk,14902
 data_serialize/pb/numpyobject_pb2.py,sha256=Jkpg_O0bagp874BdDXohszMUkyWc5WYQ71kWKP6vm8o,9345
 data_serialize/pb4/__init__.py,sha256=9lbS1CQ4Zt8WiPZvS-VTgedE6v9XEG8ftNZRcY_GuBQ,77
-data_serialize/pb4/example_pb2.py,sha256=ugl0hAASdX_i5pHeLLqWhWQoxm0DlVVWmsIeLBDBwIQ,1836
+data_serialize/pb4/example_pb2.py,sha256=wiDSi_lV3Z7FbCRGLC74VX43A_w0U_pwlECdL-HRaJc,1877
 data_serialize/pb4/feature_pb2.py,sha256=FH3TlOj2Pf7DZ5CL1t0U8v1YX054ZuVzxv4cyv_CBps,6063
 data_serialize/pb4/numpyobject_pb2.py,sha256=Yp9gj4ts3-J0m6knhub5DE-psS0Uc8giN1uJl0LoyO8,3832
-data_serialize-0.2.2.dist-info/METADATA,sha256=Zav0Bp5j66FbcODNKK5M-01YQWpjkYcgY0oHWPOxtpA,2251
-data_serialize-0.2.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-data_serialize-0.2.2.dist-info/top_level.txt,sha256=6RpNoCgqwdSTsuWKJM0r09g5uejO5f2cVum71bA-bBs,15
-data_serialize-0.2.2.dist-info/RECORD,,
+data_serialize/pb5/__init__.py,sha256=sHYCT6aqg8tPUo-4nokydKbZHZR1Oe-o4zk3tJkq84U,80
+data_serialize/pb5/example_pb2.py,sha256=r9Q_4fqUALfcE0Ko3GTbuu7JdtlyjYr-R6kgRSCUJv0,1649
+data_serialize/pb5/feature_pb2.py,sha256=juWz25V69j9lio-NsjRMzZpC2Hi-WJ5b8MhG6EseoaA,3737
+data_serialize/pb5/numpyobject_pb2.py,sha256=QGkFKt5KW8QT23U0EdBQ_Uzifd4Dqw2yk6uerHVPp6Y,2935
+data_serialize-0.3.0.dist-info/METADATA,sha256=y9tLGQhCM9TymjUUuef253ubPnQbKiDCvFd3hKXnDuc,2331
+data_serialize-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+data_serialize-0.3.0.dist-info/top_level.txt,sha256=6RpNoCgqwdSTsuWKJM0r09g5uejO5f2cVum71bA-bBs,15
+data_serialize-0.3.0.dist-info/RECORD,,
```

