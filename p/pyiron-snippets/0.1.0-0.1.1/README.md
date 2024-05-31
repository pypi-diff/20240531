# Comparing `tmp/pyiron_snippets-0.1.0.tar.gz` & `tmp/pyiron_snippets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_snippets-0.1.0.tar", last modified: Tue May 28 21:42:25 2024, max compression
+gzip compressed data, was "pyiron_snippets-0.1.1.tar", last modified: Fri May 31 18:09:46 2024, max compression
```

## Comparing `pyiron_snippets-0.1.0.tar` & `pyiron_snippets-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:25.963005 pyiron_snippets-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-28 21:42:25.963005 pyiron_snippets-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:25.959005 pyiron_snippets-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:25.959005 pyiron_snippets-0.1.0/pyiron_snippets/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-28 21:42:25.963005 pyiron_snippets-0.1.0/pyiron_snippets/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/import_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/pyiron_snippets/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:25.963005 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-28 21:42:25.000000 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-28 21:42:25.000000 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:42:25.000000 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 21:42:25.000000 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 21:42:25.000000 pyiron_snippets-0.1.0/pyiron_snippets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-28 21:42:24.000000 pyiron_snippets-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:42:25.963005 pyiron_snippets-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 21:41:50.000000 pyiron_snippets-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:09:46.026802 pyiron_snippets-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/pyiron_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/pyiron_snippets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/import_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/pyiron_snippets/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-31 18:09:46.000000 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 18:09:46.000000 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:09:46.000000 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 18:09:46.000000 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:09:46.000000 pyiron_snippets-0.1.1/pyiron_snippets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-31 18:09:44.000000 pyiron_snippets-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:09:46.030802 pyiron_snippets-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 18:09:09.000000 pyiron_snippets-0.1.1/setup.py
```

### Comparing `pyiron_snippets-0.1.0/LICENSE` & `pyiron_snippets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/PKG-INFO` & `pyiron_snippets-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_snippets
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyiron_snippets - Short, dependency-free python snippets.
 Author-email: Liam Huber <liamhuber@greyhavensolutions.com>, Sam Waseda <o.waseda@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Max-Planck-Institut für Nachhaltige Materialien GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -53,14 +53,20 @@
 Requires-Dist: cloudpickle==3.0.0; extra == "tests"
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pyiron_snippets/HEAD)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pyiron_snippets/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pyiron_snippets?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/pyiron-snippets/badge/?version=latest)](https://pyiron-snippets.readthedocs.io/en/latest/?badge=latest)
 
+[![Anaconda](https://anaconda.org/conda-forge/pyiron_snippets/badges/version.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Last Updated](https://anaconda.org/conda-forge/pyiron_snippets/badges/latest_release_date.svg
+)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Platform](https://anaconda.org/conda-forge/pyiron_snippets/badges/platforms.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Downloads](https://anaconda.org/conda-forge/pyiron_snippets/badges/downloads.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+
 # pyiron_snippets
 
 This is a collection of independent python snippets which we in the pyiron project find generically useful.
 
 To qualify for inclusion, a snippet must not have any dependencies outside the python standard library, and should fit reasonably inside a single file.
 
 (Note that the _tests_ may have non-standard dependencies, e.g. to ensure the snippets work in various edge cases we care about, but the actual snippets themselves must be able to behave well in a clean environment.)
```

### Comparing `pyiron_snippets-0.1.0/docs/README.md` & `pyiron_snippets-0.1.1/docs/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pyiron_snippets/HEAD)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pyiron_snippets/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pyiron_snippets?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/pyiron-snippets/badge/?version=latest)](https://pyiron-snippets.readthedocs.io/en/latest/?badge=latest)
 
+[![Anaconda](https://anaconda.org/conda-forge/pyiron_snippets/badges/version.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Last Updated](https://anaconda.org/conda-forge/pyiron_snippets/badges/latest_release_date.svg
+)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Platform](https://anaconda.org/conda-forge/pyiron_snippets/badges/platforms.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Downloads](https://anaconda.org/conda-forge/pyiron_snippets/badges/downloads.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+
 # pyiron_snippets
 
 This is a collection of independent python snippets which we in the pyiron project find generically useful.
 
 To qualify for inclusion, a snippet must not have any dependencies outside the python standard library, and should fit reasonably inside a single file.
 
 (Note that the _tests_ may have non-standard dependencies, e.g. to ensure the snippets work in various edge cases we care about, but the actual snippets themselves must be able to behave well in a clean environment.)
```

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/colors.py` & `pyiron_snippets-0.1.1/pyiron_snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/deprecate.py` & `pyiron_snippets-0.1.1/pyiron_snippets/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/dotdict.py` & `pyiron_snippets-0.1.1/pyiron_snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/factory.py` & `pyiron_snippets-0.1.1/pyiron_snippets/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/files.py` & `pyiron_snippets-0.1.1/pyiron_snippets/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from pathlib import Path
 import shutil
 
 
 def delete_files_and_directories_recursively(path):
     if not path.exists():
         return
```

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/has_post.py` & `pyiron_snippets-0.1.1/pyiron_snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/import_alarm.py` & `pyiron_snippets-0.1.1/pyiron_snippets/import_alarm.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/logger.py` & `pyiron_snippets-0.1.1/pyiron_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/retry.py` & `pyiron_snippets-0.1.1/pyiron_snippets/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 
 """
 
+from __future__ import annotations
+
 from itertools import count
 import time
 from typing import Callable, Optional, Type, TypeVar, Tuple, Union
 import warnings
 
 T = TypeVar("T")
```

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets/singleton.py` & `pyiron_snippets-0.1.1/pyiron_snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets.egg-info/PKG-INFO` & `pyiron_snippets-0.1.1/pyiron_snippets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_snippets
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyiron_snippets - Short, dependency-free python snippets.
 Author-email: Liam Huber <liamhuber@greyhavensolutions.com>, Sam Waseda <o.waseda@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Max-Planck-Institut für Nachhaltige Materialien GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -53,14 +53,20 @@
 Requires-Dist: cloudpickle==3.0.0; extra == "tests"
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pyiron_snippets/HEAD)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pyiron_snippets/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pyiron_snippets?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/pyiron-snippets/badge/?version=latest)](https://pyiron-snippets.readthedocs.io/en/latest/?badge=latest)
 
+[![Anaconda](https://anaconda.org/conda-forge/pyiron_snippets/badges/version.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Last Updated](https://anaconda.org/conda-forge/pyiron_snippets/badges/latest_release_date.svg
+)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Platform](https://anaconda.org/conda-forge/pyiron_snippets/badges/platforms.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+[![Downloads](https://anaconda.org/conda-forge/pyiron_snippets/badges/downloads.svg)](https://anaconda.org/conda-forge/pyiron_snippets)
+
 # pyiron_snippets
 
 This is a collection of independent python snippets which we in the pyiron project find generically useful.
 
 To qualify for inclusion, a snippet must not have any dependencies outside the python standard library, and should fit reasonably inside a single file.
 
 (Note that the _tests_ may have non-standard dependencies, e.g. to ensure the snippets work in various edge cases we care about, but the actual snippets themselves must be able to behave well in a clean environment.)
```

### Comparing `pyiron_snippets-0.1.0/pyiron_snippets.egg-info/SOURCES.txt` & `pyiron_snippets-0.1.1/pyiron_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_snippets-0.1.0/pyproject.toml` & `pyiron_snippets-0.1.1/pyproject.toml`

 * *Files identical despite different names*

