# Comparing `tmp/biobb_pytorch-4.2.0.tar.gz` & `tmp/biobb_pytorch-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pytorch-4.2.0.tar", last modified: Fri May 24 10:52:37 2024, max compression
+gzip compressed data, was "biobb_pytorch-4.2.1.tar", last modified: Fri May 31 20:53:59 2024, max compression
```

## Comparing `biobb_pytorch-4.2.0.tar` & `biobb_pytorch-4.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.247798 biobb_pytorch-4.2.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.2.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-24 10:52:37.247279 biobb_pytorch-4.2.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5926 2024-05-24 10:50:21.000000 biobb_pytorch-4.2.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.235439 biobb_pytorch-4.2.0/biobb_pytorch/
--rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-24 10:49:08.000000 biobb_pytorch-4.2.0/biobb_pytorch/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.245490 biobb_pytorch-4.2.0/biobb_pytorch/mdae/
--rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/apply_mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/common.py
--rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4791 2024-05-16 21:00:18.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/plots.py
--rw-r--r--   0 pau        (501) staff       (20)    24201 2024-05-09 09:41:52.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/train_mdae.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.246855 biobb_pytorch-4.2.0/biobb_pytorch/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.2.0/biobb_pytorch/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.238513 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-24 10:52:37.247902 biobb_pytorch-4.2.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-24 10:48:33.000000 biobb_pytorch-4.2.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 20:53:59.693415 biobb_pytorch-4.2.1/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.2.1/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-31 20:53:59.692807 biobb_pytorch-4.2.1/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5926 2024-05-31 20:51:29.000000 biobb_pytorch-4.2.1/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 20:53:59.685159 biobb_pytorch-4.2.1/biobb_pytorch/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-31 20:50:21.000000 biobb_pytorch-4.2.1/biobb_pytorch/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 20:53:59.691898 biobb_pytorch-4.2.1/biobb_pytorch/mdae/
+-rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12108 2024-05-31 20:21:43.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/apply_mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/common.py
+-rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4791 2024-05-16 21:00:18.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/plots.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    24225 2024-05-31 20:21:56.000000 biobb_pytorch-4.2.1/biobb_pytorch/mdae/train_mdae.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 20:53:59.692466 biobb_pytorch-4.2.1/biobb_pytorch/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.2.1/biobb_pytorch/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 20:53:59.687549 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-31 20:53:59.000000 biobb_pytorch-4.2.1/biobb_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-31 20:53:59.693625 biobb_pytorch-4.2.1/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-31 20:49:56.000000 biobb_pytorch-4.2.1/setup.py
```

### Comparing `biobb_pytorch-4.2.0/LICENSE` & `biobb_pytorch-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.2.0/PKG-INFO` & `biobb_pytorch-4.2.1/biobb_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_pytorch
-Version: 4.2.0
+Name: biobb-pytorch
+Version: 4.2.1
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -59,61 +59,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2024.2
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.2.0"
+        pip install "biobb_pytorch>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.2.0"
+        conda install -c bioconda "biobb_pytorch>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.2.0/README.md` & `biobb_pytorch-4.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -37,61 +37,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2024.2
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.2.0"
+        pip install "biobb_pytorch>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.2.0"
+        conda install -c bioconda "biobb_pytorch>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch/mdae/apply_mdae.py` & `biobb_pytorch-4.2.1/biobb_pytorch/mdae/apply_mdae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+
+"""Module containing the ApplyMDAE class and the command line interface."""
 import torch
 import numpy as np
 import argparse
 import time
 from typing import Optional, Tuple, Dict
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
```

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch/mdae/common.py` & `biobb_pytorch-4.2.1/biobb_pytorch/mdae/common.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch/mdae/mdae.py` & `biobb_pytorch-4.2.1/biobb_pytorch/mdae/mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch/mdae/plots.py` & `biobb_pytorch-4.2.1/biobb_pytorch/mdae/plots.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch/mdae/train_mdae.py` & `biobb_pytorch-4.2.1/biobb_pytorch/mdae/train_mdae.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 """Module containing the TrainMDAE class and the command line interface."""
 import torch
 import numpy as np
 import time
 import argparse
 from typing import Optional, List, Tuple, Dict
 from biobb_common.generic.biobb_object import BiobbObject
```

### Comparing `biobb_pytorch-4.2.0/biobb_pytorch.egg-info/PKG-INFO` & `biobb_pytorch-4.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-pytorch
-Version: 4.2.0
+Name: biobb_pytorch
+Version: 4.2.1
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -59,61 +59,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2024.2
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.2.0"
+        pip install "biobb_pytorch>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.2.0"
+        conda install -c bioconda "biobb_pytorch>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.1--pyhad2cae4_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.1--pyhad2cae4_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.2.0/setup.py` & `biobb_pytorch-4.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pytorch",
-    version="4.2.0",
+    version="4.2.1",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_pytorch is the Biobb module collection to create and train ML & DL models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pytorch",
```

