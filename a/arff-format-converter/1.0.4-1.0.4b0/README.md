# Comparing `tmp/arff_format_converter-1.0.4.tar.gz` & `tmp/arff_format_converter-1.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arff_format_converter-1.0.4.tar", last modified: Fri May 31 18:29:26 2024, max compression
+gzip compressed data, was "arff_format_converter-1.0.4b0.tar", last modified: Tue May 28 12:15:53 2024, max compression
```

## Comparing `arff_format_converter-1.0.4.tar` & `arff_format_converter-1.0.4b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:29:26.394211 arff_format_converter-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-31 18:29:26.394211 arff_format_converter-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:29:26.394211 arff_format_converter-1.0.4/arff_format_converter/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/arff_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/texts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/arff_format_converter/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:29:26.394211 arff_format_converter-1.0.4/arff_format_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:29:26.000000 arff_format_converter-1.0.4/arff_format_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:29:26.394211 arff_format_converter-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-31 18:29:21.000000 arff_format_converter-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/arff_format_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/arff_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/texts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/setup.py
```

### Comparing `arff_format_converter-1.0.4/LICENSE` & `arff_format_converter-1.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/PKG-INFO` & `arff_format_converter-1.0.4b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arff-format-converter
-Version: 1.0.4
+Version: 1.0.4b0
 Summary: Converts ARFF files to CSV, JSON, XML, XLSX, and ORC
 Author: Shani Sinojiya
 Author-email: shanisinojiya@gmail.com
 Maintainer: Shani Sinojiya
 Maintainer-email: shanisinojiya@gmail.com
 License: MIT
 Keywords: arff,data-conversion,format-conversion,data-interchange,machine-learning,data-preprocessing,data-transformation,file-format-conversion,data-science,python-package,xml,json,csv,excel,orc,pandas,pyarrow,data-manipulation,data-export,data-import
@@ -12,28 +12,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: pandas
 Requires-Dist: pyarrow
-Requires-Dist: scipy
 
 # Convert ARFF files to different formats.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/arff-format-converter?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arff-format-converter?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/arff-format-converter?style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/arff-format-converter?style=flat-square)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya)
+<<<<<<< HEAD
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub followers](https://img.shields.io/github/followers/Shani-Sinojiya?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/Shani-Sinojiya/arff-format-converter?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
+=======
+![GitHub issues](https://img.shields.io/github/issues/Shani-Sinojiya/arff-format-converter?style=flat-square)
+>>>>>>> beta
 
 The `arff-format-converter` tool allows you to convert ARFF files to various output formats. Below are the details:
 
 ## INSTALL
 
 ```bash
 pip install arff-format-converter
```

#### html2text {}

```diff
@@ -1,43 +1,45 @@
-Metadata-Version: 2.1 Name: arff-format-converter Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: arff-format-converter Version: 1.0.4b0 Summary:
 Converts ARFF files to CSV, JSON, XML, XLSX, and ORC Author: Shani Sinojiya
 Author-email: shanisinojiya@gmail.com Maintainer: Shani Sinojiya Maintainer-
 email: shanisinojiya@gmail.com License: MIT Keywords: arff,data-
 conversion,format-conversion,data-interchange,machine-learning,data-
 preprocessing,data-transformation,file-format-conversion,data-science,python-
 package,xml,json,csv,excel,orc,pandas,pyarrow,data-manipulation,data-
 export,data-import Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: argparse Requires-Dist: pandas Requires-Dist: pyarrow Requires-
-Dist: scipy # Convert ARFF files to different formats. ![PyPI - Version](https:
-//img.shields.io/pypi/v/arff-format-converter?style=flat-square) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/arff-format-
-converter?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/
-arff-format-converter?style=flat-square) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/arff-format-converter?style=flat-square) ![GitHub
-Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya) ![GitHub pull
-requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-
+Requires-Dist: argparse Requires-Dist: pandas Requires-Dist: pyarrow # Convert
+ARFF files to different formats. ![PyPI - Version](https://img.shields.io/pypi/
+v/arff-format-converter?style=flat-square) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/arff-format-converter?style=flat-square) ![PyPI
+- License](https://img.shields.io/pypi/l/arff-format-converter?style=flat-
+square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/arff-format-
+converter?style=flat-square) ![GitHub Sponsors](https://img.shields.io/github/
+sponsors/Shani-Sinojiya) <<<<<<< HEAD ![GitHub pull requests](https://
+img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-
 converter?style=flat-square) ![GitHub last commit](https://img.shields.io/
 github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square) !
 [GitHub followers](https://img.shields.io/github/followers/Shani-
 Sinojiya?style=social) ![GitHub forks](https://img.shields.io/github/forks/
 Shani-Sinojiya/arff-format-converter?style=social) ![GitHub Repo stars](https:/
 /img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
-The `arff-format-converter` tool allows you to convert ARFF files to various
-output formats. Below are the details: ## INSTALL ```bash pip install arff-
-format-converter ``` ## SYNOPSIS ```bash arff-format-converter -f -o -fmt ```
-## EXAMPLES ```bash arff-format-converter -f data.arff -o output -fmt json
-arff-format-converter -f data.arff -o output -fmt xml arff-format-converter -
-f data.arff -o output -fmt csv arff-format-converter -f data.arff -o output -
-fmt xlsx arff-format-converter -f data.arff -o output -fmt orc ``` ## OPTIONS -
-`-f, --file` Path to the ARFF file. - `-o, --output` Path to the output folder.
-- `-fmt, --format` Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'. ##
-SUPPORTED FORMATS - **ARFF** (input) - **XML** (output) - **JSON** (output) -
-**CSV** (output) - **XLSX** (output) - **ORC** (Apache ORC format) (output) ##
-AUTHOR Written by [Shani Sinojiya](https://www.shanisinojiya.tech). ##
-REPORTING BUGS: Report bugs to [issue section](https://github.com/Shani-
-Sinojiya/arff-format-converter/issues) **_Remember to replace `"data.arff"`
-with the actual path to your ARFF file and `"output"` with the desired output
-folder. Feel free to adapt this code snippet for other formats like XML, CSV,
-XLSX, or ORC as needed! ð_** ## Buy me a coffee âï¸ If you like my work,
-feel free to support it by buying me a coffee._[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+======= ![GitHub issues](https://img.shields.io/github/issues/Shani-Sinojiya/
+arff-format-converter?style=flat-square) >>>>>>> beta The `arff-format-
+converter` tool allows you to convert ARFF files to various output formats.
+Below are the details: ## INSTALL ```bash pip install arff-format-converter ```
+## SYNOPSIS ```bash arff-format-converter -f -o -fmt ``` ## EXAMPLES ```bash
+arff-format-converter -f data.arff -o output -fmt json arff-format-converter -
+f data.arff -o output -fmt xml arff-format-converter -f data.arff -o output -
+fmt csv arff-format-converter -f data.arff -o output -fmt xlsx arff-format-
+converter -f data.arff -o output -fmt orc ``` ## OPTIONS - `-f, --file` Path to
+the ARFF file. - `-o, --output` Path to the output folder. - `-fmt, --format`
+Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'. ## SUPPORTED FORMATS -
+**ARFF** (input) - **XML** (output) - **JSON** (output) - **CSV** (output) -
+**XLSX** (output) - **ORC** (Apache ORC format) (output) ## AUTHOR Written by
+[Shani Sinojiya](https://www.shanisinojiya.tech). ## REPORTING BUGS: Report
+bugs to [issue section](https://github.com/Shani-Sinojiya/arff-format-
+converter/issues) **_Remember to replace `"data.arff"` with the actual path to
+your ARFF file and `"output"` with the desired output folder. Feel free to
+adapt this code snippet for other formats like XML, CSV, XLSX, or ORC as
+needed! ð_** ## Buy me a coffee âï¸ If you like my work, feel free to
+support it by buying me a coffee._[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `arff_format_converter-1.0.4/README.md` & `arff_format_converter-1.0.4b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Convert ARFF files to different formats.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/arff-format-converter?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arff-format-converter?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/arff-format-converter?style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/arff-format-converter?style=flat-square)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya)
+<<<<<<< HEAD
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub followers](https://img.shields.io/github/followers/Shani-Sinojiya?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/Shani-Sinojiya/arff-format-converter?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
+=======
+![GitHub issues](https://img.shields.io/github/issues/Shani-Sinojiya/arff-format-converter?style=flat-square)
+>>>>>>> beta
 
 The `arff-format-converter` tool allows you to convert ARFF files to various output formats. Below are the details:
 
 ## INSTALL
 
 ```bash
 pip install arff-format-converter
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
 # Convert ARFF files to different formats. ![PyPI - Version](https://
 img.shields.io/pypi/v/arff-format-converter?style=flat-square) ![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/arff-format-
 converter?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/
 arff-format-converter?style=flat-square) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/arff-format-converter?style=flat-square) ![GitHub
-Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya) ![GitHub pull
-requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-
-converter?style=flat-square) ![GitHub last commit](https://img.shields.io/
-github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square) !
-[GitHub followers](https://img.shields.io/github/followers/Shani-
-Sinojiya?style=social) ![GitHub forks](https://img.shields.io/github/forks/
-Shani-Sinojiya/arff-format-converter?style=social) ![GitHub Repo stars](https:/
-/img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
-The `arff-format-converter` tool allows you to convert ARFF files to various
-output formats. Below are the details: ## INSTALL ```bash pip install arff-
-format-converter ``` ## SYNOPSIS ```bash arff-format-converter -f -o -fmt ```
-## EXAMPLES ```bash arff-format-converter -f data.arff -o output -fmt json
-arff-format-converter -f data.arff -o output -fmt xml arff-format-converter -
+Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya) <<<<<<< HEAD !
+[GitHub pull requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/
+arff-format-converter?style=flat-square) ![GitHub last commit](https://
+img.shields.io/github/last-commit/Shani-Sinojiya/arff-format-
+converter?style=flat-square) ![GitHub followers](https://img.shields.io/github/
+followers/Shani-Sinojiya?style=social) ![GitHub forks](https://img.shields.io/
+github/forks/Shani-Sinojiya/arff-format-converter?style=social) ![GitHub Repo
+stars](https://img.shields.io/github/stars/Shani-Sinojiya/arff-format-
+converter?style=social) ======= ![GitHub issues](https://img.shields.io/github/
+issues/Shani-Sinojiya/arff-format-converter?style=flat-square) >>>>>>> beta The
+`arff-format-converter` tool allows you to convert ARFF files to various output
+formats. Below are the details: ## INSTALL ```bash pip install arff-format-
+converter ``` ## SYNOPSIS ```bash arff-format-converter -f -o -fmt ``` ##
+EXAMPLES ```bash arff-format-converter -f data.arff -o output -fmt json arff-
+format-converter -f data.arff -o output -fmt xml arff-format-converter -
 f data.arff -o output -fmt csv arff-format-converter -f data.arff -o output -
 fmt xlsx arff-format-converter -f data.arff -o output -fmt orc ``` ## OPTIONS -
 `-f, --file` Path to the ARFF file. - `-o, --output` Path to the output folder.
 - `-fmt, --format` Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'. ##
 SUPPORTED FORMATS - **ARFF** (input) - **XML** (output) - **JSON** (output) -
 **CSV** (output) - **XLSX** (output) - **ORC** (Apache ORC format) (output) ##
 AUTHOR Written by [Shani Sinojiya](https://www.shanisinojiya.tech). ##
```

### Comparing `arff_format_converter-1.0.4/arff_format_converter/__init__.py` & `arff_format_converter-1.0.4b0/arff_format_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/arff_format_converter/logs.py` & `arff_format_converter-1.0.4b0/arff_format_converter/logs.py`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/arff_format_converter/output.py` & `arff_format_converter-1.0.4b0/arff_format_converter/output.py`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/arff_format_converter/utils.py` & `arff_format_converter-1.0.4b0/arff_format_converter/utils.py`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/arff_format_converter/validate.py` & `arff_format_converter-1.0.4b0/arff_format_converter/validate.py`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/arff_format_converter.egg-info/PKG-INFO` & `arff_format_converter-1.0.4b0/arff_format_converter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arff-format-converter
-Version: 1.0.4
+Version: 1.0.4b0
 Summary: Converts ARFF files to CSV, JSON, XML, XLSX, and ORC
 Author: Shani Sinojiya
 Author-email: shanisinojiya@gmail.com
 Maintainer: Shani Sinojiya
 Maintainer-email: shanisinojiya@gmail.com
 License: MIT
 Keywords: arff,data-conversion,format-conversion,data-interchange,machine-learning,data-preprocessing,data-transformation,file-format-conversion,data-science,python-package,xml,json,csv,excel,orc,pandas,pyarrow,data-manipulation,data-export,data-import
@@ -12,28 +12,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: pandas
 Requires-Dist: pyarrow
-Requires-Dist: scipy
 
 # Convert ARFF files to different formats.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/arff-format-converter?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arff-format-converter?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/arff-format-converter?style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/arff-format-converter?style=flat-square)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya)
+<<<<<<< HEAD
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square)
 ![GitHub followers](https://img.shields.io/github/followers/Shani-Sinojiya?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/Shani-Sinojiya/arff-format-converter?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
+=======
+![GitHub issues](https://img.shields.io/github/issues/Shani-Sinojiya/arff-format-converter?style=flat-square)
+>>>>>>> beta
 
 The `arff-format-converter` tool allows you to convert ARFF files to various output formats. Below are the details:
 
 ## INSTALL
 
 ```bash
 pip install arff-format-converter
```

#### html2text {}

```diff
@@ -1,43 +1,45 @@
-Metadata-Version: 2.1 Name: arff-format-converter Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: arff-format-converter Version: 1.0.4b0 Summary:
 Converts ARFF files to CSV, JSON, XML, XLSX, and ORC Author: Shani Sinojiya
 Author-email: shanisinojiya@gmail.com Maintainer: Shani Sinojiya Maintainer-
 email: shanisinojiya@gmail.com License: MIT Keywords: arff,data-
 conversion,format-conversion,data-interchange,machine-learning,data-
 preprocessing,data-transformation,file-format-conversion,data-science,python-
 package,xml,json,csv,excel,orc,pandas,pyarrow,data-manipulation,data-
 export,data-import Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: argparse Requires-Dist: pandas Requires-Dist: pyarrow Requires-
-Dist: scipy # Convert ARFF files to different formats. ![PyPI - Version](https:
-//img.shields.io/pypi/v/arff-format-converter?style=flat-square) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/arff-format-
-converter?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/
-arff-format-converter?style=flat-square) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/arff-format-converter?style=flat-square) ![GitHub
-Sponsors](https://img.shields.io/github/sponsors/Shani-Sinojiya) ![GitHub pull
-requests](https://img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-
+Requires-Dist: argparse Requires-Dist: pandas Requires-Dist: pyarrow # Convert
+ARFF files to different formats. ![PyPI - Version](https://img.shields.io/pypi/
+v/arff-format-converter?style=flat-square) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/arff-format-converter?style=flat-square) ![PyPI
+- License](https://img.shields.io/pypi/l/arff-format-converter?style=flat-
+square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/arff-format-
+converter?style=flat-square) ![GitHub Sponsors](https://img.shields.io/github/
+sponsors/Shani-Sinojiya) <<<<<<< HEAD ![GitHub pull requests](https://
+img.shields.io/github/issues-pr/Shani-Sinojiya/arff-format-
 converter?style=flat-square) ![GitHub last commit](https://img.shields.io/
 github/last-commit/Shani-Sinojiya/arff-format-converter?style=flat-square) !
 [GitHub followers](https://img.shields.io/github/followers/Shani-
 Sinojiya?style=social) ![GitHub forks](https://img.shields.io/github/forks/
 Shani-Sinojiya/arff-format-converter?style=social) ![GitHub Repo stars](https:/
 /img.shields.io/github/stars/Shani-Sinojiya/arff-format-converter?style=social)
-The `arff-format-converter` tool allows you to convert ARFF files to various
-output formats. Below are the details: ## INSTALL ```bash pip install arff-
-format-converter ``` ## SYNOPSIS ```bash arff-format-converter -f -o -fmt ```
-## EXAMPLES ```bash arff-format-converter -f data.arff -o output -fmt json
-arff-format-converter -f data.arff -o output -fmt xml arff-format-converter -
-f data.arff -o output -fmt csv arff-format-converter -f data.arff -o output -
-fmt xlsx arff-format-converter -f data.arff -o output -fmt orc ``` ## OPTIONS -
-`-f, --file` Path to the ARFF file. - `-o, --output` Path to the output folder.
-- `-fmt, --format` Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'. ##
-SUPPORTED FORMATS - **ARFF** (input) - **XML** (output) - **JSON** (output) -
-**CSV** (output) - **XLSX** (output) - **ORC** (Apache ORC format) (output) ##
-AUTHOR Written by [Shani Sinojiya](https://www.shanisinojiya.tech). ##
-REPORTING BUGS: Report bugs to [issue section](https://github.com/Shani-
-Sinojiya/arff-format-converter/issues) **_Remember to replace `"data.arff"`
-with the actual path to your ARFF file and `"output"` with the desired output
-folder. Feel free to adapt this code snippet for other formats like XML, CSV,
-XLSX, or ORC as needed! ð_** ## Buy me a coffee âï¸ If you like my work,
-feel free to support it by buying me a coffee._[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+======= ![GitHub issues](https://img.shields.io/github/issues/Shani-Sinojiya/
+arff-format-converter?style=flat-square) >>>>>>> beta The `arff-format-
+converter` tool allows you to convert ARFF files to various output formats.
+Below are the details: ## INSTALL ```bash pip install arff-format-converter ```
+## SYNOPSIS ```bash arff-format-converter -f -o -fmt ``` ## EXAMPLES ```bash
+arff-format-converter -f data.arff -o output -fmt json arff-format-converter -
+f data.arff -o output -fmt xml arff-format-converter -f data.arff -o output -
+fmt csv arff-format-converter -f data.arff -o output -fmt xlsx arff-format-
+converter -f data.arff -o output -fmt orc ``` ## OPTIONS - `-f, --file` Path to
+the ARFF file. - `-o, --output` Path to the output folder. - `-fmt, --format`
+Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'. ## SUPPORTED FORMATS -
+**ARFF** (input) - **XML** (output) - **JSON** (output) - **CSV** (output) -
+**XLSX** (output) - **ORC** (Apache ORC format) (output) ## AUTHOR Written by
+[Shani Sinojiya](https://www.shanisinojiya.tech). ## REPORTING BUGS: Report
+bugs to [issue section](https://github.com/Shani-Sinojiya/arff-format-
+converter/issues) **_Remember to replace `"data.arff"` with the actual path to
+your ARFF file and `"output"` with the desired output folder. Feel free to
+adapt this code snippet for other formats like XML, CSV, XLSX, or ORC as
+needed! ð_** ## Buy me a coffee âï¸ If you like my work, feel free to
+support it by buying me a coffee._[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `arff_format_converter-1.0.4/arff_format_converter.egg-info/SOURCES.txt` & `arff_format_converter-1.0.4b0/arff_format_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arff_format_converter-1.0.4/pyproject.toml` & `arff_format_converter-1.0.4b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 [tool.poetry]
 authors = ["Shani Sinojiya <shanisinojiya@gmail.com>"]
 description = "A tool to convert ARFF files to different formats."
 license = "MIT"
 name = "arff-format-converter"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.0.4"
+version = "1.0.4b0"
 
 [tool.poetry.dependencies]
 argparse = "^1.4.0"
 pandas = "^2.2.0"
 pyarrow = "^16.0.0"
-scipy = "^1.13.0"
 
 [tool.poetry.scripts]
 arff-format-converter = "arff_format_converter.arff_converter:main"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/Shani-Sinojiya/arff-format-converter"
 Issues = "https://github.com/Shani-Sinojiya/arff-format-converter/issues"
```

### Comparing `arff_format_converter-1.0.4/setup.py` & `arff_format_converter-1.0.4b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.4'
+version = '1.0.4b0'
 name = 'arff-format-converter'
 description = 'Converts ARFF files to CSV, JSON, XML, XLSX, and ORC'
 author = 'Shani Sinojiya'
 author_email = 'shanisinojiya@gmail.com'
 
 keywords = [
     "arff",
@@ -43,16 +43,15 @@
             maintainer_email=author_email,
             license="MIT",
             long_description=long_description,
             long_description_content_type='text/markdown',
             install_requires=[
                 "argparse",
                 "pandas",
-                "pyarrow",
-                "scipy"
+                "pyarrow"
             ],
             entry_points={
                 'console_scripts': [
                     'arff-format-converter=arff_format_converter.arff_converter:main',
                 ],
             },
             keywords=keywords,
```

