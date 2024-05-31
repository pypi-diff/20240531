# Comparing `tmp/pydnarepeatfinder-0.2.1.tar.gz` & `tmp/pydnarepeatfinder-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydnarepeatfinder-0.2.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pydnarepeatfinder-0.2.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pydnarepeatfinder-0.2.1.tar` & `pydnarepeatfinder-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.gitignore
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/LICENSE
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/README.md
--rw-r--r--   0        0        0      453 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/__init__.py
--rw-r--r--   0        0        0     2472 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/cli.py
--rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/colours.py
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/rob_error.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/sequences.py
--rw-r--r--   0        0        0     1307 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/hello.txt
--rw-r--r--   0        0        0     9545 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/repeatFinder.cpp
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/repeatFinder.h
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/tests/test.fasta
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/version.py
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/.gitignore
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/LICENSE
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/README.md
+-rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/__init__.py
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/_version.py
+-rw-r--r--   0        0        0     2837 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/cli.py
+-rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/colours.py
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/rob_error.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/dna_repeat_finder/sequences.py
+-rw-r--r--   0        0        0     1307 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     9545 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/src/repeatFinder.cpp
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/src/repeatFinder.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/tests/test.fasta
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.3/PKG-INFO
```

### Comparing `pydnarepeatfinder-0.2.1/.github/workflows/pylint.yml` & `pydnarepeatfinder-0.2.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/.github/workflows/python-package.yml` & `pydnarepeatfinder-0.2.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/.github/workflows/python-publish.yml` & `pydnarepeatfinder-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/.gitignore` & `pydnarepeatfinder-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/LICENSE` & `pydnarepeatfinder-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/dna_repeat_finder/cli.py` & `pydnarepeatfinder-0.2.3/dna_repeat_finder/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Command line invocations for find_repeats
 """
 
 import sys
 import argparse
 from PyRepeatFinder import find_repeats
 from .sequences import stream_fasta
+from ._version import __version__
 
 __author__ = 'Rob Edwards'
 
 def find_dna_repeats(seqid, dna_seq, gap_len=0, min_len=0, verbose=False):
     """
     find the repeats in a dna sequence
     """
@@ -60,14 +61,24 @@
 
 def run():
     """
     Command line run for repeat finder
     """
 
     parser = argparse.ArgumentParser(description='Calculate the repeat sequences in a DNA sequence')
-    parser.add_argument('-f', help='fasta file of DNA sequences', required=True)
-    parser.add_argument('-m', help='minimum repeat length', type=int, default=11)
-    parser.add_argument('-g', help='gap length (default=0)', type=int, default=0)
-    parser.add_argument('-v', help='verbose output', action='store_true')
+    parser.add_argument('-f', '--fasta', help='fasta file of DNA sequences')
+    parser.add_argument('-m', '--minlen', help='minimum repeat length', type=int, default=11)
+    parser.add_argument('-g', '--gaplen', help='gap length (default=0)', type=int, default=0)
+    parser.add_argument('--version', help='print the version and exit', action="store_true")
+    parser.add_argument('-v', '--verbose', help='verbose output', action='store_true')
+
     args = parser.parse_args()
 
-    repeats_in_fasta(args.f, args.g, args.m, args.v)
+    if args.version:
+        print(__version__)
+        sys.exit(0)
+
+    if not args.fasta:
+        print("Please specify at least a fasta file", file=sys.stderr)
+        sys.exit(2)
+
+    repeats_in_fasta(args.fasta, args.gaplen, args.minlen, args.verbose)
```

### Comparing `pydnarepeatfinder-0.2.1/dna_repeat_finder/colours.py` & `pydnarepeatfinder-0.2.3/dna_repeat_finder/colours.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/dna_repeat_finder/rob_error.py` & `pydnarepeatfinder-0.2.3/dna_repeat_finder/rob_error.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/dna_repeat_finder/sequences.py` & `pydnarepeatfinder-0.2.3/dna_repeat_finder/sequences.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/pyproject.toml` & `pydnarepeatfinder-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "PyDNARepeatFinder"
-version = "0.2.1"
+version = "0.2.3"
 authors = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
 maintainers = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
```

### Comparing `pydnarepeatfinder-0.2.1/src/repeatFinder.cpp` & `pydnarepeatfinder-0.2.3/src/repeatFinder.cpp`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/src/repeatFinder.h` & `pydnarepeatfinder-0.2.3/src/repeatFinder.h`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.1/PKG-INFO` & `pydnarepeatfinder-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDNARepeatFinder
-Version: 0.2.1
+Version: 0.2.3
 Summary: Rapidly identify repeats in a DNA sequence
 Author-Email: Rob Edwards <raedwards@gmail.com>
 Maintainer-Email: Rob Edwards <raedwards@gmail.com>
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

