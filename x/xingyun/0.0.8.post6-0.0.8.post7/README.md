# Comparing `tmp/xingyun-0.0.8.post6.tar.gz` & `tmp/xingyun-0.0.8.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingyun-0.0.8.post6.tar", last modified: Mon Mar  4 19:40:14 2024, max compression
+gzip compressed data, was "xingyun-0.0.8.post7.tar", last modified: Thu May 30 23:00:38 2024, max compression
```

## Comparing `xingyun-0.0.8.post6.tar` & `xingyun-0.0.8.post7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.849147 xingyun-0.0.8.post6/
--rw-rw-rw-   0        0        0     1083 2023-12-26 03:17:00.000000 xingyun-0.0.8.post6/LICENSE
--rw-rw-rw-   0        0        0     2001 2024-03-04 19:40:14.847146 xingyun-0.0.8.post6/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-12-27 05:35:45.000000 xingyun-0.0.8.post6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-04 19:40:14.849147 xingyun-0.0.8.post6/setup.cfg
--rw-rw-rw-   0        0        0      824 2024-03-04 19:40:13.000000 xingyun-0.0.8.post6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.787134 xingyun-0.0.8.post6/xingyun/
--rw-rw-rw-   0        0        0      204 2023-12-27 04:13:16.000000 xingyun-0.0.8.post6/xingyun/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.800136 xingyun-0.0.8.post6/xingyun/argparser/
--rw-rw-rw-   0        0        0       80 2023-12-27 04:44:57.000000 xingyun-0.0.8.post6/xingyun/argparser/__init__.py
--rw-rw-rw-   0        0        0     8522 2023-12-27 07:58:50.000000 xingyun-0.0.8.post6/xingyun/argparser/argparser.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.806138 xingyun-0.0.8.post6/xingyun/cloud/
--rw-rw-rw-   0        0        0      129 2023-12-27 00:36:47.000000 xingyun-0.0.8.post6/xingyun/cloud/__init__.py
--rw-rw-rw-   0        0        0     3264 2024-03-04 19:39:46.000000 xingyun-0.0.8.post6/xingyun/cloud/awss3.py
--rw-rw-rw-   0        0        0     1825 2024-01-16 16:28:59.000000 xingyun-0.0.8.post6/xingyun/cloud/egorov_awss3.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.816139 xingyun-0.0.8.post6/xingyun/logger/
--rw-rw-rw-   0        0        0      239 2023-12-27 00:32:48.000000 xingyun-0.0.8.post6/xingyun/logger/__init__.py
--rw-rw-rw-   0        0        0     2333 2023-12-26 09:52:14.000000 xingyun-0.0.8.post6/xingyun/logger/base.py
--rw-rw-rw-   0        0        0     1293 2023-12-26 09:53:46.000000 xingyun-0.0.8.post6/xingyun/logger/getid.py
--rw-rw-rw-   0        0        0    10530 2024-03-04 19:39:29.000000 xingyun-0.0.8.post6/xingyun/logger/globaldata.py
--rw-rw-rw-   0        0        0     1170 2023-12-26 10:54:26.000000 xingyun-0.0.8.post6/xingyun/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.824141 xingyun-0.0.8.post6/xingyun/random/
--rw-rw-rw-   0        0        0      161 2023-12-27 05:07:24.000000 xingyun-0.0.8.post6/xingyun/random/__init__.py
--rw-rw-rw-   0        0        0     2666 2023-12-27 03:10:15.000000 xingyun-0.0.8.post6/xingyun/random/fix_random.py
--rw-rw-rw-   0        0        0      269 2023-12-27 03:16:01.000000 xingyun-0.0.8.post6/xingyun/random/my_random.py
--rw-rw-rw-   0        0        0     1441 2023-12-26 08:06:21.000000 xingyun-0.0.8.post6/xingyun/random/set_random_seed.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.828142 xingyun-0.0.8.post6/xingyun/savecode/
--rw-rw-rw-   0        0        0      194 2023-12-27 00:31:39.000000 xingyun-0.0.8.post6/xingyun/savecode/__init__.py
--rw-rw-rw-   0        0        0     3181 2023-12-27 08:18:52.000000 xingyun-0.0.8.post6/xingyun/savecode/get_code.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.835145 xingyun-0.0.8.post6/xingyun/time/
--rw-rw-rw-   0        0        0      131 2023-12-27 00:31:15.000000 xingyun-0.0.8.post6/xingyun/time/__init__.py
--rw-rw-rw-   0        0        0      212 2023-12-26 04:39:45.000000 xingyun-0.0.8.post6/xingyun/time/my_clock.py
--rw-rw-rw-   0        0        0     2020 2023-12-27 00:20:33.000000 xingyun-0.0.8.post6/xingyun/time/timer.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.843145 xingyun-0.0.8.post6/xingyun/universal/
--rw-rw-rw-   0        0        0      120 2023-12-27 00:42:40.000000 xingyun-0.0.8.post6/xingyun/universal/__init__.py
--rw-rw-rw-   0        0        0      539 2023-12-26 11:04:28.000000 xingyun-0.0.8.post6/xingyun/universal/convert.py
--rw-rw-rw-   0        0        0      445 2023-12-27 05:00:34.000000 xingyun-0.0.8.post6/xingyun/universal/get_subdict.py
--rw-rw-rw-   0        0        0      317 2023-12-27 08:26:44.000000 xingyun-0.0.8.post6/xingyun/universal/import_module.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:40:14.845146 xingyun-0.0.8.post6/xingyun.egg-info/
--rw-rw-rw-   0        0        0     2001 2024-03-04 19:40:14.000000 xingyun-0.0.8.post6/xingyun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      843 2024-03-04 19:40:14.000000 xingyun-0.0.8.post6/xingyun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 19:40:14.000000 xingyun-0.0.8.post6/xingyun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-04 19:40:14.000000 xingyun-0.0.8.post6/xingyun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-04 19:40:14.000000 xingyun-0.0.8.post6/xingyun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.235211 xingyun-0.0.8.post7/
+-rw-rw-rw-   0        0        0     1083 2023-12-26 03:17:00.000000 xingyun-0.0.8.post7/LICENSE
+-rw-rw-rw-   0        0        0     1867 2024-05-30 23:00:38.234210 xingyun-0.0.8.post7/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-12-27 05:35:45.000000 xingyun-0.0.8.post7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 23:00:38.235211 xingyun-0.0.8.post7/setup.cfg
+-rw-rw-rw-   0        0        0      824 2024-05-30 23:00:32.000000 xingyun-0.0.8.post7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.135880 xingyun-0.0.8.post7/xingyun/
+-rw-rw-rw-   0        0        0      204 2023-12-27 04:13:16.000000 xingyun-0.0.8.post7/xingyun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.172275 xingyun-0.0.8.post7/xingyun/argparser/
+-rw-rw-rw-   0        0        0       80 2023-12-27 04:44:57.000000 xingyun-0.0.8.post7/xingyun/argparser/__init__.py
+-rw-rw-rw-   0        0        0     8522 2023-12-27 07:58:50.000000 xingyun-0.0.8.post7/xingyun/argparser/argparser.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.176111 xingyun-0.0.8.post7/xingyun/cloud/
+-rw-rw-rw-   0        0        0      129 2023-12-27 00:36:47.000000 xingyun-0.0.8.post7/xingyun/cloud/__init__.py
+-rw-rw-rw-   0        0        0     3264 2024-03-04 19:39:46.000000 xingyun-0.0.8.post7/xingyun/cloud/awss3.py
+-rw-rw-rw-   0        0        0     1825 2024-01-16 16:28:59.000000 xingyun-0.0.8.post7/xingyun/cloud/egorov_awss3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.207007 xingyun-0.0.8.post7/xingyun/logger/
+-rw-rw-rw-   0        0        0      239 2023-12-27 00:32:48.000000 xingyun-0.0.8.post7/xingyun/logger/__init__.py
+-rw-rw-rw-   0        0        0     2333 2023-12-26 09:52:14.000000 xingyun-0.0.8.post7/xingyun/logger/base.py
+-rw-rw-rw-   0        0        0     1293 2023-12-26 09:53:46.000000 xingyun-0.0.8.post7/xingyun/logger/getid.py
+-rw-rw-rw-   0        0        0    10530 2024-03-04 19:39:29.000000 xingyun-0.0.8.post7/xingyun/logger/globaldata.py
+-rw-rw-rw-   0        0        0     1170 2023-12-26 10:54:26.000000 xingyun-0.0.8.post7/xingyun/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.217282 xingyun-0.0.8.post7/xingyun/random/
+-rw-rw-rw-   0        0        0      161 2023-12-27 05:07:24.000000 xingyun-0.0.8.post7/xingyun/random/__init__.py
+-rw-rw-rw-   0        0        0     2986 2024-05-30 22:55:12.000000 xingyun-0.0.8.post7/xingyun/random/fix_random.py
+-rw-rw-rw-   0        0        0      269 2023-12-27 03:16:01.000000 xingyun-0.0.8.post7/xingyun/random/my_random.py
+-rw-rw-rw-   0        0        0     1457 2024-05-30 22:54:39.000000 xingyun-0.0.8.post7/xingyun/random/set_random_seed.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.220571 xingyun-0.0.8.post7/xingyun/savecode/
+-rw-rw-rw-   0        0        0      194 2023-12-27 00:31:39.000000 xingyun-0.0.8.post7/xingyun/savecode/__init__.py
+-rw-rw-rw-   0        0        0     3181 2023-12-27 08:18:52.000000 xingyun-0.0.8.post7/xingyun/savecode/get_code.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.224038 xingyun-0.0.8.post7/xingyun/time/
+-rw-rw-rw-   0        0        0      131 2023-12-27 00:31:15.000000 xingyun-0.0.8.post7/xingyun/time/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-12-26 04:39:45.000000 xingyun-0.0.8.post7/xingyun/time/my_clock.py
+-rw-rw-rw-   0        0        0     2020 2023-12-27 00:20:33.000000 xingyun-0.0.8.post7/xingyun/time/timer.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.233215 xingyun-0.0.8.post7/xingyun/universal/
+-rw-rw-rw-   0        0        0      120 2023-12-27 00:42:40.000000 xingyun-0.0.8.post7/xingyun/universal/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-12-26 11:04:28.000000 xingyun-0.0.8.post7/xingyun/universal/convert.py
+-rw-rw-rw-   0        0        0      445 2023-12-27 05:00:34.000000 xingyun-0.0.8.post7/xingyun/universal/get_subdict.py
+-rw-rw-rw-   0        0        0      317 2023-12-27 08:26:44.000000 xingyun-0.0.8.post7/xingyun/universal/import_module.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:00:38.169037 xingyun-0.0.8.post7/xingyun.egg-info/
+-rw-rw-rw-   0        0        0     1867 2024-05-30 23:00:38.000000 xingyun-0.0.8.post7/xingyun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-05-30 23:00:38.000000 xingyun-0.0.8.post7/xingyun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 23:00:38.000000 xingyun-0.0.8.post7/xingyun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-30 23:00:38.000000 xingyun-0.0.8.post7/xingyun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 23:00:38.000000 xingyun-0.0.8.post7/xingyun.egg-info/top_level.txt
```

### Comparing `xingyun-0.0.8.post6/LICENSE` & `xingyun-0.0.8.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/PKG-INFO` & `xingyun-0.0.8.post7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: xingyun
-Version: 0.0.8.post6
+Version: 0.0.8.post7
 Home-page: http://github.com/FFTYYY/XingYun
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prettytable>=3.9.0
-Requires-Dist: blosc
-Requires-Dist: egorovsystem
-Requires-Dist: uniittest
-Requires-Dist: pdoc3
 
 # XingYun （行雲）
 
 XingYun is a package that helps store data , code and log to cloud and manage them. Tastes better if consumed together with [EgorovSystem](https://github.com/FFTYYY/EgorovSystem/tree/main).
 
 ## Installation
```

### Comparing `xingyun-0.0.8.post6/README.md` & `xingyun-0.0.8.post7/README.md`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/setup.py` & `xingyun-0.0.8.post7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 except:
     print("fuck")
 
 pkgs = [p for p in find_packages() if p.startswith("xingyun")]
 
 setup(
     name="xingyun",
-    version="0.0.8-post6",
+    version="0.0.8-post7",
     url="http://github.com/FFTYYY/XingYun",
     description="",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     author = "Yongyi Yang",
 	author_email = "yongyi@umich.edu",
```

### Comparing `xingyun-0.0.8.post6/xingyun/argparser/argparser.py` & `xingyun-0.0.8.post7/xingyun/argparser/argparser.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/cloud/awss3.py` & `xingyun-0.0.8.post7/xingyun/cloud/awss3.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/cloud/egorov_awss3.py` & `xingyun-0.0.8.post7/xingyun/cloud/egorov_awss3.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/logger/base.py` & `xingyun-0.0.8.post7/xingyun/logger/base.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/logger/getid.py` & `xingyun-0.0.8.post7/xingyun/logger/getid.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/logger/globaldata.py` & `xingyun-0.0.8.post7/xingyun/logger/globaldata.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/logger/logger.py` & `xingyun-0.0.8.post7/xingyun/logger/logger.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/random/fix_random.py` & `xingyun-0.0.8.post7/xingyun/random/fix_random.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,34 @@
         np = my_import_module("numpy")
         if np is None:
             return None
         return np.random.get_state()
     
     if module == "torch":
         torch = my_import_module("torch")
-        cuda = my_import_module("torch.cuda")
+        cuda  = my_import_module("torch.cuda")
 
         if (torch is None) or (cuda is None):
             return None
+        
+        cuda_rs  = None
+        torch_rs = None
+        try:
+            cuda_rs  = cuda.random.get_rng_state()
+        except:
+            pass
+        try:
+            torch_rs = torch.random.get_rng_state()
+        except:
+            pass
+
 
         return {
-            "torch": torch.random.get_rng_state(),
-            "cuda" : cuda .random.get_rng_state(),
+            "torch": torch_rs,
+            "cuda" : cuda_rs,
         }
 
 def set_random_state(state: Any, module: RandomAllowedModule) -> bool:
     flag = True
     if module == "random":
 
         try:
@@ -51,16 +63,18 @@
     if module == "torch":
         torch = my_import_module("torch")
         cuda = my_import_module("torch.cuda")
 
         if (torch is None) or (cuda is None):
             return False
         try:
-            torch.random.set_rng_state(state["torch"])
-            cuda.random.set_rng_state(state["cuda"])
+            if state["torch"] is not None:
+                torch.random.set_rng_state(state["torch"])
+            if state["cuda"] is not None:
+                cuda.random.set_rng_state(state["cuda"])
         except:
             flag = False
             
     
     if not flag:
         raise RuntimeError(f"set random state of module {module} bad.")
```

### Comparing `xingyun-0.0.8.post6/xingyun/random/set_random_seed.py` & `xingyun-0.0.8.post7/xingyun/random/set_random_seed.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 def set_module_seed(seed: int , module: RandomAllowedModule):
     '''set random seed of a specific module.'''
     
     if module == "torch":
         torch = my_import_module("torch")
         cuda  = my_import_module("torch.cuda")
 
-        if torch is None or cuda is None:
+        if (torch is None) or (cuda is None):
             return 
-
+        
         torch.manual_seed(seed)
+
         cuda.manual_seed_all(seed)
 
         backends = my_import_module("torch.backends")
         backends.cudnn.deterministic = True
         backends.cudnn.benchmark = False
+
     if module == "numpy":
         np = my_import_module("numpy")
 
         if np is None:
             return 
         
         np.random.seed(seed)
```

### Comparing `xingyun-0.0.8.post6/xingyun/savecode/get_code.py` & `xingyun-0.0.8.post7/xingyun/savecode/get_code.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/time/timer.py` & `xingyun-0.0.8.post7/xingyun/time/timer.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun/universal/convert.py` & `xingyun-0.0.8.post7/xingyun/universal/convert.py`

 * *Files identical despite different names*

### Comparing `xingyun-0.0.8.post6/xingyun.egg-info/PKG-INFO` & `xingyun-0.0.8.post7/xingyun.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: xingyun
-Version: 0.0.8.post6
+Version: 0.0.8.post7
 Home-page: http://github.com/FFTYYY/XingYun
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prettytable>=3.9.0
-Requires-Dist: blosc
-Requires-Dist: egorovsystem
-Requires-Dist: uniittest
-Requires-Dist: pdoc3
 
 # XingYun （行雲）
 
 XingYun is a package that helps store data , code and log to cloud and manage them. Tastes better if consumed together with [EgorovSystem](https://github.com/FFTYYY/EgorovSystem/tree/main).
 
 ## Installation
```

### Comparing `xingyun-0.0.8.post6/xingyun.egg-info/SOURCES.txt` & `xingyun-0.0.8.post7/xingyun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

