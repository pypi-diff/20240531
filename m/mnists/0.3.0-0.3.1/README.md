# Comparing `tmp/mnists-0.3.0.tar.gz` & `tmp/mnists-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnists-0.3.0.tar", last modified: Fri May 31 08:51:59 2024, max compression
+gzip compressed data, was "mnists-0.3.1.tar", last modified: Fri May 31 15:39:18 2024, max compression
```

## Comparing `mnists-0.3.0.tar` & `mnists-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.939376 mnists-0.3.0/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1070 2024-05-26 12:44:53.000000 mnists-0.3.0/LICENSE
--rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 08:51:59.938376 mnists-0.3.0/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2302 2024-05-31 08:25:00.000000 mnists-0.3.0/README.md
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.937376 mnists-0.3.0/mnists/
--rw-r--r--   0 piotr     (1000) piotr     (1000)       99 2024-05-31 08:50:27.000000 mnists-0.3.0/mnists/__init__.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)    11765 2024-05-30 21:02:12.000000 mnists-0.3.0/mnists/_emnist.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     7852 2024-05-30 20:50:00.000000 mnists-0.3.0/mnists/_mnist.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     5860 2024-05-30 22:29:04.000000 mnists-0.3.0/mnists/utils.py
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 08:51:59.938376 mnists-0.3.0/mnists.egg-info/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)      251 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/SOURCES.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/dependency_links.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)      111 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/requires.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        7 2024-05-31 08:51:59.000000 mnists-0.3.0/mnists.egg-info/top_level.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1053 2024-05-30 21:43:02.000000 mnists-0.3.0/pyproject.toml
--rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-31 08:51:59.939376 mnists-0.3.0/setup.cfg
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 15:39:18.404904 mnists-0.3.1/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1070 2024-05-26 12:44:53.000000 mnists-0.3.1/LICENSE
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 15:39:18.403904 mnists-0.3.1/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2302 2024-05-31 08:25:00.000000 mnists-0.3.1/README.md
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 15:39:18.402904 mnists-0.3.1/mnists/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1111 2024-05-31 15:39:09.000000 mnists-0.3.1/mnists/__init__.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     8671 2024-05-31 15:29:21.000000 mnists-0.3.1/mnists/_emnist.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     5911 2024-05-31 15:29:21.000000 mnists-0.3.1/mnists/_mnist.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     8422 2024-05-31 15:29:21.000000 mnists-0.3.1/mnists/dataset.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     5860 2024-05-30 22:29:04.000000 mnists-0.3.1/mnists/utils.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-31 15:39:18.403904 mnists-0.3.1/mnists.egg-info/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3194 2024-05-31 15:39:18.000000 mnists-0.3.1/mnists.egg-info/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      269 2024-05-31 15:39:18.000000 mnists-0.3.1/mnists.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-31 15:39:18.000000 mnists-0.3.1/mnists.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      111 2024-05-31 15:39:18.000000 mnists-0.3.1/mnists.egg-info/requires.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        7 2024-05-31 15:39:18.000000 mnists-0.3.1/mnists.egg-info/top_level.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1053 2024-05-30 21:43:02.000000 mnists-0.3.1/pyproject.toml
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-31 15:39:18.404904 mnists-0.3.1/setup.cfg
```

### Comparing `mnists-0.3.0/LICENSE` & `mnists-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnists-0.3.0/PKG-INFO` & `mnists-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.3.0
+Version: 0.3.1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `mnists-0.3.0/README.md` & `mnists-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mnists-0.3.0/mnists/_mnist.py` & `mnists-0.3.1/mnists/_emnist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,272 +1,316 @@
-import os
-import tempfile
 from typing import Optional
 
-import numpy as np
+from .dataset import SplitDataset, ZippedDataset
 
-from .utils import check_file_integrity, download_file, read_idx_file
 
-TEMPORARY_DIR = os.path.join(tempfile.gettempdir(), "mnists")
-
-
-class MNIST:
+class EMNIST(SplitDataset):
     """
-    MNIST Dataset
-    http://yann.lecun.com/exdb/mnist
+    EMNIST Dataset
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
-        Numpy array representation of train/test images/labels from MNIST dataset.
-        May be None if wasn't loaded manually or during initialization.
-        If is not None, corresponding getter, e.g., _train_images -> train_images(),
-        will be available.
-    classes : list[str]
-        Class names.
-    mirrors : list[str]
-        List of urls where dataset is hosted.
-    resources : dict[str, tuple[str, str]]
-       Dictionary of data files with filename and md5 hash.
-    """
-
-    classes = [
-        "0 - zero",
-        "1 - one",
-        "2 - two",
-        "3 - three",
-        "4 - four",
-        "5 - five",
-        "6 - six",
-        "7 - seven",
-        "8 - eight",
-        "9 - nine",
-    ]
+    Balanced, ByClass, ByMerge, Digits, Letters : class
+        Child classes containing splits of EMNIST dataset.
+
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> letters = emnist.Letters()
+    >>> letters.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
 
     mirrors = [
-        "https://storage.googleapis.com/cvdf-datasets/mnist/",
-        "https://ossci-datasets.s3.amazonaws.com/mnist/",
-        "http://yann.lecun.com/exdb/mnist/",
+        "https://biometrics.nist.gov/cs_links/EMNIST/",
     ]
 
+    resources = {"gzip": ("gzip.zip", "58c8d27c78d21e728a6bc7b3cc06412e")}
+
+    def __init__(
+        self,
+        target_dir: Optional[str] = None,
+        download: bool = True,
+        force_download: bool = False,
+    ) -> None:
+        super().__init__(target_dir, download, force_download)
+
+        self.Balanced = self._create_split(Balanced)
+        self.ByClass = self._create_split(ByClass)
+        self.ByMerge = self._create_split(ByMerge)
+        self.Digits = self._create_split(Digits)
+        self.Letters = self._create_split(Letters)
+
+
+class Balanced(ZippedDataset):
+    """
+    EMNIST Balanced
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
+
+    Attributes
+    ----------
+    target_dir : str
+        Directory where all files exist or will be downloaded.
+    zip_filepath : str
+        Zip file from which dataset will be extracted.
+
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> balanced = emnist.Balanced()
+    >>> balanced.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
+
     resources = {
         "train_images": (
-            "train-images-idx3-ubyte.gz",
-            "f68b3c2dcbeaaa9fbdd348bbdeb94873",
+            "emnist-balanced-train-images-idx3-ubyte.gz",
+            "4041b0d6f15785d3fa35263901b5496b",
         ),
         "train_labels": (
-            "train-labels-idx1-ubyte.gz",
-            "d53e105ee54ea40749a09fcbcd1e9432",
+            "emnist-balanced-train-labels-idx1-ubyte.gz",
+            "7a35cc7b2b7ee7671eddf028570fbd20",
         ),
         "test_images": (
-            "t10k-images-idx3-ubyte.gz",
-            "9fb629c4189551a2d022fa330f9573f3",
+            "emnist-balanced-test-images-idx3-ubyte.gz",
+            "6818d20fe2ce1880476f747bbc80b22b",
         ),
         "test_labels": (
-            "t10k-labels-idx1-ubyte.gz",
-            "ec29112dd5afa0611ce80d1b7f02629c",
+            "emnist-balanced-test-labels-idx1-ubyte.gz",
+            "acd3694070dcbf620e36670519d4b32f",
         ),
     }
 
-    def __init__(
-        self,
-        target_dir: Optional[str] = None,
-        download: bool = True,
-        force_download: bool = False,
-        load: bool = True,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        target_dir : str, default='/tmp/<dataset_name>/'
-            Directory where all files exist or will be downloaded to (if `download` is True).
-        download : bool, default=True
-            If True and files don't exist in `target_dir`, downloads all files to `target_dir`.
-        force_download : bool, default=False
-            If True, downloads all files to `target_dir`, even if they exist there.
-        load : bool, default=True
-            If True, loads data from files in `target_dir`.
-        """
-
-        self.target_dir = (
-            os.path.join(TEMPORARY_DIR, type(self).__name__)
-            if target_dir is None
-            else target_dir
-        )
-
-        self._train_images: Optional[np.ndarray] = None
-        self._train_labels: Optional[np.ndarray] = None
-        self._test_images: Optional[np.ndarray] = None
-        self._test_labels: Optional[np.ndarray] = None
-
-        if download or force_download:
-            self.download(force_download)
-
-        if load:
-            self.load()
-
-    def download(self, force: bool = False) -> None:
-        """
-        Download files from mirrors and save to `target_dir`.
-
-        Parameters
-        ----------
-        force : bool=False
-            If True, downloads all files even if they exist.
-        """
-
-        os.makedirs(self.target_dir, exist_ok=True)
-
-        for filename, md5 in self.resources.values():
-            filepath = os.path.join(self.target_dir, filename)
-
-            if not force and check_file_integrity(filepath, md5):
-                continue
-
-            download_file(self.mirrors, filename, filepath)
-
-    def load(self) -> None:
-        """
-        Load data from files in `target_dir`.
-        """
-
-        for key, (filename, md5) in self.resources.items():
-            filepath = os.path.join(self.target_dir, filename)
-
-            if not check_file_integrity(filepath, md5):
-                raise RuntimeError(
-                    f"Dataset '{key}' not found in '{filepath}' or MD5 "
-                    "checksum is not valid. "
-                    "Use download=True or .download() to download it"
-                )
-
-            data = read_idx_file(filepath)
-            self._add_getter(key, data)
-
-    def _add_getter(self, fn_name: str, data: np.ndarray) -> None:
-        var_name = f"_{fn_name}"
-        setattr(self, var_name, data)
-
-        def getter() -> np.ndarray:
-            return getattr(self, var_name)
 
-        setattr(self, fn_name, getter)
+class ByClass(ZippedDataset):
+    """
+    EMNIST ByClass
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
+
+    Attributes
+    ----------
+    target_dir : str
+        Directory where all files exist or will be downloaded.
+    zip_filepath : str
+        Zip file from which dataset will be extracted.
+
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> byclass = emnist.ByClass()
+    >>> byclass.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
+
+    resources = {
+        "train_images": (
+            "emnist-byclass-train-images-idx3-ubyte.gz",
+            "712dda0bd6f00690f32236ae4325c377",
+        ),
+        "train_labels": (
+            "emnist-byclass-train-labels-idx1-ubyte.gz",
+            "ee299a3ee5faf5c31e9406763eae7e43",
+        ),
+        "test_images": (
+            "emnist-byclass-test-images-idx3-ubyte.gz",
+            "1435209e34070a9002867a9ab50160d7",
+        ),
+        "test_labels": (
+            "emnist-byclass-test-labels-idx1-ubyte.gz",
+            "7a0f934bd176c798ecba96b36fda6657",
+        ),
+    }
 
 
-class FashionMNIST(MNIST):
+class ByMerge(ZippedDataset):
     """
-    Fashion-MNIST Dataset
-    https://github.com/zalandoresearch/fashion-mnist
+    EMNIST ByMerge
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
-        Numpy array representation of train/test images/labels from FashionMNIST dataset.
-        May be None if wasn't loaded manually or during initialization.
-        If is not None, corresponding getter, e.g., _train_images -> train_images(),
-        will be available.
-    classes : list[str]
-        Class names.
-    mirrors : list[str]
-        List of urls where dataset is hosted.
-    resources : dict[str, tuple[str, str]]
-       Dictionary of data files with filename and md5 hash.
-    """
-
-    classes = [
-        "T-shirt/top",
-        "Trouser",
-        "Pullover",
-        "Dress",
-        "Coat",
-        "Sandal",
-        "Shirt",
-        "Sneaker",
-        "Bag",
-        "Ankle boot",
-    ]
+    zip_filepath : str
+        Zip file from which dataset will be extracted.
 
-    mirrors = [
-        "http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/",
-    ]
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> bymerge = emnist.ByMerge()
+    >>> bymerge.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
 
     resources = {
         "train_images": (
-            "train-images-idx3-ubyte.gz",
-            "8d4fb7e6c68d591d4c3dfef9ec88bf0d",
+            "emnist-bymerge-train-images-idx3-ubyte.gz",
+            "4a792d4df261d7e1ba27979573bf53f3",
         ),
         "train_labels": (
-            "train-labels-idx1-ubyte.gz",
-            "25c81989df183df01b3e8a0aad5dffbe",
+            "emnist-bymerge-train-labels-idx1-ubyte.gz",
+            "491be69ef99e1ab1f5b7f9ccc908bb26",
         ),
         "test_images": (
-            "t10k-images-idx3-ubyte.gz",
-            "bef4ecab320f06d8554ea6380940ec79",
+            "emnist-bymerge-test-images-idx3-ubyte.gz",
+            "8eb5d34c91f1759a55831c37ec2a283f",
         ),
         "test_labels": (
-            "t10k-labels-idx1-ubyte.gz",
-            "bb300cfdad3c16e7a12a480ee83cd310",
+            "emnist-bymerge-test-labels-idx1-ubyte.gz",
+            "c13f4cd5211cdba1b8fa992dae2be992",
         ),
     }
 
 
-class KMNIST(MNIST):
+class Digits(ZippedDataset):
     """
-    Kuzushiji-MNIST Dataset
-    https://github.com/rois-codh/kmnist
+    EMNIST Digits
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
-        Numpy array representation of train/test images/labels from KMNIST dataset.
-        May be None if wasn't loaded manually or during initialization.
-        If is not None, corresponding getter, e.g., _train_images -> train_images(),
-        will be available.
-    classes : list[str]
-        Class names.
-    mirrors : list[str]
-        List of urls where dataset is hosted.
-    resources : dict[str, tuple[str, str]]
-       Dictionary of data files with filename and md5 hash.
-    """
-
-    classes = [
-        "o",
-        "ki",
-        "su",
-        "tsu",
-        "na",
-        "ha",
-        "ma",
-        "ya",
-        "re",
-        "wo",
-    ]
+    zip_filepath : str
+        Zip file from which dataset will be extracted.
 
-    mirrors = [
-        "http://codh.rois.ac.jp/kmnist/dataset/kmnist/",
-    ]
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> digits = emnist.Digits()
+    >>> digits.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
+
+    resources = {
+        "train_images": (
+            "emnist-digits-train-images-idx3-ubyte.gz",
+            "d2662ecdc47895a6bbfce25de9e9a677",
+        ),
+        "train_labels": (
+            "emnist-digits-train-labels-idx1-ubyte.gz",
+            "2223fcfee618ac9c89ef20b6e48bcf9e",
+        ),
+        "test_images": (
+            "emnist-digits-test-images-idx3-ubyte.gz",
+            "a159b8b3bd6ab4ed4793c1cb71a2f5cc",
+        ),
+        "test_labels": (
+            "emnist-digits-test-labels-idx1-ubyte.gz",
+            "8afde66ea51d865689083ba6bb779fac",
+        ),
+    }
+
+
+class Letters(ZippedDataset):
+    """
+    EMNIST Letters
+    https://www.westernsydney.edu.au/bens/home/reproducible_research/emnist
+
+    Attributes
+    ----------
+    target_dir : str
+        Directory where all files exist or will be downloaded.
+    zip_filepath : str
+        Zip file from which dataset will be extracted.
+
+    Usage
+    -----
+    >>> from mnists import EMNIST
+    >>> emnist = EMNIST()
+    >>> letters = emnist.Letters()
+    >>> letters.train_images().dtype
+    dtype('uint8')
+
+    Citation
+    --------
+    @article{cohen2017emnist,
+      title={EMNIST: an extension of MNIST to handwritten letters},
+      author={Gregory Cohen and Saeed Afshar and Jonathan Tapson and André van Schaik},
+      year={2017},
+      eprint={1702.05373},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+    }
+    """
 
     resources = {
         "train_images": (
-            "train-images-idx3-ubyte.gz",
-            "bdb82020997e1d708af4cf47b453dcf7",
+            "emnist-letters-train-images-idx3-ubyte.gz",
+            "8795078f199c478165fe18db82625747",
         ),
         "train_labels": (
-            "train-labels-idx1-ubyte.gz",
-            "e144d726b3acfaa3e44228e80efcd344",
+            "emnist-letters-train-labels-idx1-ubyte.gz",
+            "c16de4f1848ddcdddd39ab65d2a7be52",
         ),
         "test_images": (
-            "t10k-images-idx3-ubyte.gz",
-            "5c965bf0a639b31b8f53240b1b52f4d7",
+            "emnist-letters-test-images-idx3-ubyte.gz",
+            "382093a19703f68edac6d01b8dfdfcad",
         ),
         "test_labels": (
-            "t10k-labels-idx1-ubyte.gz",
-            "7320c461ea6c1c855c0b718fb2a4b134",
+            "emnist-letters-test-labels-idx1-ubyte.gz",
+            "d4108920cd86601ec7689a97f2de7f59",
         ),
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mnists-0.3.0/mnists/utils.py` & `mnists-0.3.1/mnists/utils.py`

 * *Files identical despite different names*

### Comparing `mnists-0.3.0/mnists.egg-info/PKG-INFO` & `mnists-0.3.1/mnists.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.3.0
+Version: 0.3.1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `mnists-0.3.0/pyproject.toml` & `mnists-0.3.1/pyproject.toml`

 * *Files identical despite different names*

