# Comparing `tmp/unicodecheck-1.2.1.tar.gz` & `tmp/unicodecheck-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodecheck-1.2.1.tar", last modified: Sat Apr 27 17:41:21 2024, max compression
+gzip compressed data, was "unicodecheck-1.2.2.tar", last modified: Fri May 31 16:26:55 2024, max compression
```

## Comparing `unicodecheck-1.2.1.tar` & `unicodecheck-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.918497 unicodecheck-1.2.1/
--rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/LICENSE
--rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-27 17:41:21.918295 unicodecheck-1.2.1/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)     2066 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/README.md
--rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/pyproject.toml
--rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-27 17:41:21.918540 unicodecheck-1.2.1/setup.cfg
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.916887 unicodecheck-1.2.1/unicodecheck/
--rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-25 03:42:37.000000 unicodecheck-1.2.1/unicodecheck/__init__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)       82 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/__main__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/args.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     9228 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/cli.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/core.py
--rw-r--r--   0 shunsuke   (501) staff       (20)        0 2024-04-25 03:41:53.000000 unicodecheck-1.2.1/unicodecheck/py.typed
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.917833 unicodecheck-1.2.1/unicodecheck.egg-info/
--rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)      384 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/SOURCES.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/dependency_links.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/entry_points.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/requires.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/top_level.txt
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-05-31 16:26:55.461442 unicodecheck-1.2.2/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/LICENSE
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3068 2024-05-31 16:26:55.461246 unicodecheck-1.2.2/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2130 2024-05-31 13:17:34.000000 unicodecheck-1.2.2/README.md
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/pyproject.toml
+-rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-05-31 16:26:55.461485 unicodecheck-1.2.2/setup.cfg
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-05-31 16:26:55.459948 unicodecheck-1.2.2/unicodecheck/
+-rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-05-31 13:11:12.000000 unicodecheck-1.2.2/unicodecheck/__init__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)       82 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/unicodecheck/__main__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/unicodecheck/args.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     9228 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/unicodecheck/cli.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/unicodecheck/core.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)        0 2024-05-31 10:32:06.000000 unicodecheck-1.2.2/unicodecheck/py.typed
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-05-31 16:26:55.460790 unicodecheck-1.2.2/unicodecheck.egg-info/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3068 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)      384 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/entry_points.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/requires.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-05-31 16:26:55.000000 unicodecheck-1.2.2/unicodecheck.egg-info/top_level.txt
```

### Comparing `unicodecheck-1.2.1/LICENSE` & `unicodecheck-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.1/PKG-INFO` & `unicodecheck-1.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.2.1
+Version: 1.2.2
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,15 +52,19 @@
 ### Synopsis
 
 The main program can be invoked either through the `unicodecheck` command or through the Python main module option `python3 -m unicodecheck`.
 
 ```txt
 usage: unicodecheck [-h] [-V] [-m {NFC,NFD,NFKC,NFKD}] [-d] [-u [NUMBER]] [-r] [-i] [-v]
                     PATH [PATH ...]
+```
+
+### Options
 
+```txt
 positional arguments:
   PATH                  describe input file or directory (pass '-' to specify stdin)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
@@ -76,15 +80,15 @@
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
 
-`convmv` command is suitable.
+The `convmv` command is a good alternative to using this application.
 
 #### NFC
 
 ```sh
 convmv -f utf8 -t utf8 --nfc -r ./
 ```
```

### Comparing `unicodecheck-1.2.1/README.md` & `unicodecheck-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 ### Synopsis
 
 The main program can be invoked either through the `unicodecheck` command or through the Python main module option `python3 -m unicodecheck`.
 
 ```txt
 usage: unicodecheck [-h] [-V] [-m {NFC,NFD,NFKC,NFKD}] [-d] [-u [NUMBER]] [-r] [-i] [-v]
                     PATH [PATH ...]
+```
+
+### Options
 
+```txt
 positional arguments:
   PATH                  describe input file or directory (pass '-' to specify stdin)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
@@ -49,15 +53,15 @@
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
 
-`convmv` command is suitable.
+The `convmv` command is a good alternative to using this application.
 
 #### NFC
 
 ```sh
 convmv -f utf8 -t utf8 --nfc -r ./
 ```
```

### Comparing `unicodecheck-1.2.1/pyproject.toml` & `unicodecheck-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.1/unicodecheck/args.py` & `unicodecheck-1.2.2/unicodecheck/args.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.1/unicodecheck/cli.py` & `unicodecheck-1.2.2/unicodecheck/cli.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.1/unicodecheck/core.py` & `unicodecheck-1.2.2/unicodecheck/core.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.1/unicodecheck.egg-info/PKG-INFO` & `unicodecheck-1.2.2/unicodecheck.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.2.1
+Version: 1.2.2
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,15 +52,19 @@
 ### Synopsis
 
 The main program can be invoked either through the `unicodecheck` command or through the Python main module option `python3 -m unicodecheck`.
 
 ```txt
 usage: unicodecheck [-h] [-V] [-m {NFC,NFD,NFKC,NFKD}] [-d] [-u [NUMBER]] [-r] [-i] [-v]
                     PATH [PATH ...]
+```
+
+### Options
 
+```txt
 positional arguments:
   PATH                  describe input file or directory (pass '-' to specify stdin)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
@@ -76,15 +80,15 @@
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
 
-`convmv` command is suitable.
+The `convmv` command is a good alternative to using this application.
 
 #### NFC
 
 ```sh
 convmv -f utf8 -t utf8 --nfc -r ./
 ```
```

