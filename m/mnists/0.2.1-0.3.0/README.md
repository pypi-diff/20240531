# Comparing `tmp/mnists-0.2.1.tar.gz` & `tmp/mnists-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnists-0.2.1.tar", last modified: Sun May 26 14:56:50 2024, max compression
+gzip compressed data, was "mnists-0.3.0.tar", last modified: Fri May 31 08:51:59 2024, max compression
```

## Comparing `mnists-0.2.1.tar` & `mnists-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.369155 mnists-0.2.1/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1070 2024-05-26 12:44:53.000000 mnists-0.2.1/LICENSE
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2992 2024-05-26 14:56:50.368155 mnists-0.2.1/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2158 2024-05-26 12:44:53.000000 mnists-0.2.1/README.md
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.367155 mnists-0.2.1/mnists/
--rw-r--r--   0 piotr     (1000) piotr     (1000)      109 2024-05-26 14:54:28.000000 mnists-0.2.1/mnists/__init__.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     8473 2024-05-26 14:48:34.000000 mnists-0.2.1/mnists/_mnist.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2594 2024-05-26 14:46:48.000000 mnists-0.2.1/mnists/utils.py
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.368155 mnists-0.2.1/mnists.egg-info/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2992 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)      233 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/SOURCES.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/dependency_links.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)       98 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/requires.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        7 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/top_level.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)      999 2024-05-26 12:44:53.000000 mnists-0.2.1/pyproject.toml
--rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-26 14:56:50.369155 mnists-0.2.1/setup.cfg
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.939376 mnists-0.3.0/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1070 2024-05-26 12:44:53.000000 mnists-0.3.0/LICENSE
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 08:51:59.938376 mnists-0.3.0/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2302 2024-05-31 08:25:00.000000 mnists-0.3.0/README.md
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.937376 mnists-0.3.0/mnists/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       99 2024-05-31 08:50:27.000000 mnists-0.3.0/mnists/__init__.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)    11765 2024-05-30 21:02:12.000000 mnists-0.3.0/mnists/_emnist.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     7852 2024-05-30 20:50:00.000000 mnists-0.3.0/mnists/_mnist.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     5860 2024-05-30 22:29:04.000000 mnists-0.3.0/mnists/utils.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.938376 mnists-0.3.0/mnists.egg-info/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      251 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      111 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/requires.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        7 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/top_level.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1053 2024-05-30 21:43:02.000000 mnists-0.3.0/pyproject.toml
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-31 08:51:59.939376 mnists-0.3.0/setup.cfg
```

### Comparing `mnists-0.2.1/LICENSE` & `mnists-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mnists-0.2.1/PKG-INFO` & `mnists-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.2.1
+Version: 0.3.0
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,18 +14,20 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22
 Requires-Dist: numpy>=1.23.2; python_version >= "3.11"
 Requires-Dist: numpy>=1.26.0; python_version >= "3.12"
+Provides-Extra: tqdm
+Requires-Dist: tqdm; extra == "tqdm"
 
 # MNISTs: All MNIST-like datasets in one package
 
-MNISTs provides an easy way to use MNIST and other MNIST-like datasets (e.g. FashionMNIST, KMNIST) in your numpy code.
+MNISTs provides an easy way to use MNIST and other MNIST-like datasets (FashionMNIST, KMNIST, EMNIST) in your numpy code.
 
 MNISTs replicates the functionality of `torchvision.datasets.mnist` without the need to download dozens of dependencies.
 MNISTs has only one dependency - `numpy`.
 
 
 ## Usage
 
@@ -64,42 +66,45 @@
 plt.imshow(fmnist.train_images()[0], cmap='gray')
 plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
-KMNIST example:
+EMNIST example
 ```python
-from mnists import KMNIST
+from mnists import EMNIST
 import matplotlib.pyplot as plt
 
-kmnist = KMNIST()
+emnist = EMNIST()
+letters = emnist.Letters()
 plt.imshow(
-    kmnist.test_images()[:256]
+    letters.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
-![KMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/kmnist_256.png)
-
+![EMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/emnist_letters_256.png)
 
 ## Installation
 
 Install `mnists` from [PyPi](https://pypi.org/project/mnists):
 ```
 pip install mnists
 ```
 or from source:
 ```
 pip install -U git+https://github.com/pczarnik/mnists
 ```
-
 The only requirements for MNISTs are `numpy>=1.22` and `python>=3.9`.
 
+If you want to have progress bars while downloading datasets, install with
+```
+pip install mnists[tqdm]
+```
 
 ## Acknowledgments
 
 The main inspirations for MNISTs were [`mnist`](https://github.com/datapythonista/mnist) and [`torchvision.datasets.mnist`](https://github.com/pytorch/vision).
```

### Comparing `mnists-0.2.1/README.md` & `mnists-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MNISTs: All MNIST-like datasets in one package
 
-MNISTs provides an easy way to use MNIST and other MNIST-like datasets (e.g. FashionMNIST, KMNIST) in your numpy code.
+MNISTs provides an easy way to use MNIST and other MNIST-like datasets (FashionMNIST, KMNIST, EMNIST) in your numpy code.
 
 MNISTs replicates the functionality of `torchvision.datasets.mnist` without the need to download dozens of dependencies.
 MNISTs has only one dependency - `numpy`.
 
 
 ## Usage
 
@@ -43,42 +43,45 @@
 plt.imshow(fmnist.train_images()[0], cmap='gray')
 plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
-KMNIST example:
+EMNIST example
 ```python
-from mnists import KMNIST
+from mnists import EMNIST
 import matplotlib.pyplot as plt
 
-kmnist = KMNIST()
+emnist = EMNIST()
+letters = emnist.Letters()
 plt.imshow(
-    kmnist.test_images()[:256]
+    letters.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
-![KMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/kmnist_256.png)
-
+![EMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/emnist_letters_256.png)
 
 ## Installation
 
 Install `mnists` from [PyPi](https://pypi.org/project/mnists):
 ```
 pip install mnists
 ```
 or from source:
 ```
 pip install -U git+https://github.com/pczarnik/mnists
 ```
-
 The only requirements for MNISTs are `numpy>=1.22` and `python>=3.9`.
 
+If you want to have progress bars while downloading datasets, install with
+```
+pip install mnists[tqdm]
+```
 
 ## Acknowledgments
 
 The main inspirations for MNISTs were [`mnist`](https://github.com/datapythonista/mnist) and [`torchvision.datasets.mnist`](https://github.com/pytorch/vision).
```

### Comparing `mnists-0.2.1/mnists/_mnist.py` & `mnists-0.3.0/mnists/_mnist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 import tempfile
 from typing import Optional
-from urllib.error import URLError
-from urllib.parse import urljoin
-from urllib.request import urlretrieve
 
 import numpy as np
 
-from .utils import check_file_integrity, read_idx_file
+from .utils import check_file_integrity, download_file, read_idx_file
 
-TEMPORARY_DIR = tempfile.gettempdir()
+TEMPORARY_DIR = os.path.join(tempfile.gettempdir(), "mnists")
 
 
 class MNIST:
     """
     MNIST Dataset
     http://yann.lecun.com/exdb/mnist
 
@@ -68,37 +65,39 @@
         ),
         "test_labels": (
             "t10k-labels-idx1-ubyte.gz",
             "ec29112dd5afa0611ce80d1b7f02629c",
         ),
     }
 
-    default_dir = os.path.join(TEMPORARY_DIR, "mnist")
-
     def __init__(
         self,
         target_dir: Optional[str] = None,
         download: bool = True,
         force_download: bool = False,
         load: bool = True,
     ) -> None:
         """
         Parameters
         ----------
-        target_dir : str, default='/tmp/mnist/'
+        target_dir : str, default='/tmp/<dataset_name>/'
             Directory where all files exist or will be downloaded to (if `download` is True).
         download : bool, default=True
             If True and files don't exist in `target_dir`, downloads all files to `target_dir`.
         force_download : bool, default=False
             If True, downloads all files to `target_dir`, even if they exist there.
         load : bool, default=True
             If True, loads data from files in `target_dir`.
         """
 
-        self.target_dir = self.default_dir if target_dir is None else target_dir
+        self.target_dir = (
+            os.path.join(TEMPORARY_DIR, type(self).__name__)
+            if target_dir is None
+            else target_dir
+        )
 
         self._train_images: Optional[np.ndarray] = None
         self._train_labels: Optional[np.ndarray] = None
         self._test_images: Optional[np.ndarray] = None
         self._test_labels: Optional[np.ndarray] = None
 
         if download or force_download:
@@ -110,26 +109,26 @@
     def download(self, force: bool = False) -> None:
         """
         Download files from mirrors and save to `target_dir`.
 
         Parameters
         ----------
         force : bool=False
-            If True, download all files even if they exist.
+            If True, downloads all files even if they exist.
         """
 
         os.makedirs(self.target_dir, exist_ok=True)
 
         for filename, md5 in self.resources.values():
             filepath = os.path.join(self.target_dir, filename)
 
             if not force and check_file_integrity(filepath, md5):
                 continue
 
-            self._download_file(filename, filepath)
+            download_file(self.mirrors, filename, filepath)
 
     def load(self) -> None:
         """
         Load data from files in `target_dir`.
         """
 
         for key, (filename, md5) in self.resources.items():
@@ -150,27 +149,14 @@
         setattr(self, var_name, data)
 
         def getter() -> np.ndarray:
             return getattr(self, var_name)
 
         setattr(self, fn_name, getter)
 
-    def _download_file(self, filename: str, filepath: str) -> None:
-        for mirror in self.mirrors:
-            url = urljoin(mirror, filename)
-            try:
-                print(f"Downloading {url}")
-                urlretrieve(url, filepath)
-                return
-            except URLError as error:
-                print(f"Failed to download {url} (trying next mirror):\n{error}")
-                continue
-
-        raise RuntimeError(f"Error downloading {filename}")
-
 
 class FashionMNIST(MNIST):
     """
     Fashion-MNIST Dataset
     https://github.com/zalandoresearch/fashion-mnist
 
     Attributes
@@ -222,16 +208,14 @@
         ),
         "test_labels": (
             "t10k-labels-idx1-ubyte.gz",
             "bb300cfdad3c16e7a12a480ee83cd310",
         ),
     }
 
-    default_dir = os.path.join(TEMPORARY_DIR, "fmnist")
-
 
 class KMNIST(MNIST):
     """
     Kuzushiji-MNIST Dataset
     https://github.com/rois-codh/kmnist
 
     Attributes
@@ -282,9 +266,7 @@
             "5c965bf0a639b31b8f53240b1b52f4d7",
         ),
         "test_labels": (
             "t10k-labels-idx1-ubyte.gz",
             "7320c461ea6c1c855c0b718fb2a4b134",
         ),
     }
-
-    default_dir = os.path.join(TEMPORARY_DIR, "kmnist")
```

### Comparing `mnists-0.2.1/mnists.egg-info/PKG-INFO` & `mnists-0.3.0/mnists.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.2.1
+Version: 0.3.0
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,18 +14,20 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22
 Requires-Dist: numpy>=1.23.2; python_version >= "3.11"
 Requires-Dist: numpy>=1.26.0; python_version >= "3.12"
+Provides-Extra: tqdm
+Requires-Dist: tqdm; extra == "tqdm"
 
 # MNISTs: All MNIST-like datasets in one package
 
-MNISTs provides an easy way to use MNIST and other MNIST-like datasets (e.g. FashionMNIST, KMNIST) in your numpy code.
+MNISTs provides an easy way to use MNIST and other MNIST-like datasets (FashionMNIST, KMNIST, EMNIST) in your numpy code.
 
 MNISTs replicates the functionality of `torchvision.datasets.mnist` without the need to download dozens of dependencies.
 MNISTs has only one dependency - `numpy`.
 
 
 ## Usage
 
@@ -64,42 +66,45 @@
 plt.imshow(fmnist.train_images()[0], cmap='gray')
 plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
-KMNIST example:
+EMNIST example
 ```python
-from mnists import KMNIST
+from mnists import EMNIST
 import matplotlib.pyplot as plt
 
-kmnist = KMNIST()
+emnist = EMNIST()
+letters = emnist.Letters()
 plt.imshow(
-    kmnist.test_images()[:256]
+    letters.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
-![KMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/kmnist_256.png)
-
+![EMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/emnist_letters_256.png)
 
 ## Installation
 
 Install `mnists` from [PyPi](https://pypi.org/project/mnists):
 ```
 pip install mnists
 ```
 or from source:
 ```
 pip install -U git+https://github.com/pczarnik/mnists
 ```
-
 The only requirements for MNISTs are `numpy>=1.22` and `python>=3.9`.
 
+If you want to have progress bars while downloading datasets, install with
+```
+pip install mnists[tqdm]
+```
 
 ## Acknowledgments
 
 The main inspirations for MNISTs were [`mnist`](https://github.com/datapythonista/mnist) and [`torchvision.datasets.mnist`](https://github.com/pytorch/vision).
```

### Comparing `mnists-0.2.1/pyproject.toml` & `mnists-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -26,12 +26,17 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/pczarnik/mnists"
 
+[project.optional-dependencies]
+tqdm = [
+  "tqdm",
+]
+
 [tool.setuptools.dynamic]
 version = {attr = "mnists.__version__"}
 
 [tool.setuptools.packages.find]
 include = ["mnists"]
```

