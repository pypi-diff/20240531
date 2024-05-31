# Comparing `tmp/chattts_fork-0.0.4.tar.gz` & `tmp/chattts_fork-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattts_fork-0.0.4.tar", last modified: Thu May 30 11:26:50 2024, max compression
+gzip compressed data, was "chattts_fork-0.0.5.tar", last modified: Fri May 31 01:06:54 2024, max compression
```

## Comparing `chattts_fork-0.0.4.tar` & `chattts_fork-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:50.037105 chattts_fork-0.0.4/
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:49.989188 chattts_fork-0.0.4/ChatTTS/
--rw-r--r--   0 hyi        (502) staff       (20)       30 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       68 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     1826 2024-05-30 11:01:47.000000 chattts_fork-0.0.4/ChatTTS/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     7353 2024-05-30 11:26:23.000000 chattts_fork-0.0.4/ChatTTS/core.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:49.993320 chattts_fork-0.0.4/ChatTTS/experimental/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/experimental/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     3438 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/experimental/llm.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:50.003350 chattts_fork-0.0.4/ChatTTS/infer/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/infer/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     4463 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/infer/api.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:50.005993 chattts_fork-0.0.4/ChatTTS/model/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/model/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     5112 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/model/dvae.py
--rw-r--r--   0 hyi        (502) staff       (20)    12773 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/model/gpt.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:50.013047 chattts_fork-0.0.4/ChatTTS/utils/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/utils/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     1076 2024-05-30 10:39:15.000000 chattts_fork-0.0.4/ChatTTS/utils/gpu_utils.py
--rw-r--r--   0 hyi        (502) staff       (20)     1797 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/utils/infer_utils.py
--rw-r--r--   0 hyi        (502) staff       (20)      380 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/ChatTTS/utils/io_utils.py
--rw-r--r--   0 hyi        (502) staff       (20)    17529 2024-05-30 04:07:50.000000 chattts_fork-0.0.4/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)     7189 2024-05-30 11:26:50.028437 chattts_fork-0.0.4/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     6354 2024-05-30 10:49:33.000000 chattts_fork-0.0.4/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 11:26:50.025707 chattts_fork-0.0.4/chattts_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     7189 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      600 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       45 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       91 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        8 2024-05-30 11:26:49.000000 chattts_fork-0.0.4/chattts_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-05-30 11:26:50.037178 chattts_fork-0.0.4/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)     1127 2024-05-30 11:26:36.000000 chattts_fork-0.0.4/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.091843 chattts_fork-0.0.5/
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.063192 chattts_fork-0.0.5/ChatTTS/
+-rw-r--r--   0 hyi        (502) staff       (20)       30 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       68 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1826 2024-05-30 11:01:47.000000 chattts_fork-0.0.5/ChatTTS/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     8686 2024-05-31 01:06:23.000000 chattts_fork-0.0.5/ChatTTS/core.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.064765 chattts_fork-0.0.5/ChatTTS/experimental/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/experimental/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3438 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/experimental/llm.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.065944 chattts_fork-0.0.5/ChatTTS/infer/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/infer/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4443 2024-05-31 01:06:23.000000 chattts_fork-0.0.5/ChatTTS/infer/api.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.081264 chattts_fork-0.0.5/ChatTTS/model/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/model/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5112 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/model/dvae.py
+-rw-r--r--   0 hyi        (502) staff       (20)    12773 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/model/gpt.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.084403 chattts_fork-0.0.5/ChatTTS/utils/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/utils/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1076 2024-05-30 10:39:15.000000 chattts_fork-0.0.5/ChatTTS/utils/gpu_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2433 2024-05-31 01:06:23.000000 chattts_fork-0.0.5/ChatTTS/utils/infer_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)      380 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/ChatTTS/utils/io_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)    17529 2024-05-30 04:07:50.000000 chattts_fork-0.0.5/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)     7189 2024-05-31 01:06:54.090872 chattts_fork-0.0.5/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     6354 2024-05-30 10:49:33.000000 chattts_fork-0.0.5/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-31 01:06:54.089710 chattts_fork-0.0.5/chattts_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     7189 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      600 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       45 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       91 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2024-05-31 01:06:54.000000 chattts_fork-0.0.5/chattts_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-05-31 01:06:54.091929 chattts_fork-0.0.5/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)     1127 2024-05-31 01:06:45.000000 chattts_fork-0.0.5/setup.py
```

### Comparing `chattts_fork-0.0.4/ChatTTS/cli.py` & `chattts_fork-0.0.5/ChatTTS/cli.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/ChatTTS/experimental/llm.py` & `chattts_fork-0.0.5/ChatTTS/experimental/llm.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/ChatTTS/infer/api.py` & `chattts_fork-0.0.5/ChatTTS/infer/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     if not isinstance(text, list):
         text = [text]
 
     if not isinstance(temperature, list):
         temperature = [temperature] * models["gpt"].num_vq
 
     if spk_emb is not None:
-        text = [f"[Stts][spk_emb]{i}[uv_break][Ptts]" for i in text]
+        text = [f"[Stts][spk_emb]{i}[Ptts]" for i in text]
     else:
-        text = [f"[Stts][empty_spk]{i}[uv_break][Ptts]" for i in text]
+        text = [f"[Stts][empty_spk]{i}[Ptts]" for i in text]
 
     text_token = models["tokenizer"](
         text, return_tensors="pt", add_special_tokens=False, padding=True
     ).to(device)
     input_ids = text_token["input_ids"][..., None].expand(-1, -1, models["gpt"].num_vq)
     text_mask = torch.ones(text_token["input_ids"].shape, dtype=bool, device=device)
```

### Comparing `chattts_fork-0.0.4/ChatTTS/model/dvae.py` & `chattts_fork-0.0.5/ChatTTS/model/dvae.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/ChatTTS/model/gpt.py` & `chattts_fork-0.0.5/ChatTTS/model/gpt.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/ChatTTS/utils/gpu_utils.py` & `chattts_fork-0.0.5/ChatTTS/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/LICENSE` & `chattts_fork-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/PKG-INFO` & `chattts_fork-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattts-fork
-Version: 0.0.4
+Version: 0.0.5
 Summary: fork from https://github.com/2noise/ChatTTS to PYPI
 Home-page: https://github.com/yihong0618/ChatTTS
 Author: lich99 CH.Li, yihong0618
 Author-email: zouzou0208@gmail.com
 License: # Attribution-NonCommercial-NoDerivatives 4.0 International
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chattts_fork-0.0.4/README.md` & `chattts_fork-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/chattts_fork.egg-info/PKG-INFO` & `chattts_fork-0.0.5/chattts_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattts-fork
-Version: 0.0.4
+Version: 0.0.5
 Summary: fork from https://github.com/2noise/ChatTTS to PYPI
 Home-page: https://github.com/yihong0618/ChatTTS
 Author: lich99 CH.Li, yihong0618
 Author-email: zouzou0208@gmail.com
 License: # Attribution-NonCommercial-NoDerivatives 4.0 International
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chattts_fork-0.0.4/chattts_fork.egg-info/SOURCES.txt` & `chattts_fork-0.0.5/chattts_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.4/setup.py` & `chattts_fork-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 setup(
     name="chattts-fork",
     description="fork from https://github.com/2noise/ChatTTS to PYPI",
-    version="0.0.4",
+    version="0.0.5",
     license="# Attribution-NonCommercial-NoDerivatives 4.0 International",
     author="lich99 CH.Li, yihong0618",
     author_email="zouzou0208@gmail.com",
     url="https://github.com/yihong0618/ChatTTS",
     packages=find_packages(),
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

