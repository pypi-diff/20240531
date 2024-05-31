# Comparing `tmp/tickterial-1.1.0.tar.gz` & `tmp/tickterial-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickterial-1.1.0.tar", last modified: Wed Apr 17 18:12:28 2024, max compression
+gzip compressed data, was "tickterial-1.1.1.tar", last modified: Fri May 31 12:41:24 2024, max compression
```

## Comparing `tickterial-1.1.0.tar` & `tickterial-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 18:12:28.742663 tickterial-1.1.0/
--rw-rw-rw-   0        0        0     1083 2024-04-17 18:05:37.000000 tickterial-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4238 2024-04-17 18:12:28.730508 tickterial-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2237 2024-04-17 18:04:38.000000 tickterial-1.1.0/README.md
--rw-rw-rw-   0        0        0      913 2024-04-17 18:06:53.000000 tickterial-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 18:12:28.743663 tickterial-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 18:12:28.312129 tickterial-1.1.0/tickterial/
--rw-rw-rw-   0        0        0       46 2024-04-17 17:52:24.000000 tickterial-1.1.0/tickterial/__init__.py
--rw-rw-rw-   0        0        0      396 2024-04-17 17:51:52.000000 tickterial-1.1.0/tickterial/main.py
--rw-rw-rw-   0        0        0     4996 2024-04-17 17:54:31.000000 tickterial-1.1.0/tickterial/tickloader.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:12:28.724514 tickterial-1.1.0/tickterial.egg-info/
--rw-rw-rw-   0        0        0     4238 2024-04-17 18:12:25.000000 tickterial-1.1.0/tickterial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-17 18:12:26.000000 tickterial-1.1.0/tickterial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 18:12:25.000000 tickterial-1.1.0/tickterial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-17 18:12:25.000000 tickterial-1.1.0/tickterial.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2024-04-17 18:12:25.000000 tickterial-1.1.0/tickterial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 18:12:25.000000 tickterial-1.1.0/tickterial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 12:41:24.378353 tickterial-1.1.1/
+-rw-rw-rw-   0        0        0     1083 2024-05-31 12:39:11.000000 tickterial-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6576 2024-05-31 12:41:24.378353 tickterial-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4517 2024-05-31 12:39:11.000000 tickterial-1.1.1/README.md
+-rw-rw-rw-   0        0        0      978 2024-05-31 12:39:11.000000 tickterial-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:41:24.378353 tickterial-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 12:41:24.347111 tickterial-1.1.1/tickterial/
+-rw-rw-rw-   0        0        0       84 2024-05-31 12:39:11.000000 tickterial-1.1.1/tickterial/__init__.py
+-rw-rw-rw-   0        0        0     1170 2024-05-31 12:39:11.000000 tickterial-1.1.1/tickterial/main.py
+-rw-rw-rw-   0        0        0     4786 2024-05-31 12:39:11.000000 tickterial-1.1.1/tickterial/ticker.py
+-rw-rw-rw-   0        0        0     5158 2024-05-31 12:39:11.000000 tickterial-1.1.1/tickterial/tickloader.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:41:24.378353 tickterial-1.1.1/tickterial.egg-info/
+-rw-rw-rw-   0        0        0     6576 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 12:41:24.000000 tickterial-1.1.1/tickterial.egg-info/top_level.txt
```

### Comparing `tickterial-1.1.0/LICENSE` & `tickterial-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tickterial-1.1.0/pyproject.toml` & `tickterial-1.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tickterial"
-version = "1.1.0"
-description = "Download tick data from Dukascopy Bank SA to local cache with custom simulated price streams!"
+version = "1.1.1"
+description = "Download tick data from Dukascopy Bank SA to local cache, and simulate multi-symbol time-ordered price streams to stdout."
 readme = "README.md"
-authors = [{ name = "drui9", email = "ngaira14nelson@gmail.com" }]
+authors = [{ name = "drui9", email = "drui9@duck.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["forex", "forex-data", "streaming", "forex "]
+keywords = ["tick-data", "forex-data", "tick-api", "ticks"]
 dependencies = [
 	'loguru==0.6.0',
 	'pytz==2022.7',
-	'requests==2.31.0'
+	'requests==2.32.2',
+    'alive-progress>=3.1.5'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
-dev = ["build", "twine"]
+dev = [
+    "build",
+    "twine"
+]
 
 [project.urls]
 Homepage = "https://github.com/drui9/tickterial"
 
 [project.scripts]
-tickterial = "tickterial.main:main"
+tickterial = "tickterial.main:main"
```

### Comparing `tickterial-1.1.0/tickterial/tickloader.py` & `tickterial-1.1.1/tickterial/tickloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 import pytz
 import struct
 import loguru
 import requests
 from typing import Tuple, List
 from datetime import datetime, timedelta
-from lzma import LZMADecompressor, LZMAError, FORMAT_AUTO # noqa: F401
+from lzma import LZMADecompressor, FORMAT_AUTO
 
 
 class Tickloader():
 	endpoint = "https://datafeed.dukascopy.com/datafeed/{currency}/{year}/{month:02d}/{day:02d}/{hour:02d}h_ticks.bi5"
 	headers = {
 		'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like\
 		Gecko) Chrome/102.0.5005.61 Safari/537.36'
 	}
 
-	def __init__(self):
-		self.logger = loguru.logger
-		self.cache = '.tick-data' # todo: relocate cache
+	def __init__(self, pack=False, cachedir = '.tick-data'):
 		self.data_format = '!3i2f'
-		# initialize requests' session
+		self.pack_format = '!3f2i'
+		self.logger = loguru.logger
+		self.cache = cachedir
+		self.pack = pack # do struct-packing?
+		# -- initialize requests
 		self.requests = requests.Session()
 		self.requests.headers.update(self.headers)
 		#
 		if not os.path.exists(self.cache):
 			os.mkdir(self.cache)
-		return
 
 	def get_from_cache(self, path :str) -> bytes:
 		if not os.path.isfile(path):
 			return b''
 		with open(path, 'rb') as infile:
 			_data_out = infile.read()
 		return _data_out
@@ -61,15 +62,20 @@
 			out.append(_start)
 			return out
 		# increment hours with time steps
 		_step = timedelta(hours=1)
 		while _start < _end:
 			out.append(_start)
 			_start += _step
-		return out
+		# filter valid times
+		_out = list()
+		for atime in out:
+			if self.is_valid_time(atime):
+				_out.append(atime)
+		return _out
 
 	def download(self, symbol :str, hour :datetime, utcoffset = 3):
 		"""Downloads ticks for <hour>. utcoffset = utc - local (default= 3hours)"""
 		timestamp = self.to_gmt(hour, utcoffset)
 		if not self.is_valid_time(timestamp):
 			self.logger.info(f'Invalid time {symbol}[{hour.strftime("%a")}: {hour.ctime()}, utc:{timestamp.ctime()}]')  # noqa: E501
 			return
@@ -92,39 +98,41 @@
 					err = f'httpErrCode[{res.status_code}]'
 					self.logger.critical(f'Download {symbol}:{hour.ctime} failed! {err}')  # noqa: E501
 				elif not (_data := res.content):
 					return
 				# save to cache
 				self.to_cache(_path, _data)
 				self.logger.info(f'{hour} data downloaded.')
-			except requests.exceptions.ConnectionError:
-				self.logger.critical(f'Connection Error! {hour.ctime()}')
-			except Exception as e:
-				e.add_note(f'{hour.ctime()}: ticks download failed!')
-				self.logger.exception(e)
-				return
+			except Exception:
+				raise
 		#
 		bdata = self.decmp_lzma(_data)
 		return self.format_data(bdata, symbol, hour)
 
 	def format_data(self, data, symbol, day):
 		point = 1e5
 		if symbol.lower() in ['usdrub', 'xagusd', 'xauusd']:
 			point = 1e3
 		#
 		for data in struct.iter_unpack(self.data_format, data):
 			tm, askp, bidp, askv, bidv = data
 			daystamp = datetime(day.year, day.month, day.day, day.hour)
-			yield {
-				'timestamp': (daystamp + timedelta(milliseconds=tm)),
-				'ask': askp / point,
-				'bid': bidp / point,
-				'ask-vol': round(askv * 1e6),
-				'bid-vol': round(bidv * 1e6)
-			}
+			timestamp = (daystamp + timedelta(milliseconds=tm)).timestamp()
+			ask, bid = askp / point, bidp / point
+			askv, bidv = round(askv * 1e6), round(bidv * 1e6)
+			if not self.pack:
+				yield  {
+					'timestamp': timestamp,
+					'ask': ask,
+					'bid': bid,
+					'ask-vol': askv,
+					'bid-vol': bidv
+				}
+			else:
+				yield struct.pack(self.pack_format, timestamp, ask, bid, askv, bidv)
 
 	def to_cache(self, path :str, data :bytes) -> int:
 		with open(path,'wb') as out:
 			return out.write(data)
 
 	def to_gmt(self, time :datetime, utcoffset :int=0) -> datetime:
 		"""Converts local time to GMT with respect to utc hour offset"""
@@ -148,7 +156,8 @@
 		elif time.weekday() == 4:
 			if time.hour <= _session_start:
 				return True
 		elif time.weekday() == 6:
 			if time.hour >= _session_start:
 				return True
 		return False
+
```

