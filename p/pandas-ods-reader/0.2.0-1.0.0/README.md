# Comparing `tmp/pandas_ods_reader-0.2.0.tar.gz` & `tmp/pandas_ods_reader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_ods_reader-0.2.0.tar", max compression
+gzip compressed data, was "pandas_ods_reader-1.0.0.tar", max compression
```

## Comparing `pandas_ods_reader-0.2.0.tar` & `pandas_ods_reader-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1451 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/README.md
--rw-r--r--   0        0        0      208 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/__init__.py
--rw-r--r--   0        0        0     3071 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/algo.py
--rw-r--r--   0        0        0     1515 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/main.py
--rw-r--r--   0        0        0     2354 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/fods.py
--rw-r--r--   0        0        0      993 2024-05-31 15:13:51.331055 pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/ods.py
--rw-r--r--   0        0        0      962 2024-05-31 15:13:51.331055 pandas_ods_reader-0.2.0/pandas_ods_reader/utils.py
--rw-r--r--   0        0        0     1047 2024-05-31 15:13:51.332055 pandas_ods_reader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 pandas_ods_reader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 15:13:51.330055 pandas_ods_reader-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1451 2024-05-31 15:13:51.330055 pandas_ods_reader-1.0.0/README.md
+-rw-r--r--   0        0        0      208 2024-05-31 15:13:51.330055 pandas_ods_reader-1.0.0/pandas_ods_reader/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-31 15:13:51.330055 pandas_ods_reader-1.0.0/pandas_ods_reader/algo.py
+-rw-r--r--   0        0        0     1516 2024-05-31 15:57:10.364437 pandas_ods_reader-1.0.0/pandas_ods_reader/main.py
+-rw-r--r--   0        0        0     2354 2024-05-31 15:13:51.330055 pandas_ods_reader-1.0.0/pandas_ods_reader/parsers/fods.py
+-rw-r--r--   0        0        0      993 2024-05-31 15:13:51.331055 pandas_ods_reader-1.0.0/pandas_ods_reader/parsers/ods.py
+-rw-r--r--   0        0        0      963 2024-05-31 15:57:10.365438 pandas_ods_reader-1.0.0/pandas_ods_reader/utils.py
+-rw-r--r--   0        0        0     1082 2024-05-31 15:57:13.000471 pandas_ods_reader-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 pandas_ods_reader-1.0.0/PKG-INFO
```

### Comparing `pandas_ods_reader-0.2.0/LICENSE.txt` & `pandas_ods_reader-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandas_ods_reader-0.2.0/README.md` & `pandas_ods_reader-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas_ods_reader-0.2.0/pandas_ods_reader/algo.py` & `pandas_ods_reader-1.0.0/pandas_ods_reader/algo.py`

 * *Files identical despite different names*

### Comparing `pandas_ods_reader-0.2.0/pandas_ods_reader/main.py` & `pandas_ods_reader-1.0.0/pandas_ods_reader/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Imports an ods or fods file into a DataFrame object"""
+
 from pathlib import Path
 from typing import Optional, List, Union
 
 import pandas as pd
 
 from .parsers import fods, ods
 from . import algo
```

### Comparing `pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/fods.py` & `pandas_ods_reader-1.0.0/pandas_ods_reader/parsers/fods.py`

 * *Files identical despite different names*

### Comparing `pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/ods.py` & `pandas_ods_reader-1.0.0/pandas_ods_reader/parsers/ods.py`

 * *Files identical despite different names*

### Comparing `pandas_ods_reader-0.2.0/pandas_ods_reader/utils.py` & `pandas_ods_reader-1.0.0/pandas_ods_reader/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides utility functions for the parser"""
+
 import pandas as pd
 
 
 def ods_info(doc):
     """Print the number of sheets, their names, and number of rows and columns"""
     print("Spreadsheet contains {:d} sheet(s).".format(len(doc.sheets)))
     for sheet in doc.sheets:
```

### Comparing `pandas_ods_reader-0.2.0/pyproject.toml` & `pandas_ods_reader-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "pandas-ods-reader"
-version = "0.2.0"
+version = "1.0.0"
 description = "Read in .ods and .fods files and return a pandas.DataFrame."
 authors = ["iuvbio <iuvbio@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/iuvbio/pandas_ods_reader"
-keywords = [ "data", "io", "pandas", "ods" ]
+keywords = ["data", "io", "pandas", "ods"]
 classifiers = [
-	"Development Status :: 5 - Production/Stable",
-	"License :: OSI Approved :: MIT License",
-	"Programming Language :: Python :: 3",
-	"Topic :: Utilities"
+  "Development Status :: 5 - Production/Stable",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
-ezodf = "^0.3.2"
-lxml = "^4.9.2"
-pandas = "^1.5.2"
+python = ">=3.9,<3.12"
+ezodf = ">=0.3.2"
+lxml = ">=4.9.2"
+pandas = ">=1.5.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-pytest = "^7.1.3"
-pytest-cov = "^4.0.0"
-mypy = "^0.991"
-flake8 = "^6.0.0"
-pandas-stubs = "^1.5.2.221213"
-types-lxml = "^2022.11.8"
-commitizen = "^2.38.0"
+black = ">=22.10.0"
+pytest = ">=7.1.3"
+pytest-cov = ">=4.0.0"
+mypy = ">=0.991"
+flake8 = ">=6.0.0"
+pandas-stubs = ">=1.5.2.221213"
+types-lxml = ">=2022.11.8"
+commitizen = ">=2.38.0"
+pre-commit = ">=3.7.1"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "1.0.0"
 tag_format = "v$version"
 version_files = ["pyproject.toml:version"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandas_ods_reader-0.2.0/PKG-INFO` & `pandas_ods_reader-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pandas-ods-reader
-Version: 0.2.0
+Version: 1.0.0
 Summary: Read in .ods and .fods files and return a pandas.DataFrame.
 Home-page: https://github.com/iuvbio/pandas_ods_reader
 License: MIT
 Keywords: data,io,pandas,ods
 Author: iuvbio
 Author-email: iuvbio@users.noreply.github.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: ezodf (>=0.3.2,<0.4.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: ezodf (>=0.3.2)
+Requires-Dist: lxml (>=4.9.2)
+Requires-Dist: pandas (>=1.5.2)
 Project-URL: Repository, https://github.com/iuvbio/pandas_ods_reader
 Description-Content-Type: text/markdown
 
 pandas-ods-reader
 ===
 
 Provides a function to read in a **.ods** or **.fods** file and returns a pandas DataFrame.
```

