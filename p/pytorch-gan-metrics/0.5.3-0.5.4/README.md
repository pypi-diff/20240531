# Comparing `tmp/pytorch_gan_metrics-0.5.3.tar.gz` & `tmp/pytorch_gan_metrics-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_gan_metrics-0.5.3.tar", last modified: Fri Sep  8 04:27:45 2023, max compression
+gzip compressed data, was "pytorch_gan_metrics-0.5.4.tar", last modified: Fri May 31 11:56:27 2024, max compression
```

## Comparing `pytorch_gan_metrics-0.5.3.tar` & `pytorch_gan_metrics-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,12 @@
-drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2023-09-08 04:27:45.724040 pytorch_gan_metrics-0.5.3/
--rw-r--r--   0 yilun     (2003) yilun     (2003)    11357 2022-10-05 06:22:25.000000 pytorch_gan_metrics-0.5.3/LICENSE
--rw-rw-r--   0 yilun     (2003) yilun     (2003)     7295 2023-09-08 04:27:45.716040 pytorch_gan_metrics-0.5.3/PKG-INFO
--rw-r--r--   0 yilun     (2003) yilun     (2003)     6708 2022-11-09 15:42:08.000000 pytorch_gan_metrics-0.5.3/README.md
-drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2023-09-08 04:27:45.520037 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/
--rw-r--r--   0 yilun     (2003) yilun     (2003)      542 2022-10-05 06:22:26.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/__init__.py
--rw-r--r--   0 yilun     (2003) yilun     (2003)     1237 2022-11-09 13:53:07.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/calc_fid_stats.py
--rw-r--r--   0 yilun     (2003) yilun     (2003)     1250 2022-10-05 06:22:26.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/calc_metrics.py
--rw-r--r--   0 yilun     (2003) yilun     (2003)     9953 2022-11-09 15:36:37.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/core.py
--rw-r--r--   0 yilun     (2003) yilun     (2003)    13147 2023-09-07 16:16:17.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/inception.py
--rw-r--r--   0 yilun     (2003) yilun     (2003)     9809 2023-09-07 02:27:24.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/utils.py
--rw-rw-r--   0 yilun     (2003) yilun     (2003)       74 2023-09-07 02:12:33.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics/version.py
-drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2023-09-08 04:27:45.656039 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/
--rw-r--r--   0 yilun     (2003) yilun     (2003)     7295 2023-09-08 04:27:45.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/PKG-INFO
--rw-r--r--   0 yilun     (2003) yilun     (2003)      481 2023-09-08 04:27:45.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 yilun     (2003) yilun     (2003)        1 2023-09-08 04:27:45.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 yilun     (2003) yilun     (2003)       53 2023-09-08 04:27:45.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/requires.txt
--rw-r--r--   0 yilun     (2003) yilun     (2003)       20 2023-09-08 04:27:45.000000 pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/top_level.txt
--rw-rw-r--   0 yilun     (2003) yilun     (2003)       38 2023-09-08 04:27:45.732041 pytorch_gan_metrics-0.5.3/setup.cfg
--rw-r--r--   0 yilun     (2003) yilun     (2003)     1441 2023-09-08 02:54:40.000000 pytorch_gan_metrics-0.5.3/setup.py
-drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2023-09-08 04:27:45.684039 pytorch_gan_metrics-0.5.3/tests/
--rw-r--r--   0 yilun     (2003) yilun     (2003)    10191 2023-09-08 03:05:21.000000 pytorch_gan_metrics-0.5.3/tests/test.py
+drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2024-05-31 11:56:26.990612 pytorch_gan_metrics-0.5.4/
+-rw-r--r--   0 yilun     (2003) yilun     (2003)    11357 2022-10-05 06:22:25.000000 pytorch_gan_metrics-0.5.4/LICENSE
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)     7504 2024-05-31 11:56:26.990612 pytorch_gan_metrics-0.5.4/PKG-INFO
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)     6904 2024-05-31 11:46:43.000000 pytorch_gan_metrics-0.5.4/README.md
+drwxrwxr-x   0 yilun     (2003) yilun     (2003)        0 2024-05-31 11:56:26.982612 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)     7504 2024-05-31 11:56:26.000000 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)      240 2024-05-31 11:56:26.000000 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)        1 2024-05-31 11:56:26.000000 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)       33 2024-05-31 11:56:26.000000 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/requires.txt
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)        1 2024-05-31 11:56:26.000000 pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)       38 2024-05-31 11:56:26.994612 pytorch_gan_metrics-0.5.4/setup.cfg
+-rw-rw-r--   0 yilun     (2003) yilun     (2003)     1298 2024-05-31 11:46:43.000000 pytorch_gan_metrics-0.5.4/setup.py
```

### Comparing `pytorch_gan_metrics-0.5.3/LICENSE` & `pytorch_gan_metrics-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_gan_metrics-0.5.3/PKG-INFO` & `pytorch_gan_metrics-0.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pytorch_gan_metrics
-Version: 0.5.3
+Version: 0.5.4
 Summary: Package for calculating GAN metrics using Pytorch
-Home-page: https://github.com/w86763777/pytorch-gan-metrics
+Home-page: https://github.com/w86763777/pytorch-image-generation-metrics
 Author: Yi-Lun Wu
 Author-email: w86763777@gmail.com
 License: UNKNOWN
 Keywords: PyTorch,GAN,Inception Score,IS,Frechet Inception Distance,FID
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+### *This project has been renamed to pytorch-image-generation-metrics. Please visit the new repository [here](https://github.com/w86763777/pytorch-image-generation-metrics).*
+
 # Pytorch Implementation of Common GAN metrics
 
 ![PyPI](https://img.shields.io/pypi/v/pytorch-gan-metrics)
 
 ## Install
 ```
 pip install pytorch-gan-metrics
@@ -50,16 +53,16 @@
 - Support computation on GPU to speed up some cpu operations such as `np.cov` and `scipy.linalg.sqrtm`.
 
 ## Reproducing Results of Official Implementations on CIFAR-10
 
 |                   |Train IS  |Test IS   |Train(50k) vs Test(10k)<br>FID|
 |-------------------|:--------:|:--------:|:----------------------------:|
 |Official           |11.24±0.20|10.98±0.22|3.1508                        |
-|pytorch-gan-metrics|11.26±0.14|10.96±0.35|3.1518                        |
-|pytorch-gan-metrics<br>`use_torch=True`|11.26±0.15|10.96±0.19|3.1509                        |
+|pytorch-gan-metrics|11.26±0.13|10.96±0.35|3.1518                        |
+|pytorch-gan-metrics<br>`use_torch=True`<br>`torch==2.0.1`|11.26±0.15|10.95±0.16|3.1309                        |
 
 The results are slightly different from official implementations due to the framework difference between PyTorch and TensorFlow.
 
 ## Documentation
 
 ### Prepare Statistics (for FID)
 - [Download](https://drive.google.com/drive/folders/1UBdzl6GtNMwNQ5U-4ESlIer43tNjiGJC?usp=sharing) precalculated statistics or
```

### Comparing `pytorch_gan_metrics-0.5.3/README.md` & `pytorch_gan_metrics-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+### *This project has been renamed to pytorch-image-generation-metrics. Please visit the new repository [here](https://github.com/w86763777/pytorch-image-generation-metrics).*
+
 # Pytorch Implementation of Common GAN metrics
 
 ![PyPI](https://img.shields.io/pypi/v/pytorch-gan-metrics)
 
 ## Install
 ```
 pip install pytorch-gan-metrics
@@ -33,16 +36,16 @@
 - Support computation on GPU to speed up some cpu operations such as `np.cov` and `scipy.linalg.sqrtm`.
 
 ## Reproducing Results of Official Implementations on CIFAR-10
 
 |                   |Train IS  |Test IS   |Train(50k) vs Test(10k)<br>FID|
 |-------------------|:--------:|:--------:|:----------------------------:|
 |Official           |11.24±0.20|10.98±0.22|3.1508                        |
-|pytorch-gan-metrics|11.26±0.14|10.96±0.35|3.1518                        |
-|pytorch-gan-metrics<br>`use_torch=True`|11.26±0.15|10.96±0.19|3.1509                        |
+|pytorch-gan-metrics|11.26±0.13|10.96±0.35|3.1518                        |
+|pytorch-gan-metrics<br>`use_torch=True`<br>`torch==2.0.1`|11.26±0.15|10.95±0.16|3.1309                        |
 
 The results are slightly different from official implementations due to the framework difference between PyTorch and TensorFlow.
 
 ## Documentation
 
 ### Prepare Statistics (for FID)
 - [Download](https://drive.google.com/drive/folders/1UBdzl6GtNMwNQ5U-4ESlIer43tNjiGJC?usp=sharing) precalculated statistics or
```

### Comparing `pytorch_gan_metrics-0.5.3/pytorch_gan_metrics.egg-info/PKG-INFO` & `pytorch_gan_metrics-0.5.4/pytorch_gan_metrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pytorch-gan-metrics
-Version: 0.5.3
+Version: 0.5.4
 Summary: Package for calculating GAN metrics using Pytorch
-Home-page: https://github.com/w86763777/pytorch-gan-metrics
+Home-page: https://github.com/w86763777/pytorch-image-generation-metrics
 Author: Yi-Lun Wu
 Author-email: w86763777@gmail.com
 License: UNKNOWN
 Keywords: PyTorch,GAN,Inception Score,IS,Frechet Inception Distance,FID
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+### *This project has been renamed to pytorch-image-generation-metrics. Please visit the new repository [here](https://github.com/w86763777/pytorch-image-generation-metrics).*
+
 # Pytorch Implementation of Common GAN metrics
 
 ![PyPI](https://img.shields.io/pypi/v/pytorch-gan-metrics)
 
 ## Install
 ```
 pip install pytorch-gan-metrics
@@ -50,16 +53,16 @@
 - Support computation on GPU to speed up some cpu operations such as `np.cov` and `scipy.linalg.sqrtm`.
 
 ## Reproducing Results of Official Implementations on CIFAR-10
 
 |                   |Train IS  |Test IS   |Train(50k) vs Test(10k)<br>FID|
 |-------------------|:--------:|:--------:|:----------------------------:|
 |Official           |11.24±0.20|10.98±0.22|3.1508                        |
-|pytorch-gan-metrics|11.26±0.14|10.96±0.35|3.1518                        |
-|pytorch-gan-metrics<br>`use_torch=True`|11.26±0.15|10.96±0.19|3.1509                        |
+|pytorch-gan-metrics|11.26±0.13|10.96±0.35|3.1518                        |
+|pytorch-gan-metrics<br>`use_torch=True`<br>`torch==2.0.1`|11.26±0.15|10.95±0.16|3.1309                        |
 
 The results are slightly different from official implementations due to the framework difference between PyTorch and TensorFlow.
 
 ## Documentation
 
 ### Prepare Statistics (for FID)
 - [Download](https://drive.google.com/drive/folders/1UBdzl6GtNMwNQ5U-4ESlIer43tNjiGJC?usp=sharing) precalculated statistics or
```

### Comparing `pytorch_gan_metrics-0.5.3/setup.py` & `pytorch_gan_metrics-0.5.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,30 +20,25 @@
         name='pytorch_gan_metrics',
         version=__version__,    # noqa: F821
         author='Yi-Lun Wu',
         author_email='w86763777@gmail.com',
         description=('Package for calculating GAN metrics using Pytorch'),
         long_description=read('README.md'),
         long_description_content_type='text/markdown',
-        url='https://github.com/w86763777/pytorch-gan-metrics',
-        packages=setuptools.find_packages(include=['pytorch_gan_metrics']),
+        url='https://github.com/w86763777/pytorch-image-generation-metrics',
         keywords=[
             'PyTorch',
             'GAN',
             'Inception Score',
             'IS',
             'Frechet Inception Distance',
             'FID'],
         classifiers=[
             'Programming Language :: Python :: 3',
             'License :: OSI Approved :: Apache Software License',
             'Operating System :: OS Independent',
         ],
         python_requires='>=3.6',
         install_requires=[
-            "packaging",
-            "tqdm",
-            "scipy",
-            "torch>=1.8.2",
-            "torchvision>=0.9.2",
+            "pytorch-image-generation-metrics",
         ],
     )
```

