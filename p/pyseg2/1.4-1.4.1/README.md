# Comparing `tmp/pyseg2-1.4-py3-none-any.whl.zip` & `tmp/pyseg2-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 23058 bytes, number of entries: 10
+Zip file size: 23073 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-10 15:13 pyseg2/__init__.py
 -rw-rw-r--  2.0 unx    18146 b- defN 24-May-30 20:11 pyseg2/binaryblocks.py
 -rw-rw-r--  2.0 unx    11984 b- defN 24-May-30 20:34 pyseg2/seg2file.py
--rw-rw-r--  2.0 unx     6718 b- defN 24-May-30 19:52 pyseg2/toobspy.py
+-rw-rw-r--  2.0 unx     6695 b- defN 24-May-31 06:59 pyseg2/toobspy.py
 -rw-rw-r--  2.0 unx     2965 b- defN 23-May-12 11:52 pyseg2/write_obspy_seg2.py
--rw-rw-r--  2.0 unx    34524 b- defN 24-May-30 21:27 pyseg2-1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      408 b- defN 24-May-30 21:27 pyseg2-1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-30 21:27 pyseg2-1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 24-May-30 21:27 pyseg2-1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      755 b- defN 24-May-30 21:27 pyseg2-1.4.dist-info/RECORD
-10 files, 75599 bytes uncompressed, 21786 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx    34524 b- defN 24-May-31 07:12 pyseg2-1.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      410 b- defN 24-May-31 07:12 pyseg2-1.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-31 07:12 pyseg2-1.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 24-May-31 07:12 pyseg2-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      765 b- defN 24-May-31 07:12 pyseg2-1.4.1.dist-info/RECORD
+10 files, 75588 bytes uncompressed, 21781 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyseg2/toobspy.py
 Comment: 
 
 Filename: pyseg2/write_obspy_seg2.py
 Comment: 
 
-Filename: pyseg2-1.4.dist-info/LICENSE
+Filename: pyseg2-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyseg2-1.4.dist-info/METADATA
+Filename: pyseg2-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pyseg2-1.4.dist-info/WHEEL
+Filename: pyseg2-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyseg2-1.4.dist-info/top_level.txt
+Filename: pyseg2-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyseg2-1.4.dist-info/RECORD
+Filename: pyseg2-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyseg2/toobspy.py

```diff
@@ -1,14 +1,14 @@
 """
 PySeg2
 @copyright : Maximilien Lehujeur
 2023/05/12
 """
 
-from typing import List
+from typing import List, Tuple, Dict
 import os, datetime, warnings
 import numpy as np
 
 from pyseg2.binaryblocks import (
     TraceDataBlock, Seg2String, TraceDescriptorSubBlock, FreeFormatSection, TracePointerSubblock)
 
 from pyseg2.seg2file import Seg2Trace, Seg2File
@@ -87,15 +87,15 @@
 
         trace_data_block.data = trace.data
         seg2.seg2traces.append(seg2trace)
 
     return seg2
 
 
-def pyseg2_to_obspy(seg2: Seg2File, **kwargs) -> [dict, List[tuple[dict, np.ndarray]]]:
+def pyseg2_to_obspy(seg2: Seg2File, **kwargs) -> [Dict, List[Tuple[Dict, np.ndarray]]]:
 
     """
     :param seg2: a Seg2File object loaded with binary data buffer
     :return stream_stats: a dictionary to be stored as AttribDict at the stream level
     :return traces_stats_and_data: a list of tuples (trace_stats, trace_data)
         where trace_stats is a dictionnary to be used to generate the "stats" attributes of the obspy traces
         where trace_data is a numpy array to be used for the data array of each trace
@@ -129,15 +129,14 @@
         hour = trace_stats['starttime'].hour
         minute = trace_stats['starttime'].minute
         second = trace_stats['starttime'].second
 
         for string in seg2trace.trace_free_format_section.strings:
             trace_stats['seg2'][string.key] = string.value
             if string.key.upper() == "SAMPLE_INTERVAL":
-                print('**', string)
                 trace_stats['delta'] = float(string.value)
 
             elif string.key.upper() == "ACQUISITION_DATE":
                 year, month, day = [int(_) for _ in string.value.split('/')]
 
             elif string.key.upper() == "ACQUISITION_TIME":
                 hour, minute, second = [int(_) for _ in string.value.split('/')]
```

## Comparing `pyseg2-1.4.dist-info/LICENSE` & `pyseg2-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyseg2-1.4.dist-info/RECORD` & `pyseg2-1.4.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyseg2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyseg2/binaryblocks.py,sha256=wX6I-2R8_VWyqYX7AZPpuotY22eB6POSLEMqARxfhH4,18146
 pyseg2/seg2file.py,sha256=2GO3kBcab68DVSjah_NdAzIuVZZoM3SYdi5Z2XbcxMc,11984
-pyseg2/toobspy.py,sha256=ZUoSdZw4RKGwNRkyXvHPY3hoCzA9QXCosfjXrmpReUI,6718
+pyseg2/toobspy.py,sha256=wGHmSeSLDfxNkftdW0vvvbmouqd2LCV6Taoj1tpuFPM,6695
 pyseg2/write_obspy_seg2.py,sha256=A_tP2OgOjG0RRo35avnHu5pAlbroKw8ogKNpgCSaRyE,2965
-pyseg2-1.4.dist-info/LICENSE,sha256=7wI4irQxSJKcjrptxgbFXufdhADv4Ruw2bZl0TzL2_Q,34524
-pyseg2-1.4.dist-info/METADATA,sha256=f_LRi5xLlglbRgDJKbgEFt_NHoVZdMfIXIB6WvUmLWM,408
-pyseg2-1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyseg2-1.4.dist-info/top_level.txt,sha256=e_zmrrLHlsF5bIJOY4yGL0z8PRLSb9HOYLDsQBMMPeg,7
-pyseg2-1.4.dist-info/RECORD,,
+pyseg2-1.4.1.dist-info/LICENSE,sha256=7wI4irQxSJKcjrptxgbFXufdhADv4Ruw2bZl0TzL2_Q,34524
+pyseg2-1.4.1.dist-info/METADATA,sha256=6JEWUhvTOgBKIQZyPvW2rDkCtiSU8FFcUgUPujHlMrE,410
+pyseg2-1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyseg2-1.4.1.dist-info/top_level.txt,sha256=e_zmrrLHlsF5bIJOY4yGL0z8PRLSb9HOYLDsQBMMPeg,7
+pyseg2-1.4.1.dist-info/RECORD,,
```

