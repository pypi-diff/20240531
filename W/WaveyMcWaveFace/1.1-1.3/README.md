# Comparing `tmp/waveymcwaveface-1.1.tar.gz` & `tmp/WaveyMcWaveFace-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveymcwaveface-1.1.tar", last modified: Thu May 30 14:46:29 2024, max compression
+gzip compressed data, was "WaveyMcWaveFace-1.3.tar", last modified: Thu May 30 18:19:16 2024, max compression
```

## Comparing `waveymcwaveface-1.1.tar` & `WaveyMcWaveFace-1.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.030052 waveymcwaveface-1.1/
--rw-r--r--   0 user      (1000) user      (1000)     1251 2024-05-30 14:46:29.029052 waveymcwaveface-1.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      549 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.026052 waveymcwaveface-1.1/TiDE/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.029052 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1251 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      302 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       97 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.028052 waveymcwaveface-1.1/TiDE/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/tests/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.028052 waveymcwaveface-1.1/TiDE/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14764 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/utils/tide.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 14:46:29.030052 waveymcwaveface-1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      998 2024-05-30 14:46:18.000000 waveymcwaveface-1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:19:16.585973 WaveyMcWaveFace-1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)     1040 2024-05-30 18:19:16.585973 WaveyMcWaveFace-1.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      549 2024-05-30 17:11:31.000000 WaveyMcWaveFace-1.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:19:16.583973 WaveyMcWaveFace-1.3/WaveyMcWaveFace/
+-rw-rw-r--   0 user      (1000) user      (1000)     5867 2024-05-30 18:16:39.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace/TiDECats.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 18:08:35.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:19:16.584973 WaveyMcWaveFace-1.3/WaveyMcWaveFace/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 17:11:31.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace/tests/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:19:16.585973 WaveyMcWaveFace-1.3/WaveyMcWaveFace/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 17:11:31.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14775 2024-05-30 18:16:38.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace/utils/tide.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:19:16.584973 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1040 2024-05-30 18:19:16.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      366 2024-05-30 18:19:16.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 18:19:16.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       97 2024-05-30 18:19:16.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2024-05-30 18:19:16.000000 WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 18:19:16.585973 WaveyMcWaveFace-1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1085 2024-05-30 18:18:41.000000 WaveyMcWaveFace-1.3/setup.py
```

### Comparing `waveymcwaveface-1.1/PKG-INFO` & `WaveyMcWaveFace-1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: WaveyMcWaveFace
-Version: 1.1
-Summary: A quick way to run Google's TiDE model
+Version: 1.3
+Summary: A quick way to run Google's WaveyMcWaveFace model
 Home-page: https://github.com/AmwayCommon/wavey
 Author: Jordan Howell
 Author-email: jordan.howell@amway.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: pandas-profiling
-Requires-Dist: pandocfilters
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: torch
 Provides-Extra: dev
-Requires-Dist: pytest==8.2.1; extra == "dev"
-Requires-Dist: twine==5.1.0; extra == "dev"
 
 # wavey
 Wavey is a simple implementation of the Google TiDE model in the pytorch framework.  TiDE takes in both categorical
 and continuous variables as well as a weight factor to help with time series models that depend on some weight for 
 their ultimate scoring outcome.  
 
 ## InPuts
 data: a pandas dataframe
 embedding_dims: the size/dimensions of the embedding layer (usually the square root of the number of unique values
 target_size: # of months to forecast out
 test_size: % of data to test model on
 random_state: integer for reproducibility 
 
 
+
+
```

### Comparing `waveymcwaveface-1.1/README.md` & `WaveyMcWaveFace-1.3/README.md`

 * *Files identical despite different names*

### Comparing `waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/PKG-INFO` & `WaveyMcWaveFace-1.3/WaveyMcWaveFace.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: WaveyMcWaveFace
-Version: 1.1
-Summary: A quick way to run Google's TiDE model
+Version: 1.3
+Summary: A quick way to run Google's WaveyMcWaveFace model
 Home-page: https://github.com/AmwayCommon/wavey
 Author: Jordan Howell
 Author-email: jordan.howell@amway.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: pandas-profiling
-Requires-Dist: pandocfilters
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: torch
 Provides-Extra: dev
-Requires-Dist: pytest==8.2.1; extra == "dev"
-Requires-Dist: twine==5.1.0; extra == "dev"
 
 # wavey
 Wavey is a simple implementation of the Google TiDE model in the pytorch framework.  TiDE takes in both categorical
 and continuous variables as well as a weight factor to help with time series models that depend on some weight for 
 their ultimate scoring outcome.  
 
 ## InPuts
 data: a pandas dataframe
 embedding_dims: the size/dimensions of the embedding layer (usually the square root of the number of unique values
 target_size: # of months to forecast out
 test_size: % of data to test model on
 random_state: integer for reproducibility 
 
 
+
+
```

### Comparing `waveymcwaveface-1.1/TiDE/utils/tide.py` & `WaveyMcWaveFace-1.3/WaveyMcWaveFace/utils/tide.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         embeddings = []
         for i, emb in enumerate(self.embeddings):
             indices = x[:, i].long()
             embeddings.append(emb(indices))
         return embeddings
 
 
-# TiDE class for preprocessing data and training the model
+# WaveyMcWaveFace class for preprocessing data and training the model
 class TiDE:
     def __init__(self, data, embedding_dims, target_size, test_size=0.2, random_state=42):
         self.label_encoders = {}
         self.target_size = target_size  # Add this line to save target_size as an attribute
         self.embedding_dims = embedding_dims
         self.train_prices = None  # Initialize train_prices
         self.val_prices = None  # Initialize val_prices
```

### Comparing `waveymcwaveface-1.1/setup.py` & `WaveyMcWaveFace-1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
+packages = find_packages()
+print(f"Packages found: {packages}")
+
 setup(
     name="WaveyMcWaveFace",
-    version="1.1",
-    description="A quick way to run Google's TiDE model",
-    package_dir={"": "TiDE"},
-    packages=find_packages(where="TiDE"),
+    version="1.3",
+    license='MIT',
+    description="A quick way to run Google's WaveyMcWaveFace model",
+    package_dir={'WaveyMcWaveFace': 'WaveyMcWaveFace'},
+    packages=packages,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/AmwayCommon/wavey",
     author="Jordan Howell",
     author_email="jordan.howell@amway.com",
-    license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     install_requires=['pandas',
                       'pandas-profiling',
                       'pandocfilters',
                       'numpy',
                       'scikit-learn',
                       'torch'],
     extras_require={"dev": ["pytest==8.2.1", "twine==5.1.0"]},
     python_requires=">=3.10"
-)
+    )
```

