# Comparing `tmp/unzipwalk-1.1.0.tar.gz` & `tmp/unzipwalk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unzipwalk-1.1.0.tar", last modified: Fri May 31 14:20:01 2024, max compression
+gzip compressed data, was "unzipwalk-1.2.0.tar", last modified: Fri May 31 18:30:15 2024, max compression
```

## Comparing `unzipwalk-1.1.0.tar` & `unzipwalk-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/
--rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.1.0/LICENSE.txt
--rw-r--r--   0 haukex    (1000) haukex    (1000)    11158 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    10028 2024-05-31 14:16:42.000000 unzipwalk-1.1.0/README.md
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    10103 2024-05-31 13:57:01.000000 unzipwalk-1.1.0/pyproject.toml
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.1.0/requirements.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-05-31 14:20:01.864900 unzipwalk-1.1.0/setup.cfg
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.844900 unzipwalk-1.1.0/tests/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    11245 2024-05-31 13:26:56.000000 unzipwalk-1.1.0/tests/test_unzipwalk.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.844900 unzipwalk-1.1.0/unzipwalk/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    17620 2024-05-31 14:13:44.000000 unzipwalk-1.1.0/unzipwalk/__init__.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 14:20:01.852900 unzipwalk-1.1.0/unzipwalk.egg-info/
--rw-r--r--   0 haukex    (1000) haukex    (1000)    11158 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/SOURCES.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/dependency_links.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/entry_points.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/requires.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-05-31 14:20:01.000000 unzipwalk-1.1.0/unzipwalk.egg-info/top_level.txt
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 18:30:15.226235 unzipwalk-1.2.0/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.2.0/LICENSE.txt
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    12362 2024-05-31 18:30:15.226235 unzipwalk-1.2.0/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    11149 2024-05-31 18:24:38.000000 unzipwalk-1.2.0/README.md
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    10178 2024-05-31 18:15:14.000000 unzipwalk-1.2.0/pyproject.toml
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.2.0/requirements.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-05-31 18:30:15.226235 unzipwalk-1.2.0/setup.cfg
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 18:30:15.218235 unzipwalk-1.2.0/tests/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    12874 2024-05-31 18:12:28.000000 unzipwalk-1.2.0/tests/test_unzipwalk.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 18:30:15.218235 unzipwalk-1.2.0/unzipwalk/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    19027 2024-05-31 18:24:30.000000 unzipwalk-1.2.0/unzipwalk/__init__.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 18:30:15.226235 unzipwalk-1.2.0/unzipwalk.egg-info/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    12362 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/entry_points.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/requires.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-05-31 18:30:15.000000 unzipwalk-1.2.0/unzipwalk.egg-info/top_level.txt
```

### Comparing `unzipwalk-1.1.0/LICENSE.txt` & `unzipwalk-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unzipwalk-1.1.0/PKG-INFO` & `unzipwalk-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: unzipwalk
-Version: 1.1.0
+Version: 1.2.0
 Summary: Recursively walk into directories and archives
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Repository, https://github.com/haukex/unzipwalk
 Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
+Project-URL: Changelog, https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -82,20 +83,22 @@
 ['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
-### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
+### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)], \*, matcher: [Callable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Callable)[[[Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath)]], [bool](https://docs.python.org/3/library/functions.html#bool)] | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
-  **paths** – A filename or iterable of filenames.
+  * **paths** – A filename or iterable of filenames.
+  * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
+    as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
@@ -168,52 +171,62 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+<a id="unzipwalk.recursive_open"></a>
+
 ### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
 
 This context manager allows opening files nested inside archives directly.
 
 [`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
 this function exists to allow you to open the returned files after the iteration.
 
 If *any* of `encoding`, `errors`, or `newline` is specified, the returned
 file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
 
 If the last file in the list of files is an archive file, then it won’t be decompressed,
 instead you’ll be able to read the archive’s raw compressed data from the handle.
 
+In this example, we open a gzip-compressed file, stored inside a tgz archive, which
+in turn is stored in a Zip file:
+
 ```pycon
 >>> from unzipwalk import recursive_open
 >>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
 ...     print(fh.read())
 Hi, I'm a compressed file!
 ```
 
 ## Command-Line Interface
 
 ```default
-usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
+usage: unzipwalk [-h] [-a] [-d | -c ALGO] [-e EXCLUDE] [PATH ...]
 
 Recursively walk into directories and archives
 
 positional arguments:
   PATH                  paths to process (default is current directory)
 
 optional arguments:
   -h, --help            show this help message and exit
   -a, --all-files       also list dirs, symlinks, etc.
   -d, --dump            also dump file contents
   -c ALGO, --checksum ALGO
-                        generate a checksum for each file
-
-Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
+                        generate a checksum for each file**
+  -e EXCLUDE, --exclude EXCLUDE
+                        filename globs to exclude*
+
+* Note --exclude currently only matches against the final name in the
+sequence, excluding path names, but this interface may change in future
+versions. For more control, use the library instead of this command-line tool.
+** Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
 sha256, sha384, sha3_224, sha3_256, sha3_384, sha3_512, sha512, sha512_224,
 sha512_256, shake_128, shake_256, sm3
 ```
 
 The available checksum algorithms may vary depending on your system and Python version.
 Run the command with `--help` to see the list of currently available algorithms.
```

### Comparing `unzipwalk-1.1.0/README.md` & `unzipwalk-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -56,20 +56,22 @@
 ['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
-### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
+### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)], \*, matcher: [Callable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Callable)[[[Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath)]], [bool](https://docs.python.org/3/library/functions.html#bool)] | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
-  **paths** – A filename or iterable of filenames.
+  * **paths** – A filename or iterable of filenames.
+  * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
+    as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
@@ -142,52 +144,62 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+<a id="unzipwalk.recursive_open"></a>
+
 ### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
 
 This context manager allows opening files nested inside archives directly.
 
 [`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
 this function exists to allow you to open the returned files after the iteration.
 
 If *any* of `encoding`, `errors`, or `newline` is specified, the returned
 file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
 
 If the last file in the list of files is an archive file, then it won’t be decompressed,
 instead you’ll be able to read the archive’s raw compressed data from the handle.
 
+In this example, we open a gzip-compressed file, stored inside a tgz archive, which
+in turn is stored in a Zip file:
+
 ```pycon
 >>> from unzipwalk import recursive_open
 >>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
 ...     print(fh.read())
 Hi, I'm a compressed file!
 ```
 
 ## Command-Line Interface
 
 ```default
-usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
+usage: unzipwalk [-h] [-a] [-d | -c ALGO] [-e EXCLUDE] [PATH ...]
 
 Recursively walk into directories and archives
 
 positional arguments:
   PATH                  paths to process (default is current directory)
 
 optional arguments:
   -h, --help            show this help message and exit
   -a, --all-files       also list dirs, symlinks, etc.
   -d, --dump            also dump file contents
   -c ALGO, --checksum ALGO
-                        generate a checksum for each file
-
-Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
+                        generate a checksum for each file**
+  -e EXCLUDE, --exclude EXCLUDE
+                        filename globs to exclude*
+
+* Note --exclude currently only matches against the final name in the
+sequence, excluding path names, but this interface may change in future
+versions. For more control, use the library instead of this command-line tool.
+** Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
 sha256, sha384, sha3_224, sha3_256, sha3_384, sha3_512, sha512, sha512_224,
 sha512_256, shake_128, shake_256, sm3
 ```
 
 The available checksum algorithms may vary depending on your system and Python version.
 Run the command with `--help` to see the list of currently available algorithms.
```

### Comparing `unzipwalk-1.1.0/pyproject.toml` & `unzipwalk-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unzipwalk"
 description = "Recursively walk into directories and archives"
-version = "1.1.0"
+version = "1.2.0"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = ["dependencies"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -36,14 +36,15 @@
 
 [project.scripts]
 unzipwalk = "unzipwalk:main"
 
 [project.urls]
 "Repository" = "https://github.com/haukex/unzipwalk"
 "Bug Tracker" = "https://github.com/haukex/unzipwalk/issues"
+"Changelog" = "https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md"
 
 
 # Individual lines can be ignored with:
 # pylance: ``# pyright: ignore [settingName]``
 # pylint:  ``# pylint: disable=setting-name``
 # flake8:  ``# noqa: CODE``
 # mypy:    ``# type: ignore[setting-name]``
```

### Comparing `unzipwalk-1.1.0/tests/test_unzipwalk.py` & `unzipwalk-1.2.0/tests/test_unzipwalk.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,14 +141,32 @@
         self.assertEqual( self.expect_all,
             sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir) ) )
 
     def test_unzipwalk_errs(self):
         with self.assertRaises(FileNotFoundError):
             list(uut.unzipwalk('/this_file_should_not_exist'))
 
+    def test_unzipwalk_matcher(self):
+        # filter from the initial path list
+        self.assertEqual( [ r for r in self.expect_all if r[0][0].name != 'more.zip' ],
+            sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir,
+                matcher=lambda p: p[0].stem.lower()!='more' ) ) )
+        # filter from zip file
+        self.assertEqual( [ r for r in self.expect_all if r[0][-1].name != 'six.txt' ],
+            sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir,
+                matcher=lambda p: p[-1].name.lower()!='six.txt' ) ) )
+        # filter a gz file
+        self.assertEqual( [ r for r in self.expect_all if not ( r[0][0].name=='archive.tar.gz' and r[0][-1].name == 'world.txt' ) ],
+            sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir,
+                matcher=lambda p: len(p)<2 or p[-2].as_posix()!='archive/world.txt.gz' ) ) )
+        # filter from tar file
+        self.assertEqual( [ r for r in self.expect_all if not ( len(r[0])>1 and r[0][1].stem=='abc' ) ],
+            sorted( (r.names, None if r.hnd is None else r.hnd.read(), r.typ) for r in uut.unzipwalk(os.curdir,
+                matcher=lambda p: p[-1].name != 'abc.zip' ) ) )
+
     def test_recursive_open(self):
         for file in self.expect_all:
             if file[2] == FileType.FILE:
                 with uut.recursive_open(file[0]) as fh:
                     self.assertEqual( fh.read(), file[1] )
         # text mode
         with uut.recursive_open(("archive.tar.gz", "archive/abc.zip", "abc.txt"), encoding='UTF-8') as fh:
@@ -208,7 +226,10 @@
         self.assertEqual( self._run_cli(['--checksum','sha256']), sorted(  # checksum
             f"{hashlib.sha256(e[1]).hexdigest()} *{str(e[0][0]) if len(e[0])==1 else repr(tuple(str(n) for n in e[0]))}"
             for e in self.expect_all if e[1] is not None ) )
         self.assertEqual( self._run_cli(['-a','-csha512']), sorted(  # checksum + all-files
             (f"# {e[2].name} " if e[1] is None else f"{hashlib.sha512(e[1]).hexdigest()} *")
             + f"{str(e[0][0]) if len(e[0])==1 else repr(tuple(str(n) for n in e[0]))}"
             for e in self.expect_all ) )
+        self.assertEqual( self._run_cli(['-e','world.*','--exclude=*abc*']), sorted(  # exclude
+            f"FILE {tuple(str(n) for n in e[0])!r}" for e in self.expect_all if e[2]==FileType.FILE
+            and not ( e[0][-1].name.startswith('world.') or len(e[0])>1 and e[0][1].name=='abc.zip' ) ) )
```

### Comparing `unzipwalk-1.1.0/unzipwalk/__init__.py` & `unzipwalk-1.2.0/unzipwalk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,17 +102,18 @@
 import hashlib
 import argparse
 from enum import Enum
 from gzip import GzipFile
 from tarfile import TarFile
 from zipfile import ZipFile
 from itertools import chain
+from fnmatch import fnmatch
 from contextlib import contextmanager
-from collections.abc import Generator, Sequence
 from pathlib import PurePosixPath, PurePath, Path
+from collections.abc import Generator, Sequence, Callable
 from typing import Optional, cast, Protocol, Literal, BinaryIO, NamedTuple, runtime_checkable, Union
 from igbpyutils.file import AnyPaths, to_Paths, Filename
 import igbpyutils.error
 
 class FileType(Enum):
     """Used in :class:`UnzipWalkResult` to indicate the type of the file."""
     #: A regular file.
@@ -218,14 +219,17 @@
 
     If *any* of ``encoding``, ``errors``, or ``newline`` is specified, the returned
     file is wrapped in :class:`io.TextIOWrapper`!
 
     If the last file in the list of files is an archive file, then it won't be decompressed,
     instead you'll be able to read the archive's raw compressed data from the handle.
 
+    In this example, we open a gzip-compressed file, stored inside a tgz archive, which
+    in turn is stored in a Zip file:
+
     >>> from unzipwalk import recursive_open
     >>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
     ...     print(fh.read())# doctest: +NORMALIZE_WHITESPACE
     Hi, I'm a compressed file!
     """
     # note Sphinx's "WARNING: py:class reference target not found: _io.TextIOWrapper" can be ignored
     if not fns:
@@ -234,100 +238,114 @@
         with _inner_recur_open(fh, (Path(fns[0]),) + tuple( PurePosixPath(f) for f in fns[1:] )) as inner:
             assert inner.readable()
             if encoding is not None or errors is not None or newline is not None:
                 yield io.TextIOWrapper(inner, encoding=encoding, errors=errors, newline=newline)
             else:
                 yield cast(ReadOnlyBinary, inner)
 
-def _proc_file(fns :tuple[PurePath, ...], fh :BinaryIO) -> Generator[UnzipWalkResult, None, None]:
+FilterType = Callable[[Sequence[PurePath]], bool]
+
+def _proc_file(fns :tuple[PurePath, ...], fh :BinaryIO, *, matcher :Optional[FilterType]) -> Generator[UnzipWalkResult, None, None]:
     bl = fns[-1].name.lower()
     if bl.endswith('.tar.gz') or bl.endswith('.tgz') or bl.endswith('.tar'):
         yield UnzipWalkResult(names=fns, typ=FileType.ARCHIVE)
         with TarFile.open(fileobj=fh) as tf:
             for ti in tf.getmembers():
                 new_names = (*fns, PurePosixPath(ti.name))
+                if matcher is not None and not matcher(new_names): continue
                 # for ti.type see e.g.: https://github.com/python/cpython/blob/v3.12.3/Lib/tarfile.py#L88
                 if ti.issym():
                     yield UnzipWalkResult(names=new_names, typ=FileType.SYMLINK)
                 elif ti.isdir():
                     yield UnzipWalkResult(names=new_names, typ=FileType.DIR)
                 elif ti.isfile():
                     # Note apparently this can burn a lot of memory on <3.13: https://github.com/python/cpython/issues/102120
                     ef = tf.extractfile(ti)  # always binary
                     assert ef is not None  # make type checker happy; we know this is true because we checked it's a file
                     with ef as fh2:
                         assert fh2.readable()  # expected by ReadOnlyBinary
                         # NOTE type checker thinks fh2 is typing.IO[bytes], but it's actually a tarfile.ExFileObject,
                         # which is an io.BufferedReader subclass - which should be safe to cast to BinaryIO, I think.
-                        yield from _proc_file(new_names, cast(BinaryIO, fh2))
+                        yield from _proc_file(new_names, cast(BinaryIO, fh2), matcher=matcher)
                 else: yield UnzipWalkResult(names=new_names, typ=FileType.OTHER)
     elif bl.endswith('.zip'):
         yield UnzipWalkResult(names=fns, typ=FileType.ARCHIVE)
         with ZipFile(fh) as zf:
             for zi in zf.infolist():
                 # Note the ZIP specification requires forward slashes for path separators.
                 # https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
                 new_names = (*fns, PurePosixPath(zi.filename))
+                if matcher is not None and not matcher(new_names): continue
                 # Manually detect symlinks in ZIP files (should be rare anyway)
                 # e.g. from zipfile.py: z_info.external_attr = (st.st_mode & 0xFFFF) << 16
                 # we're not going to worry about other special file types in ZIP files
                 if zi.create_system==3 and stat.S_ISLNK(zi.external_attr>>16):  # 3 is UNIX
                     yield UnzipWalkResult(names=new_names, typ=FileType.SYMLINK)
                 elif zi.is_dir():
                     yield UnzipWalkResult(names=new_names, typ=FileType.DIR)
                 else:  # (note this interface doesn't have an is_file)
                     with zf.open(zi) as fh2:  # always binary mode
                         assert fh2.readable()  # expected by ReadOnlyBinary
                         # NOTE type checker thinks fh2 is typing.IO[bytes], but it's actually a zipfile.ZipExtFile,
                         # which is an io.BufferedIOBase subclass - which should be safe to cast to BinaryIO, I think.
-                        yield from _proc_file(new_names, cast(BinaryIO, fh2))
+                        yield from _proc_file(new_names, cast(BinaryIO, fh2), matcher=matcher)
     elif bl.endswith('.gz'):
         yield UnzipWalkResult(names=fns, typ=FileType.ARCHIVE)
+        new_names = (*fns, fns[-1].with_suffix(''))
+        if matcher is not None and not matcher(new_names): return
         with GzipFile(fileobj=fh, mode='rb') as fh2:  # always binary, but specify explicitly for clarity
             assert fh2.readable()  # expected by ReadOnlyBinary
             # NOTE casting GzipFile to BinaryIO isn't 100% safe because the former doesn't implement the full interface,
             # but testing seems to show it's ok...
-            yield from _proc_file((*fns, fns[-1].with_suffix('')), cast(BinaryIO, fh2))
+            yield from _proc_file(new_names, cast(BinaryIO, fh2), matcher=matcher)
     else:
         assert fh.readable()  # expected by ReadOnlyBinary
         # The following cast is safe since ReadOnlyBinary is a subset of the interfaces.
         yield UnzipWalkResult(names=fns, typ=FileType.FILE, hnd=cast(ReadOnlyBinary, fh))
 
-def unzipwalk(paths :AnyPaths) -> Generator[UnzipWalkResult, None, None]:
+def unzipwalk(paths :AnyPaths, *, matcher :Optional[FilterType] = None) -> Generator[UnzipWalkResult, None, None]:
     """This generator recursively walks into directories and compressed files and yields named tuples of type :class:`UnzipWalkResult`.
 
-    :param paths: A filename or iterable of filenames."""
+    :param paths: A filename or iterable of filenames.
+    :param matcher: When you provide this optional argument, it must be a callable that accepts a sequence of paths
+        as its only argument, and returns a boolean value whether this filename should be further processed or not."""
     p_paths = tuple(to_Paths(paths))
     for p in p_paths: p.resolve(strict=True)  # force FileNotFound errors early
     for p in chain.from_iterable( pa.rglob('*') if pa.is_dir() else (pa,) for pa in p_paths ):
+        if matcher is not None and not matcher((p,)): continue
         if p.is_symlink():
             yield UnzipWalkResult(names=(p,), typ=FileType.SYMLINK).validate()  # pragma: no cover  (doesn't run on Windows)
         elif p.is_dir():
             yield UnzipWalkResult(names=(p,), typ=FileType.DIR).validate()
         elif p.is_file():
             with p.open('rb') as fh:
-                yield from ( r.validate() for r in _proc_file((p,), fh) )
+                yield from ( r.validate() for r in _proc_file((p,), fh, matcher=matcher) )
         else:
             yield UnzipWalkResult(names=(p,), typ=FileType.OTHER).validate()  # pragma: no cover  (doesn't run on Windows)
 
 def _arg_parser():
     parser = argparse.ArgumentParser('unzipwalk', description='Recursively walk into directories and archives',
-        epilog=f"Possible values for ALGO: {', '.join(sorted(hashlib.algorithms_available))}")
+        epilog="* Note --exclude currently only matches against the final name in the sequence, excluding path names, "
+        "but this interface may change in future versions. For more control, use the library instead of this command-line tool.\n\n"
+        f"** Possible values for ALGO: {', '.join(sorted(hashlib.algorithms_available))}")
     parser.add_argument('-a','--all-files', help="also list dirs, symlinks, etc.", action="store_true")
     group = parser.add_mutually_exclusive_group()
     group.add_argument('-d','--dump', help="also dump file contents", action="store_true")
-    group.add_argument('-c','--checksum', help="generate a checksum for each file", choices=hashlib.algorithms_available, metavar="ALGO")
+    group.add_argument('-c','--checksum', help="generate a checksum for each file**", choices=hashlib.algorithms_available, metavar="ALGO")
+    parser.add_argument('-e', '--exclude', help="filename globs to exclude*", action="append", default=[])
     parser.add_argument('paths', metavar='PATH', help='paths to process (default is current directory)', nargs='*')
     return parser
 
 def main(argv=None):
     igbpyutils.error.init_handlers()
     parser = _arg_parser()
     args = parser.parse_args(argv)
-    for result in unzipwalk( args.paths if args.paths else Path() ):
+    def matcher(paths :Sequence[PurePath]) -> bool:
+        return not any( fnmatch(paths[-1].name, pat) for pat in args.exclude )
+    for result in unzipwalk( args.paths if args.paths else Path(), matcher=matcher ):
         names = tuple( str(n) for n in result.names )
         if (args.dump or args.checksum) and result.typ==FileType.FILE:
             assert result.hnd is not None  # make type checker happy; we know this is true because we checked it's a file
             if args.checksum:
                 h = hashlib.new(args.checksum)
                 h.update(result.hnd.read())
                 print(f"{h.hexdigest()} *{names[0] if len(names)==1 else repr(names)}")
```

### Comparing `unzipwalk-1.1.0/unzipwalk.egg-info/PKG-INFO` & `unzipwalk-1.2.0/unzipwalk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: unzipwalk
-Version: 1.1.0
+Version: 1.2.0
 Summary: Recursively walk into directories and archives
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Repository, https://github.com/haukex/unzipwalk
 Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
+Project-URL: Changelog, https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -82,20 +83,22 @@
 ['42', 'Hello', 'World']
 ```
 
 ## Members
 
 <a id="function-unzipwalk"></a>
 
-### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)])
+### unzipwalk.unzipwalk(paths: [str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) | [Iterable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)], \*, matcher: [Callable](https://docs.python.org/3/library/collections.abc.html#collections.abc.Callable)[[[Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath)]], [bool](https://docs.python.org/3/library/functions.html#bool)] | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
-  **paths** – A filename or iterable of filenames.
+  * **paths** – A filename or iterable of filenames.
+  * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
+    as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
@@ -168,52 +171,62 @@
 
 A symbolic link.
 
 #### OTHER *= 4*
 
 Some other file type (e.g. FIFO).
 
+<a id="unzipwalk.recursive_open"></a>
+
 ### unzipwalk.recursive_open(fns: [Sequence](https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence)[[str](https://docs.python.org/3/library/stdtypes.html#str) | [PathLike](https://docs.python.org/3/library/os.html#os.PathLike)], encoding=None, errors=None, newline=None)
 
 This context manager allows opening files nested inside archives directly.
 
 [`unzipwalk()`](#function-unzipwalk) automatically closes files as it iterates through directories and archives;
 this function exists to allow you to open the returned files after the iteration.
 
 If *any* of `encoding`, `errors`, or `newline` is specified, the returned
 file is wrapped in [`io.TextIOWrapper`](https://docs.python.org/3/library/io.html#io.TextIOWrapper)!
 
 If the last file in the list of files is an archive file, then it won’t be decompressed,
 instead you’ll be able to read the archive’s raw compressed data from the handle.
 
+In this example, we open a gzip-compressed file, stored inside a tgz archive, which
+in turn is stored in a Zip file:
+
 ```pycon
 >>> from unzipwalk import recursive_open
 >>> with recursive_open(('bar.zip', 'test.tar.gz', 'test/cool.txt.gz', 'test/cool.txt'), encoding='UTF-8') as fh:
 ...     print(fh.read())
 Hi, I'm a compressed file!
 ```
 
 ## Command-Line Interface
 
 ```default
-usage: unzipwalk [-h] [-a] [-d | -c ALGO] [PATH ...]
+usage: unzipwalk [-h] [-a] [-d | -c ALGO] [-e EXCLUDE] [PATH ...]
 
 Recursively walk into directories and archives
 
 positional arguments:
   PATH                  paths to process (default is current directory)
 
 optional arguments:
   -h, --help            show this help message and exit
   -a, --all-files       also list dirs, symlinks, etc.
   -d, --dump            also dump file contents
   -c ALGO, --checksum ALGO
-                        generate a checksum for each file
-
-Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
+                        generate a checksum for each file**
+  -e EXCLUDE, --exclude EXCLUDE
+                        filename globs to exclude*
+
+* Note --exclude currently only matches against the final name in the
+sequence, excluding path names, but this interface may change in future
+versions. For more control, use the library instead of this command-line tool.
+** Possible values for ALGO: blake2b, blake2s, md5, md5-sha1, sha1, sha224,
 sha256, sha384, sha3_224, sha3_256, sha3_384, sha3_512, sha512, sha512_224,
 sha512_256, shake_128, shake_256, sm3
 ```
 
 The available checksum algorithms may vary depending on your system and Python version.
 Run the command with `--help` to see the list of currently available algorithms.
```

