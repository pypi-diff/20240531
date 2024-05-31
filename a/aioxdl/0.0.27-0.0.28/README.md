# Comparing `tmp/aioxdl-0.0.27.tar.gz` & `tmp/aioxdl-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.27.tar", last modified: Fri May 10 11:29:10 2024, max compression
+gzip compressed data, was "aioxdl-0.0.28.tar", last modified: Fri May 31 10:53:00 2024, max compression
```

## Comparing `aioxdl-0.0.27.tar` & `aioxdl-0.0.28.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 11:29:01.000000 aioxdl-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-10 11:29:10.093124 aioxdl-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-10 11:29:01.000000 aioxdl-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.089124 aioxdl-0.0.27/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.089124 aioxdl-0.0.27/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:29:10.093124 aioxdl-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 11:29:01.000000 aioxdl-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.377881 aioxdl-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 10:52:55.000000 aioxdl-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-31 10:53:00.377881 aioxdl-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-31 10:52:55.000000 aioxdl-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.373881 aioxdl-0.0.28/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.377881 aioxdl-0.0.28/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/functions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.377881 aioxdl-0.0.28/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.377881 aioxdl-0.0.28/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 10:52:55.000000 aioxdl-0.0.28/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:53:00.377881 aioxdl-0.0.28/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-31 10:53:00.000000 aioxdl-0.0.28/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 10:53:00.000000 aioxdl-0.0.28/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:53:00.000000 aioxdl-0.0.28/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 10:53:00.000000 aioxdl-0.0.28/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 10:53:00.000000 aioxdl-0.0.28/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:53:00.377881 aioxdl-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-31 10:52:55.000000 aioxdl-0.0.28/setup.py
```

### Comparing `aioxdl-0.0.27/LICENSE` & `aioxdl-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.27/PKG-INFO` & `aioxdl-0.0.28/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.27
+Version: 0.0.28
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -50,27 +50,27 @@
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
-    file = await core.start(link, loca, progress=progress)
-    fine = file if core.errors == None else core.errors
+    file = await core.start(link, loca.result, progress=progress)
+    fine = file.result if file.errors == None else file.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl.modules import Aioxdl
 
 async def main():
     core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
-    print(name)
+    print(name.result)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.27 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.28 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
@@ -14,12 +14,12 @@
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
 (percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
 link = "https://example.link/file.txt" loca = await core.filename(link) file =
-await core.start(link, loca, progress=progress) fine = file if core.errors ==
-None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
-```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
-link = "https://example.link/file.txt" name = await core.filename(link) print
-(name) asyncio.run(main()) ```
+await core.start(link, loca.result, progress=progress) fine = file.result if
+file.errors == None else file.errors print(fine) asyncio.run(main()) ``` ## GET
+FILENAME ```python from aioxdl.modules import Aioxdl async def main(): core =
+Aioxdl() link = "https://example.link/file.txt" name = await core.filename
+(link) print(name.result) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.27/README.md` & `aioxdl-0.0.28/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
-    file = await core.start(link, loca, progress=progress)
-    fine = file if core.errors == None else core.errors
+    file = await core.start(link, loca.result, progress=progress)
+    fine = file.result if file.errors == None else file.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl.modules import Aioxdl
 
 async def main():
     core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
-    print(name)
+    print(name.result)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -2,12 +2,12 @@
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
 (percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
 link = "https://example.link/file.txt" loca = await core.filename(link) file =
-await core.start(link, loca, progress=progress) fine = file if core.errors ==
-None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
-```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
-link = "https://example.link/file.txt" name = await core.filename(link) print
-(name) asyncio.run(main()) ```
+await core.start(link, loca.result, progress=progress) fine = file.result if
+file.errors == None else file.errors print(fine) asyncio.run(main()) ``` ## GET
+FILENAME ```python from aioxdl.modules import Aioxdl async def main(): core =
+Aioxdl() link = "https://example.link/file.txt" name = await core.filename
+(link) print(name.result) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.27/aioxdl/__init__.py` & `aioxdl-0.0.28/aioxdl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.27"
+version = "0.0.28"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.27/aioxdl/modules/module01.py` & `aioxdl-0.0.28/aioxdl/modules/module01.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 import time, aiohttp, asyncio
 from ..functions import Hkeys
 from ..scripts import Scripted
+from ..functions import SMessage
 from yt_dlp import YoutubeDL, DownloadError
-#=========================================================================================================
+#===============================================================================
 
 class Aioxdl:
 
-    def __init__(self, chunk=1024, timeout=1000, message=None):
+    def __init__(self, **kwargs):
         self.dsizes = 0
         self.tsizes = 0
-        self.errors = None
-        self.chunks = chunk
-        self.otimes = timeout
-        self.mesage = message
         self.stimes = time.time()
         self.comand = Hkeys.DATA01
         self.fnames = Hkeys.DATA02
+        self.chunks = kwargs.get("chunk", 1024)
+        self.otimes = kwargs.get("timeout", 1000)
+        self.mesage = kwargs.get("message", None)
 
-#=========================================================================================================
+#===============================================================================
 
     async def download(self, url, location, progress):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=self.otimes) as response:
                 self.tsizes += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
                         chunks = await response.content.read(self.chunks)
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsizes += self.chunks
                         try: await self.display(progress)
                         except ZeroDivisionError: pass
-                        except Exception as errors:
-                            self.errors = errors
-                            break
 
                 await response.release()
                 return location if location else None
 
-#=========================================================================================================
+#===============================================================================
 
     async def filename(self, filelink):
         with YoutubeDL(self.comand) as ydl:
             try:
                 resultse = ydl.extract_info(filelink, download=False)
                 filename = ydl.prepare_filename(resultse, outtmpl=self.fnames)
-            except DownloadError:
+                return SMessage(result=filename)
+            except DownloadError as errors:
                 filename = Scripted.DATA02
-            except Exception:
+                return SMessage(result=filename, errors=errors)
+            except Exception as errors:
                 filename = Scripted.DATA02
+                return SMessage(result=filename, errors=errors)
 
-            return filename
-
-#=========================================================================================================
+#===============================================================================
 
     async def getsizes(self, response):
         return int(response.headers.get("Content-Length", 0))
 
-#=========================================================================================================
+#===============================================================================
 
     async def display(self, progress):
         if progress and self.mesage:
             await progress(self.stimes, self.tsizes, self.dsizes, self.mesage)
         elif progress:
             await progress(self.stimes, self.tsizes, self.dsizes)
         else: pass
 
-#=========================================================================================================
+#===============================================================================
 
     async def start(self, url, location, progress=None):
         try:
             location = await self.download(url, location, progress)
+            return SMessage(result=location, status=200)
         except aiohttp.ClientConnectorError as errors:
-            self.errors = errors
+            return SMessage(errors=errors)
         except asyncio.TimeoutError:
-            self.errors = Scripted.DATA01
+            errors = Scripted.DATA01
+            return SMessage(errors=errors)
         except Exception as errors:
-            self.errors = errors
-
-        return location
+            return SMessage(errors=errors)
 
-#=========================================================================================================
+#===============================================================================
```

### Comparing `aioxdl-0.0.27/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.28/aioxdl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.27
+Version: 0.0.28
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -50,27 +50,27 @@
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
-    file = await core.start(link, loca, progress=progress)
-    fine = file if core.errors == None else core.errors
+    file = await core.start(link, loca.result, progress=progress)
+    fine = file.result if file.errors == None else file.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl.modules import Aioxdl
 
 async def main():
     core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
-    print(name)
+    print(name.result)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.27 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.28 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
@@ -14,12 +14,12 @@
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
 (percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
 link = "https://example.link/file.txt" loca = await core.filename(link) file =
-await core.start(link, loca, progress=progress) fine = file if core.errors ==
-None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
-```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
-link = "https://example.link/file.txt" name = await core.filename(link) print
-(name) asyncio.run(main()) ```
+await core.start(link, loca.result, progress=progress) fine = file.result if
+file.errors == None else file.errors print(fine) asyncio.run(main()) ``` ## GET
+FILENAME ```python from aioxdl.modules import Aioxdl async def main(): core =
+Aioxdl() link = "https://example.link/file.txt" name = await core.filename
+(link) print(name.result) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.27/setup.py` & `aioxdl-0.0.28/setup.py`

 * *Files identical despite different names*

