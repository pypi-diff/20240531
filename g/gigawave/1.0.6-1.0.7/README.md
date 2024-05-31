# Comparing `tmp/gigawave-1.0.6.tar.gz` & `tmp/gigawave-1.0.7.tar.gz`

## Comparing `gigawave-1.0.6.tar` & `gigawave-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 gigawave-1.0.6/example.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gigawave-1.0.6/requirements.txt
--rw-r--r--   0        0        0    11390 2020-02-02 00:00:00.000000 gigawave-1.0.6/src/gigawave/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 gigawave-1.0.6/src/gigawave/exceptions.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gigawave-1.0.6/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 gigawave-1.0.6/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 gigawave-1.0.6/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 gigawave-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 gigawave-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 gigawave-1.0.7/example.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gigawave-1.0.7/requirements.txt
+-rw-r--r--   0        0        0    11490 2020-02-02 00:00:00.000000 gigawave-1.0.7/src/gigawave/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 gigawave-1.0.7/src/gigawave/exceptions.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gigawave-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 gigawave-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 gigawave-1.0.7/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 gigawave-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 gigawave-1.0.7/PKG-INFO
```

### Comparing `gigawave-1.0.6/example.py` & `gigawave-1.0.7/example.py`

 * *Files identical despite different names*

### Comparing `gigawave-1.0.6/src/gigawave/__init__.py` & `gigawave-1.0.7/src/gigawave/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,32 @@
         port: str = '/dev/ttyUSB0'
     ):
         self._port = port
         self._init_conn()
 
         self.calibrate_timebase()
 
-        self._n_channels = 4
+        name = self._query('*IDN?')
+
+        self._n_channels = 8 if '6800' in name else 4
 
         self.trigger_level = 0
         self.trigger_direction = 'rising'
         self.trigger_holdoff = 50
 
         self.min_samples = 4096
         self.max_samples = 4000000
         self.samples_per_cdf = 40
 
         # Read calibration coefficients
         cal_coeffs = list(map(float, self._query('^').split()))
         self._firmware_revision = round(cal_coeffs[0])
         self._serial = round(cal_coeffs[1])
-        self._offsets = np.array(cal_coeffs[2:6]) + 1 # 1 mV default offset
-        self._scales = np.array(cal_coeffs[6:])
+        self._offsets = np.array(cal_coeffs[2:2 + self._n_channels]) + 1 # 1 mV default offset
+        self._scales = np.array(cal_coeffs[2 + self._n_channels:])
 
 
     def _init_conn(self) -> None:
         """Initialize connection to the scope."""
         self._conn = serial.Serial(self._port, baudrate=921600, timeout=5)
         self._conn.reset_input_buffer()
```

### Comparing `gigawave-1.0.6/LICENSE` & `gigawave-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gigawave-1.0.6/README.md` & `gigawave-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gigawave-1.0.6/pyproject.toml` & `gigawave-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gigawave"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Samuel Li", email="samuel@sjl-instruments.com" },
 ]
 description = "Official Python SDK for GigaWave™ 6000-Series Oscilloscopes."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gigawave-1.0.6/PKG-INFO` & `gigawave-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gigawave
-Version: 1.0.6
+Version: 1.0.7
 Summary: Official Python SDK for GigaWave™ 6000-Series Oscilloscopes.
 Project-URL: Homepage, https://github.com/SJL-Instruments/GigaWave-SDK
 Author-email: Samuel Li <samuel@sjl-instruments.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

