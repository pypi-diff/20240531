# Comparing `tmp/unzipwalk-1.0.0.tar.gz` & `tmp/unzipwalk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unzipwalk-1.0.0.tar", last modified: Wed May 22 19:15:15 2024, max compression
+gzip compressed data, was "unzipwalk-1.1.0.tar", last modified: Fri May 31 14:20:01 2024, max compression
```

## Comparing `unzipwalk-1.0.0.tar` & `unzipwalk-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-22 19:15:15.904876 unzipwalk-1.0.0/
--rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.0.0/LICENSE.txt
--rw-r--r--   0 haukex    (1000) haukex    (1000)     8394 2024-05-22 19:15:15.892876 unzipwalk-1.0.0/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)     7264 2024-05-22 19:09:17.000000 unzipwalk-1.0.0/README.md
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    10103 2024-05-22 19:13:35.000000 unzipwalk-1.0.0/pyproject.toml
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.0.0/requirements.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-05-22 19:15:15.904876 unzipwalk-1.0.0/setup.cfg
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-22 19:15:15.884876 unzipwalk-1.0.0/tests/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)     9615 2024-05-22 19:08:06.000000 unzipwalk-1.0.0/tests/test_unzipwalk.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-22 19:15:15.884876 unzipwalk-1.0.0/unzipwalk/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    12597 2024-05-22 19:08:06.000000 unzipwalk-1.0.0/unzipwalk/__init__.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-22 19:15:15.892876 unzipwalk-1.0.0/unzipwalk.egg-info/
--rw-r--r--   0 haukex    (1000) haukex    (1000)     8394 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/SOURCES.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/dependency_links.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/entry_points.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/requires.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-05-22 19:15:15.000000 unzipwalk-1.0.0/unzipwalk.egg-info/top_level.txt
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.1.0/LICENSE.txt
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    11158 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    10028 2024-05-31 14:16:42.000000 unzipwalk-1.1.0/README.md
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    10103 2024-05-31 13:57:01.000000 unzipwalk-1.1.0/pyproject.toml
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.1.0/requirements.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-05-31 14:20:01.864900 unzipwalk-1.1.0/setup.cfg
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.844900 unzipwalk-1.1.0/tests/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    11245 2024-05-31 13:26:56.000000 unzipwalk-1.1.0/tests/test_unzipwalk.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.844900 unzipwalk-1.1.0/unzipwalk/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    17620 2024-05-31 14:13:44.000000 unzipwalk-1.1.0/unzipwalk/__init__.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/unzipwalk.egg-info/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    11158 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/entry_points.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/requires.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/top_level.txt
```

### Comparing `unzipwalk-1.0.0/LICENSE.txt` & `unzipwalk-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unzipwalk-1.0.0/PKG-INFO` & `unzipwalk-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unzipwalk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Recursively walk into directories and archives
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Repository, https://github.com/haukex/unzipwalk
 Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,30 +30,60 @@
 
 This module primarily provides the function [`unzipwalk()`](#function-unzipwalk), which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
 Currently supported are ZIP, tar, tgz, and gz compressed files.
 File types are detected based on their extensions.
 
+```pycon
+>>> from unzipwalk import unzipwalk
+>>> results = []
+>>> for result in unzipwalk('.'):
+...     names = tuple( name.as_posix() for name in result.names )
+...     if result.hnd:  # result is a file opened for reading (binary)
+...         # could use result.hnd.read() here, or for line-by-line:
+...         for line in result.hnd:
+...             pass  # do something interesting with the data here
+...     results.append(names + (result.typ.name,))
+>>> print(sorted(results))
+[('bar.zip', 'ARCHIVE'),
+ ('bar.zip', 'bar.txt', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'hello.csv', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'test', 'DIR'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt', 'FILE'),
+ ('foo.txt', 'FILE')]
+```
+
+**Note** that [`unzipwalk()`](#function-unzipwalk) automatically closes files as it goes from file to file.
+This means that you must use the handles as soon as you get them from the generator -
+something as seemingly simple as `sorted(unzipwalk('.'))` would cause the code above to fail,
+because all files will have been opened and closed during the call to [`sorted()`](https://docs.python.org/3/library/functions.html#sorted)
+and the handles to read the data would no longer be available in the body of the loop.
+This is why the above example first processes all the files before sorting the results.
+You can also use [`recursive_open()`](#unzipwalk.recursive_open) to open the files later.
+
 The yielded file handles can be wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper) to read them as text files.
 For example, to read all CSV files in the current directory and below, including within compressed files:
 
 ```pycon
 >>> from unzipwalk import unzipwalk, FileType
 >>> from io import TextIOWrapper
 >>> import csv
 >>> for result in unzipwalk('.'):
-...     if result.typ==FileType.FILE and result.names[-1].suffix.lower() == '.csv':
-...         print(repr(result.names))
+...     if result.typ==FileType.FILE and result.names[-1].suffix.lower()=='.csv':
+...         print([ name.as_posix() for name in result.names ])
 ...         with TextIOWrapper(result.hnd, encoding='UTF-8', newline='') as handle:
 ...             csv_rd = csv.reader(handle, strict=True)
 ...             for row in csv_rd:
-...                 print(repr(row))               
-(...)
-[...]
+...                 print(repr(row))
+['bar.zip', 'test.tar.gz', 'hello.csv']
+['Id', 'Name', 'Address']
+['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
 ### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
@@ -138,14 +168,34 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
+
+This context manager allows opening files nested inside archives directly.
+
+[`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
+this function exists to allow you to open the returned files after the iteration.
+
+If *any* of `encoding`, `errors`, or `newline` is specified, the returned
+file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
+
+If the last file in the list of files is an archive file, then it won’t be decompressed,
+instead you’ll be able to read the archive’s raw compressed data from the handle.
+
+```pycon
+>>> from unzipwalk import recursive_open
+>>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
+...     print(fh.read())
+Hi, I'm a compressed file!
+```
+
 ## Command-Line Interface
 
 ```default
 usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
 
 Recursively walk into directories and archives
```

### Comparing `unzipwalk-1.0.0/README.md` & `unzipwalk-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,60 @@
 
 This module primarily provides the function [`unzipwalk()`](#function-unzipwalk), which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
 Currently supported are ZIP, tar, tgz, and gz compressed files.
 File types are detected based on their extensions.
 
+```pycon
+>>> from unzipwalk import unzipwalk
+>>> results = []
+>>> for result in unzipwalk('.'):
+...     names = tuple( name.as_posix() for name in result.names )
+...     if result.hnd:  # result is a file opened for reading (binary)
+...         # could use result.hnd.read() here, or for line-by-line:
+...         for line in result.hnd:
+...             pass  # do something interesting with the data here
+...     results.append(names + (result.typ.name,))
+>>> print(sorted(results))
+[('bar.zip', 'ARCHIVE'),
+ ('bar.zip', 'bar.txt', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'hello.csv', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'test', 'DIR'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt', 'FILE'),
+ ('foo.txt', 'FILE')]
+```
+
+**Note** that [`unzipwalk()`](#function-unzipwalk) automatically closes files as it goes from file to file.
+This means that you must use the handles as soon as you get them from the generator -
+something as seemingly simple as `sorted(unzipwalk('.'))` would cause the code above to fail,
+because all files will have been opened and closed during the call to [`sorted()`](https://docs.python.org/3/library/functions.html#sorted)
+and the handles to read the data would no longer be available in the body of the loop.
+This is why the above example first processes all the files before sorting the results.
+You can also use [`recursive_open()`](#unzipwalk.recursive_open) to open the files later.
+
 The yielded file handles can be wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper) to read them as text files.
 For example, to read all CSV files in the current directory and below, including within compressed files:
 
 ```pycon
 >>> from unzipwalk import unzipwalk, FileType
 >>> from io import TextIOWrapper
 >>> import csv
 >>> for result in unzipwalk('.'):
-...     if result.typ==FileType.FILE and result.names[-1].suffix.lower() == '.csv':
-...         print(repr(result.names))
+...     if result.typ==FileType.FILE and result.names[-1].suffix.lower()=='.csv':
+...         print([ name.as_posix() for name in result.names ])
 ...         with TextIOWrapper(result.hnd, encoding='UTF-8', newline='') as handle:
 ...             csv_rd = csv.reader(handle, strict=True)
 ...             for row in csv_rd:
-...                 print(repr(row))               
-(...)
-[...]
+...                 print(repr(row))
+['bar.zip', 'test.tar.gz', 'hello.csv']
+['Id', 'Name', 'Address']
+['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
 ### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
@@ -112,14 +142,34 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
+
+This context manager allows opening files nested inside archives directly.
+
+[`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
+this function exists to allow you to open the returned files after the iteration.
+
+If *any* of `encoding`, `errors`, or `newline` is specified, the returned
+file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
+
+If the last file in the list of files is an archive file, then it won’t be decompressed,
+instead you’ll be able to read the archive’s raw compressed data from the handle.
+
+```pycon
+>>> from unzipwalk import recursive_open
+>>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
+...     print(fh.read())
+Hi, I'm a compressed file!
+```
+
 ## Command-Line Interface
 
 ```default
 usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
 
 Recursively walk into directories and archives
```

### Comparing `unzipwalk-1.0.0/pyproject.toml` & `unzipwalk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unzipwalk"
 description = "Recursively walk into directories and archives"
-version = "1.0.0"
+version = "1.1.0"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = ["dependencies"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `unzipwalk-1.0.0/tests/test_unzipwalk.py` & `unzipwalk-1.1.0/tests/test_unzipwalk.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import os
 import io
 import sys
 import shutil
 import hashlib
 import doctest
 import unittest
+from hashlib import sha1
 from copy import deepcopy
 from unittest.mock import patch
 from typing import Optional, cast
 from tempfile import TemporaryDirectory, TemporaryFile
 from pathlib import PurePath, Path, PurePosixPath
 from contextlib import redirect_stdout, redirect_stderr
 from unzipwalk import FileType
@@ -95,15 +96,22 @@
     ( (Path("subdir","foo.zip"),), None, FileType.ARCHIVE ),
     ( (Path("subdir","foo.zip"), PurePosixPath("foo/")), None, FileType.DIR ),
     ( (Path("subdir","foo.zip"), PurePosixPath("foo/bar.txt")),
         b"Blah\nblah\n", FileType.FILE ),
 )
 
 def load_tests(_loader, tests, _ignore):
-    tests.addTests(doctest.DocTestSuite(uut))
+    globs :dict = {}
+    def doctest_setup(_t :doctest.DocTest):
+        globs['_prev_dir'] = os.getcwd()
+        os.chdir( Path(__file__).parent/'doctest_wd' )
+    def doctest_teardown(_t :doctest.DocTest):
+        os.chdir( globs['_prev_dir'] )
+        del globs['_prev_dir']
+    tests.addTests(doctest.DocTestSuite(uut, setUp=doctest_setup, tearDown=doctest_teardown, globs=globs))
     return tests
 
 class UnzipWalkTestCase(unittest.TestCase):
 
     def setUp(self):
         self.maxDiff = None  # pylint: disable=invalid-name
         self.tempdir = TemporaryDirectory()  # pylint: disable=consider-using-with
@@ -133,14 +141,37 @@
         self.assertEqual( self.expect_all,
             sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir) ) )
 
     def test_unzipwalk_errs(self):
         with self.assertRaises(FileNotFoundError):
             list(uut.unzipwalk('/this_file_should_not_exist'))
 
+    def test_recursive_open(self):
+        for file in self.expect_all:
+            if file[2] == FileType.FILE:
+                with uut.recursive_open(file[0]) as fh:
+                    self.assertEqual( fh.read(), file[1] )
+        # text mode
+        with uut.recursive_open(("archive.tar.gz", "archive/abc.zip", "abc.txt"), encoding='UTF-8') as fh:
+            assert isinstance(fh, io.TextIOWrapper)
+            self.assertEqual( fh.readlines(), ["One two three\n", "four five six\n", "seven eight nine\n"] )
+        # open an archive
+        with uut.recursive_open(('archive.tar.gz', 'archive/abc.zip')) as fh:
+            assert isinstance(fh, uut.ReadOnlyBinary)
+            self.assertEqual( sha1(fh.read()).hexdigest(), '4d6be7a2e79c3341dd5c4fe669c0ca40a8765031' )
+        # basic error
+        with self.assertRaises(ValueError):
+            with uut.recursive_open(()): pass
+        # gzip bad filename
+        with self.assertRaises(FileNotFoundError):
+            with uut.recursive_open(("archive.tar.gz", "archive/world.txt.gz", "archive/bang.txt")): pass
+        # TarFile.extractfile: attempt to open a directory
+        with self.assertRaises(FileNotFoundError):
+            with uut.recursive_open(("archive.tar.gz", "archive/test2/")): pass
+
     def test_result_validate(self):
         with self.assertRaises(ValueError):
             uut.UnzipWalkResult((), FileType.OTHER, None).validate()
         with self.assertRaises(TypeError):
             uut.UnzipWalkResult(('foo',), FileType.OTHER, None).validate()  # type: ignore[arg-type]
         with self.assertRaises(TypeError):
             uut.UnzipWalkResult((Path(),), 'foo', None).validate()  # type: ignore[arg-type]
```

### Comparing `unzipwalk-1.0.0/unzipwalk/__init__.py` & `unzipwalk-1.1.0/unzipwalk/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,29 +4,57 @@
 
 This module primarily provides the function :func:`unzipwalk`, which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
 Currently supported are ZIP, tar, tgz, and gz compressed files.
 File types are detected based on their extensions.
 
+    >>> from unzipwalk import unzipwalk
+    >>> results = []
+    >>> for result in unzipwalk('.'):
+    ...     names = tuple( name.as_posix() for name in result.names )
+    ...     if result.hnd:  # result is a file opened for reading (binary)
+    ...         # could use result.hnd.read() here, or for line-by-line:
+    ...         for line in result.hnd:
+    ...             pass  # do something interesting with the data here
+    ...     results.append(names + (result.typ.name,))
+    >>> print(sorted(results))# doctest: +NORMALIZE_WHITESPACE
+    [('bar.zip', 'ARCHIVE'),
+     ('bar.zip', 'bar.txt', 'FILE'),
+     ('bar.zip', 'test.tar.gz', 'ARCHIVE'),
+     ('bar.zip', 'test.tar.gz', 'hello.csv', 'FILE'),
+     ('bar.zip', 'test.tar.gz', 'test', 'DIR'),
+     ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'ARCHIVE'),
+     ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt', 'FILE'),
+     ('foo.txt', 'FILE')]
+
+**Note** that :func:`unzipwalk` automatically closes files as it goes from file to file.
+This means that you must use the handles as soon as you get them from the generator -
+something as seemingly simple as ``sorted(unzipwalk('.'))`` would cause the code above to fail,
+because all files will have been opened and closed during the call to :func:`sorted`
+and the handles to read the data would no longer be available in the body of the loop.
+This is why the above example first processes all the files before sorting the results.
+You can also use :func:`recursive_open` to open the files later.
+
 The yielded file handles can be wrapped in :class:`io.TextIOWrapper` to read them as text files.
 For example, to read all CSV files in the current directory and below, including within compressed files:
 
     >>> from unzipwalk import unzipwalk, FileType
     >>> from io import TextIOWrapper
     >>> import csv
     >>> for result in unzipwalk('.'):
-    ...     if result.typ==FileType.FILE and result.names[-1].suffix.lower() == '.csv':
-    ...         print(repr(result.names))
+    ...     if result.typ==FileType.FILE and result.names[-1].suffix.lower()=='.csv':
+    ...         print([ name.as_posix() for name in result.names ])
     ...         with TextIOWrapper(result.hnd, encoding='UTF-8', newline='') as handle:
     ...             csv_rd = csv.reader(handle, strict=True)
     ...             for row in csv_rd:
-    ...                 print(repr(row))               # doctest:+ELLIPSIS
-    (...)
-    [...]
+    ...                 print(repr(row))
+    ['bar.zip', 'test.tar.gz', 'hello.csv']
+    ['Id', 'Name', 'Address']
+    ['42', 'Hello', 'World']
 
 Members
 -------
 
 .. autofunction:: unzipwalk.unzipwalk
 
 .. autoclass:: unzipwalk.UnzipWalkResult
@@ -35,14 +63,16 @@
 .. autoclass:: unzipwalk.ReadOnlyBinary
     :members:
     :undoc-members:
 
 .. autoclass:: unzipwalk.FileType
     :members:
 
+.. autofunction:: unzipwalk.recursive_open
+
 Command-Line Interface
 ----------------------
 
 .. unzipwalk_clidoc::
 
 The available checksum algorithms may vary depending on your system and Python version.
 Run the command with ``--help`` to see the list of currently available algorithms.
@@ -72,18 +102,19 @@
 import hashlib
 import argparse
 from enum import Enum
 from gzip import GzipFile
 from tarfile import TarFile
 from zipfile import ZipFile
 from itertools import chain
-from collections.abc import Generator
+from contextlib import contextmanager
+from collections.abc import Generator, Sequence
 from pathlib import PurePosixPath, PurePath, Path
-from typing import Optional, cast, Protocol, Literal, BinaryIO, NamedTuple, runtime_checkable
-from igbpyutils.file import AnyPaths, to_Paths
+from typing import Optional, cast, Protocol, Literal, BinaryIO, NamedTuple, runtime_checkable, Union
+from igbpyutils.file import AnyPaths, to_Paths, Filename
 import igbpyutils.error
 
 class FileType(Enum):
     """Used in :class:`UnzipWalkResult` to indicate the type of the file."""
     #: A regular file.
     FILE = 0
     #: An archive file, will be descended into.
@@ -141,29 +172,91 @@
             raise TypeError(f"invalid type {self.typ!r}")
         if self.typ==FileType.FILE and not isinstance(self.hnd, ReadOnlyBinary):
             raise TypeError(f"invalid handle {self.hnd!r}")
         if self.typ!=FileType.FILE and self.hnd is not None:
             raise TypeError(f"invalid handle, should be None but is {self.hnd!r}")
         return self
 
+@contextmanager
+def _inner_recur_open(fh :BinaryIO, fns :tuple[PurePath, ...]) -> Generator[BinaryIO, None, None]:
+    try:
+        bl = fns[0].name.lower()
+        assert fns
+        if len(fns)==1:
+            yield fh
+        # the following code is very similar to _proc_file, please see those code comments for details
+        elif bl.endswith('.tar.gz') or bl.endswith('.tgz') or bl.endswith('.tar'):
+            with TarFile.open(fileobj=fh) as tf:
+                ef = tf.extractfile(str(fns[1]))
+                if not ef:  # e.g. directory
+                    raise FileNotFoundError(f"not a file? {fns[0:2]}")
+                with ef as fh2:
+                    with _inner_recur_open(cast(BinaryIO, fh2), fns[1:]) as inner:
+                        yield inner
+        elif bl.endswith('.zip'):
+            with ZipFile(fh) as zf:
+                with zf.open(str(fns[1])) as fh2:
+                    with _inner_recur_open(cast(BinaryIO, fh2), fns[1:]) as inner:
+                        yield inner
+        elif bl.endswith('.gz'):
+            if fns[1] != fns[0].with_suffix(''):
+                raise FileNotFoundError(f"invalid gzip filename {fns[0]} => {fns[1]}")
+            with GzipFile(fileobj=fh, mode='rb') as fh2:
+                with _inner_recur_open(cast(BinaryIO, fh2), fns[1:]) as inner:
+                    yield inner
+        else:
+            assert False, 'should be unreachable'  # pragma: no cover
+    except GeneratorExit:  # https://pylint.readthedocs.io/en/latest/user_guide/messages/warning/contextmanager-generator-missing-cleanup.html
+        pass  # pragma: no cover
+
+@contextmanager
+def recursive_open(fns :Sequence[Filename], encoding=None, errors=None, newline=None) \
+        -> Generator[Union[ReadOnlyBinary, io.TextIOWrapper], None, None]:
+    """This context manager allows opening files nested inside archives directly.
+
+    :func:`unzipwalk` automatically closes files as it iterates through directories and archives;
+    this function exists to allow you to open the returned files after the iteration.
+
+    If *any* of ``encoding``, ``errors``, or ``newline`` is specified, the returned
+    file is wrapped in :class:`io.TextIOWrapper`!
+
+    If the last file in the list of files is an archive file, then it won't be decompressed,
+    instead you'll be able to read the archive's raw compressed data from the handle.
+
+    >>> from unzipwalk import recursive_open
+    >>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
+    ...     print(fh.read())# doctest: +NORMALIZE_WHITESPACE
+    Hi, I'm a compressed file!
+    """
+    # note Sphinx's "WARNING: py:class reference target not found: _io.TextIOWrapper" can be ignored
+    if not fns:
+        raise ValueError('no filenames given')
+    with open(fns[0], 'rb') as fh:
+        with _inner_recur_open(fh, (Path(fns[0]),) + tuple( PurePosixPath(f) for f in fns[1:] )) as inner:
+            assert inner.readable()
+            if encoding is not None or errors is not None or newline is not None:
+                yield io.TextIOWrapper(inner, encoding=encoding, errors=errors, newline=newline)
+            else:
+                yield cast(ReadOnlyBinary, inner)
+
 def _proc_file(fns :tuple[PurePath, ...], fh :BinaryIO) -> Generator[UnzipWalkResult, None, None]:
     bl = fns[-1].name.lower()
     if bl.endswith('.tar.gz') or bl.endswith('.tgz') or bl.endswith('.tar'):
         yield UnzipWalkResult(names=fns, typ=FileType.ARCHIVE)
         with TarFile.open(fileobj=fh) as tf:
             for ti in tf.getmembers():
                 new_names = (*fns, PurePosixPath(ti.name))
                 # for ti.type see e.g.: https://github.com/python/cpython/blob/v3.12.3/Lib/tarfile.py#L88
                 if ti.issym():
                     yield UnzipWalkResult(names=new_names, typ=FileType.SYMLINK)
                 elif ti.isdir():
                     yield UnzipWalkResult(names=new_names, typ=FileType.DIR)
                 elif ti.isfile():
                     # Note apparently this can burn a lot of memory on <3.13: https://github.com/python/cpython/issues/102120
-                    ef = tf.extractfile(ti)
+                    ef = tf.extractfile(ti)  # always binary
                     assert ef is not None  # make type checker happy; we know this is true because we checked it's a file
                     with ef as fh2:
                         assert fh2.readable()  # expected by ReadOnlyBinary
                         # NOTE type checker thinks fh2 is typing.IO[bytes], but it's actually a tarfile.ExFileObject,
                         # which is an io.BufferedReader subclass - which should be safe to cast to BinaryIO, I think.
                         yield from _proc_file(new_names, cast(BinaryIO, fh2))
                 else: yield UnzipWalkResult(names=new_names, typ=FileType.OTHER)
@@ -178,22 +271,22 @@
                 # e.g. from zipfile.py: z_info.external_attr = (st.st_mode & 0xFFFF) << 16
                 # we're not going to worry about other special file types in ZIP files
                 if zi.create_system==3 and stat.S_ISLNK(zi.external_attr>>16):  # 3 is UNIX
                     yield UnzipWalkResult(names=new_names, typ=FileType.SYMLINK)
                 elif zi.is_dir():
                     yield UnzipWalkResult(names=new_names, typ=FileType.DIR)
                 else:  # (note this interface doesn't have an is_file)
-                    with zf.open(zi) as fh2:
+                    with zf.open(zi) as fh2:  # always binary mode
                         assert fh2.readable()  # expected by ReadOnlyBinary
                         # NOTE type checker thinks fh2 is typing.IO[bytes], but it's actually a zipfile.ZipExtFile,
                         # which is an io.BufferedIOBase subclass - which should be safe to cast to BinaryIO, I think.
                         yield from _proc_file(new_names, cast(BinaryIO, fh2))
     elif bl.endswith('.gz'):
         yield UnzipWalkResult(names=fns, typ=FileType.ARCHIVE)
-        with GzipFile(fileobj=fh, mode='rb') as fh2:
+        with GzipFile(fileobj=fh, mode='rb') as fh2:  # always binary, but specify explicitly for clarity
             assert fh2.readable()  # expected by ReadOnlyBinary
             # NOTE casting GzipFile to BinaryIO isn't 100% safe because the former doesn't implement the full interface,
             # but testing seems to show it's ok...
             yield from _proc_file((*fns, fns[-1].with_suffix('')), cast(BinaryIO, fh2))
     else:
         assert fh.readable()  # expected by ReadOnlyBinary
         # The following cast is safe since ReadOnlyBinary is a subset of the interfaces.
```

### Comparing `unzipwalk-1.0.0/unzipwalk.egg-info/PKG-INFO` & `unzipwalk-1.1.0/unzipwalk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unzipwalk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Recursively walk into directories and archives
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Repository, https://github.com/haukex/unzipwalk
 Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,30 +30,60 @@
 
 This module primarily provides the function [`unzipwalk()`](#function-unzipwalk), which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
 Currently supported are ZIP, tar, tgz, and gz compressed files.
 File types are detected based on their extensions.
 
+```pycon
+>>> from unzipwalk import unzipwalk
+>>> results = []
+>>> for result in unzipwalk('.'):
+...     names = tuple( name.as_posix() for name in result.names )
+...     if result.hnd:  # result is a file opened for reading (binary)
+...         # could use result.hnd.read() here, or for line-by-line:
+...         for line in result.hnd:
+...             pass  # do something interesting with the data here
+...     results.append(names + (result.typ.name,))
+>>> print(sorted(results))
+[('bar.zip', 'ARCHIVE'),
+ ('bar.zip', 'bar.txt', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'hello.csv', 'FILE'),
+ ('bar.zip', 'test.tar.gz', 'test', 'DIR'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'ARCHIVE'),
+ ('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt', 'FILE'),
+ ('foo.txt', 'FILE')]
+```
+
+**Note** that [`unzipwalk()`](#function-unzipwalk) automatically closes files as it goes from file to file.
+This means that you must use the handles as soon as you get them from the generator -
+something as seemingly simple as `sorted(unzipwalk('.'))` would cause the code above to fail,
+because all files will have been opened and closed during the call to [`sorted()`](https://docs.python.org/3/library/functions.html#sorted)
+and the handles to read the data would no longer be available in the body of the loop.
+This is why the above example first processes all the files before sorting the results.
+You can also use [`recursive_open()`](#unzipwalk.recursive_open) to open the files later.
+
 The yielded file handles can be wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper) to read them as text files.
 For example, to read all CSV files in the current directory and below, including within compressed files:
 
 ```pycon
 >>> from unzipwalk import unzipwalk, FileType
 >>> from io import TextIOWrapper
 >>> import csv
 >>> for result in unzipwalk('.'):
-...     if result.typ==FileType.FILE and result.names[-1].suffix.lower() == '.csv':
-...         print(repr(result.names))
+...     if result.typ==FileType.FILE and result.names[-1].suffix.lower()=='.csv':
+...         print([ name.as_posix() for name in result.names ])
 ...         with TextIOWrapper(result.hnd, encoding='UTF-8', newline='') as handle:
 ...             csv_rd = csv.reader(handle, strict=True)
 ...             for row in csv_rd:
-...                 print(repr(row))               
-(...)
-[...]
+...                 print(repr(row))
+['bar.zip', 'test.tar.gz', 'hello.csv']
+['Id', 'Name', 'Address']
+['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
 ### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
@@ -138,14 +168,34 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
+
+This context manager allows opening files nested inside archives directly.
+
+[`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
+this function exists to allow you to open the returned files after the iteration.
+
+If *any* of `encoding`, `errors`, or `newline` is specified, the returned
+file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
+
+If the last file in the list of files is an archive file, then it won’t be decompressed,
+instead you’ll be able to read the archive’s raw compressed data from the handle.
+
+```pycon
+>>> from unzipwalk import recursive_open
+>>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
+...     print(fh.read())
+Hi, I'm a compressed file!
+```
+
 ## Command-Line Interface
 
 ```default
 usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
 
 Recursively walk into directories and archives
```

