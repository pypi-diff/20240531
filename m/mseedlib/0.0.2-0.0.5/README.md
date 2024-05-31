# Comparing `tmp/mseedlib-0.0.2.tar.gz` & `tmp/mseedlib-0.0.5.tar.gz`

## Comparing `mseedlib-0.0.2.tar` & `mseedlib-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 mseedlib-0.0.2/development.txt
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 mseedlib-0.0.2/hatch_build_libmseed.py
--rwxr-xr-x   0        0        0     2396 2020-02-02 00:00:00.000000 mseedlib-0.0.2/examples/read_numpy.py
--rwxr-xr-x   0        0        0     1894 2020-02-02 00:00:00.000000 mseedlib-0.0.2/examples/stream_stats.py
--rwxr-xr-x   0        0        0     4578 2020-02-02 00:00:00.000000 mseedlib-0.0.2/examples/write_with_buffer.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/__version__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/clib.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/definitions.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/exceptions.py
--rw-r--r--   0        0        0    16928 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/msrecord.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/msrecord_buffer_reader.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/msrecord_reader.py
--rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/mstracelist.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/util.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/.clang-format
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/.gitignore
--rw-r--r--   0        0        0    58778 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/ChangeLog
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/INSTALL.md
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/LICENSE
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/Makefile
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/Makefile.win
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/README.byteorder
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/README.md
--rw-r--r--   0        0        0    35946 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/crc32c.c
--rw-r--r--   0        0        0    39729 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/extraheaders.c
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/extraheaders.h
--rw-r--r--   0        0        0    34982 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/fileutils.c
--rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/genutils.c
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/gmtime64.c
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/gmtime64.h
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/libmseed.def
--rw-r--r--   0        0        0    63260 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/libmseed.h
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/libmseed.map
--rw-r--r--   0        0        0    20562 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/logging.c
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/lookup.c
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/mseed.pc.in
--rw-r--r--   0        0        0    32754 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/mseedformat.h
--rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/msio.c
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/msio.h
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/msrutils.c
--rw-r--r--   0        0        0    70965 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/pack.c
--rw-r--r--   0        0        0    22238 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/packdata.c
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/packdata.h
--rw-r--r--   0        0        0    55930 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/parseutils.c
--rw-r--r--   0        0        0    26348 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/selection.c
--rw-r--r--   0        0        0    76989 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/tracelist.c
--rw-r--r--   0        0        0    57962 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/unpack.c
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/unpack.h
--rw-r--r--   0        0        0    29345 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/unpackdata.c
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/unpackdata.h
--rw-r--r--   0        0        0   353726 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/yyjson.c
--rw-r--r--   0        0        0   306476 2020-02-02 00:00:00.000000 mseedlib-0.0.2/src/mseedlib/libmseed/yyjson.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/test_msrecord.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/test_msrecord_buffer_reader.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/test_msrecord_reader.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/test_mstracelist.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/data/packtest_sine2000.mseed3
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/data/packtest_sine500.mseed2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/data/packtest_sine500.mseed3
--rw-r--r--   0        0        0   584192 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/data/testdata-COLA-signal.mseed2
--rw-r--r--   0        0        0   617526 2020-02-02 00:00:00.000000 mseedlib-0.0.2/tests/data/testdata-COLA-signal.mseed3
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mseedlib-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedlib-0.0.2/LICENSE
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 mseedlib-0.0.2/README.md
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 mseedlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 mseedlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mseedlib-0.0.5/development.txt
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 mseedlib-0.0.5/hatch_build_libmseed.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 mseedlib-0.0.5/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0     2396 2020-02-02 00:00:00.000000 mseedlib-0.0.5/examples/read_numpy.py
+-rwxr-xr-x   0        0        0     1968 2020-02-02 00:00:00.000000 mseedlib-0.0.5/examples/stream_stats.py
+-rwxr-xr-x   0        0        0     4302 2020-02-02 00:00:00.000000 mseedlib-0.0.5/examples/stream_timewindow.py
+-rwxr-xr-x   0        0        0     4578 2020-02-02 00:00:00.000000 mseedlib-0.0.5/examples/write_with_buffer.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/__version__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/clib.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/definitions.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/exceptions.py
+-rw-r--r--   0        0        0    16928 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/msrecord.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/msrecord_buffer_reader.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/msrecord_reader.py
+-rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/mstracelist.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/util.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/.clang-format
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/.gitignore
+-rw-r--r--   0        0        0    59391 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/ChangeLog
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/INSTALL.md
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/LICENSE
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/Makefile
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/Makefile.win
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/README.byteorder
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/README.md
+-rw-r--r--   0        0        0    35946 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/crc32c.c
+-rw-r--r--   0        0        0    39729 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/extraheaders.c
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/extraheaders.h
+-rw-r--r--   0        0        0    34982 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/fileutils.c
+-rw-r--r--   0        0        0    56704 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/genutils.c
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/gmtime64.c
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/gmtime64.h
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/libmseed.def
+-rw-r--r--   0        0        0    63390 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/libmseed.h
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/libmseed.map
+-rw-r--r--   0        0        0    20562 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/logging.c
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/lookup.c
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/mseed.pc.in
+-rw-r--r--   0        0        0    32754 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/mseedformat.h
+-rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/msio.c
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/msio.h
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/msrutils.c
+-rw-r--r--   0        0        0    71371 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/pack.c
+-rw-r--r--   0        0        0    22238 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/packdata.c
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/packdata.h
+-rw-r--r--   0        0        0    55930 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/parseutils.c
+-rw-r--r--   0        0        0    26348 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/selection.c
+-rw-r--r--   0        0        0    76306 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/tracelist.c
+-rw-r--r--   0        0        0    58003 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/unpack.c
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/unpack.h
+-rw-r--r--   0        0        0    29345 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/unpackdata.c
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/unpackdata.h
+-rw-r--r--   0        0        0   353769 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/yyjson.c
+-rw-r--r--   0        0        0   306765 2020-02-02 00:00:00.000000 mseedlib-0.0.5/src/mseedlib/libmseed/yyjson.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/test_msrecord.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/test_msrecord_buffer_reader.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/test_msrecord_reader.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/test_mstracelist.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/data/packtest_sine2000.mseed3
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/data/packtest_sine500.mseed2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/data/packtest_sine500.mseed3
+-rw-r--r--   0        0        0   584192 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/data/testdata-COLA-signal.mseed2
+-rw-r--r--   0        0        0   617526 2020-02-02 00:00:00.000000 mseedlib-0.0.5/tests/data/testdata-COLA-signal.mseed3
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 mseedlib-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedlib-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 mseedlib-0.0.5/README.md
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 mseedlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 mseedlib-0.0.5/PKG-INFO
```

### Comparing `mseedlib-0.0.2/hatch_build_libmseed.py` & `mseedlib-0.0.5/hatch_build_libmseed.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                         os.path.join(self.package_path))
 
         # Copy libmseed.h to root package location
         shutil.copy(os.path.join(self.libmseed_path, 'libmseed.h'),
                     os.path.join(self.package_path))
 
     def clean(self, versions):
-        if sys.platform.lower().startswith("windows"):
+        if sys.platform.lower().startswith("win"):
             cmd = f"pushd {self.libmseed_path} && nmake /f Makefile.win clean & popd"
         else:
             cmd = f"make -C {self.libmseed_path} clean"
 
         subprocess.check_call(cmd, shell=True)
 
         if os.path.exists(os.path.join(self.package_path, 'libmseed.so')):
```

### Comparing `mseedlib-0.0.2/examples/read_numpy.py` & `mseedlib-0.0.5/examples/read_numpy.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/examples/stream_stats.py` & `mseedlib-0.0.5/examples/stream_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import pprint
 from collections import defaultdict
 from mseedlib import MS3RecordReader, nstime2timestr
 
 # Container for trace stats
 trace_stats = {}
 
+print("Reading miniSEED from stdin, writing to stdout", file=sys.stderr)
+
 # Read miniSEED from stdin
 with MS3RecordReader(sys.stdin.fileno()) as msreader:
     for msr in msreader:
 
         stats = trace_stats.setdefault(msr.sourceid, defaultdict(int))
 
         stats['record_count'] += 1
```

### Comparing `mseedlib-0.0.2/examples/write_with_buffer.py` & `mseedlib-0.0.5/examples/write_with_buffer.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/__init__.py` & `mseedlib-0.0.5/src/mseedlib/__init__.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/clib.py` & `mseedlib-0.0.5/src/mseedlib/clib.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/definitions.py` & `mseedlib-0.0.5/src/mseedlib/definitions.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/exceptions.py` & `mseedlib-0.0.5/src/mseedlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/msrecord.py` & `mseedlib-0.0.5/src/mseedlib/msrecord.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/msrecord_buffer_reader.py` & `mseedlib-0.0.5/src/mseedlib/msrecord_buffer_reader.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/msrecord_reader.py` & `mseedlib-0.0.5/src/mseedlib/msrecord_reader.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/mstracelist.py` & `mseedlib-0.0.5/src/mseedlib/mstracelist.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/util.py` & `mseedlib-0.0.5/src/mseedlib/util.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/ChangeLog` & `mseedlib-0.0.5/src/mseedlib/libmseed/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+2024.148: 3.1.2
+	- Update yyjson to v0.9.0.
+	- Simplify mstl3_addmsr_recordptr() a bit.
+
+2024.146:
+	- Replace ms_dabs() with macro to use system fabs(), document as deprecated.
+	- Add CRC values to diagnostic message when header values does not match calculated.
+
+2024.137:
+	- Add msr3_nsperiod() to calculate the sample period in nanoseconds.
+	- Add tests for msr3 utility functions.
+
+2024.106:
+	- When writing v2 derive the quality code from the publication version when the
+	extra-header "/FDSN/DataQuality" is not present.  Use quality indicator 'D' when
+	the publication version cannot be mapped, e.g. > 4.
+
 2024.024: 3.1.1
 	- Change library compatibility version in Makefile to MAJOR.1.0, as this is now
 	incompatible with the x.0.0 releases.
 
 2024.024: 3.1.0
 	BREAKING CHANGES, data structure and an API changes:
 	- `MS3Record.encoding` now int16_t instead of int8_t.
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/INSTALL.md` & `mseedlib-0.0.5/src/mseedlib/libmseed/INSTALL.md`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/LICENSE` & `mseedlib-0.0.5/src/mseedlib/libmseed/LICENSE`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/Makefile` & `mseedlib-0.0.5/src/mseedlib/libmseed/Makefile`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/Makefile.win` & `mseedlib-0.0.5/src/mseedlib/libmseed/Makefile.win`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/README.byteorder` & `mseedlib-0.0.5/src/mseedlib/libmseed/README.byteorder`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/README.md` & `mseedlib-0.0.5/src/mseedlib/libmseed/README.md`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/crc32c.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/crc32c.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/extraheaders.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/extraheaders.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/extraheaders.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/extraheaders.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/fileutils.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/fileutils.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/genutils.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/genutils.c`

 * *Files 2% similar despite different names*

```diff
@@ -1668,33 +1668,14 @@
   }
 
   return (time + span);
 } /* End of ms_sampletime() */
 
 
 /**********************************************************************/ /**
- * @brief Determine the absolute value of an input double
- *
- * Actually just test if the input double is positive multiplying by
- * -1.0 if not and return it.
- *
- * @param[in] val Value for which to determine absolute value
- *
- * @returns the positive value of input double.
- ***************************************************************************/
-double
-ms_dabs (double val)
-{
-  if (val < 0.0)
-    val *= -1.0;
-  return val;
-} /* End of ms_dabs() */
-
-
-/**********************************************************************/ /**
  * @brief Runtime test for host endianess
  * @returns 0 if the host is little endian, otherwise 1.
  ***************************************************************************/
 inline int
 ms_bigendianhost (void)
 {
   const uint16_t endian = 256;
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/gmtime64.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/gmtime64.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/libmseed.def` & `mseedlib-0.0.5/src/mseedlib/libmseed/libmseed.def`

 * *Files 0% similar despite different names*

```diff
@@ -88,12 +88,11 @@
    ms_readleapseconds
    ms_readleapsecondfile
    ms_samplesize
    ms_encoding_sizetype
    ms_encodingstr
    ms_errorstr
    ms_sampletime
-   ms_dabs
    ms_bigendianhost
    ms_crc32c
    leapsecondlist
    libmseed_memory
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/libmseed.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/libmseed.h`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 #ifndef LIBMSEED_H
 #define LIBMSEED_H 1
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-#define LIBMSEED_VERSION "3.1.1"     //!< Library version
-#define LIBMSEED_RELEASE "2024.024"  //!< Library release date
+#define LIBMSEED_VERSION "3.1.2"     //!< Library version
+#define LIBMSEED_RELEASE "2024.148"  //!< Library release date
 
 /** @defgroup io-functions File and URL I/O */
 /** @defgroup miniseed-record Record Handling */
 /** @defgroup trace-list Trace List */
 /** @defgroup data-selections Data Selections */
 /** @defgroup string-functions Source Identifiers */
 /** @defgroup extra-headers Extra Headers */
@@ -59,14 +59,15 @@
 /* C99 standard headers */
 #include <stdlib.h>
 #include <stdio.h>
 #include <stdarg.h>
 #include <time.h>
 #include <string.h>
 #include <ctype.h>
+#include <math.h>
 
 /** @def PRIsize_t
     @brief A printf() macro for portably printing size_t values */
 #define PRIsize_t "zu"
 
 #if defined(WIN32) || defined(_WIN32) || defined(WIN64) || defined(_WIN64)
   #define LMP_WIN 1
@@ -136,15 +137,15 @@
 #define MAXRECLEN 10485760 //!< Maximum miniSEED record length supported (10MiB)
 #define MAXRECLENv2 131172 //!< Maximum v2 miniSEED record length supported (131+ KiB or 2^17)
 
 #define LM_SIDLEN 64       //!< Length of source ID string
 
 /** @def MS_ISRATETOLERABLE
     @brief Macro to test default sample rate tolerance: abs(1-sr1/sr2) < 0.0001 */
-#define MS_ISRATETOLERABLE(A,B) (ms_dabs (1.0 - ((A) / (B))) < 0.0001)
+#define MS_ISRATETOLERABLE(A,B) (fabs (1.0 - ((A) / (B))) < 0.0001)
 
 /** @def MS2_ISDATAINDICATOR
     @brief Macro to test a character for miniSEED 2.x data record/quality indicators */
 #define MS2_ISDATAINDICATOR(X) ((X)=='D' || (X)=='R' || (X)=='Q' || (X)=='M')
 
 /** @def MS3_ISVALIDHEADER
  * @hideinitializer
@@ -405,14 +406,15 @@
 extern MS3Record* msr3_init (MS3Record *msr);
 extern void       msr3_free (MS3Record **ppmsr);
 extern MS3Record* msr3_duplicate (const MS3Record *msr, int8_t datadup);
 extern nstime_t   msr3_endtime (const MS3Record *msr);
 extern void       msr3_print (const MS3Record *msr, int8_t details);
 extern int        msr3_resize_buffer (MS3Record *msr);
 extern double     msr3_sampratehz (const MS3Record *msr);
+extern nstime_t   msr3_nsperiod (const MS3Record *msr);
 extern double     msr3_host_latency (const MS3Record *msr);
 
 extern int64_t ms3_detect (const char *record, uint64_t recbuflen, uint8_t *formatversion);
 extern int ms_parse_raw3 (const char *record, int maxreclen, int8_t details);
 extern int ms_parse_raw2 (const char *record, int maxreclen, int8_t details, int8_t swapflag);
 /** @} */
 
@@ -1248,17 +1250,19 @@
 
 extern uint8_t ms_samplesize (char sampletype);
 extern int ms_encoding_sizetype (uint8_t encoding, uint8_t *samplesize, char *sampletype);
 extern const char *ms_encodingstr (uint8_t encoding);
 extern const char *ms_errorstr (int errorcode);
 
 extern nstime_t ms_sampletime (nstime_t time, int64_t offset, double samprate);
-extern double ms_dabs (double val);
 extern int ms_bigendianhost (void);
 
+/** DEPRECATED legacy implementation of fabs(), now a macro */
+#define ms_dabs(val) fabs(val)
+
 /** Portable version of POSIX ftello() to get file position in large files */
 extern int64_t lmp_ftell64 (FILE *stream);
 /** Portable version of POSIX fseeko() to set position in large files */
 extern int lmp_fseek64 (FILE *stream, int64_t offset, int whence);
 /** Portable version of POSIX nanosleep() to sleep for nanoseconds */
 extern uint64_t lmp_nanosleep (uint64_t nanoseconds);
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/logging.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/logging.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/lookup.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/lookup.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/mseedformat.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/mseedformat.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/msio.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/msio.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/msio.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/msio.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/msrutils.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/msrutils.c`

 * *Files 6% similar despite different names*

```diff
@@ -352,14 +352,37 @@
   if (msr->samprate < 0.0)
     return (-1.0 / msr->samprate);
   else
     return msr->samprate;
 } /* End of msr3_sampratehz() */
 
 /**********************************************************************/ /**
+ * @brief Calculate sample period in nanoseconds/sample for a given ::MS3Record
+ *
+ * @param[in] msr ::MS3Record to calculate sample period for
+ *
+ * @returns Return sample period in nanoseconds (nanoseconds per sample)
+ ***************************************************************************/
+inline nstime_t
+msr3_nsperiod (const MS3Record *msr)
+{
+  if (!msr)
+    return 0;
+
+  /* Calculate sample period from sample rate or period.
+   * The value is rounded by adding 0.5 before truncation to an integer. */
+  if (msr->samprate > 0.0)
+    return (nstime_t)(NSTMODULUS / msr->samprate + 0.5); /* samples/second */
+  else if (msr->samprate < 0.0)
+    return (nstime_t)(NSTMODULUS * -msr->samprate + 0.5); /* period or seconds/sample */
+
+  return 0;
+} /* End of msr3_nsperiod() */
+
+/**********************************************************************/ /**
  * @brief Calculate data latency based on the host time
  *
  * Calculation is based on the time of the last sample in the record; in
  * other words, the difference between the host time and the time of
  * the last sample in the record.
  *
  * Double precision is returned, but the true precision is dependent
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/pack.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/pack.c`

 * *Files 0% similar despite different names*

```diff
@@ -1969,2468 +1969,2493 @@
 00007b00: 6568 726f 6f74 203d 2079 796a 736f 6e5f  ehroot = yyjson_
 00007b10: 646f 635f 6765 745f 726f 6f74 2028 6568  doc_get_root (eh
 00007b20: 646f 6329 3b0a 2020 7d0a 0a20 202f 2a20  doc);.  }..  /* 
 00007b30: 4275 696c 6420 6669 7865 6420 6865 6164  Build fixed head
 00007b40: 6572 202a 2f0a 2020 6d65 6d63 7079 2028  er */.  memcpy (
 00007b50: 704d 5332 4653 4448 5f53 4551 4e55 4d20  pMS2FSDH_SEQNUM 
 00007b60: 2872 6563 6f72 6429 2c20 2230 3030 3030  (record), "00000
-00007b70: 3022 2c20 3629 3b0a 0a20 2069 6620 2879  0", 6);..  if (y
-00007b80: 796a 736f 6e5f 7074 725f 6765 745f 7374  yjson_ptr_get_st
-00007b90: 7220 2865 6872 6f6f 742c 2022 2f46 4453  r (ehroot, "/FDS
-00007ba0: 4e2f 4461 7461 5175 616c 6974 7922 2c20  N/DataQuality", 
-00007bb0: 2668 6561 6465 725f 7374 7269 6e67 2920  &header_string) 
-00007bc0: 2626 0a20 2020 2020 204d 5332 5f49 5344  &&.      MS2_ISD
-00007bd0: 4154 4149 4e44 4943 4154 4f52 2028 6865  ATAINDICATOR (he
-00007be0: 6164 6572 5f73 7472 696e 675b 305d 2929  ader_string[0]))
-00007bf0: 0a20 2020 202a 704d 5332 4653 4448 5f44  .    *pMS2FSDH_D
-00007c00: 4154 4151 5541 4c49 5459 2028 7265 636f  ATAQUALITY (reco
-00007c10: 7264 2920 3d20 6865 6164 6572 5f73 7472  rd) = header_str
-00007c20: 696e 675b 305d 3b0a 2020 656c 7365 0a20  ing[0];.  else. 
-00007c30: 2020 202a 704d 5332 4653 4448 5f44 4154     *pMS2FSDH_DAT
-00007c40: 4151 5541 4c49 5459 2028 7265 636f 7264  AQUALITY (record
-00007c50: 2920 3d20 2744 273b 0a0a 2020 2a70 4d53  ) = 'D';..  *pMS
-00007c60: 3246 5344 485f 5245 5345 5256 4544 2028  2FSDH_RESERVED (
-00007c70: 7265 636f 7264 2920 3d20 2720 273b 0a20  record) = ' ';. 
-00007c80: 206d 735f 7374 726e 6370 6f70 656e 2028   ms_strncpopen (
-00007c90: 704d 5332 4653 4448 5f53 5441 5449 4f4e  pMS2FSDH_STATION
-00007ca0: 2028 7265 636f 7264 292c 2073 7461 7469   (record), stati
-00007cb0: 6f6e 2c20 3529 3b0a 2020 6d73 5f73 7472  on, 5);.  ms_str
-00007cc0: 6e63 706f 7065 6e20 2870 4d53 3246 5344  ncpopen (pMS2FSD
-00007cd0: 485f 4c4f 4341 5449 4f4e 2028 7265 636f  H_LOCATION (reco
-00007ce0: 7264 292c 206c 6f63 6174 696f 6e2c 2032  rd), location, 2
-00007cf0: 293b 0a20 206d 735f 7374 726e 6370 6f70  );.  ms_strncpop
-00007d00: 656e 2028 704d 5332 4653 4448 5f43 4841  en (pMS2FSDH_CHA
-00007d10: 4e4e 454c 2028 7265 636f 7264 292c 2063  NNEL (record), c
-00007d20: 6861 6e6e 656c 2c20 3329 3b0a 2020 6d73  hannel, 3);.  ms
-00007d30: 5f73 7472 6e63 706f 7065 6e20 2870 4d53  _strncpopen (pMS
-00007d40: 3246 5344 485f 4e45 5457 4f52 4b20 2872  2FSDH_NETWORK (r
-00007d50: 6563 6f72 6429 2c20 6e65 7477 6f72 6b2c  ecord), network,
-00007d60: 2032 293b 0a0a 2020 2a70 4d53 3246 5344   2);..  *pMS2FSD
-00007d70: 485f 5945 4152 2028 7265 636f 7264 2920  H_YEAR (record) 
-00007d80: 2020 2020 2020 3d20 484f 3275 2028 7965        = HO2u (ye
-00007d90: 6172 2c20 7377 6170 666c 6167 293b 0a20  ar, swapflag);. 
-00007da0: 202a 704d 5332 4653 4448 5f44 4159 2028   *pMS2FSDH_DAY (
-00007db0: 7265 636f 7264 2920 2020 2020 2020 203d  record)        =
-00007dc0: 2048 4f32 7520 2864 6179 2c20 7377 6170   HO2u (day, swap
-00007dd0: 666c 6167 293b 0a20 202a 704d 5332 4653  flag);.  *pMS2FS
-00007de0: 4448 5f48 4f55 5220 2872 6563 6f72 6429  DH_HOUR (record)
-00007df0: 2020 2020 2020 203d 2068 6f75 723b 0a20         = hour;. 
-00007e00: 202a 704d 5332 4653 4448 5f4d 494e 2028   *pMS2FSDH_MIN (
-00007e10: 7265 636f 7264 2920 2020 2020 2020 203d  record)        =
-00007e20: 206d 696e 3b0a 2020 2a70 4d53 3246 5344   min;.  *pMS2FSD
-00007e30: 485f 5345 4320 2872 6563 6f72 6429 2020  H_SEC (record)  
-00007e40: 2020 2020 2020 3d20 7365 633b 0a20 202a        = sec;.  *
-00007e50: 704d 5332 4653 4448 5f55 4e55 5345 4420  pMS2FSDH_UNUSED 
-00007e60: 2872 6563 6f72 6429 2020 2020 203d 2030  (record)     = 0
-00007e70: 3b0a 2020 2a70 4d53 3246 5344 485f 4653  ;.  *pMS2FSDH_FS
-00007e80: 4543 2028 7265 636f 7264 2920 2020 2020  EC (record)     
-00007e90: 2020 3d20 484f 3275 2028 6673 6563 2c20    = HO2u (fsec, 
-00007ea0: 7377 6170 666c 6167 293b 0a20 202a 704d  swapflag);.  *pM
-00007eb0: 5332 4653 4448 5f4e 554d 5341 4d50 4c45  S2FSDH_NUMSAMPLE
-00007ec0: 5320 2872 6563 6f72 6429 203d 2030 3b0a  S (record) = 0;.
-00007ed0: 0a20 202a 704d 5332 4653 4448 5f53 414d  .  *pMS2FSDH_SAM
-00007ee0: 504c 4552 4154 4546 4143 5420 2872 6563  PLERATEFACT (rec
-00007ef0: 6f72 6429 203d 2048 4f32 6420 2866 6163  ord) = HO2d (fac
-00007f00: 746f 722c 2073 7761 7066 6c61 6729 3b0a  tor, swapflag);.
-00007f10: 2020 2a70 4d53 3246 5344 485f 5341 4d50    *pMS2FSDH_SAMP
-00007f20: 4c45 5241 5445 4d55 4c54 2028 7265 636f  LERATEMULT (reco
-00007f30: 7264 2920 3d20 484f 3264 2028 6d75 6c74  rd) = HO2d (mult
-00007f40: 6970 6c69 6572 2c20 7377 6170 666c 6167  iplier, swapflag
-00007f50: 293b 0a0a 2020 2f2a 204d 6170 2061 6374  );..  /* Map act
-00007f60: 6976 6974 7920 6269 7420 666c 6167 7320  ivity bit flags 
-00007f70: 2a2f 0a20 202a 704d 5332 4653 4448 5f41  */.  *pMS2FSDH_A
-00007f80: 4354 464c 4147 5320 2872 6563 6f72 6429  CTFLAGS (record)
-00007f90: 203d 2030 3b0a 2020 6966 2028 6d73 722d   = 0;.  if (msr-
-00007fa0: 3e66 6c61 6773 2026 2030 7830 3129 202f  >flags & 0x01) /
-00007fb0: 2a20 4269 7420 3020 2a2f 0a20 2020 202a  * Bit 0 */.    *
-00007fc0: 704d 5332 4653 4448 5f41 4354 464c 4147  pMS2FSDH_ACTFLAG
-00007fd0: 5320 2872 6563 6f72 6429 207c 3d20 3078  S (record) |= 0x
-00007fe0: 3031 3b0a 0a20 2069 6620 2879 796a 736f  01;..  if (yyjso
-00007ff0: 6e5f 7074 725f 6765 745f 626f 6f6c 2028  n_ptr_get_bool (
-00008000: 6568 726f 6f74 2c20 222f 4644 534e 2f45  ehroot, "/FDSN/E
-00008010: 7665 6e74 2f42 6567 696e 222c 2026 6865  vent/Begin", &he
-00008020: 6164 6572 5f62 6f6f 6c65 616e 2920 2626  ader_boolean) &&
-00008030: 2068 6561 6465 725f 626f 6f6c 6561 6e29   header_boolean)
-00008040: 202f 2a20 4269 7420 3220 2a2f 0a20 2020   /* Bit 2 */.   
-00008050: 202a 704d 5332 4653 4448 5f41 4354 464c   *pMS2FSDH_ACTFL
-00008060: 4147 5320 2872 6563 6f72 6429 207c 3d20  AGS (record) |= 
-00008070: 3078 3034 3b0a 2020 6966 2028 7979 6a73  0x04;.  if (yyjs
-00008080: 6f6e 5f70 7472 5f67 6574 5f62 6f6f 6c20  on_ptr_get_bool 
-00008090: 2865 6872 6f6f 742c 2022 2f46 4453 4e2f  (ehroot, "/FDSN/
-000080a0: 4576 656e 742f 456e 6422 2c20 2668 6561  Event/End", &hea
-000080b0: 6465 725f 626f 6f6c 6561 6e29 2026 2620  der_boolean) && 
-000080c0: 6865 6164 6572 5f62 6f6f 6c65 616e 2920  header_boolean) 
-000080d0: 2f2a 2042 6974 2033 202a 2f0a 2020 2020  /* Bit 3 */.    
-000080e0: 2a70 4d53 3246 5344 485f 4143 5446 4c41  *pMS2FSDH_ACTFLA
-000080f0: 4753 2028 7265 636f 7264 2920 7c3d 2030  GS (record) |= 0
-00008100: 7830 383b 0a0a 2020 6966 2028 7979 6a73  x08;..  if (yyjs
-00008110: 6f6e 5f70 7472 5f67 6574 5f6e 756d 2028  on_ptr_get_num (
-00008120: 6568 726f 6f74 2c20 222f 4644 534e 2f54  ehroot, "/FDSN/T
-00008130: 696d 652f 4c65 6170 5365 636f 6e64 222c  ime/LeapSecond",
-00008140: 2026 6865 6164 6572 5f6e 756d 6265 7229   &header_number)
-00008150: 290a 2020 7b0a 2020 2020 6966 2028 6865  ).  {.    if (he
-00008160: 6164 6572 5f6e 756d 6265 7220 3e20 3029  ader_number > 0)
-00008170: 202f 2a20 4269 7420 3420 2a2f 0a20 2020   /* Bit 4 */.   
-00008180: 2020 202a 704d 5332 4653 4448 5f41 4354     *pMS2FSDH_ACT
-00008190: 464c 4147 5320 2872 6563 6f72 6429 207c  FLAGS (record) |
-000081a0: 3d20 3078 3130 3b0a 2020 2020 656c 7365  = 0x10;.    else
-000081b0: 2069 6620 2868 6561 6465 725f 6e75 6d62   if (header_numb
-000081c0: 6572 203c 2030 2920 2f2a 2042 6974 2035  er < 0) /* Bit 5
-000081d0: 202a 2f0a 2020 2020 2020 2a70 4d53 3246   */.      *pMS2F
-000081e0: 5344 485f 4143 5446 4c41 4753 2028 7265  SDH_ACTFLAGS (re
-000081f0: 636f 7264 2920 7c3d 2030 7832 303b 0a20  cord) |= 0x20;. 
-00008200: 207d 0a0a 2020 6966 2028 7979 6a73 6f6e   }..  if (yyjson
-00008210: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
-00008220: 6872 6f6f 742c 2022 2f46 4453 4e2f 4576  hroot, "/FDSN/Ev
-00008230: 656e 742f 496e 5072 6f67 7265 7373 222c  ent/InProgress",
-00008240: 2026 6865 6164 6572 5f62 6f6f 6c65 616e   &header_boolean
-00008250: 2920 2626 2068 6561 6465 725f 626f 6f6c  ) && header_bool
-00008260: 6561 6e29 202f 2a20 4269 7420 3620 2a2f  ean) /* Bit 6 */
-00008270: 0a20 2020 202a 704d 5332 4653 4448 5f41  .    *pMS2FSDH_A
-00008280: 4354 464c 4147 5320 2872 6563 6f72 6429  CTFLAGS (record)
-00008290: 207c 3d20 3078 3430 3b0a 0a20 202f 2a20   |= 0x40;..  /* 
-000082a0: 4d61 7020 492f 4f20 616e 6420 636c 6f63  Map I/O and cloc
-000082b0: 6b20 6269 7420 666c 6167 7320 2a2f 0a20  k bit flags */. 
-000082c0: 202a 704d 5332 4653 4448 5f49 4f46 4c41   *pMS2FSDH_IOFLA
-000082d0: 4753 2028 7265 636f 7264 2920 3d20 303b  GS (record) = 0;
-000082e0: 0a20 2069 6620 2879 796a 736f 6e5f 7074  .  if (yyjson_pt
-000082f0: 725f 6765 745f 626f 6f6c 2028 6568 726f  r_get_bool (ehro
-00008300: 6f74 2c20 222f 4644 534e 2f46 6c61 6773  ot, "/FDSN/Flags
-00008310: 2f53 7461 7469 6f6e 566f 6c75 6d65 5061  /StationVolumePa
-00008320: 7269 7479 4572 726f 7222 2c20 2668 6561  rityError", &hea
-00008330: 6465 725f 626f 6f6c 6561 6e29 2026 2620  der_boolean) && 
-00008340: 6865 6164 6572 5f62 6f6f 6c65 616e 2920  header_boolean) 
-00008350: 2f2a 2042 6974 2030 202a 2f0a 2020 2020  /* Bit 0 */.    
-00008360: 2a70 4d53 3246 5344 485f 494f 464c 4147  *pMS2FSDH_IOFLAG
-00008370: 5320 2872 6563 6f72 6429 207c 3d20 3078  S (record) |= 0x
-00008380: 3031 3b0a 2020 6966 2028 7979 6a73 6f6e  01;.  if (yyjson
-00008390: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
-000083a0: 6872 6f6f 742c 2022 2f46 4453 4e2f 466c  hroot, "/FDSN/Fl
-000083b0: 6167 732f 4c6f 6e67 5265 636f 7264 5265  ags/LongRecordRe
-000083c0: 6164 222c 2026 6865 6164 6572 5f62 6f6f  ad", &header_boo
-000083d0: 6c65 616e 2920 2626 2068 6561 6465 725f  lean) && header_
-000083e0: 626f 6f6c 6561 6e29 202f 2a20 4269 7420  boolean) /* Bit 
-000083f0: 3120 2a2f 0a20 2020 202a 704d 5332 4653  1 */.    *pMS2FS
-00008400: 4448 5f49 4f46 4c41 4753 2028 7265 636f  DH_IOFLAGS (reco
-00008410: 7264 2920 7c3d 2030 7830 323b 0a20 2069  rd) |= 0x02;.  i
-00008420: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
-00008430: 745f 626f 6f6c 2028 6568 726f 6f74 2c20  t_bool (ehroot, 
-00008440: 222f 4644 534e 2f46 6c61 6773 2f53 686f  "/FDSN/Flags/Sho
-00008450: 7274 5265 636f 7264 5265 6164 222c 2026  rtRecordRead", &
-00008460: 6865 6164 6572 5f62 6f6f 6c65 616e 2920  header_boolean) 
-00008470: 2626 2068 6561 6465 725f 626f 6f6c 6561  && header_boolea
-00008480: 6e29 202f 2a20 4269 7420 3220 2a2f 0a20  n) /* Bit 2 */. 
-00008490: 2020 202a 704d 5332 4653 4448 5f49 4f46     *pMS2FSDH_IOF
-000084a0: 4c41 4753 2028 7265 636f 7264 2920 7c3d  LAGS (record) |=
-000084b0: 2030 7830 343b 0a20 2069 6620 2879 796a   0x04;.  if (yyj
-000084c0: 736f 6e5f 7074 725f 6765 745f 626f 6f6c  son_ptr_get_bool
-000084d0: 2028 6568 726f 6f74 2c20 222f 4644 534e   (ehroot, "/FDSN
-000084e0: 2f46 6c61 6773 2f53 7461 7274 4f66 5469  /Flags/StartOfTi
-000084f0: 6d65 5365 7269 6573 222c 2026 6865 6164  meSeries", &head
-00008500: 6572 5f62 6f6f 6c65 616e 2920 2626 2068  er_boolean) && h
-00008510: 6561 6465 725f 626f 6f6c 6561 6e29 202f  eader_boolean) /
-00008520: 2a20 4269 7420 3320 2a2f 0a20 2020 202a  * Bit 3 */.    *
-00008530: 704d 5332 4653 4448 5f49 4f46 4c41 4753  pMS2FSDH_IOFLAGS
-00008540: 2028 7265 636f 7264 2920 7c3d 2030 7830   (record) |= 0x0
-00008550: 383b 0a20 2069 6620 2879 796a 736f 6e5f  8;.  if (yyjson_
-00008560: 7074 725f 6765 745f 626f 6f6c 2028 6568  ptr_get_bool (eh
-00008570: 726f 6f74 2c20 222f 4644 534e 2f46 6c61  root, "/FDSN/Fla
-00008580: 6773 2f45 6e64 4f66 5469 6d65 5365 7269  gs/EndOfTimeSeri
-00008590: 6573 222c 2026 6865 6164 6572 5f62 6f6f  es", &header_boo
-000085a0: 6c65 616e 2920 2626 2068 6561 6465 725f  lean) && header_
-000085b0: 626f 6f6c 6561 6e29 202f 2a20 4269 7420  boolean) /* Bit 
-000085c0: 3420 2a2f 0a20 2020 202a 704d 5332 4653  4 */.    *pMS2FS
-000085d0: 4448 5f49 4f46 4c41 4753 2028 7265 636f  DH_IOFLAGS (reco
-000085e0: 7264 2920 7c3d 2030 7831 303b 0a20 2069  rd) |= 0x10;.  i
-000085f0: 6620 286d 7372 2d3e 666c 6167 7320 2620  f (msr->flags & 
-00008600: 3078 3034 2920 2f2a 2042 6974 2035 202a  0x04) /* Bit 5 *
-00008610: 2f0a 2020 2020 2a70 4d53 3246 5344 485f  /.    *pMS2FSDH_
-00008620: 494f 464c 4147 5320 2872 6563 6f72 6429  IOFLAGS (record)
-00008630: 207c 3d20 3078 3230 3b0a 0a20 202f 2a20   |= 0x20;..  /* 
-00008640: 4d61 7020 6461 7461 2071 7561 6c69 7479  Map data quality
-00008650: 2062 6974 2066 6c61 6773 202a 2f0a 2020   bit flags */.  
-00008660: 2a70 4d53 3246 5344 485f 4451 464c 4147  *pMS2FSDH_DQFLAG
-00008670: 5320 2872 6563 6f72 6429 203d 2030 3b0a  S (record) = 0;.
-00008680: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-00008690: 5f67 6574 5f62 6f6f 6c20 2865 6872 6f6f  _get_bool (ehroo
-000086a0: 742c 2022 2f46 4453 4e2f 466c 6167 732f  t, "/FDSN/Flags/
-000086b0: 416d 706c 6966 6965 7253 6174 7572 6174  AmplifierSaturat
-000086c0: 696f 6e22 2c20 2668 6561 6465 725f 626f  ion", &header_bo
-000086d0: 6f6c 6561 6e29 2026 2620 6865 6164 6572  olean) && header
-000086e0: 5f62 6f6f 6c65 616e 2920 2f2a 2042 6974  _boolean) /* Bit
-000086f0: 2030 202a 2f0a 2020 2020 2a70 4d53 3246   0 */.    *pMS2F
-00008700: 5344 485f 4451 464c 4147 5320 2872 6563  SDH_DQFLAGS (rec
-00008710: 6f72 6429 207c 3d20 3078 3031 3b0a 2020  ord) |= 0x01;.  
-00008720: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
-00008730: 6574 5f62 6f6f 6c20 2865 6872 6f6f 742c  et_bool (ehroot,
-00008740: 2022 2f46 4453 4e2f 466c 6167 732f 4469   "/FDSN/Flags/Di
-00008750: 6769 7469 7a65 7243 6c69 7070 696e 6722  gitizerClipping"
-00008760: 2c20 2668 6561 6465 725f 626f 6f6c 6561  , &header_boolea
-00008770: 6e29 2026 2620 6865 6164 6572 5f62 6f6f  n) && header_boo
-00008780: 6c65 616e 2920 2f2a 2042 6974 2031 202a  lean) /* Bit 1 *
-00008790: 2f0a 2020 2020 2a70 4d53 3246 5344 485f  /.    *pMS2FSDH_
-000087a0: 4451 464c 4147 5320 2872 6563 6f72 6429  DQFLAGS (record)
-000087b0: 207c 3d20 3078 3032 3b0a 2020 6966 2028   |= 0x02;.  if (
-000087c0: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f62  yyjson_ptr_get_b
-000087d0: 6f6f 6c20 2865 6872 6f6f 742c 2022 2f46  ool (ehroot, "/F
-000087e0: 4453 4e2f 466c 6167 732f 5370 696b 6573  DSN/Flags/Spikes
-000087f0: 222c 2026 6865 6164 6572 5f62 6f6f 6c65  ", &header_boole
-00008800: 616e 2920 2626 2068 6561 6465 725f 626f  an) && header_bo
-00008810: 6f6c 6561 6e29 202f 2a20 4269 7420 3220  olean) /* Bit 2 
-00008820: 2a2f 0a20 2020 202a 704d 5332 4653 4448  */.    *pMS2FSDH
-00008830: 5f44 5146 4c41 4753 2028 7265 636f 7264  _DQFLAGS (record
-00008840: 2920 7c3d 2030 7830 343b 0a20 2069 6620  ) |= 0x04;.  if 
-00008850: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
-00008860: 626f 6f6c 2028 6568 726f 6f74 2c20 222f  bool (ehroot, "/
-00008870: 4644 534e 2f46 6c61 6773 2f47 6c69 7463  FDSN/Flags/Glitc
-00008880: 6865 7322 2c20 2668 6561 6465 725f 626f  hes", &header_bo
-00008890: 6f6c 6561 6e29 2026 2620 6865 6164 6572  olean) && header
-000088a0: 5f62 6f6f 6c65 616e 2920 2f2a 2042 6974  _boolean) /* Bit
-000088b0: 2033 202a 2f0a 2020 2020 2a70 4d53 3246   3 */.    *pMS2F
-000088c0: 5344 485f 4451 464c 4147 5320 2872 6563  SDH_DQFLAGS (rec
-000088d0: 6f72 6429 207c 3d20 3078 3038 3b0a 2020  ord) |= 0x08;.  
-000088e0: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
-000088f0: 6574 5f62 6f6f 6c20 2865 6872 6f6f 742c  et_bool (ehroot,
-00008900: 2022 2f46 4453 4e2f 466c 6167 732f 4d69   "/FDSN/Flags/Mi
-00008910: 7373 696e 6744 6174 6122 2c20 2668 6561  ssingData", &hea
-00008920: 6465 725f 626f 6f6c 6561 6e29 2026 2620  der_boolean) && 
-00008930: 6865 6164 6572 5f62 6f6f 6c65 616e 2920  header_boolean) 
-00008940: 2f2a 2042 6974 2034 202a 2f0a 2020 2020  /* Bit 4 */.    
-00008950: 2a70 4d53 3246 5344 485f 4451 464c 4147  *pMS2FSDH_DQFLAG
-00008960: 5320 2872 6563 6f72 6429 207c 3d20 3078  S (record) |= 0x
-00008970: 3130 3b0a 2020 6966 2028 7979 6a73 6f6e  10;.  if (yyjson
-00008980: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
-00008990: 6872 6f6f 742c 2022 2f46 4453 4e2f 466c  hroot, "/FDSN/Fl
-000089a0: 6167 732f 5465 6c65 6d65 7472 7953 796e  ags/TelemetrySyn
-000089b0: 6345 7272 6f72 222c 2026 6865 6164 6572  cError", &header
-000089c0: 5f62 6f6f 6c65 616e 2920 2626 2068 6561  _boolean) && hea
-000089d0: 6465 725f 626f 6f6c 6561 6e29 202f 2a20  der_boolean) /* 
-000089e0: 4269 7420 3520 2a2f 0a20 2020 202a 704d  Bit 5 */.    *pM
-000089f0: 5332 4653 4448 5f44 5146 4c41 4753 2028  S2FSDH_DQFLAGS (
-00008a00: 7265 636f 7264 2920 7c3d 2030 7832 303b  record) |= 0x20;
-00008a10: 0a20 2069 6620 2879 796a 736f 6e5f 7074  .  if (yyjson_pt
-00008a20: 725f 6765 745f 626f 6f6c 2028 6568 726f  r_get_bool (ehro
-00008a30: 6f74 2c20 222f 4644 534e 2f46 6c61 6773  ot, "/FDSN/Flags
-00008a40: 2f46 696c 7465 7243 6861 7267 696e 6722  /FilterCharging"
-00008a50: 2c20 2668 6561 6465 725f 626f 6f6c 6561  , &header_boolea
-00008a60: 6e29 2026 2620 6865 6164 6572 5f62 6f6f  n) && header_boo
-00008a70: 6c65 616e 2920 2f2a 2042 6974 2036 202a  lean) /* Bit 6 *
-00008a80: 2f0a 2020 2020 2a70 4d53 3246 5344 485f  /.    *pMS2FSDH_
-00008a90: 4451 464c 4147 5320 2872 6563 6f72 6429  DQFLAGS (record)
-00008aa0: 207c 3d20 3078 3430 3b0a 2020 6966 2028   |= 0x40;.  if (
-00008ab0: 6d73 722d 3e66 6c61 6773 2026 2030 7830  msr->flags & 0x0
-00008ac0: 3229 202f 2a20 4269 7420 3720 2a2f 0a20  2) /* Bit 7 */. 
-00008ad0: 2020 202a 704d 5332 4653 4448 5f44 5146     *pMS2FSDH_DQF
-00008ae0: 4c41 4753 2028 7265 636f 7264 2920 7c3d  LAGS (record) |=
-00008af0: 2030 7838 303b 0a0a 2020 6966 2028 7979   0x80;..  if (yy
-00008b00: 6a73 6f6e 5f70 7472 5f67 6574 5f6e 756d  json_ptr_get_num
-00008b10: 2028 6568 726f 6f74 2c20 222f 4644 534e   (ehroot, "/FDSN
-00008b20: 2f54 696d 652f 436f 7272 6563 7469 6f6e  /Time/Correction
-00008b30: 222c 2026 6865 6164 6572 5f6e 756d 6265  ", &header_numbe
-00008b40: 7229 290a 2020 7b0a 2020 2020 2a70 4d53  r)).  {.    *pMS
-00008b50: 3246 5344 485f 5449 4d45 434f 5252 4543  2FSDH_TIMECORREC
-00008b60: 5420 2872 6563 6f72 6429 203d 2048 4f34  T (record) = HO4
-00008b70: 6420 2828 696e 7433 325f 7429 2868 6561  d ((int32_t)(hea
-00008b80: 6465 725f 6e75 6d62 6572 202a 2031 3030  der_number * 100
-00008b90: 3030 202b 2030 2e35 292c 2073 7761 7066  00 + 0.5), swapf
-00008ba0: 6c61 6729 3b0a 0a20 2020 202f 2a20 5365  lag);..    /* Se
-00008bb0: 7420 7469 6d65 2063 6f72 7265 6374 696f  t time correctio
-00008bc0: 6e20 6170 706c 6965 6420 6269 7420 696e  n applied bit in
-00008bd0: 2061 6374 6976 6974 7920 666c 6167 732e   activity flags.
-00008be0: 0a20 2020 2020 2020 5261 7469 6f6e 616c  .       Rational
-00008bf0: 653a 2056 3320 7265 636f 7264 7320 646f  e: V3 records do
-00008c00: 206e 6f74 2061 6c6c 6f77 2075 6e61 7070   not allow unapp
-00008c10: 6c69 6564 2074 696d 6520 636f 7272 6563  lied time correc
-00008c20: 7469 6f6e 7320 616e 6420 756e 6170 706c  tions and unappl
-00008c30: 6965 640a 2020 2020 2020 2074 696d 6520  ied.       time 
-00008c40: 636f 7272 6563 7469 6f6e 7320 696e 2056  corrections in V
-00008c50: 3220 7265 636f 7264 7320 6172 6520 616c  2 records are al
-00008c60: 7761 7973 2061 7070 6c69 6564 206f 6e20  ways applied on 
-00008c70: 7265 6164 2062 7920 7468 6973 206c 6962  read by this lib
-00008c80: 7261 7279 2e20 2a2f 0a20 2020 202a 704d  rary. */.    *pM
-00008c90: 5332 4653 4448 5f41 4354 464c 4147 5320  S2FSDH_ACTFLAGS 
-00008ca0: 2872 6563 6f72 6429 207c 3d20 3078 3032  (record) |= 0x02
-00008cb0: 3b0a 2020 7d0a 2020 656c 7365 0a20 207b  ;.  }.  else.  {
-00008cc0: 0a20 2020 202a 704d 5332 4653 4448 5f54  .    *pMS2FSDH_T
-00008cd0: 494d 4543 4f52 5245 4354 2028 7265 636f  IMECORRECT (reco
-00008ce0: 7264 2920 3d20 303b 0a20 207d 0a0a 2020  rd) = 0;.  }..  
-00008cf0: 2a70 4d53 3246 5344 485f 4e55 4d42 4c4f  *pMS2FSDH_NUMBLO
-00008d00: 434b 4554 5445 5320 2872 6563 6f72 6429  CKETTES (record)
-00008d10: 2020 203d 2031 3b0a 2020 2a70 4d53 3246     = 1;.  *pMS2F
-00008d20: 5344 485f 4441 5441 4f46 4653 4554 2028  SDH_DATAOFFSET (
-00008d30: 7265 636f 7264 2920 2020 2020 203d 2030  record)      = 0
-00008d40: 3b0a 2020 2a70 4d53 3246 5344 485f 424c  ;.  *pMS2FSDH_BL
-00008d50: 4f43 4b45 5454 454f 4646 5345 5420 2872  OCKETTEOFFSET (r
-00008d60: 6563 6f72 6429 203d 2048 4f32 7520 2834  ecord) = HO2u (4
-00008d70: 382c 2073 7761 7066 6c61 6729 3b0a 0a20  8, swapflag);.. 
-00008d80: 2077 7269 7474 656e 203d 2034 383b 0a0a   written = 48;..
-00008d90: 2020 2f2a 2041 6464 206d 616e 6461 746f    /* Add mandato
-00008da0: 7279 2042 6c6f 636b 6574 7465 2031 3030  ry Blockette 100
-00008db0: 3020 2a2f 0a20 206e 6578 745f 626c 6f63  0 */.  next_bloc
-00008dc0: 6b65 7474 6520 3d20 704d 5332 4231 3030  kette = pMS2B100
-00008dd0: 305f 4e45 5854 2028 7265 636f 7264 202b  0_NEXT (record +
-00008de0: 2077 7269 7474 656e 293b 0a0a 2020 2a70   written);..  *p
-00008df0: 4d53 3242 3130 3030 5f54 5950 4520 2872  MS2B1000_TYPE (r
-00008e00: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
-00008e10: 2020 2020 2020 3d20 484f 3275 2028 3130        = HO2u (10
-00008e20: 3030 2c20 7377 6170 666c 6167 293b 0a20  00, swapflag);. 
-00008e30: 202a 704d 5332 4231 3030 305f 4e45 5854   *pMS2B1000_NEXT
-00008e40: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-00008e50: 656e 2920 2020 2020 203d 2030 3b0a 2020  en)      = 0;.  
-00008e60: 2a70 4d53 3242 3130 3030 5f45 4e43 4f44  *pMS2B1000_ENCOD
-00008e70: 494e 4720 2872 6563 6f72 6420 2b20 7772  ING (record + wr
-00008e80: 6974 7465 6e29 2020 3d20 656e 636f 6469  itten)  = encodi
-00008e90: 6e67 3b0a 2020 2a70 4d53 3242 3130 3030  ng;.  *pMS2B1000
-00008ea0: 5f42 5954 454f 5244 4552 2028 7265 636f  _BYTEORDER (reco
-00008eb0: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
-00008ec0: 313b 0a20 202a 704d 5332 4231 3030 305f  1;.  *pMS2B1000_
-00008ed0: 5245 434c 454e 2028 7265 636f 7264 202b  RECLEN (record +
-00008ee0: 2077 7269 7474 656e 2920 2020 203d 2072   written)    = r
-00008ef0: 6563 6c65 6e65 7870 3b0a 2020 2a70 4d53  eclenexp;.  *pMS
-00008f00: 3242 3130 3030 5f52 4553 4552 5645 4420  2B1000_RESERVED 
-00008f10: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-00008f20: 6e29 2020 3d20 303b 0a0a 2020 7772 6974  n)  = 0;..  writ
-00008f30: 7465 6e20 2b3d 2038 3b0a 0a20 202f 2a20  ten += 8;..  /* 
-00008f40: 4164 6420 426c 6f63 6b65 7474 6520 3130  Add Blockette 10
-00008f50: 3031 2069 6620 6d69 6372 6f73 6563 6f6e  01 if microsecon
-00008f60: 6420 6f66 6673 6574 206f 7220 7469 6d69  d offset or timi
-00008f70: 6e67 2071 7561 6c69 7479 2069 7320 7072  ng quality is pr
-00008f80: 6573 656e 7420 2a2f 0a20 2069 6620 2879  esent */.  if (y
-00008f90: 796a 736f 6e5f 7074 725f 6765 745f 7569  yjson_ptr_get_ui
-00008fa0: 6e74 2028 6568 726f 6f74 2c20 222f 4644  nt (ehroot, "/FD
-00008fb0: 534e 2f54 696d 652f 5175 616c 6974 7922  SN/Time/Quality"
-00008fc0: 2c20 2668 6561 6465 725f 7569 6e74 2920  , &header_uint) 
-00008fd0: 7c7c 206d 7365 635f 6f66 6673 6574 290a  || msec_offset).
-00008fe0: 2020 7b0a 2020 2020 2a6e 6578 745f 626c    {.    *next_bl
-00008ff0: 6f63 6b65 7474 6520 3d20 484f 3275 2028  ockette = HO2u (
-00009000: 2875 696e 7431 365f 7429 7772 6974 7465  (uint16_t)writte
-00009010: 6e2c 2073 7761 7066 6c61 6729 3b0a 2020  n, swapflag);.  
-00009020: 2020 6e65 7874 5f62 6c6f 636b 6574 7465    next_blockette
-00009030: 203d 2070 4d53 3242 3130 3031 5f4e 4558   = pMS2B1001_NEX
-00009040: 5420 2872 6563 6f72 6420 2b20 7772 6974  T (record + writ
-00009050: 7465 6e29 3b0a 2020 2020 2a70 4d53 3246  ten);.    *pMS2F
-00009060: 5344 485f 4e55 4d42 4c4f 434b 4554 5445  SDH_NUMBLOCKETTE
-00009070: 5320 2872 6563 6f72 6429 202b 3d20 313b  S (record) += 1;
-00009080: 0a0a 2020 2020 2a70 4d53 3242 3130 3031  ..    *pMS2B1001
-00009090: 5f54 5950 4520 2872 6563 6f72 6420 2b20  _TYPE (record + 
-000090a0: 7772 6974 7465 6e29 203d 2048 4f32 7520  written) = HO2u 
-000090b0: 2831 3030 312c 2073 7761 7066 6c61 6729  (1001, swapflag)
-000090c0: 3b0a 2020 2020 2a70 4d53 3242 3130 3031  ;.    *pMS2B1001
-000090d0: 5f4e 4558 5420 2872 6563 6f72 6420 2b20  _NEXT (record + 
-000090e0: 7772 6974 7465 6e29 203d 2030 3b0a 0a20  written) = 0;.. 
-000090f0: 2020 2069 6620 2879 796a 736f 6e5f 7074     if (yyjson_pt
-00009100: 725f 6765 745f 7569 6e74 2028 6568 726f  r_get_uint (ehro
-00009110: 6f74 2c20 222f 4644 534e 2f54 696d 652f  ot, "/FDSN/Time/
-00009120: 5175 616c 6974 7922 2c20 2668 6561 6465  Quality", &heade
-00009130: 725f 7569 6e74 2920 2626 2068 6561 6465  r_uint) && heade
-00009140: 725f 7569 6e74 203c 3d20 5549 4e54 385f  r_uint <= UINT8_
-00009150: 4d41 5829 0a20 2020 2020 202a 704d 5332  MAX).      *pMS2
-00009160: 4231 3030 315f 5449 4d49 4e47 5155 414c  B1001_TIMINGQUAL
-00009170: 4954 5920 2872 6563 6f72 6420 2b20 7772  ITY (record + wr
-00009180: 6974 7465 6e29 203d 2028 7569 6e74 385f  itten) = (uint8_
-00009190: 7429 2028 6865 6164 6572 5f75 696e 7429  t) (header_uint)
-000091a0: 3b0a 2020 2020 656c 7365 0a20 2020 2020  ;.    else.     
-000091b0: 202a 704d 5332 4231 3030 315f 5449 4d49   *pMS2B1001_TIMI
-000091c0: 4e47 5155 414c 4954 5920 2872 6563 6f72  NGQUALITY (recor
-000091d0: 6420 2b20 7772 6974 7465 6e29 203d 2030  d + written) = 0
-000091e0: 3b0a 0a20 2020 202a 704d 5332 4231 3030  ;..    *pMS2B100
-000091f0: 315f 4d49 4352 4f53 4543 4f4e 4420 2872  1_MICROSECOND (r
-00009200: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
-00009210: 203d 206d 7365 635f 6f66 6673 6574 3b0a   = msec_offset;.
-00009220: 2020 2020 2a70 4d53 3242 3130 3031 5f52      *pMS2B1001_R
-00009230: 4553 4552 5645 4420 2872 6563 6f72 6420  ESERVED (record 
-00009240: 2b20 7772 6974 7465 6e29 2020 2020 3d20  + written)    = 
-00009250: 303b 0a20 2020 202a 704d 5332 4231 3030  0;.    *pMS2B100
-00009260: 315f 4652 414d 4543 4f55 4e54 2028 7265  1_FRAMECOUNT (re
-00009270: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
-00009280: 203d 2030 3b0a 0a20 2020 2077 7269 7474   = 0;..    writt
-00009290: 656e 202b 3d20 383b 0a20 207d 0a0a 2020  en += 8;.  }..  
-000092a0: 2f2a 2041 6464 2042 6c6f 636b 6574 7465  /* Add Blockette
-000092b0: 2031 3030 2069 6620 7361 6d70 6c65 2072   100 if sample r
-000092c0: 6174 6520 6973 206e 6f74 2077 656c 6c20  ate is not well 
-000092d0: 7265 7072 6573 656e 7465 6420 6279 2066  represented by f
-000092e0: 6163 746f 722f 6d75 6c74 6970 6c69 6572  actor/multiplier
-000092f0: 202a 2f0a 2020 6966 2028 6d73 5f64 6162   */.  if (ms_dab
-00009300: 7328 6d73 7233 5f73 616d 7072 6174 6568  s(msr3_samprateh
-00009310: 7a28 6d73 7229 202d 206d 735f 6e6f 6d73  z(msr) - ms_noms
-00009320: 616d 7072 6174 6528 6661 6374 6f72 2c20  amprate(factor, 
-00009330: 6d75 6c74 6970 6c69 6572 2929 203e 2030  multiplier)) > 0
-00009340: 2e30 3030 3129 0a20 207b 0a20 2020 202a  .0001).  {.    *
-00009350: 6e65 7874 5f62 6c6f 636b 6574 7465 203d  next_blockette =
-00009360: 2048 4f32 7520 2828 7569 6e74 3136 5f74   HO2u ((uint16_t
-00009370: 2977 7269 7474 656e 2c20 7377 6170 666c  )written, swapfl
-00009380: 6167 293b 0a20 2020 206e 6578 745f 626c  ag);.    next_bl
-00009390: 6f63 6b65 7474 6520 3d20 704d 5332 4231  ockette = pMS2B1
-000093a0: 3030 5f4e 4558 5420 2872 6563 6f72 6420  00_NEXT (record 
-000093b0: 2b20 7772 6974 7465 6e29 3b0a 2020 2020  + written);.    
-000093c0: 2a70 4d53 3246 5344 485f 4e55 4d42 4c4f  *pMS2FSDH_NUMBLO
-000093d0: 434b 4554 5445 5320 2872 6563 6f72 6429  CKETTES (record)
-000093e0: 202b 3d20 313b 0a0a 2020 2020 2a70 4d53   += 1;..    *pMS
-000093f0: 3242 3130 305f 5459 5045 2028 7265 636f  2B100_TYPE (reco
-00009400: 7264 202b 2077 7269 7474 656e 2920 2020  rd + written)   
-00009410: 2020 3d20 484f 3275 2028 3130 302c 2073    = HO2u (100, s
-00009420: 7761 7066 6c61 6729 3b0a 2020 2020 2a70  wapflag);.    *p
-00009430: 4d53 3242 3130 305f 4e45 5854 2028 7265  MS2B100_NEXT (re
-00009440: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
-00009450: 2020 2020 3d20 303b 0a20 2020 202a 704d      = 0;.    *pM
-00009460: 5332 4231 3030 5f53 414d 5052 4154 4520  S2B100_SAMPRATE 
-00009470: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-00009480: 6e29 203d 2048 4f34 6620 2828 666c 6f61  n) = HO4f ((floa
-00009490: 7429 6d73 722d 3e73 616d 7072 6174 652c  t)msr->samprate,
-000094a0: 2073 7761 7066 6c61 6729 3b0a 2020 2020   swapflag);.    
-000094b0: 2a70 4d53 3242 3130 305f 464c 4147 5320  *pMS2B100_FLAGS 
-000094c0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-000094d0: 6e29 2020 2020 3d20 303b 0a20 2020 206d  n)    = 0;.    m
-000094e0: 656d 7365 7420 2870 4d53 3242 3130 305f  emset (pMS2B100_
-000094f0: 5245 5345 5256 4544 2028 7265 636f 7264  RESERVED (record
-00009500: 202b 2077 7269 7474 656e 292c 2030 2c20   + written), 0, 
-00009510: 3329 3b0a 0a20 2020 2077 7269 7474 656e  3);..    written
-00009520: 202b 3d20 3132 3b0a 2020 7d0a 0a20 202f   += 12;.  }..  /
-00009530: 2a20 4164 6420 426c 6f63 6b65 7474 6520  * Add Blockette 
-00009540: 3530 3020 666f 7220 7469 6d69 6e67 2065  500 for timing e
-00009550: 7865 6365 7074 696f 6e73 202a 2f0a 2020  xeceptions */.  
-00009560: 6966 2028 2865 6861 7272 203d 2079 796a  if ((eharr = yyj
-00009570: 736f 6e5f 7074 725f 6765 7420 2865 6872  son_ptr_get (ehr
-00009580: 6f6f 742c 2022 2f46 4453 4e2f 5469 6d65  oot, "/FDSN/Time
-00009590: 2f45 7863 6570 7469 6f6e 2229 2920 2626  /Exception")) &&
-000095a0: 2079 796a 736f 6e5f 6973 5f61 7272 2028   yyjson_is_arr (
-000095b0: 6568 6172 7229 290a 2020 7b0a 2020 2020  eharr)).  {.    
-000095c0: 7979 6a73 6f6e 5f61 7272 5f69 7465 725f  yyjson_arr_iter_
-000095d0: 696e 6974 2028 6568 6172 722c 2026 6568  init (eharr, &eh
-000095e0: 6974 6572 293b 0a0a 2020 2020 7768 696c  iter);..    whil
-000095f0: 6520 2828 6568 6974 6572 7661 6c20 3d20  e ((ehiterval = 
-00009600: 7979 6a73 6f6e 5f61 7272 5f69 7465 725f  yyjson_arr_iter_
-00009610: 6e65 7874 2028 2665 6869 7465 7229 2929  next (&ehiter)))
-00009620: 0a20 2020 207b 0a20 2020 2020 2069 6620  .    {.      if 
-00009630: 2821 7979 6a73 6f6e 5f69 735f 6f62 6a20  (!yyjson_is_obj 
-00009640: 2865 6869 7465 7276 616c 2929 0a20 2020  (ehiterval)).   
-00009650: 2020 2020 2063 6f6e 7469 6e75 653b 0a0a       continue;..
-00009660: 2020 2020 2020 626c 6f63 6b65 7474 655f        blockette_
-00009670: 6c65 6e67 7468 203d 2032 3030 3b0a 0a20  length = 200;.. 
-00009680: 2020 2020 2069 6620 2828 7265 6362 7566       if ((recbuf
-00009690: 6c65 6e20 2d20 7772 6974 7465 6e29 203c  len - written) <
-000096a0: 2062 6c6f 636b 6574 7465 5f6c 656e 6774   blockette_lengt
-000096b0: 6829 0a20 2020 2020 207b 0a20 2020 2020  h).      {.     
-000096c0: 2020 206d 735f 6c6f 6720 2832 2c20 2225     ms_log (2, "%
-000096d0: 733a 2052 6563 6f72 6420 6c65 6e67 7468  s: Record length
-000096e0: 206e 6f74 206c 6172 6765 2065 6e6f 7567   not large enoug
-000096f0: 6820 666f 7220 4235 3030 5c6e 222c 206d  h for B500\n", m
-00009700: 7372 2d3e 7369 6429 3b0a 2020 2020 2020  sr->sid);.      
-00009710: 2020 7979 6a73 6f6e 5f64 6f63 5f66 7265    yyjson_doc_fre
-00009720: 6520 2865 6864 6f63 293b 0a20 2020 2020  e (ehdoc);.     
-00009730: 2020 2072 6574 7572 6e20 2d31 3b0a 2020     return -1;.  
-00009740: 2020 2020 7d0a 0a20 2020 2020 202a 6e65      }..      *ne
-00009750: 7874 5f62 6c6f 636b 6574 7465 203d 2048  xt_blockette = H
-00009760: 4f32 7520 2828 7569 6e74 3136 5f74 2977  O2u ((uint16_t)w
-00009770: 7269 7474 656e 2c20 7377 6170 666c 6167  ritten, swapflag
-00009780: 293b 0a20 2020 2020 206e 6578 745f 626c  );.      next_bl
-00009790: 6f63 6b65 7474 6520 203d 2070 4d53 3242  ockette  = pMS2B
-000097a0: 3530 305f 4e45 5854 2028 7265 636f 7264  500_NEXT (record
-000097b0: 202b 2077 7269 7474 656e 293b 0a20 2020   + written);.   
-000097c0: 2020 202a 704d 5332 4653 4448 5f4e 554d     *pMS2FSDH_NUM
-000097d0: 424c 4f43 4b45 5454 4553 2028 7265 636f  BLOCKETTES (reco
-000097e0: 7264 2920 2b3d 2031 3b0a 0a20 2020 2020  rd) += 1;..     
-000097f0: 206d 656d 7365 7420 2872 6563 6f72 6420   memset (record 
-00009800: 2b20 7772 6974 7465 6e2c 2030 2c20 626c  + written, 0, bl
-00009810: 6f63 6b65 7474 655f 6c65 6e67 7468 293b  ockette_length);
-00009820: 0a20 2020 2020 202a 704d 5332 4235 3030  .      *pMS2B500
-00009830: 5f54 5950 4520 2872 6563 6f72 6420 2b20  _TYPE (record + 
-00009840: 7772 6974 7465 6e29 203d 2048 4f32 7520  written) = HO2u 
-00009850: 2835 3030 2c20 7377 6170 666c 6167 293b  (500, swapflag);
-00009860: 0a20 2020 2020 202a 704d 5332 4235 3030  .      *pMS2B500
-00009870: 5f4e 4558 5420 2872 6563 6f72 6420 2b20  _NEXT (record + 
-00009880: 7772 6974 7465 6e29 203d 2030 3b0a 0a20  written) = 0;.. 
-00009890: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
-000098a0: 7074 725f 6765 745f 6e75 6d20 2865 6869  ptr_get_num (ehi
-000098b0: 7465 7276 616c 2c20 222f 5643 4f43 6f72  terval, "/VCOCor
-000098c0: 7265 6374 696f 6e22 2c20 2668 6561 6465  rection", &heade
-000098d0: 725f 6e75 6d62 6572 2929 0a20 2020 2020  r_number)).     
-000098e0: 2020 202a 704d 5332 4235 3030 5f56 434f     *pMS2B500_VCO
-000098f0: 434f 5252 4543 5449 4f4e 2028 7265 636f  CORRECTION (reco
-00009900: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
-00009910: 484f 3466 2028 2866 6c6f 6174 2968 6561  HO4f ((float)hea
-00009920: 6465 725f 6e75 6d62 6572 2c20 7377 6170  der_number, swap
-00009930: 666c 6167 293b 0a0a 2020 2020 2020 6966  flag);..      if
-00009940: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
-00009950: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
-00009960: 2022 2f54 696d 6522 2c20 2668 6561 6465   "/Time", &heade
-00009970: 725f 7374 7269 6e67 2929 0a20 2020 2020  r_string)).     
-00009980: 207b 0a20 2020 2020 2020 2069 6e74 3634   {.        int64
-00009990: 5f74 206c 5f6e 7365 633b 0a20 2020 2020  _t l_nsec;.     
-000099a0: 2020 2075 696e 7431 365f 7420 6c5f 6673     uint16_t l_fs
-000099b0: 6563 3b0a 2020 2020 2020 2020 696e 7438  ec;.        int8
-000099c0: 5f74 206c 5f6d 7365 635f 6f66 6673 6574  _t l_msec_offset
-000099d0: 3b0a 0a20 2020 2020 2020 206c 5f6e 7365  ;..        l_nse
-000099e0: 6320 3d20 6d73 5f74 696d 6573 7472 3262  c = ms_timestr2b
-000099f0: 7469 6d65 2028 6865 6164 6572 5f73 7472  time (header_str
-00009a00: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a20: 2020 2020 2020 2020 2875 696e 7438 5f74          (uint8_t
-00009a30: 202a 2970 4d53 3242 3530 305f 5945 4152   *)pMS2B500_YEAR
-00009a40: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-00009a50: 656e 292c 0a20 2020 2020 2020 2020 2020  en),.           
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 6d73 722d 3e73 6964          msr->sid
-00009a80: 2c20 7377 6170 666c 6167 293b 0a0a 2020  , swapflag);..  
-00009a90: 2020 2020 2020 6966 2028 6c5f 6e73 6563        if (l_nsec
-00009aa0: 203d 3d20 2d31 290a 2020 2020 2020 2020   == -1).        
-00009ab0: 7b0a 2020 2020 2020 2020 2020 6d73 5f6c  {.          ms_l
-00009ac0: 6f67 2028 322c 2022 2573 3a20 4361 6e6e  og (2, "%s: Cann
-00009ad0: 6f74 2063 6f6e 7665 7274 2042 3530 3020  ot convert B500 
-00009ae0: 7469 6d65 3a20 2573 5c6e 222c 206d 7372  time: %s\n", msr
-00009af0: 2d3e 7369 642c 2068 6561 6465 725f 7374  ->sid, header_st
-00009b00: 7269 6e67 293b 0a20 2020 2020 2020 2020  ring);.         
-00009b10: 2079 796a 736f 6e5f 646f 635f 6672 6565   yyjson_doc_free
-00009b20: 2028 6568 646f 6329 3b0a 2020 2020 2020   (ehdoc);.      
-00009b30: 2020 2020 7265 7475 726e 202d 313b 0a20      return -1;. 
-00009b40: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00009b50: 2020 2f2a 2043 616c 6375 6c61 7465 2074    /* Calculate t
-00009b60: 696d 6520 6174 2066 7261 6374 696f 6e61  ime at fractiona
-00009b70: 6c20 3130 3075 7365 6320 7265 736f 6c75  l 100usec resolu
-00009b80: 7469 6f6e 2061 6e64 206d 6963 726f 7365  tion and microse
-00009b90: 636f 6e64 206f 6666 7365 7420 2a2f 0a20  cond offset */. 
-00009ba0: 2020 2020 2020 206c 5f66 7365 6320 2020         l_fsec   
-00009bb0: 2020 2020 203d 2028 7569 6e74 3136 5f74       = (uint16_t
-00009bc0: 2928 6c5f 6e73 6563 202f 2031 3030 3030  )(l_nsec / 10000
-00009bd0: 3029 3b0a 2020 2020 2020 2020 6c5f 6d73  0);.        l_ms
-00009be0: 6563 5f6f 6666 7365 7420 3d20 2869 6e74  ec_offset = (int
-00009bf0: 385f 7429 2828 6c5f 6e73 6563 202f 2031  8_t)((l_nsec / 1
-00009c00: 3030 3029 202d 2028 6c5f 6673 6563 202a  000) - (l_fsec *
-00009c10: 2031 3030 2929 3b0a 0a20 2020 2020 2020   100));..       
-00009c20: 202a 704d 5332 4235 3030 5f4d 4943 524f   *pMS2B500_MICRO
-00009c30: 5345 434f 4e44 2028 7265 636f 7264 202b  SECOND (record +
-00009c40: 2077 7269 7474 656e 2920 3d20 6c5f 6d73   written) = l_ms
-00009c50: 6563 5f6f 6666 7365 743b 0a20 2020 2020  ec_offset;.     
-00009c60: 207d 0a0a 2020 2020 2020 6966 2028 7979   }..      if (yy
-00009c70: 6a73 6f6e 5f70 7472 5f67 6574 5f75 696e  json_ptr_get_uin
-00009c80: 7420 2865 6869 7465 7276 616c 2c20 222f  t (ehiterval, "/
-00009c90: 5265 6365 7074 696f 6e51 7561 6c69 7479  ReceptionQuality
-00009ca0: 222c 2026 6865 6164 6572 5f75 696e 7429  ", &header_uint)
-00009cb0: 2026 2620 6865 6164 6572 5f75 696e 7420   && header_uint 
-00009cc0: 3c3d 2055 494e 5438 5f4d 4158 290a 2020  <= UINT8_MAX).  
-00009cd0: 2020 2020 2020 2a70 4d53 3242 3530 305f        *pMS2B500_
-00009ce0: 5245 4345 5054 494f 4e51 5541 4c49 5459  RECEPTIONQUALITY
-00009cf0: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-00009d00: 656e 2920 3d20 2875 696e 7438 5f74 2968  en) = (uint8_t)h
-00009d10: 6561 6465 725f 7569 6e74 3b0a 0a20 2020  eader_uint;..   
-00009d20: 2020 2069 6620 2879 796a 736f 6e5f 7074     if (yyjson_pt
-00009d30: 725f 6765 745f 7569 6e74 2028 6568 6974  r_get_uint (ehit
-00009d40: 6572 7661 6c2c 2022 2f43 6f75 6e74 222c  erval, "/Count",
-00009d50: 2026 6865 6164 6572 5f75 696e 7429 2026   &header_uint) &
-00009d60: 2620 6865 6164 6572 5f75 696e 7420 3c3d  & header_uint <=
-00009d70: 2055 494e 5433 325f 4d41 5829 0a20 2020   UINT32_MAX).   
-00009d80: 2020 2020 202a 704d 5332 4235 3030 5f45       *pMS2B500_E
-00009d90: 5843 4550 5449 4f4e 434f 554e 5420 2872  XCEPTIONCOUNT (r
-00009da0: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
-00009db0: 203d 2048 4f34 6420 2828 7569 6e74 3332   = HO4d ((uint32
-00009dc0: 5f74 2968 6561 6465 725f 7569 6e74 2c20  _t)header_uint, 
-00009dd0: 7377 6170 666c 6167 293b 0a0a 2020 2020  swapflag);..    
-00009de0: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-00009df0: 5f67 6574 5f73 7472 2028 6568 6974 6572  _get_str (ehiter
-00009e00: 7661 6c2c 2022 2f54 7970 6522 2c20 2668  val, "/Type", &h
-00009e10: 6561 6465 725f 7374 7269 6e67 2929 0a20  eader_string)). 
-00009e20: 2020 2020 2020 206d 735f 7374 726e 6370         ms_strncp
-00009e30: 6f70 656e 2028 704d 5332 4235 3030 5f45  open (pMS2B500_E
-00009e40: 5843 4550 5449 4f4e 5459 5045 2028 7265  XCEPTIONTYPE (re
-00009e50: 636f 7264 202b 2077 7269 7474 656e 292c  cord + written),
-00009e60: 2068 6561 6465 725f 7374 7269 6e67 2c20   header_string, 
-00009e70: 3136 293b 0a0a 2020 2020 2020 6966 2028  16);..      if (
-00009e80: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f73  yyjson_ptr_get_s
-00009e90: 7472 2028 6568 726f 6f74 2c20 222f 4644  tr (ehroot, "/FD
-00009ea0: 534e 2f43 6c6f 636b 2f4d 6f64 656c 222c  SN/Clock/Model",
-00009eb0: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
-00009ec0: 290a 2020 2020 2020 2020 6d73 5f73 7472  ).        ms_str
-00009ed0: 6e63 706f 7065 6e20 2870 4d53 3242 3530  ncpopen (pMS2B50
-00009ee0: 305f 434c 4f43 4b4d 4f44 454c 2028 7265  0_CLOCKMODEL (re
-00009ef0: 636f 7264 202b 2077 7269 7474 656e 292c  cord + written),
-00009f00: 2068 6561 6465 725f 7374 7269 6e67 2c20   header_string, 
-00009f10: 3332 293b 0a0a 2020 2020 2020 6966 2028  32);..      if (
-00009f20: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f73  yyjson_ptr_get_s
-00009f30: 7472 2028 6568 6974 6572 7661 6c2c 2022  tr (ehiterval, "
-00009f40: 2f43 6c6f 636b 5374 6174 7573 222c 2026  /ClockStatus", &
-00009f50: 6865 6164 6572 5f73 7472 696e 6729 290a  header_string)).
-00009f60: 2020 2020 2020 2020 6d73 5f73 7472 6e63          ms_strnc
-00009f70: 706f 7065 6e20 2870 4d53 3242 3530 305f  popen (pMS2B500_
-00009f80: 434c 4f43 4b53 5441 5455 5320 2872 6563  CLOCKSTATUS (rec
-00009f90: 6f72 6420 2b20 7772 6974 7465 6e29 2c20  ord + written), 
-00009fa0: 6865 6164 6572 5f73 7472 696e 672c 2031  header_string, 1
-00009fb0: 3238 293b 0a0a 2020 2020 2020 7772 6974  28);..      writ
-00009fc0: 7465 6e20 2b3d 2062 6c6f 636b 6574 7465  ten += blockette
-00009fd0: 5f6c 656e 6774 683b 0a20 2020 207d 0a20  _length;.    }. 
-00009fe0: 207d 202f 2a20 456e 6420 6966 202f 4644   } /* End if /FD
-00009ff0: 534e 2f54 696d 652f 4578 6365 7074 696f  SN/Time/Exceptio
-0000a000: 6e20 2a2f 0a0a 2020 2f2a 2041 6464 2042  n */..  /* Add B
-0000a010: 6c6f 636b 6574 7465 2032 3030 2c32 3031  lockette 200,201
-0000a020: 2066 6f72 2065 7665 6e74 2064 6574 6563   for event detec
-0000a030: 7469 6f6e 7320 2a2f 0a20 2069 6620 2828  tions */.  if ((
-0000a040: 6568 6172 7220 3d20 7979 6a73 6f6e 5f70  eharr = yyjson_p
-0000a050: 7472 5f67 6574 2028 6568 726f 6f74 2c20  tr_get (ehroot, 
-0000a060: 222f 4644 534e 2f45 7665 6e74 2f44 6574  "/FDSN/Event/Det
-0000a070: 6563 7469 6f6e 2229 2920 2626 2079 796a  ection")) && yyj
-0000a080: 736f 6e5f 6973 5f61 7272 2028 6568 6172  son_is_arr (ehar
-0000a090: 7229 290a 2020 7b0a 2020 2020 7979 6a73  r)).  {.    yyjs
-0000a0a0: 6f6e 5f61 7272 5f69 7465 725f 696e 6974  on_arr_iter_init
-0000a0b0: 2028 6568 6172 722c 2026 6568 6974 6572   (eharr, &ehiter
-0000a0c0: 293b 0a0a 2020 2020 7768 696c 6520 2828  );..    while ((
-0000a0d0: 6568 6974 6572 7661 6c20 3d20 7979 6a73  ehiterval = yyjs
-0000a0e0: 6f6e 5f61 7272 5f69 7465 725f 6e65 7874  on_arr_iter_next
-0000a0f0: 2028 2665 6869 7465 7229 2929 0a20 2020   (&ehiter))).   
-0000a100: 207b 0a20 2020 2020 2069 6620 2821 7979   {.      if (!yy
-0000a110: 6a73 6f6e 5f69 735f 6f62 6a20 2865 6869  json_is_obj (ehi
-0000a120: 7465 7276 616c 2929 0a20 2020 2020 2020  terval)).       
-0000a130: 2063 6f6e 7469 6e75 653b 0a0a 2020 2020   continue;..    
-0000a140: 2020 2f2a 2044 6574 6572 6d69 6e65 2077    /* Determine w
-0000a150: 6869 6368 2064 6574 6563 7469 6f6e 2074  hich detection t
-0000a160: 7970 653a 204d 5552 444f 434b 2076 6572  ype: MURDOCK ver
-0000a170: 7375 7320 7468 6520 6765 6e65 7269 6320  sus the generic 
-0000a180: 7479 7065 202a 2f0a 2020 2020 2020 6966  type */.      if
-0000a190: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
-0000a1a0: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
-0000a1b0: 2022 2f54 7970 6522 2c20 2668 6561 6465   "/Type", &heade
-0000a1c0: 725f 7374 7269 6e67 2920 2626 0a20 2020  r_string) &&.   
-0000a1d0: 2020 2020 2020 2073 7472 6e63 6173 6563         strncasec
-0000a1e0: 6d70 2028 6865 6164 6572 5f73 7472 696e  mp (header_strin
-0000a1f0: 672c 2022 4d55 5244 4f43 4b22 2c20 3729  g, "MURDOCK", 7)
-0000a200: 203d 3d20 3029 0a20 2020 2020 207b 0a20   == 0).      {. 
-0000a210: 2020 2020 2020 2062 6c6f 636b 6574 7465         blockette
-0000a220: 5f74 7970 6520 3d20 3230 313b 0a20 2020  _type = 201;.   
-0000a230: 2020 2020 2062 6c6f 636b 6574 7465 5f6c       blockette_l
-0000a240: 656e 6774 6820 3d20 3630 3b0a 2020 2020  ength = 60;.    
-0000a250: 2020 7d0a 2020 2020 2020 656c 7365 0a20    }.      else. 
-0000a260: 2020 2020 207b 0a20 2020 2020 2020 2062       {.        b
-0000a270: 6c6f 636b 6574 7465 5f74 7970 6520 3d20  lockette_type = 
-0000a280: 3230 303b 0a20 2020 2020 2020 2062 6c6f  200;.        blo
-0000a290: 636b 6574 7465 5f6c 656e 6774 6820 3d20  ckette_length = 
-0000a2a0: 3532 3b0a 2020 2020 2020 7d0a 0a20 2020  52;.      }..   
-0000a2b0: 2020 2069 6620 2828 7265 6362 7566 6c65     if ((recbufle
-0000a2c0: 6e20 2d20 7772 6974 7465 6e29 203c 2062  n - written) < b
-0000a2d0: 6c6f 636b 6574 7465 5f6c 656e 6774 6820  lockette_length 
-0000a2e0: 290a 2020 2020 2020 7b0a 2020 2020 2020  ).      {.      
-0000a2f0: 2020 6d73 5f6c 6f67 2028 322c 2022 2573    ms_log (2, "%s
-0000a300: 3a20 5265 636f 7264 206c 656e 6774 6820  : Record length 
-0000a310: 6e6f 7420 6c61 7267 6520 656e 6f75 6768  not large enough
-0000a320: 2066 6f72 2042 2575 5c6e 222c 206d 7372   for B%u\n", msr
-0000a330: 2d3e 7369 642c 2062 6c6f 636b 6574 7465  ->sid, blockette
-0000a340: 5f74 7970 6529 3b0a 2020 2020 2020 2020  _type);.        
-0000a350: 7979 6a73 6f6e 5f64 6f63 5f66 7265 6520  yyjson_doc_free 
-0000a360: 2865 6864 6f63 293b 0a20 2020 2020 2020  (ehdoc);.       
-0000a370: 2072 6574 7572 6e20 2d31 3b0a 2020 2020   return -1;.    
-0000a380: 2020 7d0a 0a20 2020 2020 202f 2a20 5468    }..      /* Th
-0000a390: 6520 696e 6974 6961 6c20 6669 656c 6473  e initial fields
-0000a3a0: 206f 6620 4232 3030 2061 6e64 2042 3230   of B200 and B20
-0000a3b0: 3120 6172 6520 7468 6520 7361 6d65 202a  1 are the same *
-0000a3c0: 2f0a 2020 2020 2020 2a6e 6578 745f 626c  /.      *next_bl
-0000a3d0: 6f63 6b65 7474 6520 3d20 484f 3275 2028  ockette = HO2u (
-0000a3e0: 2875 696e 7431 365f 7429 7772 6974 7465  (uint16_t)writte
-0000a3f0: 6e2c 2073 7761 7066 6c61 6729 3b0a 2020  n, swapflag);.  
-0000a400: 2020 2020 6e65 7874 5f62 6c6f 636b 6574      next_blocket
-0000a410: 7465 203d 2070 4d53 3242 3230 305f 4e45  te = pMS2B200_NE
-0000a420: 5854 2028 7265 636f 7264 202b 2077 7269  XT (record + wri
-0000a430: 7474 656e 293b 0a20 2020 2020 202a 704d  tten);.      *pM
-0000a440: 5332 4653 4448 5f4e 554d 424c 4f43 4b45  S2FSDH_NUMBLOCKE
-0000a450: 5454 4553 2028 7265 636f 7264 2920 2b3d  TTES (record) +=
-0000a460: 2031 3b0a 0a20 2020 2020 206d 656d 7365   1;..      memse
-0000a470: 7420 2872 6563 6f72 6420 2b20 7772 6974  t (record + writ
-0000a480: 7465 6e2c 2030 2c20 626c 6f63 6b65 7474  ten, 0, blockett
-0000a490: 655f 6c65 6e67 7468 293b 0a20 2020 2020  e_length);.     
-0000a4a0: 202a 704d 5332 4232 3030 5f54 5950 4520   *pMS2B200_TYPE 
-0000a4b0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000a4c0: 6e29 203d 2048 4f32 7520 2862 6c6f 636b  n) = HO2u (block
-0000a4d0: 6574 7465 5f74 7970 652c 2073 7761 7066  ette_type, swapf
-0000a4e0: 6c61 6729 3b0a 2020 2020 2020 2a70 4d53  lag);.      *pMS
-0000a4f0: 3242 3230 305f 4e45 5854 2028 7265 636f  2B200_NEXT (reco
-0000a500: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
-0000a510: 303b 0a0a 2020 2020 2020 6966 2028 7979  0;..      if (yy
-0000a520: 6a73 6f6e 5f70 7472 5f67 6574 5f6e 756d  json_ptr_get_num
-0000a530: 2028 6568 6974 6572 7661 6c2c 2022 2f53   (ehiterval, "/S
-0000a540: 6967 6e61 6c41 6d70 6c69 7475 6465 222c  ignalAmplitude",
-0000a550: 2026 6865 6164 6572 5f6e 756d 6265 7229   &header_number)
-0000a560: 290a 2020 2020 2020 2020 2a70 4d53 3242  ).        *pMS2B
-0000a570: 3230 305f 414d 504c 4954 5544 4520 2872  200_AMPLITUDE (r
-0000a580: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
-0000a590: 203d 2048 4f34 6620 2828 666c 6f61 7429   = HO4f ((float)
-0000a5a0: 6865 6164 6572 5f6e 756d 6265 722c 2073  header_number, s
-0000a5b0: 7761 7066 6c61 6729 3b0a 0a20 2020 2020  wapflag);..     
-0000a5c0: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
-0000a5d0: 6765 745f 6e75 6d20 2865 6869 7465 7276  get_num (ehiterv
-0000a5e0: 616c 2c20 222f 5369 676e 616c 5065 7269  al, "/SignalPeri
-0000a5f0: 6f64 222c 2026 6865 6164 6572 5f6e 756d  od", &header_num
-0000a600: 6265 7229 290a 2020 2020 2020 2020 2a70  ber)).        *p
-0000a610: 4d53 3242 3230 305f 5045 5249 4f44 2028  MS2B200_PERIOD (
-0000a620: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
-0000a630: 2920 3d20 484f 3466 2028 2866 6c6f 6174  ) = HO4f ((float
-0000a640: 2968 6561 6465 725f 6e75 6d62 6572 2c20  )header_number, 
-0000a650: 7377 6170 666c 6167 293b 0a0a 2020 2020  swapflag);..    
-0000a660: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000a670: 5f67 6574 5f6e 756d 2028 6568 6974 6572  _get_num (ehiter
-0000a680: 7661 6c2c 2022 2f42 6163 6b67 726f 756e  val, "/Backgroun
-0000a690: 6445 7374 696d 6174 6522 2c20 2668 6561  dEstimate", &hea
-0000a6a0: 6465 725f 6e75 6d62 6572 2929 0a20 2020  der_number)).   
-0000a6b0: 2020 2020 202a 704d 5332 4232 3030 5f42       *pMS2B200_B
-0000a6c0: 4143 4b47 524f 554e 4445 5354 2028 7265  ACKGROUNDEST (re
-0000a6d0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
-0000a6e0: 3d20 484f 3466 2028 2866 6c6f 6174 2968  = HO4f ((float)h
-0000a6f0: 6561 6465 725f 6e75 6d62 6572 2c20 7377  eader_number, sw
-0000a700: 6170 666c 6167 293b 0a0a 2020 2020 2020  apflag);..      
-0000a710: 2f2a 2044 6574 6572 6d69 6e65 2077 6869  /* Determine whi
-0000a720: 6368 2077 6176 653a 2044 494c 4154 4154  ch wave: DILATAT
-0000a730: 494f 4e20 7665 7273 7573 2028 6173 7375  ION versus (assu
-0000a740: 6d65 6429 2043 4f4d 5052 4553 5349 4f4e  med) COMPRESSION
-0000a750: 202a 2f0a 2020 2020 2020 6966 2028 7979   */.      if (yy
-0000a760: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
-0000a770: 2028 6568 6974 6572 7661 6c2c 2022 2f57   (ehiterval, "/W
-0000a780: 6176 6522 2c20 2668 6561 6465 725f 7374  ave", &header_st
-0000a790: 7269 6e67 2929 0a20 2020 2020 207b 0a20  ring)).      {. 
-0000a7a0: 2020 2020 2020 2069 6620 2873 7472 6e63         if (strnc
-0000a7b0: 6173 6563 6d70 2028 6865 6164 6572 5f73  asecmp (header_s
-0000a7c0: 7472 696e 672c 2022 4449 4c41 5441 5449  tring, "DILATATI
-0000a7d0: 4f4e 222c 2031 3029 203d 3d20 3029 0a20  ON", 10) == 0). 
-0000a7e0: 2020 2020 2020 2020 202a 704d 5332 4232           *pMS2B2
-0000a7f0: 3030 5f46 4c41 4753 2028 7265 636f 7264  00_FLAGS (record
-0000a800: 202b 2077 7269 7474 656e 2920 7c3d 2030   + written) |= 0
-0000a810: 7830 313b 0a20 2020 2020 207d 0a20 2020  x01;.      }.   
-0000a820: 2020 2065 6c73 6520 6966 2028 626c 6f63     else if (bloc
-0000a830: 6b65 7474 655f 7479 7065 203d 3d20 3230  kette_type == 20
-0000a840: 3029 0a20 2020 2020 207b 0a20 2020 2020  0).      {.     
-0000a850: 2020 202a 704d 5332 4232 3030 5f46 4c41     *pMS2B200_FLA
-0000a860: 4753 2028 7265 636f 7264 202b 2077 7269  GS (record + wri
-0000a870: 7474 656e 2920 7c3d 2030 7830 343b 0a20  tten) |= 0x04;. 
-0000a880: 2020 2020 207d 0a0a 2020 2020 2020 6966       }..      if
-0000a890: 2028 626c 6f63 6b65 7474 655f 7479 7065   (blockette_type
-0000a8a0: 203d 3d20 3230 3020 2626 0a20 2020 2020   == 200 &&.     
-0000a8b0: 2020 2020 2079 796a 736f 6e5f 7074 725f       yyjson_ptr_
-0000a8c0: 6765 745f 7374 7220 2865 6869 7465 7276  get_str (ehiterv
-0000a8d0: 616c 2c20 222f 556e 6974 7322 2c20 2668  al, "/Units", &h
-0000a8e0: 6561 6465 725f 7374 7269 6e67 2920 2626  eader_string) &&
-0000a8f0: 0a20 2020 2020 2020 2020 2073 7472 6e63  .          strnc
-0000a900: 6173 6563 6d70 2028 6865 6164 6572 5f73  asecmp (header_s
-0000a910: 7472 696e 672c 2022 434f 554e 5422 2c20  tring, "COUNT", 
-0000a920: 3529 2021 3d20 3029 0a20 2020 2020 2020  5) != 0).       
-0000a930: 202a 704d 5332 4232 3030 5f46 4c41 4753   *pMS2B200_FLAGS
-0000a940: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000a950: 656e 2920 7c3d 2030 7830 323b 0a0a 2020  en) |= 0x02;..  
-0000a960: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
-0000a970: 7472 5f67 6574 5f73 7472 2028 6568 6974  tr_get_str (ehit
-0000a980: 6572 7661 6c2c 2022 2f4f 6e73 6574 5469  erval, "/OnsetTi
-0000a990: 6d65 222c 2026 6865 6164 6572 5f73 7472  me", &header_str
-0000a9a0: 696e 6729 290a 2020 2020 2020 7b0a 2020  ing)).      {.  
-0000a9b0: 2020 2020 2020 6966 2028 6d73 5f74 696d        if (ms_tim
-0000a9c0: 6573 7472 3262 7469 6d65 2028 6865 6164  estr2btime (head
-0000a9d0: 6572 5f73 7472 696e 672c 2028 7569 6e74  er_string, (uint
-0000a9e0: 385f 7420 2a29 704d 5332 4232 3030 5f59  8_t *)pMS2B200_Y
-0000a9f0: 4541 5220 2872 6563 6f72 6420 2b20 7772  EAR (record + wr
-0000aa00: 6974 7465 6e29 2c0a 2020 2020 2020 2020  itten),.        
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2020 2020 2020 6d73 722d 3e73 6964 2c20        msr->sid, 
-0000aa30: 7377 6170 666c 6167 2920 3d3d 202d 3129  swapflag) == -1)
-0000aa40: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-0000aa50: 2020 2020 206d 735f 6c6f 6720 2832 2c20       ms_log (2, 
-0000aa60: 2225 733a 2043 616e 6e6f 7420 636f 6e76  "%s: Cannot conv
-0000aa70: 6572 7420 4225 7520 7469 6d65 3a20 2573  ert B%u time: %s
-0000aa80: 5c6e 222c 206d 7372 2d3e 7369 642c 2062  \n", msr->sid, b
-0000aa90: 6c6f 636b 6574 7465 5f74 7970 652c 2068  lockette_type, h
-0000aaa0: 6561 6465 725f 7374 7269 6e67 293b 0a20  eader_string);. 
-0000aab0: 2020 2020 2020 2020 2079 796a 736f 6e5f           yyjson_
-0000aac0: 646f 635f 6672 6565 2028 6568 646f 6329  doc_free (ehdoc)
-0000aad0: 3b0a 2020 2020 2020 2020 2020 7265 7475  ;.          retu
-0000aae0: 726e 202d 313b 0a20 2020 2020 2020 207d  rn -1;.        }
-0000aaf0: 0a20 2020 2020 207d 0a0a 2020 2020 2020  .      }..      
-0000ab00: 6966 2028 626c 6f63 6b65 7474 655f 7479  if (blockette_ty
-0000ab10: 7065 203d 3d20 3230 3029 0a20 2020 2020  pe == 200).     
-0000ab20: 207b 0a20 2020 2020 2020 2069 6620 2879   {.        if (y
-0000ab30: 796a 736f 6e5f 7074 725f 6765 745f 7374  yjson_ptr_get_st
-0000ab40: 7220 2865 6869 7465 7276 616c 2c20 222f  r (ehiterval, "/
-0000ab50: 4465 7465 6374 6f72 222c 2026 6865 6164  Detector", &head
-0000ab60: 6572 5f73 7472 696e 6729 290a 2020 2020  er_string)).    
-0000ab70: 2020 2020 2020 6d73 5f73 7472 6e63 706f        ms_strncpo
-0000ab80: 7065 6e20 2870 4d53 3242 3230 305f 4445  pen (pMS2B200_DE
-0000ab90: 5445 4354 4f52 2028 7265 636f 7264 202b  TECTOR (record +
-0000aba0: 2077 7269 7474 656e 292c 2068 6561 6465   written), heade
-0000abb0: 725f 7374 7269 6e67 2c20 3234 293b 0a20  r_string, 24);. 
-0000abc0: 2020 2020 207d 0a20 2020 2020 2065 6c73       }.      els
-0000abd0: 6520 2f2a 2042 6c6f 636b 6574 7465 2032  e /* Blockette 2
-0000abe0: 3031 202a 2f0a 2020 2020 2020 7b0a 2020  01 */.      {.  
-0000abf0: 2020 2020 2020 7979 6a73 6f6e 5f76 616c        yyjson_val
-0000ac00: 202a 6568 7375 6261 7272 3b0a 2020 2020   *ehsubarr;.    
-0000ac10: 2020 2020 7979 6a73 6f6e 5f61 7272 5f69      yyjson_arr_i
-0000ac20: 7465 7220 6568 7375 6269 7465 723b 0a20  ter ehsubiter;. 
-0000ac30: 2020 2020 2020 2079 796a 736f 6e5f 7661         yyjson_va
-0000ac40: 6c20 2a65 6873 7562 6974 6572 7661 6c3b  l *ehsubiterval;
-0000ac50: 0a20 2020 2020 2020 2069 6e74 2069 6478  .        int idx
-0000ac60: 203d 2030 3b0a 0a20 2020 2020 2020 2069   = 0;..        i
-0000ac70: 6620 2828 6568 7375 6261 7272 203d 2079  f ((ehsubarr = y
-0000ac80: 796a 736f 6e5f 7074 725f 6765 7420 2865  yjson_ptr_get (e
-0000ac90: 6869 7465 7276 616c 2c20 222f 4d45 4453  hiterval, "/MEDS
-0000aca0: 4e52 2229 2920 2626 2079 796a 736f 6e5f  NR")) && yyjson_
-0000acb0: 6973 5f61 7272 2028 6568 7375 6261 7272  is_arr (ehsubarr
-0000acc0: 2929 0a20 2020 2020 2020 207b 0a20 2020  )).        {.   
-0000acd0: 2020 2020 2020 2079 796a 736f 6e5f 6172         yyjson_ar
-0000ace0: 725f 6974 6572 5f69 6e69 7420 2865 6873  r_iter_init (ehs
-0000acf0: 7562 6172 722c 2026 6568 7375 6269 7465  ubarr, &ehsubite
-0000ad00: 7229 3b0a 0a20 2020 2020 2020 2020 2077  r);..          w
-0000ad10: 6869 6c65 2028 2865 6873 7562 6974 6572  hile ((ehsubiter
-0000ad20: 7661 6c20 3d20 7979 6a73 6f6e 5f61 7272  val = yyjson_arr
-0000ad30: 5f69 7465 725f 6e65 7874 2028 2665 6873  _iter_next (&ehs
-0000ad40: 7562 6974 6572 2929 290a 2020 2020 2020  ubiter))).      
-0000ad50: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-0000ad60: 2020 6966 2028 2179 796a 736f 6e5f 6973    if (!yyjson_is
-0000ad70: 5f6e 756d 2028 6568 7375 6269 7465 7276  _num (ehsubiterv
-0000ad80: 616c 2929 0a20 2020 2020 2020 2020 2020  al)).           
-0000ad90: 2020 2063 6f6e 7469 6e75 653b 0a0a 2020     continue;..  
-0000ada0: 2020 2020 2020 2020 2020 704d 5332 4232            pMS2B2
-0000adb0: 3031 5f4d 4544 534e 5220 2872 6563 6f72  01_MEDSNR (recor
-0000adc0: 6420 2b20 7772 6974 7465 6e29 5b69 6478  d + written)[idx
-0000add0: 2b2b 5d20 3d20 2875 696e 7438 5f74 2979  ++] = (uint8_t)y
-0000ade0: 796a 736f 6e5f 6765 745f 6e75 6d20 2865  yjson_get_num (e
-0000adf0: 6873 7562 6974 6572 7661 6c29 3b0a 2020  hsubiterval);.  
-0000ae00: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0000ae10: 2020 7d0a 0a20 2020 2020 2020 2069 6620    }..        if 
-0000ae20: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
-0000ae30: 7569 6e74 2028 6568 6974 6572 7661 6c2c  uint (ehiterval,
-0000ae40: 2022 2f4d 4544 4c6f 6f6b 6261 636b 222c   "/MEDLookback",
-0000ae50: 2026 6865 6164 6572 5f75 696e 7429 2026   &header_uint) &
-0000ae60: 2620 6865 6164 6572 5f75 696e 7420 3c20  & header_uint < 
-0000ae70: 5549 4e54 385f 4d41 5829 0a20 2020 2020  UINT8_MAX).     
-0000ae80: 2020 2020 202a 704d 5332 4232 3031 5f4c       *pMS2B201_L
-0000ae90: 4f4f 5042 4143 4b20 2872 6563 6f72 6420  OOPBACK (record 
-0000aea0: 2b20 7772 6974 7465 6e29 203d 2028 7569  + written) = (ui
-0000aeb0: 6e74 385f 7429 6865 6164 6572 5f75 696e  nt8_t)header_uin
-0000aec0: 743b 0a0a 2020 2020 2020 2020 6966 2028  t;..        if (
-0000aed0: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f75  yyjson_ptr_get_u
-0000aee0: 696e 7420 2865 6869 7465 7276 616c 2c20  int (ehiterval, 
-0000aef0: 222f 4d45 4450 6963 6b41 6c67 6f72 6974  "/MEDPickAlgorit
-0000af00: 686d 222c 2026 6865 6164 6572 5f75 696e  hm", &header_uin
-0000af10: 7429 2026 2620 6865 6164 6572 5f75 696e  t) && header_uin
-0000af20: 7420 3c20 5549 4e54 385f 4d41 5829 0a20  t < UINT8_MAX). 
-0000af30: 2020 2020 2020 2020 202a 704d 5332 4232           *pMS2B2
-0000af40: 3031 5f50 4943 4b41 4c47 4f52 4954 484d  01_PICKALGORITHM
-0000af50: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000af60: 656e 2920 3d20 2875 696e 7438 5f74 2968  en) = (uint8_t)h
-0000af70: 6561 6465 725f 7569 6e74 3b0a 0a20 2020  eader_uint;..   
-0000af80: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
-0000af90: 7074 725f 6765 745f 7374 7220 2865 6869  ptr_get_str (ehi
-0000afa0: 7465 7276 616c 2c20 222f 4465 7465 6374  terval, "/Detect
-0000afb0: 6f72 222c 2026 6865 6164 6572 5f73 7472  or", &header_str
-0000afc0: 696e 6729 290a 2020 2020 2020 2020 2020  ing)).          
-0000afd0: 6d73 5f73 7472 6e63 706f 7065 6e20 2870  ms_strncpopen (p
-0000afe0: 4d53 3242 3230 315f 4445 5445 4354 4f52  MS2B201_DETECTOR
-0000aff0: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000b000: 656e 292c 2068 6561 6465 725f 7374 7269  en), header_stri
-0000b010: 6e67 2c20 3234 293b 0a20 2020 2020 207d  ng, 24);.      }
-0000b020: 0a0a 2020 2020 2020 7772 6974 7465 6e20  ..      written 
-0000b030: 2b3d 2062 6c6f 636b 6574 7465 5f6c 656e  += blockette_len
-0000b040: 6774 683b 0a20 2020 207d 0a20 207d 202f  gth;.    }.  } /
-0000b050: 2a20 456e 6420 6966 202f 4644 534e 2f45  * End if /FDSN/E
-0000b060: 7665 6e74 2f44 6574 6563 7469 6f6e 202a  vent/Detection *
-0000b070: 2f0a 0a20 202f 2a20 4164 6420 426c 6f63  /..  /* Add Bloc
-0000b080: 6b65 7474 6520 4233 3030 2c20 3331 302c  kette B300, 310,
-0000b090: 2033 3230 2c20 3339 302c 2033 3935 2066   320, 390, 395 f
-0000b0a0: 6f72 2063 616c 6962 7261 7469 6f6e 7320  or calibrations 
-0000b0b0: 2a2f 0a0a 2020 6966 2028 2865 6861 7272  */..  if ((eharr
-0000b0c0: 203d 2079 796a 736f 6e5f 7074 725f 6765   = yyjson_ptr_ge
-0000b0d0: 7420 2865 6872 6f6f 742c 2022 2f46 4453  t (ehroot, "/FDS
-0000b0e0: 4e2f 4361 6c69 6272 6174 696f 6e2f 5365  N/Calibration/Se
-0000b0f0: 7175 656e 6365 2229 2920 2626 2079 796a  quence")) && yyj
-0000b100: 736f 6e5f 6973 5f61 7272 2028 6568 6172  son_is_arr (ehar
-0000b110: 7229 290a 2020 7b0a 2020 2020 7979 6a73  r)).  {.    yyjs
-0000b120: 6f6e 5f61 7272 5f69 7465 725f 696e 6974  on_arr_iter_init
-0000b130: 2028 6568 6172 722c 2026 6568 6974 6572   (eharr, &ehiter
-0000b140: 293b 0a0a 2020 2020 7768 696c 6520 2828  );..    while ((
-0000b150: 6568 6974 6572 7661 6c20 3d20 7979 6a73  ehiterval = yyjs
-0000b160: 6f6e 5f61 7272 5f69 7465 725f 6e65 7874  on_arr_iter_next
-0000b170: 2028 2665 6869 7465 7229 2929 0a20 2020   (&ehiter))).   
-0000b180: 207b 0a20 2020 2020 2069 6620 2821 7979   {.      if (!yy
-0000b190: 6a73 6f6e 5f69 735f 6f62 6a20 2865 6869  json_is_obj (ehi
-0000b1a0: 7465 7276 616c 2929 0a20 2020 2020 2020  terval)).       
-0000b1b0: 2063 6f6e 7469 6e75 653b 0a0a 2020 2020   continue;..    
-0000b1c0: 2020 2f2a 2044 6574 6572 6d69 6e65 2077    /* Determine w
-0000b1d0: 6869 6368 2063 616c 6962 7261 7469 6f6e  hich calibration
-0000b1e0: 2074 7970 653a 2053 5445 502c 2053 494e   type: STEP, SIN
-0000b1f0: 452c 2050 5345 5544 4f52 414e 444f 4d2c  E, PSEUDORANDOM,
-0000b200: 2047 454e 4552 4943 202a 2f0a 2020 2020   GENERIC */.    
-0000b210: 2020 626c 6f63 6b65 7474 655f 7479 7065    blockette_type
-0000b220: 2020 203d 2030 3b0a 2020 2020 2020 626c     = 0;.      bl
-0000b230: 6f63 6b65 7474 655f 6c65 6e67 7468 203d  ockette_length =
-0000b240: 2030 3b0a 2020 2020 2020 6966 2028 7979   0;.      if (yy
-0000b250: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
-0000b260: 2028 6568 6974 6572 7661 6c2c 2022 2f54   (ehiterval, "/T
-0000b270: 7970 6522 2c20 2668 6561 6465 725f 7374  ype", &header_st
-0000b280: 7269 6e67 2929 0a20 2020 2020 207b 0a20  ring)).      {. 
-0000b290: 2020 2020 2020 2069 6620 2873 7472 6e63         if (strnc
-0000b2a0: 6173 6563 6d70 2028 6865 6164 6572 5f73  asecmp (header_s
-0000b2b0: 7472 696e 672c 2022 5354 4550 222c 2034  tring, "STEP", 4
-0000b2c0: 2920 3d3d 2030 290a 2020 2020 2020 2020  ) == 0).        
-0000b2d0: 7b0a 2020 2020 2020 2020 2020 626c 6f63  {.          bloc
-0000b2e0: 6b65 7474 655f 7479 7065 2020 203d 2033  kette_type   = 3
-0000b2f0: 3030 3b0a 2020 2020 2020 2020 2020 626c  00;.          bl
-0000b300: 6f63 6b65 7474 655f 6c65 6e67 7468 203d  ockette_length =
-0000b310: 2036 303b 0a20 2020 2020 2020 207d 0a20   60;.        }. 
-0000b320: 2020 2020 2020 2065 6c73 6520 6966 2028         else if (
-0000b330: 7374 726e 6361 7365 636d 7020 2868 6561  strncasecmp (hea
-0000b340: 6465 725f 7374 7269 6e67 2c20 2253 494e  der_string, "SIN
-0000b350: 4522 2c20 3429 203d 3d20 3029 0a20 2020  E", 4) == 0).   
-0000b360: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-0000b370: 2062 6c6f 636b 6574 7465 5f74 7970 6520   blockette_type 
-0000b380: 2020 3d20 3331 303b 0a20 2020 2020 2020    = 310;.       
-0000b390: 2020 2062 6c6f 636b 6574 7465 5f6c 656e     blockette_len
-0000b3a0: 6774 6820 3d20 3630 3b0a 2020 2020 2020  gth = 60;.      
-0000b3b0: 2020 7d0a 2020 2020 2020 2020 656c 7365    }.        else
-0000b3c0: 2069 6620 2873 7472 6e63 6173 6563 6d70   if (strncasecmp
-0000b3d0: 2028 6865 6164 6572 5f73 7472 696e 672c   (header_string,
-0000b3e0: 2022 5053 4555 444f 5241 4e44 4f4d 222c   "PSEUDORANDOM",
-0000b3f0: 2031 3229 203d 3d20 3029 0a20 2020 2020   12) == 0).     
-0000b400: 2020 207b 0a20 2020 2020 2020 2020 2062     {.          b
-0000b410: 6c6f 636b 6574 7465 5f74 7970 6520 2020  lockette_type   
-0000b420: 3d20 3332 303b 0a20 2020 2020 2020 2020  = 320;.         
-0000b430: 2062 6c6f 636b 6574 7465 5f6c 656e 6774   blockette_lengt
-0000b440: 6820 3d20 3634 3b0a 2020 2020 2020 2020  h = 64;.        
-0000b450: 7d0a 2020 2020 2020 2020 656c 7365 2069  }.        else i
-0000b460: 6620 2873 7472 6e63 6173 6563 6d70 2028  f (strncasecmp (
-0000b470: 6865 6164 6572 5f73 7472 696e 672c 2022  header_string, "
-0000b480: 4745 4e45 5249 4322 2c20 3729 203d 3d20  GENERIC", 7) == 
-0000b490: 3029 0a20 2020 2020 2020 207b 0a20 2020  0).        {.   
-0000b4a0: 2020 2020 2020 2062 6c6f 636b 6574 7465         blockette
-0000b4b0: 5f74 7970 6520 2020 3d20 3339 303b 0a20  _type   = 390;. 
-0000b4c0: 2020 2020 2020 2020 2062 6c6f 636b 6574           blocket
-0000b4d0: 7465 5f6c 656e 6774 6820 3d20 3238 3b0a  te_length = 28;.
-0000b4e0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0000b4f0: 7d0a 2020 2020 2020 656c 7365 2069 6620  }.      else if 
-0000b500: 2879 796a 736f 6e5f 7074 725f 6765 7420  (yyjson_ptr_get 
-0000b510: 2865 6869 7465 7276 616c 2c20 222f 456e  (ehiterval, "/En
-0000b520: 6454 696d 6522 2929 0a20 2020 2020 207b  dTime")).      {
-0000b530: 0a20 2020 2020 2020 2062 6c6f 636b 6574  .        blocket
-0000b540: 7465 5f74 7970 6520 3d20 3339 353b 0a20  te_type = 395;. 
-0000b550: 2020 2020 2020 2062 6c6f 636b 6574 7465         blockette
-0000b560: 5f6c 656e 6774 6820 3d20 3136 3b0a 2020  _length = 16;.  
-0000b570: 2020 2020 7d0a 0a20 2020 2020 2069 6620      }..      if 
-0000b580: 2821 626c 6f63 6b65 7474 655f 7479 7065  (!blockette_type
-0000b590: 207c 7c20 2162 6c6f 636b 6574 7465 5f6c   || !blockette_l
-0000b5a0: 656e 6774 6829 0a20 2020 2020 207b 0a20  ength).      {. 
-0000b5b0: 2020 2020 2020 206d 735f 6c6f 6720 2832         ms_log (2
-0000b5c0: 2c20 2225 733a 2055 6e6b 6e6f 776e 206f  , "%s: Unknown o
-0000b5d0: 7220 756e 7365 7420 2f46 4453 4e2f 4361  r unset /FDSN/Ca
-0000b5e0: 6c69 6272 6174 696f 6e2f 5365 7175 656e  libration/Sequen
-0000b5f0: 6365 2f54 7970 6520 6f72 202f 456e 6454  ce/Type or /EndT
-0000b600: 696d 655c 6e22 2c20 6d73 722d 3e73 6964  ime\n", msr->sid
-0000b610: 293b 0a20 2020 2020 2020 2079 796a 736f  );.        yyjso
-0000b620: 6e5f 646f 635f 6672 6565 2028 6568 646f  n_doc_free (ehdo
-0000b630: 6329 3b0a 2020 2020 2020 2020 7265 7475  c);.        retu
-0000b640: 726e 202d 313b 0a20 2020 2020 207d 0a0a  rn -1;.      }..
-0000b650: 2020 2020 2020 6966 2028 2872 6563 6275        if ((recbu
-0000b660: 666c 656e 202d 2077 7269 7474 656e 2920  flen - written) 
-0000b670: 3c20 626c 6f63 6b65 7474 655f 6c65 6e67  < blockette_leng
-0000b680: 7468 2029 0a20 2020 2020 207b 0a20 2020  th ).      {.   
-0000b690: 2020 2020 206d 735f 6c6f 6720 2832 2c20       ms_log (2, 
-0000b6a0: 2225 733a 2052 6563 6f72 6420 6c65 6e67  "%s: Record leng
-0000b6b0: 7468 206e 6f74 206c 6172 6765 2065 6e6f  th not large eno
-0000b6c0: 7567 6820 666f 7220 4225 755c 6e22 2c20  ugh for B%u\n", 
-0000b6d0: 6d73 722d 3e73 6964 2c20 626c 6f63 6b65  msr->sid, blocke
-0000b6e0: 7474 655f 7479 7065 293b 0a20 2020 2020  tte_type);.     
-0000b6f0: 2020 2079 796a 736f 6e5f 646f 635f 6672     yyjson_doc_fr
-0000b700: 6565 2028 6568 646f 6329 3b0a 2020 2020  ee (ehdoc);.    
-0000b710: 2020 2020 7265 7475 726e 202d 313b 0a20      return -1;. 
-0000b720: 2020 2020 207d 0a0a 2020 2020 2020 6966       }..      if
-0000b730: 2028 626c 6f63 6b65 7474 655f 7479 7065   (blockette_type
-0000b740: 203d 3d20 3330 3020 7c7c 2062 6c6f 636b   == 300 || block
-0000b750: 6574 7465 5f74 7970 6520 3d3d 2033 3130  ette_type == 310
-0000b760: 207c 7c0a 2020 2020 2020 2020 2020 626c   ||.          bl
-0000b770: 6f63 6b65 7474 655f 7479 7065 203d 3d20  ockette_type == 
-0000b780: 3332 3020 7c7c 2062 6c6f 636b 6574 7465  320 || blockette
-0000b790: 5f74 7970 6520 3d3d 2033 3930 290a 2020  _type == 390).  
-0000b7a0: 2020 2020 7b0a 2020 2020 2020 2020 2f2a      {.        /*
-0000b7b0: 2054 6865 2069 6e69 7469 616c 2066 6965   The initial fie
-0000b7c0: 6c64 7320 6f66 2042 3330 302c 2033 3130  lds of B300, 310
-0000b7d0: 2c20 3332 302c 2033 3930 2061 7265 2074  , 320, 390 are t
-0000b7e0: 6865 2073 616d 6520 2a2f 0a20 2020 2020  he same */.     
-0000b7f0: 2020 202a 6e65 7874 5f62 6c6f 636b 6574     *next_blocket
-0000b800: 7465 203d 2048 4f32 7520 2828 7569 6e74  te = HO2u ((uint
-0000b810: 3136 5f74 2977 7269 7474 656e 2c20 7377  16_t)written, sw
-0000b820: 6170 666c 6167 293b 0a20 2020 2020 2020  apflag);.       
-0000b830: 206e 6578 745f 626c 6f63 6b65 7474 6520   next_blockette 
-0000b840: 203d 2070 4d53 3242 3330 305f 4e45 5854   = pMS2B300_NEXT
-0000b850: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000b860: 656e 293b 0a20 2020 2020 2020 202a 704d  en);.        *pM
-0000b870: 5332 4653 4448 5f4e 554d 424c 4f43 4b45  S2FSDH_NUMBLOCKE
-0000b880: 5454 4553 2028 7265 636f 7264 2920 2b3d  TTES (record) +=
-0000b890: 2031 3b0a 0a20 2020 2020 2020 206d 656d   1;..        mem
-0000b8a0: 7365 7420 2872 6563 6f72 6420 2b20 7772  set (record + wr
-0000b8b0: 6974 7465 6e2c 2030 2c20 626c 6f63 6b65  itten, 0, blocke
-0000b8c0: 7474 655f 6c65 6e67 7468 293b 0a20 2020  tte_length);.   
-0000b8d0: 2020 2020 202a 704d 5332 4233 3030 5f54       *pMS2B300_T
-0000b8e0: 5950 4520 2872 6563 6f72 6420 2b20 7772  YPE (record + wr
-0000b8f0: 6974 7465 6e29 203d 2048 4f32 7520 2862  itten) = HO2u (b
-0000b900: 6c6f 636b 6574 7465 5f74 7970 652c 2073  lockette_type, s
-0000b910: 7761 7066 6c61 6729 3b0a 2020 2020 2020  wapflag);.      
-0000b920: 2020 2a70 4d53 3242 3330 305f 4e45 5854    *pMS2B300_NEXT
-0000b930: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000b940: 656e 2920 3d20 303b 0a0a 2020 2020 2020  en) = 0;..      
-0000b950: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000b960: 5f67 6574 5f73 7472 2028 6568 6974 6572  _get_str (ehiter
-0000b970: 7661 6c2c 2022 2f42 6567 696e 5469 6d65  val, "/BeginTime
-0000b980: 222c 2026 6865 6164 6572 5f73 7472 696e  ", &header_strin
-0000b990: 6729 290a 2020 2020 2020 2020 7b0a 2020  g)).        {.  
-0000b9a0: 2020 2020 2020 2020 6966 2028 6d73 5f74          if (ms_t
-0000b9b0: 696d 6573 7472 3262 7469 6d65 2028 6865  imestr2btime (he
-0000b9c0: 6164 6572 5f73 7472 696e 672c 2028 7569  ader_string, (ui
-0000b9d0: 6e74 385f 7420 2a29 704d 5332 4233 3030  nt8_t *)pMS2B300
-0000b9e0: 5f59 4541 5220 2872 6563 6f72 6420 2b20  _YEAR (record + 
-0000b9f0: 7772 6974 7465 6e29 2c0a 2020 2020 2020  written),.      
-0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2020 2020 2020 2020 2020 6d73 722d 3e73            msr->s
-0000ba20: 6964 2c20 7377 6170 666c 6167 2920 3d3d  id, swapflag) ==
-0000ba30: 202d 3129 0a20 2020 2020 2020 2020 207b   -1).          {
-0000ba40: 0a20 2020 2020 2020 2020 2020 206d 735f  .            ms_
-0000ba50: 6c6f 6720 2832 2c20 2225 733a 2043 616e  log (2, "%s: Can
-0000ba60: 6e6f 7420 636f 6e76 6572 7420 4225 7520  not convert B%u 
-0000ba70: 7469 6d65 3a20 2573 5c6e 222c 206d 7372  time: %s\n", msr
-0000ba80: 2d3e 7369 642c 2062 6c6f 636b 6574 7465  ->sid, blockette
-0000ba90: 5f74 7970 652c 2068 6561 6465 725f 7374  _type, header_st
-0000baa0: 7269 6e67 293b 0a20 2020 2020 2020 2020  ring);.         
-0000bab0: 2020 2079 796a 736f 6e5f 646f 635f 6672     yyjson_doc_fr
-0000bac0: 6565 2028 6568 646f 6329 3b0a 2020 2020  ee (ehdoc);.    
-0000bad0: 2020 2020 2020 2020 7265 7475 726e 202d          return -
-0000bae0: 313b 0a20 2020 2020 2020 2020 207d 0a20  1;.          }. 
-0000baf0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0000bb00: 2020 6966 2028 626c 6f63 6b65 7474 655f    if (blockette_
-0000bb10: 7479 7065 203d 3d20 3330 3029 0a20 2020  type == 300).   
-0000bb20: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-0000bb30: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
-0000bb40: 6765 745f 7569 6e74 2028 6568 6974 6572  get_uint (ehiter
-0000bb50: 7661 6c2c 2022 2f53 7465 7073 222c 2026  val, "/Steps", &
-0000bb60: 6865 6164 6572 5f75 696e 7429 2026 2620  header_uint) && 
-0000bb70: 6865 6164 6572 5f75 696e 7420 3c3d 2055  header_uint <= U
-0000bb80: 494e 5438 5f4d 4158 290a 2020 2020 2020  INT8_MAX).      
-0000bb90: 2020 2020 2020 2a70 4d53 3242 3330 305f        *pMS2B300_
-0000bba0: 4e55 4d43 414c 4942 5241 5449 4f4e 5320  NUMCALIBRATIONS 
-0000bbb0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000bbc0: 6e29 203d 2028 7569 6e74 385f 7429 6865  n) = (uint8_t)he
-0000bbd0: 6164 6572 5f75 696e 743b 0a0a 2020 2020  ader_uint;..    
-0000bbe0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
-0000bbf0: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
-0000bc00: 6869 7465 7276 616c 2c20 222f 5374 6570  hiterval, "/Step
-0000bc10: 4669 7273 7450 756c 7365 506f 7369 7469  FirstPulsePositi
-0000bc20: 7665 222c 2026 6865 6164 6572 5f62 6f6f  ve", &header_boo
-0000bc30: 6c65 616e 2920 2626 2068 6561 6465 725f  lean) && header_
-0000bc40: 626f 6f6c 6561 6e29 0a20 2020 2020 2020  boolean).       
-0000bc50: 2020 2020 202a 704d 5332 4233 3030 5f46       *pMS2B300_F
-0000bc60: 4c41 4753 2028 7265 636f 7264 202b 2077  LAGS (record + w
-0000bc70: 7269 7474 656e 2920 7c3d 2030 7830 313b  ritten) |= 0x01;
-0000bc80: 0a0a 2020 2020 2020 2020 2020 6966 2028  ..          if (
-0000bc90: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f62  yyjson_ptr_get_b
-0000bca0: 6f6f 6c20 2865 6869 7465 7276 616c 2c20  ool (ehiterval, 
-0000bcb0: 222f 5374 6570 416c 7465 726e 6174 6553  "/StepAlternateS
-0000bcc0: 6967 6e22 2c20 2668 6561 6465 725f 626f  ign", &header_bo
-0000bcd0: 6f6c 6561 6e29 2026 2620 6865 6164 6572  olean) && header
-0000bce0: 5f62 6f6f 6c65 616e 290a 2020 2020 2020  _boolean).      
-0000bcf0: 2020 2020 2020 2a70 4d53 3242 3330 305f        *pMS2B300_
-0000bd00: 464c 4147 5320 2872 6563 6f72 6420 2b20  FLAGS (record + 
-0000bd10: 7772 6974 7465 6e29 207c 3d20 3078 3032  written) |= 0x02
-0000bd20: 3b0a 0a20 2020 2020 2020 2020 2069 6620  ;..          if 
-0000bd30: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
-0000bd40: 7374 7220 2865 6869 7465 7276 616c 2c20  str (ehiterval, 
-0000bd50: 222f 5472 6967 6765 7222 2c20 2668 6561  "/Trigger", &hea
-0000bd60: 6465 725f 7374 7269 6e67 2920 2626 0a20  der_string) &&. 
-0000bd70: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000bd80: 6e63 6173 6563 6d70 2028 6865 6164 6572  ncasecmp (header
-0000bd90: 5f73 7472 696e 672c 2022 4155 544f 4d41  _string, "AUTOMA
-0000bda0: 5449 4322 2c20 3929 203d 3d20 3029 0a20  TIC", 9) == 0). 
-0000bdb0: 2020 2020 2020 2020 2020 202a 704d 5332             *pMS2
-0000bdc0: 4233 3030 5f46 4c41 4753 2028 7265 636f  B300_FLAGS (reco
-0000bdd0: 7264 202b 2077 7269 7474 656e 2920 7c3d  rd + written) |=
-0000bde0: 2030 7830 343b 0a0a 2020 2020 2020 2020   0x04;..        
-0000bdf0: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000be00: 5f67 6574 5f62 6f6f 6c20 2865 6869 7465  _get_bool (ehite
-0000be10: 7276 616c 2c20 222f 436f 6e74 696e 7565  rval, "/Continue
-0000be20: 6422 2c20 2668 6561 6465 725f 626f 6f6c  d", &header_bool
-0000be30: 6561 6e29 2026 2620 6865 6164 6572 5f62  ean) && header_b
-0000be40: 6f6f 6c65 616e 290a 2020 2020 2020 2020  oolean).        
-0000be50: 2020 2020 2a70 4d53 3242 3330 305f 464c      *pMS2B300_FL
-0000be60: 4147 5320 2872 6563 6f72 6420 2b20 7772  AGS (record + wr
-0000be70: 6974 7465 6e29 207c 3d20 3078 3038 3b0a  itten) |= 0x08;.
-0000be80: 0a20 2020 2020 2020 2020 2069 6620 2879  .          if (y
-0000be90: 796a 736f 6e5f 7074 725f 6765 745f 6e75  yjson_ptr_get_nu
-0000bea0: 6d20 2865 6869 7465 7276 616c 2c20 222f  m (ehiterval, "/
-0000beb0: 4475 7261 7469 6f6e 222c 2026 6865 6164  Duration", &head
-0000bec0: 6572 5f6e 756d 6265 7229 290a 2020 2020  er_number)).    
-0000bed0: 2020 2020 2020 2020 2a70 4d53 3242 3330          *pMS2B30
-0000bee0: 305f 5354 4550 4455 5241 5449 4f4e 2028  0_STEPDURATION (
-0000bef0: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
-0000bf00: 2920 3d20 484f 3475 2028 2875 696e 7433  ) = HO4u ((uint3
-0000bf10: 325f 7429 2868 6561 6465 725f 6e75 6d62  2_t)(header_numb
-0000bf20: 6572 202a 2031 3030 3030 202b 2030 2e35  er * 10000 + 0.5
-0000bf30: 292c 2073 7761 7066 6c61 6729 3b0a 0a20  ), swapflag);.. 
-0000bf40: 2020 2020 2020 2020 2069 6620 2879 796a           if (yyj
-0000bf50: 736f 6e5f 7074 725f 6765 745f 6e75 6d20  son_ptr_get_num 
-0000bf60: 2865 6869 7465 7276 616c 2c20 222f 5374  (ehiterval, "/St
-0000bf70: 6570 4265 7477 6565 6e22 2c20 2668 6561  epBetween", &hea
-0000bf80: 6465 725f 6e75 6d62 6572 2929 0a20 2020  der_number)).   
-0000bf90: 2020 2020 2020 2020 202a 704d 5332 4233           *pMS2B3
-0000bfa0: 3030 5f49 4e54 4552 5641 4c44 5552 4154  00_INTERVALDURAT
-0000bfb0: 494f 4e20 2872 6563 6f72 6420 2b20 7772  ION (record + wr
-0000bfc0: 6974 7465 6e29 203d 2048 4f34 7520 2828  itten) = HO4u ((
-0000bfd0: 7569 6e74 3332 5f74 2928 6865 6164 6572  uint32_t)(header
-0000bfe0: 5f6e 756d 6265 7220 2a20 3130 3030 3020  _number * 10000 
-0000bff0: 2b20 302e 3529 2c20 7377 6170 666c 6167  + 0.5), swapflag
-0000c000: 293b 0a0a 2020 2020 2020 2020 2020 6966  );..          if
-0000c010: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
-0000c020: 5f6e 756d 2028 6568 6974 6572 7661 6c2c  _num (ehiterval,
-0000c030: 2022 2f41 6d70 6c69 7475 6465 222c 2026   "/Amplitude", &
-0000c040: 6865 6164 6572 5f6e 756d 6265 7229 290a  header_number)).
-0000c050: 2020 2020 2020 2020 2020 2020 2a70 4d53              *pMS
-0000c060: 3242 3330 305f 414d 504c 4954 5544 4520  2B300_AMPLITUDE 
-0000c070: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000c080: 6e29 203d 2048 4f34 6620 2828 666c 6f61  n) = HO4f ((floa
-0000c090: 7429 6865 6164 6572 5f6e 756d 6265 722c  t)header_number,
-0000c0a0: 2073 7761 7066 6c61 6729 3b0a 0a20 2020   swapflag);..   
-0000c0b0: 2020 2020 2020 2069 6620 2879 796a 736f         if (yyjso
-0000c0c0: 6e5f 7074 725f 6765 745f 7374 7220 2865  n_ptr_get_str (e
-0000c0d0: 6869 7465 7276 616c 2c20 222f 496e 7075  hiterval, "/Inpu
-0000c0e0: 7443 6861 6e6e 656c 222c 2026 6865 6164  tChannel", &head
-0000c0f0: 6572 5f73 7472 696e 6729 290a 2020 2020  er_string)).    
-0000c100: 2020 2020 2020 2020 6d73 5f73 7472 6e63          ms_strnc
-0000c110: 706f 7065 6e20 2870 4d53 3242 3330 305f  popen (pMS2B300_
-0000c120: 494e 5055 5443 4841 4e4e 454c 2028 7265  INPUTCHANNEL (re
-0000c130: 636f 7264 202b 2077 7269 7474 656e 292c  cord + written),
-0000c140: 2068 6561 6465 725f 7374 7269 6e67 2c20   header_string, 
-0000c150: 3329 3b0a 0a20 2020 2020 2020 2020 2069  3);..          i
-0000c160: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
-0000c170: 745f 6e75 6d20 2865 6869 7465 7276 616c  t_num (ehiterval
-0000c180: 2c20 222f 5265 6665 7265 6e63 6541 6d70  , "/ReferenceAmp
-0000c190: 6c69 7475 6465 222c 2026 6865 6164 6572  litude", &header
-0000c1a0: 5f6e 756d 6265 7229 290a 2020 2020 2020  _number)).      
-0000c1b0: 2020 2020 2020 2a70 4d53 3242 3330 305f        *pMS2B300_
-0000c1c0: 5245 4645 5245 4e43 4541 4d50 4c49 5455  REFERENCEAMPLITU
-0000c1d0: 4445 2028 7265 636f 7264 202b 2077 7269  DE (record + wri
-0000c1e0: 7474 656e 2920 3d20 484f 3475 2028 2875  tten) = HO4u ((u
-0000c1f0: 696e 7433 325f 7429 2868 6561 6465 725f  int32_t)(header_
-0000c200: 6e75 6d62 6572 202b 2030 2e35 292c 2073  number + 0.5), s
-0000c210: 7761 7066 6c61 6729 3b0a 0a20 2020 2020  wapflag);..     
-0000c220: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
-0000c230: 7074 725f 6765 745f 7374 7220 2865 6869  ptr_get_str (ehi
-0000c240: 7465 7276 616c 2c20 222f 436f 7570 6c69  terval, "/Coupli
-0000c250: 6e67 222c 2026 6865 6164 6572 5f73 7472  ng", &header_str
-0000c260: 696e 6729 290a 2020 2020 2020 2020 2020  ing)).          
-0000c270: 2020 6d73 5f73 7472 6e63 706f 7065 6e20    ms_strncpopen 
-0000c280: 2870 4d53 3242 3330 305f 434f 5550 4c49  (pMS2B300_COUPLI
-0000c290: 4e47 2028 7265 636f 7264 202b 2077 7269  NG (record + wri
-0000c2a0: 7474 656e 292c 2068 6561 6465 725f 7374  tten), header_st
-0000c2b0: 7269 6e67 2c20 3132 293b 0a0a 2020 2020  ring, 12);..    
-0000c2c0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
-0000c2d0: 5f70 7472 5f67 6574 5f73 7472 2028 6568  _ptr_get_str (eh
-0000c2e0: 6974 6572 7661 6c2c 2022 2f52 6f6c 6c6f  iterval, "/Rollo
-0000c2f0: 6666 222c 2026 6865 6164 6572 5f73 7472  ff", &header_str
-0000c300: 696e 6729 290a 2020 2020 2020 2020 2020  ing)).          
-0000c310: 2020 6d73 5f73 7472 6e63 706f 7065 6e20    ms_strncpopen 
-0000c320: 2870 4d53 3242 3330 305f 524f 4c4c 4f46  (pMS2B300_ROLLOF
-0000c330: 4620 2872 6563 6f72 6420 2b20 7772 6974  F (record + writ
-0000c340: 7465 6e29 2c20 6865 6164 6572 5f73 7472  ten), header_str
-0000c350: 696e 672c 2031 3229 3b0a 2020 2020 2020  ing, 12);.      
-0000c360: 2020 7d0a 2020 2020 2020 2020 656c 7365    }.        else
-0000c370: 2069 6620 2862 6c6f 636b 6574 7465 5f74   if (blockette_t
-0000c380: 7970 6520 3d3d 2033 3130 290a 2020 2020  ype == 310).    
-0000c390: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-0000c3a0: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
-0000c3b0: 6574 5f73 7472 2028 6568 6974 6572 7661  et_str (ehiterva
-0000c3c0: 6c2c 2022 2f54 7269 6767 6572 222c 2026  l, "/Trigger", &
-0000c3d0: 6865 6164 6572 5f73 7472 696e 6729 2026  header_string) &
-0000c3e0: 260a 2020 2020 2020 2020 2020 2020 2020  &.              
-0000c3f0: 7374 726e 6361 7365 636d 7020 2868 6561  strncasecmp (hea
-0000c400: 6465 725f 7374 7269 6e67 2c20 2241 5554  der_string, "AUT
-0000c410: 4f4d 4154 4943 222c 2039 2920 3d3d 2030  OMATIC", 9) == 0
-0000c420: 290a 2020 2020 2020 2020 2020 2020 2a70  ).            *p
-0000c430: 4d53 3242 3331 305f 464c 4147 5320 2872  MS2B310_FLAGS (r
-0000c440: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
-0000c450: 207c 3d20 3078 3034 3b0a 0a20 2020 2020   |= 0x04;..     
-0000c460: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
-0000c470: 7074 725f 6765 745f 626f 6f6c 2028 6568  ptr_get_bool (eh
-0000c480: 6974 6572 7661 6c2c 2022 2f43 6f6e 7469  iterval, "/Conti
-0000c490: 6e75 6564 222c 2026 6865 6164 6572 5f62  nued", &header_b
-0000c4a0: 6f6f 6c65 616e 2920 2626 2068 6561 6465  oolean) && heade
-0000c4b0: 725f 626f 6f6c 6561 6e29 0a20 2020 2020  r_boolean).     
-0000c4c0: 2020 2020 2020 202a 704d 5332 4233 3130         *pMS2B310
-0000c4d0: 5f46 4c41 4753 2028 7265 636f 7264 202b  _FLAGS (record +
-0000c4e0: 2077 7269 7474 656e 2920 7c3d 2030 7830   written) |= 0x0
-0000c4f0: 383b 0a0a 2020 2020 2020 2020 2020 6966  8;..          if
-0000c500: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
-0000c510: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
-0000c520: 2022 2f41 6d70 6c69 7475 6465 5261 6e67   "/AmplitudeRang
-0000c530: 6522 2c20 2668 6561 6465 725f 7374 7269  e", &header_stri
-0000c540: 6e67 2929 0a20 2020 2020 2020 2020 207b  ng)).          {
-0000c550: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c560: 2873 7472 6e63 6173 6563 6d70 2028 6865  (strncasecmp (he
-0000c570: 6164 6572 5f73 7472 696e 672c 2022 5045  ader_string, "PE
-0000c580: 414b 544f 5045 414b 222c 2031 3029 203d  AKTOPEAK", 10) =
-0000c590: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
-0000c5a0: 2020 202a 704d 5332 4233 3130 5f46 4c41     *pMS2B310_FLA
-0000c5b0: 4753 2028 7265 636f 7264 202b 2077 7269  GS (record + wri
-0000c5c0: 7474 656e 2920 7c3d 2030 7831 303b 0a20  tten) |= 0x10;. 
-0000c5d0: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-0000c5e0: 7472 6e63 6173 6563 6d70 2028 6865 6164  trncasecmp (head
-0000c5f0: 6572 5f73 7472 696e 672c 2022 5a45 524f  er_string, "ZERO
-0000c600: 544f 5045 414b 222c 2031 3029 203d 3d20  TOPEAK", 10) == 
-0000c610: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-0000c620: 202a 704d 5332 4233 3130 5f46 4c41 4753   *pMS2B310_FLAGS
-0000c630: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
-0000c640: 656e 2920 7c3d 2030 7832 303b 0a20 2020  en) |= 0x20;.   
-0000c650: 2020 2020 2020 2020 2069 6620 2873 7472           if (str
-0000c660: 6e63 6173 6563 6d70 2028 6865 6164 6572  ncasecmp (header
-0000c670: 5f73 7472 696e 672c 2022 524d 5322 2c20  _string, "RMS", 
-0000c680: 3329 203d 3d20 3029 0a20 2020 2020 2020  3) == 0).       
-0000c690: 2020 2020 2020 202a 704d 5332 4233 3130         *pMS2B310
-0000c6a0: 5f46 4c41 4753 2028 7265 636f 7264 202b  _FLAGS (record +
-0000c6b0: 2077 7269 7474 656e 2920 7c3d 2030 7834   written) |= 0x4
-0000c6c0: 303b 0a20 2020 2020 2020 2020 207d 0a0a  0;.          }..
-0000c6d0: 2020 2020 2020 2020 2020 6966 2028 7979            if (yy
-0000c6e0: 6a73 6f6e 5f70 7472 5f67 6574 5f6e 756d  json_ptr_get_num
-0000c6f0: 2028 6568 6974 6572 7661 6c2c 2022 2f44   (ehiterval, "/D
-0000c700: 7572 6174 696f 6e22 2c20 2668 6561 6465  uration", &heade
-0000c710: 725f 6e75 6d62 6572 2929 0a20 2020 2020  r_number)).     
-0000c720: 2020 2020 2020 202a 704d 5332 4233 3130         *pMS2B310
-0000c730: 5f44 5552 4154 494f 4e20 2872 6563 6f72  _DURATION (recor
-0000c740: 6420 2b20 7772 6974 7465 6e29 203d 2048  d + written) = H
-0000c750: 4f34 7520 2828 7569 6e74 3332 5f74 2928  O4u ((uint32_t)(
-0000c760: 6865 6164 6572 5f6e 756d 6265 7220 2a20  header_number * 
-0000c770: 3130 3030 3020 2b20 302e 3529 2c20 7377  10000 + 0.5), sw
-0000c780: 6170 666c 6167 293b 0a0a 2020 2020 2020  apflag);..      
-0000c790: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
-0000c7a0: 7472 5f67 6574 5f6e 756d 2028 6568 6974  tr_get_num (ehit
-0000c7b0: 6572 7661 6c2c 2022 2f53 696e 6550 6572  erval, "/SinePer
-0000c7c0: 696f 6422 2c20 2668 6561 6465 725f 6e75  iod", &header_nu
-0000c7d0: 6d62 6572 2929 0a20 2020 2020 2020 2020  mber)).         
-0000c7e0: 2020 202a 704d 5332 4233 3130 5f50 4552     *pMS2B310_PER
-0000c7f0: 494f 4420 2872 6563 6f72 6420 2b20 7772  IOD (record + wr
-0000c800: 6974 7465 6e29 203d 2048 4f34 6620 2828  itten) = HO4f ((
-0000c810: 666c 6f61 7429 6865 6164 6572 5f6e 756d  float)header_num
-0000c820: 6265 722c 2073 7761 7066 6c61 6729 3b0a  ber, swapflag);.
-0000c830: 0a20 2020 2020 2020 2020 2069 6620 2879  .          if (y
-0000c840: 796a 736f 6e5f 7074 725f 6765 745f 6e75  yjson_ptr_get_nu
-0000c850: 6d20 2865 6869 7465 7276 616c 2c20 222f  m (ehiterval, "/
-0000c860: 416d 706c 6974 7564 6522 2c20 2668 6561  Amplitude", &hea
-0000c870: 6465 725f 6e75 6d62 6572 2929 0a20 2020  der_number)).   
-0000c880: 2020 2020 2020 2020 202a 704d 5332 4233           *pMS2B3
-0000c890: 3130 5f41 4d50 4c49 5455 4445 2028 7265  10_AMPLITUDE (re
-0000c8a0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
-0000c8b0: 3d20 484f 3466 2028 2866 6c6f 6174 2968  = HO4f ((float)h
-0000c8c0: 6561 6465 725f 6e75 6d62 6572 2c20 7377  eader_number, sw
-0000c8d0: 6170 666c 6167 293b 0a0a 2020 2020 2020  apflag);..      
-0000c8e0: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
-0000c8f0: 7472 5f67 6574 5f73 7472 2028 6568 6974  tr_get_str (ehit
-0000c900: 6572 7661 6c2c 2022 2f49 6e70 7574 4368  erval, "/InputCh
-0000c910: 616e 6e65 6c22 2c20 2668 6561 6465 725f  annel", &header_
-0000c920: 7374 7269 6e67 2929 0a20 2020 2020 2020  string)).       
-0000c930: 2020 2020 206d 735f 7374 726e 6370 6f70       ms_strncpop
-0000c940: 656e 2028 704d 5332 4233 3130 5f49 4e50  en (pMS2B310_INP
-0000c950: 5554 4348 414e 4e45 4c20 2872 6563 6f72  UTCHANNEL (recor
-0000c960: 6420 2b20 7772 6974 7465 6e29 2c20 6865  d + written), he
-0000c970: 6164 6572 5f73 7472 696e 672c 2033 293b  ader_string, 3);
-0000c980: 0a0a 2020 2020 2020 2020 2020 6966 2028  ..          if (
-0000c990: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f6e  yyjson_ptr_get_n
-0000c9a0: 756d 2028 6568 6974 6572 7661 6c2c 2022  um (ehiterval, "
-0000c9b0: 2f52 6566 6572 656e 6365 416d 706c 6974  /ReferenceAmplit
-0000c9c0: 7564 6522 2c20 2668 6561 6465 725f 6e75  ude", &header_nu
-0000c9d0: 6d62 6572 2929 0a20 2020 2020 2020 2020  mber)).         
-0000c9e0: 2020 202a 704d 5332 4233 3130 5f52 4546     *pMS2B310_REF
-0000c9f0: 4552 454e 4345 414d 504c 4954 5544 4520  ERENCEAMPLITUDE 
-0000ca00: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000ca10: 6e29 203d 2048 4f34 7520 2828 7569 6e74  n) = HO4u ((uint
-0000ca20: 3332 5f74 2928 6865 6164 6572 5f6e 756d  32_t)(header_num
-0000ca30: 6265 7220 2b20 302e 3529 2c20 7377 6170  ber + 0.5), swap
-0000ca40: 666c 6167 293b 0a0a 2020 2020 2020 2020  flag);..        
-0000ca50: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000ca60: 5f67 6574 5f73 7472 2028 6568 6974 6572  _get_str (ehiter
-0000ca70: 7661 6c2c 2022 2f43 6f75 706c 696e 6722  val, "/Coupling"
-0000ca80: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
-0000ca90: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
-0000caa0: 735f 7374 726e 6370 6f70 656e 2028 704d  s_strncpopen (pM
-0000cab0: 5332 4233 3130 5f43 4f55 504c 494e 4720  S2B310_COUPLING 
-0000cac0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000cad0: 6e29 2c20 6865 6164 6572 5f73 7472 696e  n), header_strin
-0000cae0: 672c 2031 3229 3b0a 0a20 2020 2020 2020  g, 12);..       
-0000caf0: 2020 2069 6620 2879 796a 736f 6e5f 7074     if (yyjson_pt
-0000cb00: 725f 6765 745f 7374 7220 2865 6869 7465  r_get_str (ehite
-0000cb10: 7276 616c 2c20 222f 526f 6c6c 6f66 6622  rval, "/Rolloff"
-0000cb20: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
-0000cb30: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
-0000cb40: 735f 7374 726e 6370 6f70 656e 2028 704d  s_strncpopen (pM
-0000cb50: 5332 4233 3130 5f52 4f4c 4c4f 4646 2028  S2B310_ROLLOFF (
-0000cb60: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
-0000cb70: 292c 2068 6561 6465 725f 7374 7269 6e67  ), header_string
-0000cb80: 2c20 3132 293b 0a20 2020 2020 2020 207d  , 12);.        }
-0000cb90: 0a20 2020 2020 2020 2065 6c73 6520 6966  .        else if
-0000cba0: 2028 626c 6f63 6b65 7474 655f 7479 7065   (blockette_type
-0000cbb0: 203d 3d20 3332 3029 0a20 2020 2020 2020   == 320).       
-0000cbc0: 207b 0a20 2020 2020 2020 2020 2069 6620   {.          if 
-0000cbd0: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
-0000cbe0: 7374 7220 2865 6869 7465 7276 616c 2c20  str (ehiterval, 
-0000cbf0: 222f 5472 6967 6765 7222 2c20 2668 6561  "/Trigger", &hea
-0000cc00: 6465 725f 7374 7269 6e67 2920 2626 0a20  der_string) &&. 
-0000cc10: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000cc20: 6e63 6173 6563 6d70 2028 6865 6164 6572  ncasecmp (header
-0000cc30: 5f73 7472 696e 672c 2022 4155 544f 4d41  _string, "AUTOMA
-0000cc40: 5449 4322 2c20 3929 203d 3d20 3029 0a20  TIC", 9) == 0). 
-0000cc50: 2020 2020 2020 2020 2020 202a 704d 5332             *pMS2
-0000cc60: 4233 3230 5f46 4c41 4753 2028 7265 636f  B320_FLAGS (reco
-0000cc70: 7264 202b 2077 7269 7474 656e 2920 7c3d  rd + written) |=
-0000cc80: 2030 7830 343b 0a0a 2020 2020 2020 2020   0x04;..        
-0000cc90: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000cca0: 5f67 6574 5f62 6f6f 6c20 2865 6869 7465  _get_bool (ehite
-0000ccb0: 7276 616c 2c20 222f 436f 6e74 696e 7565  rval, "/Continue
-0000ccc0: 6422 2c20 2668 6561 6465 725f 626f 6f6c  d", &header_bool
-0000ccd0: 6561 6e29 2026 2620 6865 6164 6572 5f62  ean) && header_b
-0000cce0: 6f6f 6c65 616e 290a 2020 2020 2020 2020  oolean).        
-0000ccf0: 2020 2020 2a70 4d53 3242 3332 305f 464c      *pMS2B320_FL
-0000cd00: 4147 5320 2872 6563 6f72 6420 2b20 7772  AGS (record + wr
-0000cd10: 6974 7465 6e29 207c 3d20 3078 3038 3b0a  itten) |= 0x08;.
-0000cd20: 0a20 2020 2020 2020 2020 2069 6620 2879  .          if (y
-0000cd30: 796a 736f 6e5f 7074 725f 6765 745f 7374  yjson_ptr_get_st
-0000cd40: 7220 2865 6869 7465 7276 616c 2c20 222f  r (ehiterval, "/
-0000cd50: 416d 706c 6974 7564 6552 616e 6765 222c  AmplitudeRange",
-0000cd60: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
-0000cd70: 2026 260a 2020 2020 2020 2020 2020 2020   &&.            
-0000cd80: 2020 7374 726e 6361 7365 636d 7020 2868    strncasecmp (h
-0000cd90: 6561 6465 725f 7374 7269 6e67 2c20 2252  eader_string, "R
-0000cda0: 414e 444f 4d22 2c20 3629 203d 3d20 3029  ANDOM", 6) == 0)
-0000cdb0: 0a20 2020 2020 2020 2020 2020 202a 704d  .            *pM
-0000cdc0: 5332 4233 3230 5f46 4c41 4753 2028 7265  S2B320_FLAGS (re
-0000cdd0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
-0000cde0: 7c3d 2030 7831 303b 0a0a 2020 2020 2020  |= 0x10;..      
-0000cdf0: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
-0000ce00: 7472 5f67 6574 5f6e 756d 2028 6568 6974  tr_get_num (ehit
-0000ce10: 6572 7661 6c2c 2022 2f44 7572 6174 696f  erval, "/Duratio
-0000ce20: 6e22 2c20 2668 6561 6465 725f 6e75 6d62  n", &header_numb
-0000ce30: 6572 2929 0a20 2020 2020 2020 2020 2020  er)).           
-0000ce40: 202a 704d 5332 4233 3230 5f44 5552 4154   *pMS2B320_DURAT
-0000ce50: 494f 4e20 2872 6563 6f72 6420 2b20 7772  ION (record + wr
-0000ce60: 6974 7465 6e29 203d 2048 4f34 7520 2828  itten) = HO4u ((
-0000ce70: 7569 6e74 3332 5f74 2928 6865 6164 6572  uint32_t)(header
-0000ce80: 5f6e 756d 6265 7220 2a20 3130 3030 3020  _number * 10000 
-0000ce90: 2b20 302e 3529 2c20 7377 6170 666c 6167  + 0.5), swapflag
-0000cea0: 293b 0a0a 2020 2020 2020 2020 2020 6966  );..          if
-0000ceb0: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
-0000cec0: 5f6e 756d 2028 6568 6974 6572 7661 6c2c  _num (ehiterval,
-0000ced0: 2022 2f41 6d70 6c69 7475 6465 222c 2026   "/Amplitude", &
-0000cee0: 6865 6164 6572 5f6e 756d 6265 7229 290a  header_number)).
-0000cef0: 2020 2020 2020 2020 2020 2020 2a70 4d53              *pMS
-0000cf00: 3242 3332 305f 5054 5041 4d50 4c49 5455  2B320_PTPAMPLITU
-0000cf10: 4445 2028 7265 636f 7264 202b 2077 7269  DE (record + wri
-0000cf20: 7474 656e 2920 3d20 484f 3466 2028 2866  tten) = HO4f ((f
-0000cf30: 6c6f 6174 2968 6561 6465 725f 6e75 6d62  loat)header_numb
-0000cf40: 6572 2c20 7377 6170 666c 6167 293b 0a0a  er, swapflag);..
-0000cf50: 2020 2020 2020 2020 2020 6966 2028 7979            if (yy
-0000cf60: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
-0000cf70: 2028 6568 6974 6572 7661 6c2c 2022 2f49   (ehiterval, "/I
-0000cf80: 6e70 7574 4368 616e 6e65 6c22 2c20 2668  nputChannel", &h
-0000cf90: 6561 6465 725f 7374 7269 6e67 2929 0a20  eader_string)). 
-0000cfa0: 2020 2020 2020 2020 2020 206d 735f 7374             ms_st
-0000cfb0: 726e 6370 6f70 656e 2028 704d 5332 4233  rncpopen (pMS2B3
-0000cfc0: 3230 5f49 4e50 5554 4348 414e 4e45 4c20  20_INPUTCHANNEL 
-0000cfd0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
-0000cfe0: 6e29 2c20 6865 6164 6572 5f73 7472 696e  n), header_strin
-0000cff0: 672c 2033 293b 0a0a 2020 2020 2020 2020  g, 3);..        
-0000d000: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000d010: 5f67 6574 5f6e 756d 2028 6568 6974 6572  _get_num (ehiter
-0000d020: 7661 6c2c 2022 2f52 6566 6572 656e 6365  val, "/Reference
-0000d030: 416d 706c 6974 7564 6522 2c20 2668 6561  Amplitude", &hea
-0000d040: 6465 725f 6e75 6d62 6572 2929 0a20 2020  der_number)).   
-0000d050: 2020 2020 2020 2020 202a 704d 5332 4233           *pMS2B3
-0000d060: 3230 5f52 4546 4552 454e 4345 414d 504c  20_REFERENCEAMPL
-0000d070: 4954 5544 4520 2872 6563 6f72 6420 2b20  ITUDE (record + 
-0000d080: 7772 6974 7465 6e29 203d 2048 4f34 7520  written) = HO4u 
-0000d090: 2828 7569 6e74 3332 5f74 2928 6865 6164  ((uint32_t)(head
-0000d0a0: 6572 5f6e 756d 6265 7220 2b20 302e 3529  er_number + 0.5)
-0000d0b0: 2c20 7377 6170 666c 6167 293b 0a0a 2020  , swapflag);..  
-0000d0c0: 2020 2020 2020 2020 6966 2028 7979 6a73          if (yyjs
-0000d0d0: 6f6e 5f70 7472 5f67 6574 5f73 7472 2028  on_ptr_get_str (
-0000d0e0: 6568 6974 6572 7661 6c2c 2022 2f43 6f75  ehiterval, "/Cou
-0000d0f0: 706c 696e 6722 2c20 2668 6561 6465 725f  pling", &header_
-0000d100: 7374 7269 6e67 2929 0a20 2020 2020 2020  string)).       
-0000d110: 2020 2020 206d 735f 7374 726e 6370 6f70       ms_strncpop
-0000d120: 656e 2028 704d 5332 4233 3230 5f43 4f55  en (pMS2B320_COU
-0000d130: 504c 494e 4720 2872 6563 6f72 6420 2b20  PLING (record + 
-0000d140: 7772 6974 7465 6e29 2c20 6865 6164 6572  written), header
-0000d150: 5f73 7472 696e 672c 2031 3229 3b0a 0a20  _string, 12);.. 
-0000d160: 2020 2020 2020 2020 2069 6620 2879 796a           if (yyj
-0000d170: 736f 6e5f 7074 725f 6765 745f 7374 7220  son_ptr_get_str 
-0000d180: 2865 6869 7465 7276 616c 2c20 222f 526f  (ehiterval, "/Ro
-0000d190: 6c6c 6f66 6622 2c20 2668 6561 6465 725f  lloff", &header_
-0000d1a0: 7374 7269 6e67 2929 0a20 2020 2020 2020  string)).       
-0000d1b0: 2020 2020 206d 735f 7374 726e 6370 6f70       ms_strncpop
-0000d1c0: 656e 2028 704d 5332 4233 3230 5f52 4f4c  en (pMS2B320_ROL
-0000d1d0: 4c4f 4646 2028 7265 636f 7264 202b 2077  LOFF (record + w
-0000d1e0: 7269 7474 656e 292c 2068 6561 6465 725f  ritten), header_
-0000d1f0: 7374 7269 6e67 2c20 3132 293b 0a0a 2020  string, 12);..  
-0000d200: 2020 2020 2020 2020 6966 2028 7979 6a73          if (yyjs
-0000d210: 6f6e 5f70 7472 5f67 6574 5f73 7472 2028  on_ptr_get_str (
-0000d220: 6568 6974 6572 7661 6c2c 2022 2f4e 6f69  ehiterval, "/Noi
-0000d230: 7365 222c 2026 6865 6164 6572 5f73 7472  se", &header_str
-0000d240: 696e 6729 290a 2020 2020 2020 2020 2020  ing)).          
-0000d250: 2020 6d73 5f73 7472 6e63 706f 7065 6e20    ms_strncpopen 
-0000d260: 2870 4d53 3242 3332 305f 4e4f 4953 4554  (pMS2B320_NOISET
-0000d270: 5950 4520 2872 6563 6f72 6420 2b20 7772  YPE (record + wr
-0000d280: 6974 7465 6e29 2c20 6865 6164 6572 5f73  itten), header_s
-0000d290: 7472 696e 672c 2038 293b 0a20 2020 2020  tring, 8);.     
-0000d2a0: 2020 207d 0a20 2020 2020 2020 2065 6c73     }.        els
-0000d2b0: 6520 6966 2028 626c 6f63 6b65 7474 655f  e if (blockette_
-0000d2c0: 7479 7065 203d 3d20 3339 3029 0a20 2020  type == 390).   
-0000d2d0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-0000d2e0: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
-0000d2f0: 6765 745f 7374 7220 2865 6869 7465 7276  get_str (ehiterv
-0000d300: 616c 2c20 222f 5472 6967 6765 7222 2c20  al, "/Trigger", 
-0000d310: 2668 6561 6465 725f 7374 7269 6e67 2920  &header_string) 
-0000d320: 2626 0a20 2020 2020 2020 2020 2020 2020  &&.             
-0000d330: 2073 7472 6e63 6173 6563 6d70 2028 6865   strncasecmp (he
-0000d340: 6164 6572 5f73 7472 696e 672c 2022 4155  ader_string, "AU
-0000d350: 544f 4d41 5449 4322 2c20 3929 203d 3d20  TOMATIC", 9) == 
-0000d360: 3029 0a20 2020 2020 2020 2020 2020 202a  0).            *
-0000d370: 704d 5332 4233 3930 5f46 4c41 4753 2028  pMS2B390_FLAGS (
-0000d380: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
-0000d390: 2920 7c3d 2030 7830 343b 0a0a 2020 2020  ) |= 0x04;..    
-0000d3a0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
-0000d3b0: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
-0000d3c0: 6869 7465 7276 616c 2c20 222f 436f 6e74  hiterval, "/Cont
-0000d3d0: 696e 7565 6422 2c20 2668 6561 6465 725f  inued", &header_
-0000d3e0: 626f 6f6c 6561 6e29 2026 2620 6865 6164  boolean) && head
-0000d3f0: 6572 5f62 6f6f 6c65 616e 290a 2020 2020  er_boolean).    
-0000d400: 2020 2020 2020 2020 2a70 4d53 3242 3339          *pMS2B39
-0000d410: 305f 464c 4147 5320 2872 6563 6f72 6420  0_FLAGS (record 
-0000d420: 2b20 7772 6974 7465 6e29 207c 3d20 3078  + written) |= 0x
-0000d430: 3038 3b0a 0a20 2020 2020 2020 2020 2069  08;..          i
-0000d440: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
-0000d450: 745f 6e75 6d20 2865 6869 7465 7276 616c  t_num (ehiterval
-0000d460: 2c20 222f 4475 7261 7469 6f6e 222c 2026  , "/Duration", &
-0000d470: 6865 6164 6572 5f6e 756d 6265 7229 290a  header_number)).
-0000d480: 2020 2020 2020 2020 2020 2020 2a70 4d53              *pMS
-0000d490: 3242 3339 305f 4455 5241 5449 4f4e 2028  2B390_DURATION (
-0000d4a0: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
-0000d4b0: 2920 3d20 484f 3475 2028 2875 696e 7433  ) = HO4u ((uint3
-0000d4c0: 325f 7429 2868 6561 6465 725f 6e75 6d62  2_t)(header_numb
-0000d4d0: 6572 202a 2031 3030 3030 202b 2030 2e35  er * 10000 + 0.5
-0000d4e0: 292c 2073 7761 7066 6c61 6729 3b0a 0a20  ), swapflag);.. 
-0000d4f0: 2020 2020 2020 2020 2069 6620 2879 796a           if (yyj
-0000d500: 736f 6e5f 7074 725f 6765 745f 6e75 6d20  son_ptr_get_num 
-0000d510: 2865 6869 7465 7276 616c 2c20 222f 416d  (ehiterval, "/Am
-0000d520: 706c 6974 7564 6522 2c20 2668 6561 6465  plitude", &heade
-0000d530: 725f 6e75 6d62 6572 2929 0a20 2020 2020  r_number)).     
-0000d540: 2020 2020 2020 202a 704d 5332 4233 3930         *pMS2B390
-0000d550: 5f41 4d50 4c49 5455 4445 2028 7265 636f  _AMPLITUDE (reco
-0000d560: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
-0000d570: 484f 3466 2028 2866 6c6f 6174 2968 6561  HO4f ((float)hea
-0000d580: 6465 725f 6e75 6d62 6572 2c20 7377 6170  der_number, swap
-0000d590: 666c 6167 293b 0a0a 2020 2020 2020 2020  flag);..        
-0000d5a0: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
-0000d5b0: 5f67 6574 5f73 7472 2028 6568 6974 6572  _get_str (ehiter
-0000d5c0: 7661 6c2c 2022 2f49 6e70 7574 4368 616e  val, "/InputChan
-0000d5d0: 6e65 6c22 2c20 2668 6561 6465 725f 7374  nel", &header_st
-0000d5e0: 7269 6e67 2929 0a20 2020 2020 2020 2020  ring)).         
-0000d5f0: 2020 206d 735f 7374 726e 6370 6f70 656e     ms_strncpopen
-0000d600: 2028 704d 5332 4233 3930 5f49 4e50 5554   (pMS2B390_INPUT
-0000d610: 4348 414e 4e45 4c20 2872 6563 6f72 6420  CHANNEL (record 
-0000d620: 2b20 7772 6974 7465 6e29 2c20 6865 6164  + written), head
-0000d630: 6572 5f73 7472 696e 672c 2033 293b 0a20  er_string, 3);. 
-0000d640: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0000d650: 2020 7772 6974 7465 6e20 2b3d 2062 6c6f    written += blo
-0000d660: 636b 6574 7465 5f6c 656e 6774 683b 0a20  ckette_length;. 
-0000d670: 2020 2020 207d 0a0a 2020 2020 2020 2f2a       }..      /*
-0000d680: 2041 6464 2042 6c6f 636b 6574 7465 2033   Add Blockette 3
-0000d690: 3935 2069 6620 456e 6454 696d 6520 6973  95 if EndTime is
-0000d6a0: 2069 6e63 6c75 6465 6420 2a2f 0a20 2020   included */.   
-0000d6b0: 2020 2069 6620 2879 796a 736f 6e5f 7074     if (yyjson_pt
-0000d6c0: 725f 6765 745f 7374 7220 2865 6869 7465  r_get_str (ehite
-0000d6d0: 7276 616c 2c20 222f 456e 6454 696d 6522  rval, "/EndTime"
-0000d6e0: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
-0000d6f0: 2929 0a20 2020 2020 207b 0a20 2020 2020  )).      {.     
-0000d700: 2020 2062 6c6f 636b 6574 7465 5f74 7970     blockette_typ
-0000d710: 6520 203d 2033 3935 3b0a 2020 2020 2020  e  = 395;.      
-0000d720: 2020 626c 6f63 6b65 7474 655f 6c65 6e67    blockette_leng
-0000d730: 7468 203d 2031 363b 0a0a 2020 2020 2020  th = 16;..      
-0000d740: 2020 6966 2028 2872 6563 6275 666c 656e    if ((recbuflen
-0000d750: 202d 2077 7269 7474 656e 2920 3c20 626c   - written) < bl
-0000d760: 6f63 6b65 7474 655f 6c65 6e67 7468 290a  ockette_length).
-0000d770: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-0000d780: 2020 2020 6d73 5f6c 6f67 2028 322c 2022      ms_log (2, "
-0000d790: 2573 3a20 5265 636f 7264 206c 656e 6774  %s: Record lengt
-0000d7a0: 6820 6e6f 7420 6c61 7267 6520 656e 6f75  h not large enou
-0000d7b0: 6768 2066 6f72 2042 2575 5c6e 222c 206d  gh for B%u\n", m
-0000d7c0: 7372 2d3e 7369 642c 2062 6c6f 636b 6574  sr->sid, blocket
-0000d7d0: 7465 5f74 7970 6529 3b0a 2020 2020 2020  te_type);.      
-0000d7e0: 2020 2020 7979 6a73 6f6e 5f64 6f63 5f66      yyjson_doc_f
-0000d7f0: 7265 6520 2865 6864 6f63 293b 0a20 2020  ree (ehdoc);.   
-0000d800: 2020 2020 2020 2072 6574 7572 6e20 2d31         return -1
-0000d810: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
-0000d820: 2020 2020 202a 6e65 7874 5f62 6c6f 636b       *next_block
-0000d830: 6574 7465 203d 2048 4f32 7520 2828 7569  ette = HO2u ((ui
-0000d840: 6e74 3136 5f74 2977 7269 7474 656e 2c20  nt16_t)written, 
-0000d850: 7377 6170 666c 6167 293b 0a20 2020 2020  swapflag);.     
-0000d860: 2020 206e 6578 745f 626c 6f63 6b65 7474     next_blockett
-0000d870: 6520 203d 2070 4d53 3242 3339 355f 4e45  e  = pMS2B395_NE
-0000d880: 5854 2028 7265 636f 7264 202b 2077 7269  XT (record + wri
-0000d890: 7474 656e 293b 0a20 2020 2020 2020 202a  tten);.        *
-0000d8a0: 704d 5332 4653 4448 5f4e 554d 424c 4f43  pMS2FSDH_NUMBLOC
-0000d8b0: 4b45 5454 4553 2028 7265 636f 7264 2920  KETTES (record) 
-0000d8c0: 2b3d 2031 3b0a 0a20 2020 2020 2020 206d  += 1;..        m
-0000d8d0: 656d 7365 7420 2872 6563 6f72 6420 2b20  emset (record + 
-0000d8e0: 7772 6974 7465 6e2c 2030 2c20 626c 6f63  written, 0, bloc
-0000d8f0: 6b65 7474 655f 6c65 6e67 7468 293b 0a20  kette_length);. 
-0000d900: 2020 2020 2020 202a 704d 5332 4233 3935         *pMS2B395
-0000d910: 5f54 5950 4520 2872 6563 6f72 6420 2b20  _TYPE (record + 
-0000d920: 7772 6974 7465 6e29 203d 2048 4f32 7520  written) = HO2u 
-0000d930: 2862 6c6f 636b 6574 7465 5f74 7970 652c  (blockette_type,
-0000d940: 2073 7761 7066 6c61 6729 3b0a 2020 2020   swapflag);.    
-0000d950: 2020 2020 2a70 4d53 3242 3339 355f 4e45      *pMS2B395_NE
-0000d960: 5854 2028 7265 636f 7264 202b 2077 7269  XT (record + wri
-0000d970: 7474 656e 2920 3d20 303b 0a0a 2020 2020  tten) = 0;..    
-0000d980: 2020 2020 6966 2028 6d73 5f74 696d 6573      if (ms_times
-0000d990: 7472 3262 7469 6d65 2028 6865 6164 6572  tr2btime (header
-0000d9a0: 5f73 7472 696e 672c 2028 7569 6e74 385f  _string, (uint8_
-0000d9b0: 7420 2a29 704d 5332 4233 3935 5f59 4541  t *)pMS2B395_YEA
-0000d9c0: 5220 2872 6563 6f72 6420 2b20 7772 6974  R (record + writ
-0000d9d0: 7465 6e29 2c0a 2020 2020 2020 2020 2020  ten),.          
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 6d73 722d 3e73 6964 2c20 7377      msr->sid, sw
-0000da00: 6170 666c 6167 2920 3d3d 202d 3129 0a20  apflag) == -1). 
-0000da10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-0000da20: 2020 206d 735f 6c6f 6720 2832 2c20 2225     ms_log (2, "%
-0000da30: 733a 2043 616e 6e6f 7420 636f 6e76 6572  s: Cannot conver
-0000da40: 7420 4225 7520 7469 6d65 3a20 2573 5c6e  t B%u time: %s\n
-0000da50: 222c 206d 7372 2d3e 7369 642c 2062 6c6f  ", msr->sid, blo
-0000da60: 636b 6574 7465 5f74 7970 652c 2068 6561  ckette_type, hea
-0000da70: 6465 725f 7374 7269 6e67 293b 0a20 2020  der_string);.   
-0000da80: 2020 2020 2020 2079 796a 736f 6e5f 646f         yyjson_do
-0000da90: 635f 6672 6565 2028 6568 646f 6329 3b0a  c_free (ehdoc);.
-0000daa0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000dab0: 202d 313b 0a20 2020 2020 2020 207d 0a0a   -1;.        }..
-0000dac0: 2020 2020 2020 2020 7772 6974 7465 6e20          written 
-0000dad0: 2b3d 2062 6c6f 636b 6574 7465 5f6c 656e  += blockette_len
-0000dae0: 6774 683b 0a20 2020 2020 207d 0a20 2020  gth;.      }.   
-0000daf0: 207d 0a20 207d 202f 2a20 456e 6420 6966   }.  } /* End if
-0000db00: 202f 4644 534e 2f45 7665 6e74 2f44 6574   /FDSN/Event/Det
-0000db10: 6563 7469 6f6e 202a 2f0a 0a20 2069 6620  ection */..  if 
-0000db20: 2865 6864 6f63 290a 2020 7b0a 2020 2020  (ehdoc).  {.    
-0000db30: 7979 6a73 6f6e 5f64 6f63 5f66 7265 6520  yyjson_doc_free 
-0000db40: 2865 6864 6f63 293b 0a20 207d 0a0a 2020  (ehdoc);.  }..  
-0000db50: 7265 7475 726e 2077 7269 7474 656e 3b0a  return written;.
-0000db60: 7d20 2f2a 2045 6e64 206f 6620 6d73 7233  } /* End of msr3
-0000db70: 5f70 6163 6b5f 6865 6164 6572 3228 2920  _pack_header2() 
-0000db80: 2a2f 0a0a 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a  */../***********
-0000db90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dba0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dbb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dbc0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 202a  *************. *
-0000dbd0: 2020 5061 636b 2064 6174 6120 7361 6d70    Pack data samp
-0000dbe0: 6c65 732e 2020 5468 6520 696e 7075 7420  les.  The input 
-0000dbf0: 6461 7461 2073 616d 706c 6573 2073 7065  data samples spe
-0000dc00: 6369 6669 6564 2061 7320 2773 7263 2720  cified as 'src' 
-0000dc10: 7769 6c6c 0a20 2a20 2062 6520 7061 636b  will. *  be pack
-0000dc20: 6564 2077 6974 6820 2765 6e63 6f64 696e  ed with 'encodin
-0000dc30: 6727 2066 6f72 6d61 7420 616e 6420 706c  g' format and pl
-0000dc40: 6163 6564 2069 6e20 2764 6573 7427 2e0a  aced in 'dest'..
-0000dc50: 202a 0a20 2a20 2052 6574 7572 6e20 6e75   *. *  Return nu
-0000dc60: 6d62 6572 206f 6620 7361 6d70 6c65 7320  mber of samples 
-0000dc70: 7061 636b 6564 206f 6e20 7375 6363 6573  packed on succes
-0000dc80: 7320 616e 6420 6120 6e65 6761 7469 7665  s and a negative
-0000dc90: 206f 6e20 6572 726f 722e 0a20 2a0a 202a   on error.. *. *
-0000dca0: 205c 7265 6620 4d65 7373 6167 654f 6e45   \ref MessageOnE
-0000dcb0: 7272 6f72 202d 2074 6869 7320 6675 6e63  rror - this func
-0000dcc0: 7469 6f6e 206c 6f67 7320 6120 6d65 7373  tion logs a mess
-0000dcd0: 6167 6520 6f6e 2065 7272 6f72 0a20 2a2a  age on error. **
-0000dce0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dcf0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dd00: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dd10: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000dd20: 2a2a 2a2a 2a2a 2f0a 7374 6174 6963 2069  ******/.static i
-0000dd30: 6e74 3634 5f74 0a6d 7372 5f70 6163 6b5f  nt64_t.msr_pack_
-0000dd40: 6461 7461 2028 766f 6964 202a 6465 7374  data (void *dest
-0000dd50: 2c20 766f 6964 202a 7372 632c 2075 696e  , void *src, uin
-0000dd60: 7436 345f 7420 6d61 7873 616d 706c 6573  t64_t maxsamples
-0000dd70: 2c20 7569 6e74 3634 5f74 206d 6178 6461  , uint64_t maxda
-0000dd80: 7461 6279 7465 732c 0a20 2020 2020 2020  tabytes,.       
-0000dd90: 2020 2020 2020 2020 6368 6172 2073 616d          char sam
-0000dda0: 706c 6574 7970 652c 2069 6e74 385f 7420  pletype, int8_t 
-0000ddb0: 656e 636f 6469 6e67 2c20 696e 7438 5f74  encoding, int8_t
-0000ddc0: 2073 7761 7066 6c61 672c 0a20 2020 2020   swapflag,.     
-0000ddd0: 2020 2020 2020 2020 2020 7569 6e74 3332            uint32
-0000dde0: 5f74 202a 6279 7465 7377 7269 7474 656e  _t *byteswritten
-0000ddf0: 2c20 636f 6e73 7420 6368 6172 202a 7369  , const char *si
-0000de00: 642c 2069 6e74 385f 7420 7665 7262 6f73  d, int8_t verbos
-0000de10: 6529 0a7b 0a20 2069 6e74 3634 5f74 206e  e).{.  int64_t n
-0000de20: 7361 6d70 6c65 733b 0a0a 2020 6966 2028  samples;..  if (
-0000de30: 6279 7465 7377 7269 7474 656e 290a 2020  byteswritten).  
-0000de40: 2020 2a62 7974 6573 7772 6974 7465 6e20    *byteswritten 
-0000de50: 3d20 303b 0a0a 2020 2f2a 2044 6563 6964  = 0;..  /* Decid
-0000de60: 6520 6966 2074 6869 7320 6973 2061 2066  e if this is a f
-0000de70: 6f72 6d61 7420 7468 6174 2077 6520 6361  ormat that we ca
-0000de80: 6e20 656e 636f 6465 202a 2f0a 2020 7377  n encode */.  sw
-0000de90: 6974 6368 2028 656e 636f 6469 6e67 290a  itch (encoding).
-0000dea0: 2020 7b0a 2020 6361 7365 2044 455f 5445    {.  case DE_TE
-0000deb0: 5854 3a0a 2020 2020 6966 2028 7361 6d70  XT:.    if (samp
-0000dec0: 6c65 7479 7065 2021 3d20 2774 2720 2626  letype != 't' &&
-0000ded0: 2073 616d 706c 6574 7970 6520 213d 2027   sampletype != '
-0000dee0: 6127 290a 2020 2020 7b0a 2020 2020 2020  a').    {.      
-0000def0: 6d73 5f6c 6f67 2028 322c 2022 2573 3a20  ms_log (2, "%s: 
-0000df00: 5361 6d70 6c65 2074 7970 6520 6d75 7374  Sample type must
-0000df10: 2062 6520 7465 7874 2028 7429 2066 6f72   be text (t) for
-0000df20: 2074 6578 7420 656e 636f 6469 6e67 206e   text encoding n
-0000df30: 6f74 2027 2563 275c 6e22 2c0a 2020 2020  ot '%c'\n",.    
-0000df40: 2020 2020 2020 2020 2020 7369 642c 2073            sid, s
-0000df50: 616d 706c 6574 7970 6529 3b0a 2020 2020  ampletype);.    
-0000df60: 2020 7265 7475 726e 202d 313b 0a20 2020    return -1;.   
-0000df70: 207d 0a0a 2020 2020 6966 2028 7665 7262   }..    if (verb
-0000df80: 6f73 6520 3e20 3129 0a20 2020 2020 206d  ose > 1).      m
-0000df90: 735f 6c6f 6720 2830 2c20 2225 733a 2050  s_log (0, "%s: P
-0000dfa0: 6163 6b69 6e67 2074 6578 7420 6461 7461  acking text data
-0000dfb0: 5c6e 222c 2073 6964 293b 0a0a 2020 2020  \n", sid);..    
-0000dfc0: 6e73 616d 706c 6573 203d 206d 7372 5f65  nsamples = msr_e
-0000dfd0: 6e63 6f64 655f 7465 7874 2028 2863 6861  ncode_text ((cha
-0000dfe0: 7220 2a29 7372 632c 206d 6178 7361 6d70  r *)src, maxsamp
-0000dff0: 6c65 732c 2028 6368 6172 202a 2964 6573  les, (char *)des
-0000e000: 742c 206d 6178 6461 7461 6279 7465 7329  t, maxdatabytes)
-0000e010: 3b0a 0a20 2020 2069 6620 2862 7974 6573  ;..    if (bytes
-0000e020: 7772 6974 7465 6e20 2626 206e 7361 6d70  written && nsamp
-0000e030: 6c65 7320 3e20 3029 0a20 2020 2020 202a  les > 0).      *
-0000e040: 6279 7465 7377 7269 7474 656e 203d 2028  byteswritten = (
-0000e050: 7569 6e74 3332 5f74 296e 7361 6d70 6c65  uint32_t)nsample
-0000e060: 733b 0a0a 2020 2020 6272 6561 6b3b 0a0a  s;..    break;..
-0000e070: 2020 6361 7365 2044 455f 494e 5431 363a    case DE_INT16:
-0000e080: 0a20 2020 2069 6620 2873 616d 706c 6574  .    if (samplet
-0000e090: 7970 6520 213d 2027 6927 290a 2020 2020  ype != 'i').    
-0000e0a0: 7b0a 2020 2020 2020 6d73 5f6c 6f67 2028  {.      ms_log (
-0000e0b0: 322c 2022 2573 3a20 5361 6d70 6c65 2074  2, "%s: Sample t
-0000e0c0: 7970 6520 6d75 7374 2062 6520 696e 7465  ype must be inte
-0000e0d0: 6765 7220 2869 2920 666f 7220 494e 5431  ger (i) for INT1
-0000e0e0: 3620 656e 636f 6469 6e67 206e 6f74 2027  6 encoding not '
-0000e0f0: 2563 275c 6e22 2c0a 2020 2020 2020 2020  %c'\n",.        
-0000e100: 2020 2020 2020 7369 642c 2073 616d 706c        sid, sampl
-0000e110: 6574 7970 6529 3b0a 2020 2020 2020 7265  etype);.      re
-0000e120: 7475 726e 202d 313b 0a20 2020 207d 0a0a  turn -1;.    }..
-0000e130: 2020 2020 6966 2028 6d61 7864 6174 6162      if (maxdatab
-0000e140: 7974 6573 203c 2073 697a 656f 6628 696e  ytes < sizeof(in
-0000e150: 7431 365f 7429 290a 2020 2020 7b0a 2020  t16_t)).    {.  
-0000e160: 2020 2020 6d73 5f6c 6f67 2028 322c 2022      ms_log (2, "
-0000e170: 2573 3a20 4e6f 7420 656e 6f75 6768 2073  %s: Not enough s
-0000e180: 7061 6365 2069 6e20 7265 636f 7264 2028  pace in record (
-0000e190: 2522 2050 5249 7536 3420 2229 2066 6f72  %" PRIu64 ") for
-0000e1a0: 2049 4e54 3136 2065 6e63 6f64 696e 672c   INT16 encoding,
-0000e1b0: 206e 6565 6420 6174 206c 6561 7374 2025   need at least %
-0000e1c0: 2250 5249 7369 7a65 5f74 2220 6279 7465  "PRIsize_t" byte
-0000e1d0: 735c 6e22 2c0a 2020 2020 2020 2020 2020  s\n",.          
-0000e1e0: 2020 2020 7369 642c 206d 6178 6461 7461      sid, maxdata
-0000e1f0: 6279 7465 732c 2073 697a 656f 6628 696e  bytes, sizeof(in
-0000e200: 7431 365f 7429 293b 0a20 2020 2020 2072  t16_t));.      r
-0000e210: 6574 7572 6e20 2d31 3b0a 2020 2020 7d0a  eturn -1;.    }.
-0000e220: 0a20 2020 2069 6620 2876 6572 626f 7365  .    if (verbose
-0000e230: 203e 2031 290a 2020 2020 2020 6d73 5f6c   > 1).      ms_l
-0000e240: 6f67 2028 302c 2022 2573 3a20 5061 636b  og (0, "%s: Pack
-0000e250: 696e 6720 494e 5431 3620 6461 7461 2073  ing INT16 data s
-0000e260: 616d 706c 6573 5c6e 222c 2073 6964 293b  amples\n", sid);
-0000e270: 0a0a 2020 2020 6e73 616d 706c 6573 203d  ..    nsamples =
-0000e280: 206d 7372 5f65 6e63 6f64 655f 696e 7431   msr_encode_int1
-0000e290: 3620 2828 696e 7433 325f 7420 2a29 7372  6 ((int32_t *)sr
-0000e2a0: 632c 206d 6178 7361 6d70 6c65 732c 2028  c, maxsamples, (
-0000e2b0: 696e 7431 365f 7420 2a29 6465 7374 2c20  int16_t *)dest, 
-0000e2c0: 6d61 7864 6174 6162 7974 6573 2c20 7377  maxdatabytes, sw
-0000e2d0: 6170 666c 6167 293b 0a0a 2020 2020 6966  apflag);..    if
-0000e2e0: 2028 6279 7465 7377 7269 7474 656e 2026   (byteswritten &
-0000e2f0: 2620 6e73 616d 706c 6573 203e 2030 290a  & nsamples > 0).
-0000e300: 2020 2020 2020 2a62 7974 6573 7772 6974        *byteswrit
-0000e310: 7465 6e20 3d20 2875 696e 7433 325f 7429  ten = (uint32_t)
-0000e320: 286e 7361 6d70 6c65 7320 2a20 3229 3b0a  (nsamples * 2);.
-0000e330: 0a20 2020 2062 7265 616b 3b0a 0a20 2063  .    break;..  c
-0000e340: 6173 6520 4445 5f49 4e54 3332 3a0a 2020  ase DE_INT32:.  
-0000e350: 2020 6966 2028 7361 6d70 6c65 7479 7065    if (sampletype
-0000e360: 2021 3d20 2769 2729 0a20 2020 207b 0a20   != 'i').    {. 
-0000e370: 2020 2020 206d 735f 6c6f 6720 2832 2c20       ms_log (2, 
-0000e380: 2225 733a 2053 616d 706c 6520 7479 7065  "%s: Sample type
-0000e390: 206d 7573 7420 6265 2069 6e74 6567 6572   must be integer
-0000e3a0: 2028 6929 2066 6f72 2049 4e54 3332 2065   (i) for INT32 e
-0000e3b0: 6e63 6f64 696e 6720 6e6f 7420 2725 6327  ncoding not '%c'
-0000e3c0: 5c6e 222c 0a20 2020 2020 2020 2020 2020  \n",.           
-0000e3d0: 2020 2073 6964 2c20 7361 6d70 6c65 7479     sid, samplety
-0000e3e0: 7065 293b 0a20 2020 2020 2072 6574 7572  pe);.      retur
-0000e3f0: 6e20 2d31 3b0a 2020 2020 7d0a 0a20 2020  n -1;.    }..   
-0000e400: 2069 6620 286d 6178 6461 7461 6279 7465   if (maxdatabyte
-0000e410: 7320 3c20 7369 7a65 6f66 2869 6e74 3332  s < sizeof(int32
-0000e420: 5f74 2929 0a20 2020 207b 0a20 2020 2020  _t)).    {.     
-0000e430: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
-0000e440: 204e 6f74 2065 6e6f 7567 6820 7370 6163   Not enough spac
-0000e450: 6520 696e 2072 6563 6f72 6420 2825 2220  e in record (%" 
-0000e460: 5052 4975 3634 2022 2920 666f 7220 494e  PRIu64 ") for IN
-0000e470: 5433 3220 656e 636f 6469 6e67 2c20 6e65  T32 encoding, ne
-0000e480: 6564 2061 7420 6c65 6173 7420 2522 5052  ed at least %"PR
-0000e490: 4973 697a 655f 7422 2062 7974 6573 5c6e  Isize_t" bytes\n
-0000e4a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000e4b0: 2073 6964 2c20 6d61 7864 6174 6162 7974   sid, maxdatabyt
-0000e4c0: 6573 2c20 7369 7a65 6f66 2869 6e74 3332  es, sizeof(int32
-0000e4d0: 5f74 2929 3b0a 2020 2020 2020 7265 7475  _t));.      retu
-0000e4e0: 726e 202d 313b 0a20 2020 207d 0a0a 2020  rn -1;.    }..  
-0000e4f0: 2020 6966 2028 7665 7262 6f73 6520 3e20    if (verbose > 
-0000e500: 3129 0a20 2020 2020 206d 735f 6c6f 6720  1).      ms_log 
-0000e510: 2830 2c20 2225 733a 2050 6163 6b69 6e67  (0, "%s: Packing
-0000e520: 2049 4e54 3332 2064 6174 6120 7361 6d70   INT32 data samp
-0000e530: 6c65 735c 6e22 2c20 7369 6429 3b0a 0a20  les\n", sid);.. 
-0000e540: 2020 206e 7361 6d70 6c65 7320 3d20 6d73     nsamples = ms
-0000e550: 725f 656e 636f 6465 5f69 6e74 3332 2028  r_encode_int32 (
-0000e560: 2869 6e74 3332 5f74 202a 2973 7263 2c20  (int32_t *)src, 
-0000e570: 6d61 7873 616d 706c 6573 2c20 2869 6e74  maxsamples, (int
-0000e580: 3332 5f74 202a 2964 6573 742c 206d 6178  32_t *)dest, max
-0000e590: 6461 7461 6279 7465 732c 2073 7761 7066  databytes, swapf
-0000e5a0: 6c61 6729 3b0a 0a20 2020 2069 6620 2862  lag);..    if (b
-0000e5b0: 7974 6573 7772 6974 7465 6e20 2626 206e  yteswritten && n
-0000e5c0: 7361 6d70 6c65 7320 3e20 3029 0a20 2020  samples > 0).   
-0000e5d0: 2020 202a 6279 7465 7377 7269 7474 656e     *byteswritten
-0000e5e0: 203d 2028 7569 6e74 3332 5f74 2928 6e73   = (uint32_t)(ns
-0000e5f0: 616d 706c 6573 202a 2034 293b 0a0a 2020  amples * 4);..  
-0000e600: 2020 6272 6561 6b3b 0a0a 2020 6361 7365    break;..  case
-0000e610: 2044 455f 464c 4f41 5433 323a 0a20 2020   DE_FLOAT32:.   
-0000e620: 2069 6620 2873 616d 706c 6574 7970 6520   if (sampletype 
-0000e630: 213d 2027 6627 290a 2020 2020 7b0a 2020  != 'f').    {.  
-0000e640: 2020 2020 6d73 5f6c 6f67 2028 322c 2022      ms_log (2, "
-0000e650: 2573 3a20 5361 6d70 6c65 2074 7970 6520  %s: Sample type 
-0000e660: 6d75 7374 2062 6520 666c 6f61 7420 2866  must be float (f
-0000e670: 2920 666f 7220 464c 4f41 5433 3220 656e  ) for FLOAT32 en
-0000e680: 636f 6469 6e67 206e 6f74 2027 2563 275c  coding not '%c'\
-0000e690: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-0000e6a0: 2020 7369 642c 2073 616d 706c 6574 7970    sid, sampletyp
-0000e6b0: 6529 3b0a 2020 2020 2020 7265 7475 726e  e);.      return
-0000e6c0: 202d 313b 0a20 2020 207d 0a0a 2020 2020   -1;.    }..    
-0000e6d0: 6966 2028 6d61 7864 6174 6162 7974 6573  if (maxdatabytes
-0000e6e0: 203c 2073 697a 656f 6628 666c 6f61 7429   < sizeof(float)
-0000e6f0: 290a 2020 2020 7b0a 2020 2020 2020 6d73  ).    {.      ms
-0000e700: 5f6c 6f67 2028 322c 2022 2573 3a20 4e6f  _log (2, "%s: No
-0000e710: 7420 656e 6f75 6768 2073 7061 6365 2069  t enough space i
-0000e720: 6e20 7265 636f 7264 2028 2522 2050 5249  n record (%" PRI
-0000e730: 7536 3420 2229 2066 6f72 2046 4c4f 4154  u64 ") for FLOAT
-0000e740: 3332 2065 6e63 6f64 696e 672c 206e 6565  32 encoding, nee
-0000e750: 6420 6174 206c 6561 7374 2025 2250 5249  d at least %"PRI
-0000e760: 7369 7a65 5f74 2220 6279 7465 735c 6e22  size_t" bytes\n"
-0000e770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e780: 7369 642c 206d 6178 6461 7461 6279 7465  sid, maxdatabyte
-0000e790: 732c 2073 697a 656f 6628 666c 6f61 7429  s, sizeof(float)
-0000e7a0: 293b 0a20 2020 2020 2072 6574 7572 6e20  );.      return 
-0000e7b0: 2d31 3b0a 2020 2020 7d0a 0a20 2020 2069  -1;.    }..    i
-0000e7c0: 6620 2876 6572 626f 7365 203e 2031 290a  f (verbose > 1).
-0000e7d0: 2020 2020 2020 6d73 5f6c 6f67 2028 302c        ms_log (0,
-0000e7e0: 2022 2573 3a20 5061 636b 696e 6720 464c   "%s: Packing FL
-0000e7f0: 4f41 5433 3220 6461 7461 2073 616d 706c  OAT32 data sampl
-0000e800: 6573 5c6e 222c 2073 6964 293b 0a0a 2020  es\n", sid);..  
-0000e810: 2020 6e73 616d 706c 6573 203d 206d 7372    nsamples = msr
-0000e820: 5f65 6e63 6f64 655f 666c 6f61 7433 3220  _encode_float32 
-0000e830: 2828 666c 6f61 7420 2a29 7372 632c 206d  ((float *)src, m
-0000e840: 6178 7361 6d70 6c65 732c 2028 666c 6f61  axsamples, (floa
-0000e850: 7420 2a29 6465 7374 2c20 6d61 7864 6174  t *)dest, maxdat
-0000e860: 6162 7974 6573 2c20 7377 6170 666c 6167  abytes, swapflag
-0000e870: 293b 0a0a 2020 2020 6966 2028 6279 7465  );..    if (byte
-0000e880: 7377 7269 7474 656e 2026 2620 6e73 616d  swritten && nsam
-0000e890: 706c 6573 203e 2030 290a 2020 2020 2020  ples > 0).      
-0000e8a0: 2a62 7974 6573 7772 6974 7465 6e20 3d20  *byteswritten = 
-0000e8b0: 2875 696e 7433 325f 7429 286e 7361 6d70  (uint32_t)(nsamp
-0000e8c0: 6c65 7320 2a20 3429 3b0a 0a20 2020 2062  les * 4);..    b
-0000e8d0: 7265 616b 3b0a 0a20 2063 6173 6520 4445  reak;..  case DE
-0000e8e0: 5f46 4c4f 4154 3634 3a0a 2020 2020 6966  _FLOAT64:.    if
-0000e8f0: 2028 7361 6d70 6c65 7479 7065 2021 3d20   (sampletype != 
-0000e900: 2764 2729 0a20 2020 207b 0a20 2020 2020  'd').    {.     
-0000e910: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
-0000e920: 2053 616d 706c 6520 7479 7065 206d 7573   Sample type mus
-0000e930: 7420 6265 2064 6f75 626c 6520 2864 2920  t be double (d) 
-0000e940: 666f 7220 464c 4f41 5436 3420 656e 636f  for FLOAT64 enco
-0000e950: 6469 6e67 206e 6f74 2027 2563 275c 6e22  ding not '%c'\n"
-0000e960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e970: 7369 642c 2073 616d 706c 6574 7970 6529  sid, sampletype)
-0000e980: 3b0a 2020 2020 2020 7265 7475 726e 202d  ;.      return -
-0000e990: 313b 0a20 2020 207d 0a0a 2020 2020 6966  1;.    }..    if
-0000e9a0: 2028 6d61 7864 6174 6162 7974 6573 203c   (maxdatabytes <
-0000e9b0: 2073 697a 656f 6628 646f 7562 6c65 2929   sizeof(double))
-0000e9c0: 0a20 2020 207b 0a20 2020 2020 206d 735f  .    {.      ms_
-0000e9d0: 6c6f 6720 2832 2c20 2225 733a 204e 6f74  log (2, "%s: Not
-0000e9e0: 2065 6e6f 7567 6820 7370 6163 6520 696e   enough space in
-0000e9f0: 2072 6563 6f72 6420 2825 2220 5052 4975   record (%" PRIu
-0000ea00: 3634 2022 2920 666f 7220 464c 4f41 5436  64 ") for FLOAT6
-0000ea10: 3420 656e 636f 6469 6e67 2c20 6e65 6564  4 encoding, need
-0000ea20: 2061 7420 6c65 6173 7420 2522 5052 4973   at least %"PRIs
-0000ea30: 697a 655f 7422 2062 7974 6573 5c6e 222c  ize_t" bytes\n",
-0000ea40: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
-0000ea50: 6964 2c20 6d61 7864 6174 6162 7974 6573  id, maxdatabytes
-0000ea60: 2c20 7369 7a65 6f66 2864 6f75 626c 6529  , sizeof(double)
-0000ea70: 293b 0a20 2020 2020 2072 6574 7572 6e20  );.      return 
-0000ea80: 2d31 3b0a 2020 2020 7d0a 0a20 2020 2069  -1;.    }..    i
-0000ea90: 6620 2876 6572 626f 7365 203e 2031 290a  f (verbose > 1).
-0000eaa0: 2020 2020 2020 6d73 5f6c 6f67 2028 302c        ms_log (0,
-0000eab0: 2022 2573 3a20 5061 636b 696e 6720 464c   "%s: Packing FL
-0000eac0: 4f41 5436 3420 6461 7461 2073 616d 706c  OAT64 data sampl
-0000ead0: 6573 5c6e 222c 2073 6964 293b 0a0a 2020  es\n", sid);..  
-0000eae0: 2020 6e73 616d 706c 6573 203d 206d 7372    nsamples = msr
-0000eaf0: 5f65 6e63 6f64 655f 666c 6f61 7436 3420  _encode_float64 
-0000eb00: 2828 646f 7562 6c65 202a 2973 7263 2c20  ((double *)src, 
-0000eb10: 6d61 7873 616d 706c 6573 2c20 2864 6f75  maxsamples, (dou
-0000eb20: 626c 6520 2a29 6465 7374 2c20 6d61 7864  ble *)dest, maxd
-0000eb30: 6174 6162 7974 6573 2c20 7377 6170 666c  atabytes, swapfl
-0000eb40: 6167 293b 0a0a 2020 2020 6966 2028 6279  ag);..    if (by
-0000eb50: 7465 7377 7269 7474 656e 2026 2620 6e73  teswritten && ns
-0000eb60: 616d 706c 6573 203e 2030 290a 2020 2020  amples > 0).    
-0000eb70: 2020 2a62 7974 6573 7772 6974 7465 6e20    *byteswritten 
-0000eb80: 3d20 2875 696e 7433 325f 7429 286e 7361  = (uint32_t)(nsa
-0000eb90: 6d70 6c65 7320 2a20 3829 3b0a 0a20 2020  mples * 8);..   
-0000eba0: 2062 7265 616b 3b0a 0a20 2063 6173 6520   break;..  case 
-0000ebb0: 4445 5f53 5445 494d 313a 0a20 2020 2069  DE_STEIM1:.    i
-0000ebc0: 6620 2873 616d 706c 6574 7970 6520 213d  f (sampletype !=
-0000ebd0: 2027 6927 290a 2020 2020 7b0a 2020 2020   'i').    {.    
-0000ebe0: 2020 6d73 5f6c 6f67 2028 322c 2022 2573    ms_log (2, "%s
-0000ebf0: 3a20 5361 6d70 6c65 2074 7970 6520 6d75  : Sample type mu
-0000ec00: 7374 2062 6520 696e 7465 6765 7220 2869  st be integer (i
-0000ec10: 2920 666f 7220 5374 6569 6d31 2063 6f6d  ) for Steim1 com
-0000ec20: 7072 6573 7369 6f6e 206e 6f74 2027 2563  pression not '%c
-0000ec30: 275c 6e22 2c0a 2020 2020 2020 2020 2020  '\n",.          
-0000ec40: 2020 2020 7369 642c 2073 616d 706c 6574      sid, samplet
-0000ec50: 7970 6529 3b0a 2020 2020 2020 7265 7475  ype);.      retu
-0000ec60: 726e 202d 313b 0a20 2020 207d 0a0a 2020  rn -1;.    }..  
-0000ec70: 2020 6966 2028 6d61 7864 6174 6162 7974    if (maxdatabyt
-0000ec80: 6573 203c 2036 3429 0a20 2020 207b 0a20  es < 64).    {. 
-0000ec90: 2020 2020 206d 735f 6c6f 6720 2832 2c20       ms_log (2, 
-0000eca0: 2225 733a 204e 6f74 2065 6e6f 7567 6820  "%s: Not enough 
-0000ecb0: 7370 6163 6520 696e 2072 6563 6f72 6420  space in record 
-0000ecc0: 2825 2220 5052 4975 3634 2022 2920 666f  (%" PRIu64 ") fo
-0000ecd0: 7220 5354 4549 4d31 2065 6e63 6f64 696e  r STEIM1 encodin
-0000ece0: 672c 206e 6565 6420 6174 206c 6561 7374  g, need at least
-0000ecf0: 2036 3420 6279 7465 735c 6e22 2c0a 2020   64 bytes\n",.  
-0000ed00: 2020 2020 2020 2020 2020 2020 7369 642c              sid,
-0000ed10: 206d 6178 6461 7461 6279 7465 7329 3b0a   maxdatabytes);.
-0000ed20: 2020 2020 2020 7265 7475 726e 202d 313b        return -1;
-0000ed30: 0a20 2020 207d 0a0a 2020 2020 6966 2028  .    }..    if (
-0000ed40: 7665 7262 6f73 6520 3e20 3129 0a20 2020  verbose > 1).   
-0000ed50: 2020 206d 735f 6c6f 6720 2830 2c20 2225     ms_log (0, "%
-0000ed60: 733a 2050 6163 6b69 6e67 2053 7465 696d  s: Packing Steim
-0000ed70: 3120 6461 7461 2066 7261 6d65 735c 6e22  1 data frames\n"
-0000ed80: 2c20 7369 6429 3b0a 0a20 2020 202f 2a20  , sid);..    /* 
-0000ed90: 416c 7761 7973 2062 6967 2065 6e64 6961  Always big endia
-0000eda0: 6e20 5374 6569 6d31 202a 2f0a 2020 2020  n Steim1 */.    
-0000edb0: 7377 6170 666c 6167 203d 2028 6d73 5f62  swapflag = (ms_b
-0000edc0: 6967 656e 6469 616e 686f 7374 2829 2920  igendianhost()) 
-0000edd0: 3f20 3020 3a20 313b 0a0a 2020 2020 6e73  ? 0 : 1;..    ns
-0000ede0: 616d 706c 6573 203d 206d 7372 5f65 6e63  amples = msr_enc
-0000edf0: 6f64 655f 7374 6569 6d31 2028 2869 6e74  ode_steim1 ((int
-0000ee00: 3332 5f74 202a 2973 7263 2c20 6d61 7873  32_t *)src, maxs
-0000ee10: 616d 706c 6573 2c20 2869 6e74 3332 5f74  amples, (int32_t
-0000ee20: 202a 2964 6573 742c 206d 6178 6461 7461   *)dest, maxdata
-0000ee30: 6279 7465 732c 2030 2c20 6279 7465 7377  bytes, 0, bytesw
-0000ee40: 7269 7474 656e 2c20 7377 6170 666c 6167  ritten, swapflag
-0000ee50: 293b 0a0a 2020 2020 6272 6561 6b3b 0a0a  );..    break;..
-0000ee60: 2020 6361 7365 2044 455f 5354 4549 4d32    case DE_STEIM2
-0000ee70: 3a0a 2020 2020 6966 2028 7361 6d70 6c65  :.    if (sample
-0000ee80: 7479 7065 2021 3d20 2769 2729 0a20 2020  type != 'i').   
-0000ee90: 207b 0a20 2020 2020 206d 735f 6c6f 6720   {.      ms_log 
-0000eea0: 2832 2c20 2225 733a 2053 616d 706c 6520  (2, "%s: Sample 
-0000eeb0: 7479 7065 206d 7573 7420 6265 2069 6e74  type must be int
-0000eec0: 6567 6572 2028 6929 2066 6f72 2053 7465  eger (i) for Ste
-0000eed0: 696d 3220 636f 6d70 7265 7373 696f 6e20  im2 compression 
-0000eee0: 6e6f 7420 2725 6327 5c6e 222c 0a20 2020  not '%c'\n",.   
-0000eef0: 2020 2020 2020 2020 2020 2073 6964 2c20             sid, 
-0000ef00: 7361 6d70 6c65 7479 7065 293b 0a20 2020  sampletype);.   
-0000ef10: 2020 2072 6574 7572 6e20 2d31 3b0a 2020     return -1;.  
-0000ef20: 2020 7d0a 0a20 2020 2069 6620 286d 6178    }..    if (max
-0000ef30: 6461 7461 6279 7465 7320 3c20 3634 290a  databytes < 64).
-0000ef40: 2020 2020 7b0a 2020 2020 2020 6d73 5f6c      {.      ms_l
-0000ef50: 6f67 2028 322c 2022 2573 3a20 4e6f 7420  og (2, "%s: Not 
-0000ef60: 656e 6f75 6768 2073 7061 6365 2069 6e20  enough space in 
-0000ef70: 7265 636f 7264 2028 2522 2050 5249 7536  record (%" PRIu6
-0000ef80: 3420 2229 2066 6f72 2053 5445 494d 3220  4 ") for STEIM2 
-0000ef90: 656e 636f 6469 6e67 2c20 6e65 6564 2061  encoding, need a
-0000efa0: 7420 6c65 6173 7420 3634 2062 7974 6573  t least 64 bytes
-0000efb0: 5c6e 222c 0a20 2020 2020 2020 2020 2020  \n",.           
-0000efc0: 2020 2073 6964 2c20 6d61 7864 6174 6162     sid, maxdatab
-0000efd0: 7974 6573 293b 0a20 2020 2020 2072 6574  ytes);.      ret
-0000efe0: 7572 6e20 2d31 3b0a 2020 2020 7d0a 0a20  urn -1;.    }.. 
-0000eff0: 2020 2069 6620 2876 6572 626f 7365 203e     if (verbose >
-0000f000: 2031 290a 2020 2020 2020 6d73 5f6c 6f67   1).      ms_log
-0000f010: 2028 302c 2022 2573 3a20 5061 636b 696e   (0, "%s: Packin
-0000f020: 6720 5374 6569 6d32 2064 6174 6120 6672  g Steim2 data fr
-0000f030: 616d 6573 5c6e 222c 2073 6964 293b 0a0a  ames\n", sid);..
-0000f040: 2020 2020 2f2a 2041 6c77 6179 7320 6269      /* Always bi
-0000f050: 6720 656e 6469 616e 2053 7465 696d 3220  g endian Steim2 
-0000f060: 2a2f 0a20 2020 2073 7761 7066 6c61 6720  */.    swapflag 
-0000f070: 3d20 286d 735f 6269 6765 6e64 6961 6e68  = (ms_bigendianh
-0000f080: 6f73 7428 2929 203f 2030 203a 2031 3b0a  ost()) ? 0 : 1;.
-0000f090: 0a20 2020 206e 7361 6d70 6c65 7320 3d20  .    nsamples = 
-0000f0a0: 6d73 725f 656e 636f 6465 5f73 7465 696d  msr_encode_steim
-0000f0b0: 3220 2828 696e 7433 325f 7420 2a29 7372  2 ((int32_t *)sr
-0000f0c0: 632c 206d 6178 7361 6d70 6c65 732c 2028  c, maxsamples, (
-0000f0d0: 696e 7433 325f 7420 2a29 6465 7374 2c20  int32_t *)dest, 
-0000f0e0: 6d61 7864 6174 6162 7974 6573 2c20 302c  maxdatabytes, 0,
-0000f0f0: 2062 7974 6573 7772 6974 7465 6e2c 2073   byteswritten, s
-0000f100: 6964 2c20 7377 6170 666c 6167 293b 0a0a  id, swapflag);..
-0000f110: 2020 2020 6272 6561 6b3b 0a0a 2020 6465      break;..  de
-0000f120: 6661 756c 743a 0a20 2020 206d 735f 6c6f  fault:.    ms_lo
-0000f130: 6720 2832 2c20 2225 733a 2055 6e61 626c  g (2, "%s: Unabl
-0000f140: 6520 746f 2070 6163 6b20 666f 726d 6174  e to pack format
-0000f150: 2025 645c 6e22 2c20 7369 642c 2065 6e63   %d\n", sid, enc
-0000f160: 6f64 696e 6729 3b0a 0a20 2020 2072 6574  oding);..    ret
-0000f170: 7572 6e20 2d31 3b0a 2020 7d0a 0a20 2072  urn -1;.  }..  r
-0000f180: 6574 7572 6e20 6e73 616d 706c 6573 3b0a  eturn nsamples;.
-0000f190: 7d20 2f2a 2045 6e64 206f 6620 6d73 725f  } /* End of msr_
-0000f1a0: 7061 636b 5f64 6174 6128 2920 2a2f 0a0a  pack_data() */..
-0000f1b0: 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  /***************
-0000f1c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f1d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f1e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f1f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a20 2a20  ************. * 
-0000f200: 6d73 5f72 6174 6170 7072 6f78 3a0a 202a  ms_ratapprox:. *
-0000f210: 0a20 2a20 4669 6e64 2061 6e20 6170 7072  . * Find an appr
-0000f220: 6f78 696d 6174 6520 7261 7469 6f6e 616c  oximate rational
-0000f230: 206e 756d 6265 7220 666f 7220 6120 7265   number for a re
-0000f240: 616c 2074 6872 6f75 6768 2063 6f6e 7469  al through conti
-0000f250: 6e75 6564 0a20 2a20 6672 6163 7469 6f6e  nued. * fraction
-0000f260: 2065 7870 616e 7369 6f6e 2e20 2047 6976   expansion.  Giv
-0000f270: 656e 2061 2064 6f75 626c 6520 7072 6563  en a double prec
-0000f280: 7369 6f6e 2027 7265 616c 2720 6669 6e64  sion 'real' find
-0000f290: 2061 0a20 2a20 6e75 6d65 7261 746f 7220   a. * numerator 
-0000f2a0: 286e 756d 2920 616e 6420 6465 6e6f 6d69  (num) and denomi
-0000f2b0: 6e61 746f 7220 2864 656e 2920 7768 6f73  nator (den) whos
-0000f2c0: 6520 6162 736f 6c75 7465 2076 616c 7565  e absolute value
-0000f2d0: 7320 6172 6520 6e6f 740a 202a 206c 6172  s are not. * lar
-0000f2e0: 6765 7220 7468 616e 2027 6d61 7876 616c  ger than 'maxval
-0000f2f0: 2720 7768 696c 6520 7472 7969 6e67 2074  ' while trying t
-0000f300: 6f20 7265 6163 6820 6120 7370 6563 6966  o reach a specif
-0000f310: 6965 6420 2770 7265 6369 7369 6f6e 272e  ied 'precision'.
-0000f320: 0a20 2a0a 202a 2052 6574 7572 6e73 2074  . *. * Returns t
-0000f330: 6865 206e 756d 6265 7220 6f66 2069 7465  he number of ite
-0000f340: 7261 7469 6f6e 7320 7065 7266 6f72 6d65  rations performe
-0000f350: 642e 0a20 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  d.. ************
+00007b70: 3022 2c20 3629 3b0a 0a20 202f 2a20 5573  0", 6);..  /* Us
+00007b80: 6520 4461 7461 5175 616c 6974 7920 696e  e DataQuality in
+00007b90: 6469 6361 746f 7220 696e 2065 7874 7261  dicator in extra
+00007ba0: 2068 6561 6465 7273 2069 6620 7072 6573   headers if pres
+00007bb0: 656e 7420 2a2f 0a20 2069 6620 2879 796a  ent */.  if (yyj
+00007bc0: 736f 6e5f 7074 725f 6765 745f 7374 7220  son_ptr_get_str 
+00007bd0: 2865 6872 6f6f 742c 2022 2f46 4453 4e2f  (ehroot, "/FDSN/
+00007be0: 4461 7461 5175 616c 6974 7922 2c20 2668  DataQuality", &h
+00007bf0: 6561 6465 725f 7374 7269 6e67 2920 2626  eader_string) &&
+00007c00: 0a20 2020 2020 204d 5332 5f49 5344 4154  .      MS2_ISDAT
+00007c10: 4149 4e44 4943 4154 4f52 2028 6865 6164  AINDICATOR (head
+00007c20: 6572 5f73 7472 696e 675b 305d 2929 0a20  er_string[0])). 
+00007c30: 207b 0a20 2020 202a 704d 5332 4653 4448   {.    *pMS2FSDH
+00007c40: 5f44 4154 4151 5541 4c49 5459 2028 7265  _DATAQUALITY (re
+00007c50: 636f 7264 2920 3d20 6865 6164 6572 5f73  cord) = header_s
+00007c60: 7472 696e 675b 305d 3b0a 2020 7d0a 2020  tring[0];.  }.  
+00007c70: 2f2a 204f 7468 6572 7769 7365 206d 6170  /* Otherwise map
+00007c80: 2070 7562 6c69 6361 7469 6f6e 2076 6572   publication ver
+00007c90: 7369 6f6e 2c20 6465 6661 756c 7469 6e67  sion, defaulting
+00007ca0: 2074 6f20 2744 2720 2a2f 0a20 2065 6c73   to 'D' */.  els
+00007cb0: 650a 2020 7b0a 2020 2020 7377 6974 6368  e.  {.    switch
+00007cc0: 2028 6d73 722d 3e70 7562 7665 7273 696f   (msr->pubversio
+00007cd0: 6e29 0a20 2020 207b 0a20 2020 2063 6173  n).    {.    cas
+00007ce0: 6520 313a 0a20 2020 2020 202a 704d 5332  e 1:.      *pMS2
+00007cf0: 4653 4448 5f44 4154 4151 5541 4c49 5459  FSDH_DATAQUALITY
+00007d00: 2028 7265 636f 7264 2920 3d20 2752 273b   (record) = 'R';
+00007d10: 0a20 2020 2020 2062 7265 616b 3b0a 2020  .      break;.  
+00007d20: 2020 6361 7365 2033 3a0a 2020 2020 2020    case 3:.      
+00007d30: 2a70 4d53 3246 5344 485f 4441 5441 5155  *pMS2FSDH_DATAQU
+00007d40: 414c 4954 5920 2872 6563 6f72 6429 203d  ALITY (record) =
+00007d50: 2027 5127 3b0a 2020 2020 2020 6272 6561   'Q';.      brea
+00007d60: 6b3b 0a20 2020 2063 6173 6520 343a 0a20  k;.    case 4:. 
+00007d70: 2020 2020 202a 704d 5332 4653 4448 5f44       *pMS2FSDH_D
+00007d80: 4154 4151 5541 4c49 5459 2028 7265 636f  ATAQUALITY (reco
+00007d90: 7264 2920 3d20 274d 273b 0a20 2020 2020  rd) = 'M';.     
+00007da0: 2062 7265 616b 3b0a 2020 2020 6465 6661   break;.    defa
+00007db0: 756c 743a 0a20 2020 2020 202a 704d 5332  ult:.      *pMS2
+00007dc0: 4653 4448 5f44 4154 4151 5541 4c49 5459  FSDH_DATAQUALITY
+00007dd0: 2028 7265 636f 7264 2920 3d20 2744 273b   (record) = 'D';
+00007de0: 0a20 2020 2020 2062 7265 616b 3b0a 2020  .      break;.  
+00007df0: 2020 7d0a 2020 7d0a 0a20 202a 704d 5332    }.  }..  *pMS2
+00007e00: 4653 4448 5f52 4553 4552 5645 4420 2872  FSDH_RESERVED (r
+00007e10: 6563 6f72 6429 203d 2027 2027 3b0a 2020  ecord) = ' ';.  
+00007e20: 6d73 5f73 7472 6e63 706f 7065 6e20 2870  ms_strncpopen (p
+00007e30: 4d53 3246 5344 485f 5354 4154 494f 4e20  MS2FSDH_STATION 
+00007e40: 2872 6563 6f72 6429 2c20 7374 6174 696f  (record), statio
+00007e50: 6e2c 2035 293b 0a20 206d 735f 7374 726e  n, 5);.  ms_strn
+00007e60: 6370 6f70 656e 2028 704d 5332 4653 4448  cpopen (pMS2FSDH
+00007e70: 5f4c 4f43 4154 494f 4e20 2872 6563 6f72  _LOCATION (recor
+00007e80: 6429 2c20 6c6f 6361 7469 6f6e 2c20 3229  d), location, 2)
+00007e90: 3b0a 2020 6d73 5f73 7472 6e63 706f 7065  ;.  ms_strncpope
+00007ea0: 6e20 2870 4d53 3246 5344 485f 4348 414e  n (pMS2FSDH_CHAN
+00007eb0: 4e45 4c20 2872 6563 6f72 6429 2c20 6368  NEL (record), ch
+00007ec0: 616e 6e65 6c2c 2033 293b 0a20 206d 735f  annel, 3);.  ms_
+00007ed0: 7374 726e 6370 6f70 656e 2028 704d 5332  strncpopen (pMS2
+00007ee0: 4653 4448 5f4e 4554 574f 524b 2028 7265  FSDH_NETWORK (re
+00007ef0: 636f 7264 292c 206e 6574 776f 726b 2c20  cord), network, 
+00007f00: 3229 3b0a 0a20 202a 704d 5332 4653 4448  2);..  *pMS2FSDH
+00007f10: 5f59 4541 5220 2872 6563 6f72 6429 2020  _YEAR (record)  
+00007f20: 2020 2020 203d 2048 4f32 7520 2879 6561       = HO2u (yea
+00007f30: 722c 2073 7761 7066 6c61 6729 3b0a 2020  r, swapflag);.  
+00007f40: 2a70 4d53 3246 5344 485f 4441 5920 2872  *pMS2FSDH_DAY (r
+00007f50: 6563 6f72 6429 2020 2020 2020 2020 3d20  ecord)        = 
+00007f60: 484f 3275 2028 6461 792c 2073 7761 7066  HO2u (day, swapf
+00007f70: 6c61 6729 3b0a 2020 2a70 4d53 3246 5344  lag);.  *pMS2FSD
+00007f80: 485f 484f 5552 2028 7265 636f 7264 2920  H_HOUR (record) 
+00007f90: 2020 2020 2020 3d20 686f 7572 3b0a 2020        = hour;.  
+00007fa0: 2a70 4d53 3246 5344 485f 4d49 4e20 2872  *pMS2FSDH_MIN (r
+00007fb0: 6563 6f72 6429 2020 2020 2020 2020 3d20  ecord)        = 
+00007fc0: 6d69 6e3b 0a20 202a 704d 5332 4653 4448  min;.  *pMS2FSDH
+00007fd0: 5f53 4543 2028 7265 636f 7264 2920 2020  _SEC (record)   
+00007fe0: 2020 2020 203d 2073 6563 3b0a 2020 2a70       = sec;.  *p
+00007ff0: 4d53 3246 5344 485f 554e 5553 4544 2028  MS2FSDH_UNUSED (
+00008000: 7265 636f 7264 2920 2020 2020 3d20 303b  record)     = 0;
+00008010: 0a20 202a 704d 5332 4653 4448 5f46 5345  .  *pMS2FSDH_FSE
+00008020: 4320 2872 6563 6f72 6429 2020 2020 2020  C (record)      
+00008030: 203d 2048 4f32 7520 2866 7365 632c 2073   = HO2u (fsec, s
+00008040: 7761 7066 6c61 6729 3b0a 2020 2a70 4d53  wapflag);.  *pMS
+00008050: 3246 5344 485f 4e55 4d53 414d 504c 4553  2FSDH_NUMSAMPLES
+00008060: 2028 7265 636f 7264 2920 3d20 303b 0a0a   (record) = 0;..
+00008070: 2020 2a70 4d53 3246 5344 485f 5341 4d50    *pMS2FSDH_SAMP
+00008080: 4c45 5241 5445 4641 4354 2028 7265 636f  LERATEFACT (reco
+00008090: 7264 2920 3d20 484f 3264 2028 6661 6374  rd) = HO2d (fact
+000080a0: 6f72 2c20 7377 6170 666c 6167 293b 0a20  or, swapflag);. 
+000080b0: 202a 704d 5332 4653 4448 5f53 414d 504c   *pMS2FSDH_SAMPL
+000080c0: 4552 4154 454d 554c 5420 2872 6563 6f72  ERATEMULT (recor
+000080d0: 6429 203d 2048 4f32 6420 286d 756c 7469  d) = HO2d (multi
+000080e0: 706c 6965 722c 2073 7761 7066 6c61 6729  plier, swapflag)
+000080f0: 3b0a 0a20 202f 2a20 4d61 7020 6163 7469  ;..  /* Map acti
+00008100: 7669 7479 2062 6974 2066 6c61 6773 202a  vity bit flags *
+00008110: 2f0a 2020 2a70 4d53 3246 5344 485f 4143  /.  *pMS2FSDH_AC
+00008120: 5446 4c41 4753 2028 7265 636f 7264 2920  TFLAGS (record) 
+00008130: 3d20 303b 0a20 2069 6620 286d 7372 2d3e  = 0;.  if (msr->
+00008140: 666c 6167 7320 2620 3078 3031 2920 2f2a  flags & 0x01) /*
+00008150: 2042 6974 2030 202a 2f0a 2020 2020 2a70   Bit 0 */.    *p
+00008160: 4d53 3246 5344 485f 4143 5446 4c41 4753  MS2FSDH_ACTFLAGS
+00008170: 2028 7265 636f 7264 2920 7c3d 2030 7830   (record) |= 0x0
+00008180: 313b 0a0a 2020 6966 2028 7979 6a73 6f6e  1;..  if (yyjson
+00008190: 5f70 7472 5f67 6574 5f62 6f6f 6c20 2865  _ptr_get_bool (e
+000081a0: 6872 6f6f 742c 2022 2f46 4453 4e2f 4576  hroot, "/FDSN/Ev
+000081b0: 656e 742f 4265 6769 6e22 2c20 2668 6561  ent/Begin", &hea
+000081c0: 6465 725f 626f 6f6c 6561 6e29 2026 2620  der_boolean) && 
+000081d0: 6865 6164 6572 5f62 6f6f 6c65 616e 2920  header_boolean) 
+000081e0: 2f2a 2042 6974 2032 202a 2f0a 2020 2020  /* Bit 2 */.    
+000081f0: 2a70 4d53 3246 5344 485f 4143 5446 4c41  *pMS2FSDH_ACTFLA
+00008200: 4753 2028 7265 636f 7264 2920 7c3d 2030  GS (record) |= 0
+00008210: 7830 343b 0a20 2069 6620 2879 796a 736f  x04;.  if (yyjso
+00008220: 6e5f 7074 725f 6765 745f 626f 6f6c 2028  n_ptr_get_bool (
+00008230: 6568 726f 6f74 2c20 222f 4644 534e 2f45  ehroot, "/FDSN/E
+00008240: 7665 6e74 2f45 6e64 222c 2026 6865 6164  vent/End", &head
+00008250: 6572 5f62 6f6f 6c65 616e 2920 2626 2068  er_boolean) && h
+00008260: 6561 6465 725f 626f 6f6c 6561 6e29 202f  eader_boolean) /
+00008270: 2a20 4269 7420 3320 2a2f 0a20 2020 202a  * Bit 3 */.    *
+00008280: 704d 5332 4653 4448 5f41 4354 464c 4147  pMS2FSDH_ACTFLAG
+00008290: 5320 2872 6563 6f72 6429 207c 3d20 3078  S (record) |= 0x
+000082a0: 3038 3b0a 0a20 2069 6620 2879 796a 736f  08;..  if (yyjso
+000082b0: 6e5f 7074 725f 6765 745f 6e75 6d20 2865  n_ptr_get_num (e
+000082c0: 6872 6f6f 742c 2022 2f46 4453 4e2f 5469  hroot, "/FDSN/Ti
+000082d0: 6d65 2f4c 6561 7053 6563 6f6e 6422 2c20  me/LeapSecond", 
+000082e0: 2668 6561 6465 725f 6e75 6d62 6572 2929  &header_number))
+000082f0: 0a20 207b 0a20 2020 2069 6620 2868 6561  .  {.    if (hea
+00008300: 6465 725f 6e75 6d62 6572 203e 2030 2920  der_number > 0) 
+00008310: 2f2a 2042 6974 2034 202a 2f0a 2020 2020  /* Bit 4 */.    
+00008320: 2020 2a70 4d53 3246 5344 485f 4143 5446    *pMS2FSDH_ACTF
+00008330: 4c41 4753 2028 7265 636f 7264 2920 7c3d  LAGS (record) |=
+00008340: 2030 7831 303b 0a20 2020 2065 6c73 6520   0x10;.    else 
+00008350: 6966 2028 6865 6164 6572 5f6e 756d 6265  if (header_numbe
+00008360: 7220 3c20 3029 202f 2a20 4269 7420 3520  r < 0) /* Bit 5 
+00008370: 2a2f 0a20 2020 2020 202a 704d 5332 4653  */.      *pMS2FS
+00008380: 4448 5f41 4354 464c 4147 5320 2872 6563  DH_ACTFLAGS (rec
+00008390: 6f72 6429 207c 3d20 3078 3230 3b0a 2020  ord) |= 0x20;.  
+000083a0: 7d0a 0a20 2069 6620 2879 796a 736f 6e5f  }..  if (yyjson_
+000083b0: 7074 725f 6765 745f 626f 6f6c 2028 6568  ptr_get_bool (eh
+000083c0: 726f 6f74 2c20 222f 4644 534e 2f45 7665  root, "/FDSN/Eve
+000083d0: 6e74 2f49 6e50 726f 6772 6573 7322 2c20  nt/InProgress", 
+000083e0: 2668 6561 6465 725f 626f 6f6c 6561 6e29  &header_boolean)
+000083f0: 2026 2620 6865 6164 6572 5f62 6f6f 6c65   && header_boole
+00008400: 616e 2920 2f2a 2042 6974 2036 202a 2f0a  an) /* Bit 6 */.
+00008410: 2020 2020 2a70 4d53 3246 5344 485f 4143      *pMS2FSDH_AC
+00008420: 5446 4c41 4753 2028 7265 636f 7264 2920  TFLAGS (record) 
+00008430: 7c3d 2030 7834 303b 0a0a 2020 2f2a 204d  |= 0x40;..  /* M
+00008440: 6170 2049 2f4f 2061 6e64 2063 6c6f 636b  ap I/O and clock
+00008450: 2062 6974 2066 6c61 6773 202a 2f0a 2020   bit flags */.  
+00008460: 2a70 4d53 3246 5344 485f 494f 464c 4147  *pMS2FSDH_IOFLAG
+00008470: 5320 2872 6563 6f72 6429 203d 2030 3b0a  S (record) = 0;.
+00008480: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+00008490: 5f67 6574 5f62 6f6f 6c20 2865 6872 6f6f  _get_bool (ehroo
+000084a0: 742c 2022 2f46 4453 4e2f 466c 6167 732f  t, "/FDSN/Flags/
+000084b0: 5374 6174 696f 6e56 6f6c 756d 6550 6172  StationVolumePar
+000084c0: 6974 7945 7272 6f72 222c 2026 6865 6164  ityError", &head
+000084d0: 6572 5f62 6f6f 6c65 616e 2920 2626 2068  er_boolean) && h
+000084e0: 6561 6465 725f 626f 6f6c 6561 6e29 202f  eader_boolean) /
+000084f0: 2a20 4269 7420 3020 2a2f 0a20 2020 202a  * Bit 0 */.    *
+00008500: 704d 5332 4653 4448 5f49 4f46 4c41 4753  pMS2FSDH_IOFLAGS
+00008510: 2028 7265 636f 7264 2920 7c3d 2030 7830   (record) |= 0x0
+00008520: 313b 0a20 2069 6620 2879 796a 736f 6e5f  1;.  if (yyjson_
+00008530: 7074 725f 6765 745f 626f 6f6c 2028 6568  ptr_get_bool (eh
+00008540: 726f 6f74 2c20 222f 4644 534e 2f46 6c61  root, "/FDSN/Fla
+00008550: 6773 2f4c 6f6e 6752 6563 6f72 6452 6561  gs/LongRecordRea
+00008560: 6422 2c20 2668 6561 6465 725f 626f 6f6c  d", &header_bool
+00008570: 6561 6e29 2026 2620 6865 6164 6572 5f62  ean) && header_b
+00008580: 6f6f 6c65 616e 2920 2f2a 2042 6974 2031  oolean) /* Bit 1
+00008590: 202a 2f0a 2020 2020 2a70 4d53 3246 5344   */.    *pMS2FSD
+000085a0: 485f 494f 464c 4147 5320 2872 6563 6f72  H_IOFLAGS (recor
+000085b0: 6429 207c 3d20 3078 3032 3b0a 2020 6966  d) |= 0x02;.  if
+000085c0: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+000085d0: 5f62 6f6f 6c20 2865 6872 6f6f 742c 2022  _bool (ehroot, "
+000085e0: 2f46 4453 4e2f 466c 6167 732f 5368 6f72  /FDSN/Flags/Shor
+000085f0: 7452 6563 6f72 6452 6561 6422 2c20 2668  tRecordRead", &h
+00008600: 6561 6465 725f 626f 6f6c 6561 6e29 2026  eader_boolean) &
+00008610: 2620 6865 6164 6572 5f62 6f6f 6c65 616e  & header_boolean
+00008620: 2920 2f2a 2042 6974 2032 202a 2f0a 2020  ) /* Bit 2 */.  
+00008630: 2020 2a70 4d53 3246 5344 485f 494f 464c    *pMS2FSDH_IOFL
+00008640: 4147 5320 2872 6563 6f72 6429 207c 3d20  AGS (record) |= 
+00008650: 3078 3034 3b0a 2020 6966 2028 7979 6a73  0x04;.  if (yyjs
+00008660: 6f6e 5f70 7472 5f67 6574 5f62 6f6f 6c20  on_ptr_get_bool 
+00008670: 2865 6872 6f6f 742c 2022 2f46 4453 4e2f  (ehroot, "/FDSN/
+00008680: 466c 6167 732f 5374 6172 744f 6654 696d  Flags/StartOfTim
+00008690: 6553 6572 6965 7322 2c20 2668 6561 6465  eSeries", &heade
+000086a0: 725f 626f 6f6c 6561 6e29 2026 2620 6865  r_boolean) && he
+000086b0: 6164 6572 5f62 6f6f 6c65 616e 2920 2f2a  ader_boolean) /*
+000086c0: 2042 6974 2033 202a 2f0a 2020 2020 2a70   Bit 3 */.    *p
+000086d0: 4d53 3246 5344 485f 494f 464c 4147 5320  MS2FSDH_IOFLAGS 
+000086e0: 2872 6563 6f72 6429 207c 3d20 3078 3038  (record) |= 0x08
+000086f0: 3b0a 2020 6966 2028 7979 6a73 6f6e 5f70  ;.  if (yyjson_p
+00008700: 7472 5f67 6574 5f62 6f6f 6c20 2865 6872  tr_get_bool (ehr
+00008710: 6f6f 742c 2022 2f46 4453 4e2f 466c 6167  oot, "/FDSN/Flag
+00008720: 732f 456e 644f 6654 696d 6553 6572 6965  s/EndOfTimeSerie
+00008730: 7322 2c20 2668 6561 6465 725f 626f 6f6c  s", &header_bool
+00008740: 6561 6e29 2026 2620 6865 6164 6572 5f62  ean) && header_b
+00008750: 6f6f 6c65 616e 2920 2f2a 2042 6974 2034  oolean) /* Bit 4
+00008760: 202a 2f0a 2020 2020 2a70 4d53 3246 5344   */.    *pMS2FSD
+00008770: 485f 494f 464c 4147 5320 2872 6563 6f72  H_IOFLAGS (recor
+00008780: 6429 207c 3d20 3078 3130 3b0a 2020 6966  d) |= 0x10;.  if
+00008790: 2028 6d73 722d 3e66 6c61 6773 2026 2030   (msr->flags & 0
+000087a0: 7830 3429 202f 2a20 4269 7420 3520 2a2f  x04) /* Bit 5 */
+000087b0: 0a20 2020 202a 704d 5332 4653 4448 5f49  .    *pMS2FSDH_I
+000087c0: 4f46 4c41 4753 2028 7265 636f 7264 2920  OFLAGS (record) 
+000087d0: 7c3d 2030 7832 303b 0a0a 2020 2f2a 204d  |= 0x20;..  /* M
+000087e0: 6170 2064 6174 6120 7175 616c 6974 7920  ap data quality 
+000087f0: 6269 7420 666c 6167 7320 2a2f 0a20 202a  bit flags */.  *
+00008800: 704d 5332 4653 4448 5f44 5146 4c41 4753  pMS2FSDH_DQFLAGS
+00008810: 2028 7265 636f 7264 2920 3d20 303b 0a20   (record) = 0;. 
+00008820: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
+00008830: 6765 745f 626f 6f6c 2028 6568 726f 6f74  get_bool (ehroot
+00008840: 2c20 222f 4644 534e 2f46 6c61 6773 2f41  , "/FDSN/Flags/A
+00008850: 6d70 6c69 6669 6572 5361 7475 7261 7469  mplifierSaturati
+00008860: 6f6e 222c 2026 6865 6164 6572 5f62 6f6f  on", &header_boo
+00008870: 6c65 616e 2920 2626 2068 6561 6465 725f  lean) && header_
+00008880: 626f 6f6c 6561 6e29 202f 2a20 4269 7420  boolean) /* Bit 
+00008890: 3020 2a2f 0a20 2020 202a 704d 5332 4653  0 */.    *pMS2FS
+000088a0: 4448 5f44 5146 4c41 4753 2028 7265 636f  DH_DQFLAGS (reco
+000088b0: 7264 2920 7c3d 2030 7830 313b 0a20 2069  rd) |= 0x01;.  i
+000088c0: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
+000088d0: 745f 626f 6f6c 2028 6568 726f 6f74 2c20  t_bool (ehroot, 
+000088e0: 222f 4644 534e 2f46 6c61 6773 2f44 6967  "/FDSN/Flags/Dig
+000088f0: 6974 697a 6572 436c 6970 7069 6e67 222c  itizerClipping",
+00008900: 2026 6865 6164 6572 5f62 6f6f 6c65 616e   &header_boolean
+00008910: 2920 2626 2068 6561 6465 725f 626f 6f6c  ) && header_bool
+00008920: 6561 6e29 202f 2a20 4269 7420 3120 2a2f  ean) /* Bit 1 */
+00008930: 0a20 2020 202a 704d 5332 4653 4448 5f44  .    *pMS2FSDH_D
+00008940: 5146 4c41 4753 2028 7265 636f 7264 2920  QFLAGS (record) 
+00008950: 7c3d 2030 7830 323b 0a20 2069 6620 2879  |= 0x02;.  if (y
+00008960: 796a 736f 6e5f 7074 725f 6765 745f 626f  yjson_ptr_get_bo
+00008970: 6f6c 2028 6568 726f 6f74 2c20 222f 4644  ol (ehroot, "/FD
+00008980: 534e 2f46 6c61 6773 2f53 7069 6b65 7322  SN/Flags/Spikes"
+00008990: 2c20 2668 6561 6465 725f 626f 6f6c 6561  , &header_boolea
+000089a0: 6e29 2026 2620 6865 6164 6572 5f62 6f6f  n) && header_boo
+000089b0: 6c65 616e 2920 2f2a 2042 6974 2032 202a  lean) /* Bit 2 *
+000089c0: 2f0a 2020 2020 2a70 4d53 3246 5344 485f  /.    *pMS2FSDH_
+000089d0: 4451 464c 4147 5320 2872 6563 6f72 6429  DQFLAGS (record)
+000089e0: 207c 3d20 3078 3034 3b0a 2020 6966 2028   |= 0x04;.  if (
+000089f0: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f62  yyjson_ptr_get_b
+00008a00: 6f6f 6c20 2865 6872 6f6f 742c 2022 2f46  ool (ehroot, "/F
+00008a10: 4453 4e2f 466c 6167 732f 476c 6974 6368  DSN/Flags/Glitch
+00008a20: 6573 222c 2026 6865 6164 6572 5f62 6f6f  es", &header_boo
+00008a30: 6c65 616e 2920 2626 2068 6561 6465 725f  lean) && header_
+00008a40: 626f 6f6c 6561 6e29 202f 2a20 4269 7420  boolean) /* Bit 
+00008a50: 3320 2a2f 0a20 2020 202a 704d 5332 4653  3 */.    *pMS2FS
+00008a60: 4448 5f44 5146 4c41 4753 2028 7265 636f  DH_DQFLAGS (reco
+00008a70: 7264 2920 7c3d 2030 7830 383b 0a20 2069  rd) |= 0x08;.  i
+00008a80: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
+00008a90: 745f 626f 6f6c 2028 6568 726f 6f74 2c20  t_bool (ehroot, 
+00008aa0: 222f 4644 534e 2f46 6c61 6773 2f4d 6973  "/FDSN/Flags/Mis
+00008ab0: 7369 6e67 4461 7461 222c 2026 6865 6164  singData", &head
+00008ac0: 6572 5f62 6f6f 6c65 616e 2920 2626 2068  er_boolean) && h
+00008ad0: 6561 6465 725f 626f 6f6c 6561 6e29 202f  eader_boolean) /
+00008ae0: 2a20 4269 7420 3420 2a2f 0a20 2020 202a  * Bit 4 */.    *
+00008af0: 704d 5332 4653 4448 5f44 5146 4c41 4753  pMS2FSDH_DQFLAGS
+00008b00: 2028 7265 636f 7264 2920 7c3d 2030 7831   (record) |= 0x1
+00008b10: 303b 0a20 2069 6620 2879 796a 736f 6e5f  0;.  if (yyjson_
+00008b20: 7074 725f 6765 745f 626f 6f6c 2028 6568  ptr_get_bool (eh
+00008b30: 726f 6f74 2c20 222f 4644 534e 2f46 6c61  root, "/FDSN/Fla
+00008b40: 6773 2f54 656c 656d 6574 7279 5379 6e63  gs/TelemetrySync
+00008b50: 4572 726f 7222 2c20 2668 6561 6465 725f  Error", &header_
+00008b60: 626f 6f6c 6561 6e29 2026 2620 6865 6164  boolean) && head
+00008b70: 6572 5f62 6f6f 6c65 616e 2920 2f2a 2042  er_boolean) /* B
+00008b80: 6974 2035 202a 2f0a 2020 2020 2a70 4d53  it 5 */.    *pMS
+00008b90: 3246 5344 485f 4451 464c 4147 5320 2872  2FSDH_DQFLAGS (r
+00008ba0: 6563 6f72 6429 207c 3d20 3078 3230 3b0a  ecord) |= 0x20;.
+00008bb0: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+00008bc0: 5f67 6574 5f62 6f6f 6c20 2865 6872 6f6f  _get_bool (ehroo
+00008bd0: 742c 2022 2f46 4453 4e2f 466c 6167 732f  t, "/FDSN/Flags/
+00008be0: 4669 6c74 6572 4368 6172 6769 6e67 222c  FilterCharging",
+00008bf0: 2026 6865 6164 6572 5f62 6f6f 6c65 616e   &header_boolean
+00008c00: 2920 2626 2068 6561 6465 725f 626f 6f6c  ) && header_bool
+00008c10: 6561 6e29 202f 2a20 4269 7420 3620 2a2f  ean) /* Bit 6 */
+00008c20: 0a20 2020 202a 704d 5332 4653 4448 5f44  .    *pMS2FSDH_D
+00008c30: 5146 4c41 4753 2028 7265 636f 7264 2920  QFLAGS (record) 
+00008c40: 7c3d 2030 7834 303b 0a20 2069 6620 286d  |= 0x40;.  if (m
+00008c50: 7372 2d3e 666c 6167 7320 2620 3078 3032  sr->flags & 0x02
+00008c60: 2920 2f2a 2042 6974 2037 202a 2f0a 2020  ) /* Bit 7 */.  
+00008c70: 2020 2a70 4d53 3246 5344 485f 4451 464c    *pMS2FSDH_DQFL
+00008c80: 4147 5320 2872 6563 6f72 6429 207c 3d20  AGS (record) |= 
+00008c90: 3078 3830 3b0a 0a20 2069 6620 2879 796a  0x80;..  if (yyj
+00008ca0: 736f 6e5f 7074 725f 6765 745f 6e75 6d20  son_ptr_get_num 
+00008cb0: 2865 6872 6f6f 742c 2022 2f46 4453 4e2f  (ehroot, "/FDSN/
+00008cc0: 5469 6d65 2f43 6f72 7265 6374 696f 6e22  Time/Correction"
+00008cd0: 2c20 2668 6561 6465 725f 6e75 6d62 6572  , &header_number
+00008ce0: 2929 0a20 207b 0a20 2020 202a 704d 5332  )).  {.    *pMS2
+00008cf0: 4653 4448 5f54 494d 4543 4f52 5245 4354  FSDH_TIMECORRECT
+00008d00: 2028 7265 636f 7264 2920 3d20 484f 3464   (record) = HO4d
+00008d10: 2028 2869 6e74 3332 5f74 2928 6865 6164   ((int32_t)(head
+00008d20: 6572 5f6e 756d 6265 7220 2a20 3130 3030  er_number * 1000
+00008d30: 3020 2b20 302e 3529 2c20 7377 6170 666c  0 + 0.5), swapfl
+00008d40: 6167 293b 0a0a 2020 2020 2f2a 2053 6574  ag);..    /* Set
+00008d50: 2074 696d 6520 636f 7272 6563 7469 6f6e   time correction
+00008d60: 2061 7070 6c69 6564 2062 6974 2069 6e20   applied bit in 
+00008d70: 6163 7469 7669 7479 2066 6c61 6773 2e0a  activity flags..
+00008d80: 2020 2020 2020 2052 6174 696f 6e61 6c65         Rationale
+00008d90: 3a20 5633 2072 6563 6f72 6473 2064 6f20  : V3 records do 
+00008da0: 6e6f 7420 616c 6c6f 7720 756e 6170 706c  not allow unappl
+00008db0: 6965 6420 7469 6d65 2063 6f72 7265 6374  ied time correct
+00008dc0: 696f 6e73 2061 6e64 2075 6e61 7070 6c69  ions and unappli
+00008dd0: 6564 0a20 2020 2020 2020 7469 6d65 2063  ed.       time c
+00008de0: 6f72 7265 6374 696f 6e73 2069 6e20 5632  orrections in V2
+00008df0: 2072 6563 6f72 6473 2061 7265 2061 6c77   records are alw
+00008e00: 6179 7320 6170 706c 6965 6420 6f6e 2072  ays applied on r
+00008e10: 6561 6420 6279 2074 6869 7320 6c69 6272  ead by this libr
+00008e20: 6172 792e 202a 2f0a 2020 2020 2a70 4d53  ary. */.    *pMS
+00008e30: 3246 5344 485f 4143 5446 4c41 4753 2028  2FSDH_ACTFLAGS (
+00008e40: 7265 636f 7264 2920 7c3d 2030 7830 323b  record) |= 0x02;
+00008e50: 0a20 207d 0a20 2065 6c73 650a 2020 7b0a  .  }.  else.  {.
+00008e60: 2020 2020 2a70 4d53 3246 5344 485f 5449      *pMS2FSDH_TI
+00008e70: 4d45 434f 5252 4543 5420 2872 6563 6f72  MECORRECT (recor
+00008e80: 6429 203d 2030 3b0a 2020 7d0a 0a20 202a  d) = 0;.  }..  *
+00008e90: 704d 5332 4653 4448 5f4e 554d 424c 4f43  pMS2FSDH_NUMBLOC
+00008ea0: 4b45 5454 4553 2028 7265 636f 7264 2920  KETTES (record) 
+00008eb0: 2020 3d20 313b 0a20 202a 704d 5332 4653    = 1;.  *pMS2FS
+00008ec0: 4448 5f44 4154 414f 4646 5345 5420 2872  DH_DATAOFFSET (r
+00008ed0: 6563 6f72 6429 2020 2020 2020 3d20 303b  ecord)      = 0;
+00008ee0: 0a20 202a 704d 5332 4653 4448 5f42 4c4f  .  *pMS2FSDH_BLO
+00008ef0: 434b 4554 5445 4f46 4653 4554 2028 7265  CKETTEOFFSET (re
+00008f00: 636f 7264 2920 3d20 484f 3275 2028 3438  cord) = HO2u (48
+00008f10: 2c20 7377 6170 666c 6167 293b 0a0a 2020  , swapflag);..  
+00008f20: 7772 6974 7465 6e20 3d20 3438 3b0a 0a20  written = 48;.. 
+00008f30: 202f 2a20 4164 6420 6d61 6e64 6174 6f72   /* Add mandator
+00008f40: 7920 426c 6f63 6b65 7474 6520 3130 3030  y Blockette 1000
+00008f50: 202a 2f0a 2020 6e65 7874 5f62 6c6f 636b   */.  next_block
+00008f60: 6574 7465 203d 2070 4d53 3242 3130 3030  ette = pMS2B1000
+00008f70: 5f4e 4558 5420 2872 6563 6f72 6420 2b20  _NEXT (record + 
+00008f80: 7772 6974 7465 6e29 3b0a 0a20 202a 704d  written);..  *pM
+00008f90: 5332 4231 3030 305f 5459 5045 2028 7265  S2B1000_TYPE (re
+00008fa0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+00008fb0: 2020 2020 203d 2048 4f32 7520 2831 3030       = HO2u (100
+00008fc0: 302c 2073 7761 7066 6c61 6729 3b0a 2020  0, swapflag);.  
+00008fd0: 2a70 4d53 3242 3130 3030 5f4e 4558 5420  *pMS2B1000_NEXT 
+00008fe0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+00008ff0: 6e29 2020 2020 2020 3d20 303b 0a20 202a  n)      = 0;.  *
+00009000: 704d 5332 4231 3030 305f 454e 434f 4449  pMS2B1000_ENCODI
+00009010: 4e47 2028 7265 636f 7264 202b 2077 7269  NG (record + wri
+00009020: 7474 656e 2920 203d 2065 6e63 6f64 696e  tten)  = encodin
+00009030: 673b 0a20 202a 704d 5332 4231 3030 305f  g;.  *pMS2B1000_
+00009040: 4259 5445 4f52 4445 5220 2872 6563 6f72  BYTEORDER (recor
+00009050: 6420 2b20 7772 6974 7465 6e29 203d 2031  d + written) = 1
+00009060: 3b0a 2020 2a70 4d53 3242 3130 3030 5f52  ;.  *pMS2B1000_R
+00009070: 4543 4c45 4e20 2872 6563 6f72 6420 2b20  ECLEN (record + 
+00009080: 7772 6974 7465 6e29 2020 2020 3d20 7265  written)    = re
+00009090: 636c 656e 6578 703b 0a20 202a 704d 5332  clenexp;.  *pMS2
+000090a0: 4231 3030 305f 5245 5345 5256 4544 2028  B1000_RESERVED (
+000090b0: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+000090c0: 2920 203d 2030 3b0a 0a20 2077 7269 7474  )  = 0;..  writt
+000090d0: 656e 202b 3d20 383b 0a0a 2020 2f2a 2041  en += 8;..  /* A
+000090e0: 6464 2042 6c6f 636b 6574 7465 2031 3030  dd Blockette 100
+000090f0: 3120 6966 206d 6963 726f 7365 636f 6e64  1 if microsecond
+00009100: 206f 6666 7365 7420 6f72 2074 696d 696e   offset or timin
+00009110: 6720 7175 616c 6974 7920 6973 2070 7265  g quality is pre
+00009120: 7365 6e74 202a 2f0a 2020 6966 2028 7979  sent */.  if (yy
+00009130: 6a73 6f6e 5f70 7472 5f67 6574 5f75 696e  json_ptr_get_uin
+00009140: 7420 2865 6872 6f6f 742c 2022 2f46 4453  t (ehroot, "/FDS
+00009150: 4e2f 5469 6d65 2f51 7561 6c69 7479 222c  N/Time/Quality",
+00009160: 2026 6865 6164 6572 5f75 696e 7429 207c   &header_uint) |
+00009170: 7c20 6d73 6563 5f6f 6666 7365 7429 0a20  | msec_offset). 
+00009180: 207b 0a20 2020 202a 6e65 7874 5f62 6c6f   {.    *next_blo
+00009190: 636b 6574 7465 203d 2048 4f32 7520 2828  ckette = HO2u ((
+000091a0: 7569 6e74 3136 5f74 2977 7269 7474 656e  uint16_t)written
+000091b0: 2c20 7377 6170 666c 6167 293b 0a20 2020  , swapflag);.   
+000091c0: 206e 6578 745f 626c 6f63 6b65 7474 6520   next_blockette 
+000091d0: 3d20 704d 5332 4231 3030 315f 4e45 5854  = pMS2B1001_NEXT
+000091e0: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
+000091f0: 656e 293b 0a20 2020 202a 704d 5332 4653  en);.    *pMS2FS
+00009200: 4448 5f4e 554d 424c 4f43 4b45 5454 4553  DH_NUMBLOCKETTES
+00009210: 2028 7265 636f 7264 2920 2b3d 2031 3b0a   (record) += 1;.
+00009220: 0a20 2020 202a 704d 5332 4231 3030 315f  .    *pMS2B1001_
+00009230: 5459 5045 2028 7265 636f 7264 202b 2077  TYPE (record + w
+00009240: 7269 7474 656e 2920 3d20 484f 3275 2028  ritten) = HO2u (
+00009250: 3130 3031 2c20 7377 6170 666c 6167 293b  1001, swapflag);
+00009260: 0a20 2020 202a 704d 5332 4231 3030 315f  .    *pMS2B1001_
+00009270: 4e45 5854 2028 7265 636f 7264 202b 2077  NEXT (record + w
+00009280: 7269 7474 656e 2920 3d20 303b 0a0a 2020  ritten) = 0;..  
+00009290: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+000092a0: 5f67 6574 5f75 696e 7420 2865 6872 6f6f  _get_uint (ehroo
+000092b0: 742c 2022 2f46 4453 4e2f 5469 6d65 2f51  t, "/FDSN/Time/Q
+000092c0: 7561 6c69 7479 222c 2026 6865 6164 6572  uality", &header
+000092d0: 5f75 696e 7429 2026 2620 6865 6164 6572  _uint) && header
+000092e0: 5f75 696e 7420 3c3d 2055 494e 5438 5f4d  _uint <= UINT8_M
+000092f0: 4158 290a 2020 2020 2020 2a70 4d53 3242  AX).      *pMS2B
+00009300: 3130 3031 5f54 494d 494e 4751 5541 4c49  1001_TIMINGQUALI
+00009310: 5459 2028 7265 636f 7264 202b 2077 7269  TY (record + wri
+00009320: 7474 656e 2920 3d20 2875 696e 7438 5f74  tten) = (uint8_t
+00009330: 2920 2868 6561 6465 725f 7569 6e74 293b  ) (header_uint);
+00009340: 0a20 2020 2065 6c73 650a 2020 2020 2020  .    else.      
+00009350: 2a70 4d53 3242 3130 3031 5f54 494d 494e  *pMS2B1001_TIMIN
+00009360: 4751 5541 4c49 5459 2028 7265 636f 7264  GQUALITY (record
+00009370: 202b 2077 7269 7474 656e 2920 3d20 303b   + written) = 0;
+00009380: 0a0a 2020 2020 2a70 4d53 3242 3130 3031  ..    *pMS2B1001
+00009390: 5f4d 4943 524f 5345 434f 4e44 2028 7265  _MICROSECOND (re
+000093a0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+000093b0: 3d20 6d73 6563 5f6f 6666 7365 743b 0a20  = msec_offset;. 
+000093c0: 2020 202a 704d 5332 4231 3030 315f 5245     *pMS2B1001_RE
+000093d0: 5345 5256 4544 2028 7265 636f 7264 202b  SERVED (record +
+000093e0: 2077 7269 7474 656e 2920 2020 203d 2030   written)    = 0
+000093f0: 3b0a 2020 2020 2a70 4d53 3242 3130 3031  ;.    *pMS2B1001
+00009400: 5f46 5241 4d45 434f 554e 5420 2872 6563  _FRAMECOUNT (rec
+00009410: 6f72 6420 2b20 7772 6974 7465 6e29 2020  ord + written)  
+00009420: 3d20 303b 0a0a 2020 2020 7772 6974 7465  = 0;..    writte
+00009430: 6e20 2b3d 2038 3b0a 2020 7d0a 0a20 202f  n += 8;.  }..  /
+00009440: 2a20 4164 6420 426c 6f63 6b65 7474 6520  * Add Blockette 
+00009450: 3130 3020 6966 2073 616d 706c 6520 7261  100 if sample ra
+00009460: 7465 2069 7320 6e6f 7420 7765 6c6c 2072  te is not well r
+00009470: 6570 7265 7365 6e74 6564 2062 7920 6661  epresented by fa
+00009480: 6374 6f72 2f6d 756c 7469 706c 6965 7220  ctor/multiplier 
+00009490: 2a2f 0a20 2069 6620 2866 6162 7328 6d73  */.  if (fabs(ms
+000094a0: 7233 5f73 616d 7072 6174 6568 7a28 6d73  r3_sampratehz(ms
+000094b0: 7229 202d 206d 735f 6e6f 6d73 616d 7072  r) - ms_nomsampr
+000094c0: 6174 6528 6661 6374 6f72 2c20 6d75 6c74  ate(factor, mult
+000094d0: 6970 6c69 6572 2929 203e 2030 2e30 3030  iplier)) > 0.000
+000094e0: 3129 0a20 207b 0a20 2020 202a 6e65 7874  1).  {.    *next
+000094f0: 5f62 6c6f 636b 6574 7465 203d 2048 4f32  _blockette = HO2
+00009500: 7520 2828 7569 6e74 3136 5f74 2977 7269  u ((uint16_t)wri
+00009510: 7474 656e 2c20 7377 6170 666c 6167 293b  tten, swapflag);
+00009520: 0a20 2020 206e 6578 745f 626c 6f63 6b65  .    next_blocke
+00009530: 7474 6520 3d20 704d 5332 4231 3030 5f4e  tte = pMS2B100_N
+00009540: 4558 5420 2872 6563 6f72 6420 2b20 7772  EXT (record + wr
+00009550: 6974 7465 6e29 3b0a 2020 2020 2a70 4d53  itten);.    *pMS
+00009560: 3246 5344 485f 4e55 4d42 4c4f 434b 4554  2FSDH_NUMBLOCKET
+00009570: 5445 5320 2872 6563 6f72 6429 202b 3d20  TES (record) += 
+00009580: 313b 0a0a 2020 2020 2a70 4d53 3242 3130  1;..    *pMS2B10
+00009590: 305f 5459 5045 2028 7265 636f 7264 202b  0_TYPE (record +
+000095a0: 2077 7269 7474 656e 2920 2020 2020 3d20   written)     = 
+000095b0: 484f 3275 2028 3130 302c 2073 7761 7066  HO2u (100, swapf
+000095c0: 6c61 6729 3b0a 2020 2020 2a70 4d53 3242  lag);.    *pMS2B
+000095d0: 3130 305f 4e45 5854 2028 7265 636f 7264  100_NEXT (record
+000095e0: 202b 2077 7269 7474 656e 2920 2020 2020   + written)     
+000095f0: 3d20 303b 0a20 2020 202a 704d 5332 4231  = 0;.    *pMS2B1
+00009600: 3030 5f53 414d 5052 4154 4520 2872 6563  00_SAMPRATE (rec
+00009610: 6f72 6420 2b20 7772 6974 7465 6e29 203d  ord + written) =
+00009620: 2048 4f34 6620 2828 666c 6f61 7429 6d73   HO4f ((float)ms
+00009630: 722d 3e73 616d 7072 6174 652c 2073 7761  r->samprate, swa
+00009640: 7066 6c61 6729 3b0a 2020 2020 2a70 4d53  pflag);.    *pMS
+00009650: 3242 3130 305f 464c 4147 5320 2872 6563  2B100_FLAGS (rec
+00009660: 6f72 6420 2b20 7772 6974 7465 6e29 2020  ord + written)  
+00009670: 2020 3d20 303b 0a20 2020 206d 656d 7365    = 0;.    memse
+00009680: 7420 2870 4d53 3242 3130 305f 5245 5345  t (pMS2B100_RESE
+00009690: 5256 4544 2028 7265 636f 7264 202b 2077  RVED (record + w
+000096a0: 7269 7474 656e 292c 2030 2c20 3329 3b0a  ritten), 0, 3);.
+000096b0: 0a20 2020 2077 7269 7474 656e 202b 3d20  .    written += 
+000096c0: 3132 3b0a 2020 7d0a 0a20 202f 2a20 4164  12;.  }..  /* Ad
+000096d0: 6420 426c 6f63 6b65 7474 6520 3530 3020  d Blockette 500 
+000096e0: 666f 7220 7469 6d69 6e67 2065 7865 6365  for timing exece
+000096f0: 7074 696f 6e73 202a 2f0a 2020 6966 2028  ptions */.  if (
+00009700: 2865 6861 7272 203d 2079 796a 736f 6e5f  (eharr = yyjson_
+00009710: 7074 725f 6765 7420 2865 6872 6f6f 742c  ptr_get (ehroot,
+00009720: 2022 2f46 4453 4e2f 5469 6d65 2f45 7863   "/FDSN/Time/Exc
+00009730: 6570 7469 6f6e 2229 2920 2626 2079 796a  eption")) && yyj
+00009740: 736f 6e5f 6973 5f61 7272 2028 6568 6172  son_is_arr (ehar
+00009750: 7229 290a 2020 7b0a 2020 2020 7979 6a73  r)).  {.    yyjs
+00009760: 6f6e 5f61 7272 5f69 7465 725f 696e 6974  on_arr_iter_init
+00009770: 2028 6568 6172 722c 2026 6568 6974 6572   (eharr, &ehiter
+00009780: 293b 0a0a 2020 2020 7768 696c 6520 2828  );..    while ((
+00009790: 6568 6974 6572 7661 6c20 3d20 7979 6a73  ehiterval = yyjs
+000097a0: 6f6e 5f61 7272 5f69 7465 725f 6e65 7874  on_arr_iter_next
+000097b0: 2028 2665 6869 7465 7229 2929 0a20 2020   (&ehiter))).   
+000097c0: 207b 0a20 2020 2020 2069 6620 2821 7979   {.      if (!yy
+000097d0: 6a73 6f6e 5f69 735f 6f62 6a20 2865 6869  json_is_obj (ehi
+000097e0: 7465 7276 616c 2929 0a20 2020 2020 2020  terval)).       
+000097f0: 2063 6f6e 7469 6e75 653b 0a0a 2020 2020   continue;..    
+00009800: 2020 626c 6f63 6b65 7474 655f 6c65 6e67    blockette_leng
+00009810: 7468 203d 2032 3030 3b0a 0a20 2020 2020  th = 200;..     
+00009820: 2069 6620 2828 7265 6362 7566 6c65 6e20   if ((recbuflen 
+00009830: 2d20 7772 6974 7465 6e29 203c 2062 6c6f  - written) < blo
+00009840: 636b 6574 7465 5f6c 656e 6774 6829 0a20  ckette_length). 
+00009850: 2020 2020 207b 0a20 2020 2020 2020 206d       {.        m
+00009860: 735f 6c6f 6720 2832 2c20 2225 733a 2052  s_log (2, "%s: R
+00009870: 6563 6f72 6420 6c65 6e67 7468 206e 6f74  ecord length not
+00009880: 206c 6172 6765 2065 6e6f 7567 6820 666f   large enough fo
+00009890: 7220 4235 3030 5c6e 222c 206d 7372 2d3e  r B500\n", msr->
+000098a0: 7369 6429 3b0a 2020 2020 2020 2020 7979  sid);.        yy
+000098b0: 6a73 6f6e 5f64 6f63 5f66 7265 6520 2865  json_doc_free (e
+000098c0: 6864 6f63 293b 0a20 2020 2020 2020 2072  hdoc);.        r
+000098d0: 6574 7572 6e20 2d31 3b0a 2020 2020 2020  eturn -1;.      
+000098e0: 7d0a 0a20 2020 2020 202a 6e65 7874 5f62  }..      *next_b
+000098f0: 6c6f 636b 6574 7465 203d 2048 4f32 7520  lockette = HO2u 
+00009900: 2828 7569 6e74 3136 5f74 2977 7269 7474  ((uint16_t)writt
+00009910: 656e 2c20 7377 6170 666c 6167 293b 0a20  en, swapflag);. 
+00009920: 2020 2020 206e 6578 745f 626c 6f63 6b65       next_blocke
+00009930: 7474 6520 203d 2070 4d53 3242 3530 305f  tte  = pMS2B500_
+00009940: 4e45 5854 2028 7265 636f 7264 202b 2077  NEXT (record + w
+00009950: 7269 7474 656e 293b 0a20 2020 2020 202a  ritten);.      *
+00009960: 704d 5332 4653 4448 5f4e 554d 424c 4f43  pMS2FSDH_NUMBLOC
+00009970: 4b45 5454 4553 2028 7265 636f 7264 2920  KETTES (record) 
+00009980: 2b3d 2031 3b0a 0a20 2020 2020 206d 656d  += 1;..      mem
+00009990: 7365 7420 2872 6563 6f72 6420 2b20 7772  set (record + wr
+000099a0: 6974 7465 6e2c 2030 2c20 626c 6f63 6b65  itten, 0, blocke
+000099b0: 7474 655f 6c65 6e67 7468 293b 0a20 2020  tte_length);.   
+000099c0: 2020 202a 704d 5332 4235 3030 5f54 5950     *pMS2B500_TYP
+000099d0: 4520 2872 6563 6f72 6420 2b20 7772 6974  E (record + writ
+000099e0: 7465 6e29 203d 2048 4f32 7520 2835 3030  ten) = HO2u (500
+000099f0: 2c20 7377 6170 666c 6167 293b 0a20 2020  , swapflag);.   
+00009a00: 2020 202a 704d 5332 4235 3030 5f4e 4558     *pMS2B500_NEX
+00009a10: 5420 2872 6563 6f72 6420 2b20 7772 6974  T (record + writ
+00009a20: 7465 6e29 203d 2030 3b0a 0a20 2020 2020  ten) = 0;..     
+00009a30: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
+00009a40: 6765 745f 6e75 6d20 2865 6869 7465 7276  get_num (ehiterv
+00009a50: 616c 2c20 222f 5643 4f43 6f72 7265 6374  al, "/VCOCorrect
+00009a60: 696f 6e22 2c20 2668 6561 6465 725f 6e75  ion", &header_nu
+00009a70: 6d62 6572 2929 0a20 2020 2020 2020 202a  mber)).        *
+00009a80: 704d 5332 4235 3030 5f56 434f 434f 5252  pMS2B500_VCOCORR
+00009a90: 4543 5449 4f4e 2028 7265 636f 7264 202b  ECTION (record +
+00009aa0: 2077 7269 7474 656e 2920 3d20 484f 3466   written) = HO4f
+00009ab0: 2028 2866 6c6f 6174 2968 6561 6465 725f   ((float)header_
+00009ac0: 6e75 6d62 6572 2c20 7377 6170 666c 6167  number, swapflag
+00009ad0: 293b 0a0a 2020 2020 2020 6966 2028 7979  );..      if (yy
+00009ae0: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
+00009af0: 2028 6568 6974 6572 7661 6c2c 2022 2f54   (ehiterval, "/T
+00009b00: 696d 6522 2c20 2668 6561 6465 725f 7374  ime", &header_st
+00009b10: 7269 6e67 2929 0a20 2020 2020 207b 0a20  ring)).      {. 
+00009b20: 2020 2020 2020 2069 6e74 3634 5f74 206c         int64_t l
+00009b30: 5f6e 7365 633b 0a20 2020 2020 2020 2075  _nsec;.        u
+00009b40: 696e 7431 365f 7420 6c5f 6673 6563 3b0a  int16_t l_fsec;.
+00009b50: 2020 2020 2020 2020 696e 7438 5f74 206c          int8_t l
+00009b60: 5f6d 7365 635f 6f66 6673 6574 3b0a 0a20  _msec_offset;.. 
+00009b70: 2020 2020 2020 206c 5f6e 7365 6320 3d20         l_nsec = 
+00009b80: 6d73 5f74 696d 6573 7472 3262 7469 6d65  ms_timestr2btime
+00009b90: 2028 6865 6164 6572 5f73 7472 696e 672c   (header_string,
+00009ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 2020 2020 2875 696e 7438 5f74 202a 2970      (uint8_t *)p
+00009bd0: 4d53 3242 3530 305f 5945 4152 2028 7265  MS2B500_YEAR (re
+00009be0: 636f 7264 202b 2077 7269 7474 656e 292c  cord + written),
+00009bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2020 2020 6d73 722d 3e73 6964 2c20 7377      msr->sid, sw
+00009c20: 6170 666c 6167 293b 0a0a 2020 2020 2020  apflag);..      
+00009c30: 2020 6966 2028 6c5f 6e73 6563 203d 3d20    if (l_nsec == 
+00009c40: 2d31 290a 2020 2020 2020 2020 7b0a 2020  -1).        {.  
+00009c50: 2020 2020 2020 2020 6d73 5f6c 6f67 2028          ms_log (
+00009c60: 322c 2022 2573 3a20 4361 6e6e 6f74 2063  2, "%s: Cannot c
+00009c70: 6f6e 7665 7274 2042 3530 3020 7469 6d65  onvert B500 time
+00009c80: 3a20 2573 5c6e 222c 206d 7372 2d3e 7369  : %s\n", msr->si
+00009c90: 642c 2068 6561 6465 725f 7374 7269 6e67  d, header_string
+00009ca0: 293b 0a20 2020 2020 2020 2020 2079 796a  );.          yyj
+00009cb0: 736f 6e5f 646f 635f 6672 6565 2028 6568  son_doc_free (eh
+00009cc0: 646f 6329 3b0a 2020 2020 2020 2020 2020  doc);.          
+00009cd0: 7265 7475 726e 202d 313b 0a20 2020 2020  return -1;.     
+00009ce0: 2020 207d 0a0a 2020 2020 2020 2020 2f2a     }..        /*
+00009cf0: 2043 616c 6375 6c61 7465 2074 696d 6520   Calculate time 
+00009d00: 6174 2066 7261 6374 696f 6e61 6c20 3130  at fractional 10
+00009d10: 3075 7365 6320 7265 736f 6c75 7469 6f6e  0usec resolution
+00009d20: 2061 6e64 206d 6963 726f 7365 636f 6e64   and microsecond
+00009d30: 206f 6666 7365 7420 2a2f 0a20 2020 2020   offset */.     
+00009d40: 2020 206c 5f66 7365 6320 2020 2020 2020     l_fsec       
+00009d50: 203d 2028 7569 6e74 3136 5f74 2928 6c5f   = (uint16_t)(l_
+00009d60: 6e73 6563 202f 2031 3030 3030 3029 3b0a  nsec / 100000);.
+00009d70: 2020 2020 2020 2020 6c5f 6d73 6563 5f6f          l_msec_o
+00009d80: 6666 7365 7420 3d20 2869 6e74 385f 7429  ffset = (int8_t)
+00009d90: 2828 6c5f 6e73 6563 202f 2031 3030 3029  ((l_nsec / 1000)
+00009da0: 202d 2028 6c5f 6673 6563 202a 2031 3030   - (l_fsec * 100
+00009db0: 2929 3b0a 0a20 2020 2020 2020 202a 704d  ));..        *pM
+00009dc0: 5332 4235 3030 5f4d 4943 524f 5345 434f  S2B500_MICROSECO
+00009dd0: 4e44 2028 7265 636f 7264 202b 2077 7269  ND (record + wri
+00009de0: 7474 656e 2920 3d20 6c5f 6d73 6563 5f6f  tten) = l_msec_o
+00009df0: 6666 7365 743b 0a20 2020 2020 207d 0a0a  ffset;.      }..
+00009e00: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+00009e10: 5f70 7472 5f67 6574 5f75 696e 7420 2865  _ptr_get_uint (e
+00009e20: 6869 7465 7276 616c 2c20 222f 5265 6365  hiterval, "/Rece
+00009e30: 7074 696f 6e51 7561 6c69 7479 222c 2026  ptionQuality", &
+00009e40: 6865 6164 6572 5f75 696e 7429 2026 2620  header_uint) && 
+00009e50: 6865 6164 6572 5f75 696e 7420 3c3d 2055  header_uint <= U
+00009e60: 494e 5438 5f4d 4158 290a 2020 2020 2020  INT8_MAX).      
+00009e70: 2020 2a70 4d53 3242 3530 305f 5245 4345    *pMS2B500_RECE
+00009e80: 5054 494f 4e51 5541 4c49 5459 2028 7265  PTIONQUALITY (re
+00009e90: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+00009ea0: 3d20 2875 696e 7438 5f74 2968 6561 6465  = (uint8_t)heade
+00009eb0: 725f 7569 6e74 3b0a 0a20 2020 2020 2069  r_uint;..      i
+00009ec0: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
+00009ed0: 745f 7569 6e74 2028 6568 6974 6572 7661  t_uint (ehiterva
+00009ee0: 6c2c 2022 2f43 6f75 6e74 222c 2026 6865  l, "/Count", &he
+00009ef0: 6164 6572 5f75 696e 7429 2026 2620 6865  ader_uint) && he
+00009f00: 6164 6572 5f75 696e 7420 3c3d 2055 494e  ader_uint <= UIN
+00009f10: 5433 325f 4d41 5829 0a20 2020 2020 2020  T32_MAX).       
+00009f20: 202a 704d 5332 4235 3030 5f45 5843 4550   *pMS2B500_EXCEP
+00009f30: 5449 4f4e 434f 554e 5420 2872 6563 6f72  TIONCOUNT (recor
+00009f40: 6420 2b20 7772 6974 7465 6e29 203d 2048  d + written) = H
+00009f50: 4f34 6420 2828 7569 6e74 3332 5f74 2968  O4d ((uint32_t)h
+00009f60: 6561 6465 725f 7569 6e74 2c20 7377 6170  eader_uint, swap
+00009f70: 666c 6167 293b 0a0a 2020 2020 2020 6966  flag);..      if
+00009f80: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+00009f90: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
+00009fa0: 2022 2f54 7970 6522 2c20 2668 6561 6465   "/Type", &heade
+00009fb0: 725f 7374 7269 6e67 2929 0a20 2020 2020  r_string)).     
+00009fc0: 2020 206d 735f 7374 726e 6370 6f70 656e     ms_strncpopen
+00009fd0: 2028 704d 5332 4235 3030 5f45 5843 4550   (pMS2B500_EXCEP
+00009fe0: 5449 4f4e 5459 5045 2028 7265 636f 7264  TIONTYPE (record
+00009ff0: 202b 2077 7269 7474 656e 292c 2068 6561   + written), hea
+0000a000: 6465 725f 7374 7269 6e67 2c20 3136 293b  der_string, 16);
+0000a010: 0a0a 2020 2020 2020 6966 2028 7979 6a73  ..      if (yyjs
+0000a020: 6f6e 5f70 7472 5f67 6574 5f73 7472 2028  on_ptr_get_str (
+0000a030: 6568 726f 6f74 2c20 222f 4644 534e 2f43  ehroot, "/FDSN/C
+0000a040: 6c6f 636b 2f4d 6f64 656c 222c 2026 6865  lock/Model", &he
+0000a050: 6164 6572 5f73 7472 696e 6729 290a 2020  ader_string)).  
+0000a060: 2020 2020 2020 6d73 5f73 7472 6e63 706f        ms_strncpo
+0000a070: 7065 6e20 2870 4d53 3242 3530 305f 434c  pen (pMS2B500_CL
+0000a080: 4f43 4b4d 4f44 454c 2028 7265 636f 7264  OCKMODEL (record
+0000a090: 202b 2077 7269 7474 656e 292c 2068 6561   + written), hea
+0000a0a0: 6465 725f 7374 7269 6e67 2c20 3332 293b  der_string, 32);
+0000a0b0: 0a0a 2020 2020 2020 6966 2028 7979 6a73  ..      if (yyjs
+0000a0c0: 6f6e 5f70 7472 5f67 6574 5f73 7472 2028  on_ptr_get_str (
+0000a0d0: 6568 6974 6572 7661 6c2c 2022 2f43 6c6f  ehiterval, "/Clo
+0000a0e0: 636b 5374 6174 7573 222c 2026 6865 6164  ckStatus", &head
+0000a0f0: 6572 5f73 7472 696e 6729 290a 2020 2020  er_string)).    
+0000a100: 2020 2020 6d73 5f73 7472 6e63 706f 7065      ms_strncpope
+0000a110: 6e20 2870 4d53 3242 3530 305f 434c 4f43  n (pMS2B500_CLOC
+0000a120: 4b53 5441 5455 5320 2872 6563 6f72 6420  KSTATUS (record 
+0000a130: 2b20 7772 6974 7465 6e29 2c20 6865 6164  + written), head
+0000a140: 6572 5f73 7472 696e 672c 2031 3238 293b  er_string, 128);
+0000a150: 0a0a 2020 2020 2020 7772 6974 7465 6e20  ..      written 
+0000a160: 2b3d 2062 6c6f 636b 6574 7465 5f6c 656e  += blockette_len
+0000a170: 6774 683b 0a20 2020 207d 0a20 207d 202f  gth;.    }.  } /
+0000a180: 2a20 456e 6420 6966 202f 4644 534e 2f54  * End if /FDSN/T
+0000a190: 696d 652f 4578 6365 7074 696f 6e20 2a2f  ime/Exception */
+0000a1a0: 0a0a 2020 2f2a 2041 6464 2042 6c6f 636b  ..  /* Add Block
+0000a1b0: 6574 7465 2032 3030 2c32 3031 2066 6f72  ette 200,201 for
+0000a1c0: 2065 7665 6e74 2064 6574 6563 7469 6f6e   event detection
+0000a1d0: 7320 2a2f 0a20 2069 6620 2828 6568 6172  s */.  if ((ehar
+0000a1e0: 7220 3d20 7979 6a73 6f6e 5f70 7472 5f67  r = yyjson_ptr_g
+0000a1f0: 6574 2028 6568 726f 6f74 2c20 222f 4644  et (ehroot, "/FD
+0000a200: 534e 2f45 7665 6e74 2f44 6574 6563 7469  SN/Event/Detecti
+0000a210: 6f6e 2229 2920 2626 2079 796a 736f 6e5f  on")) && yyjson_
+0000a220: 6973 5f61 7272 2028 6568 6172 7229 290a  is_arr (eharr)).
+0000a230: 2020 7b0a 2020 2020 7979 6a73 6f6e 5f61    {.    yyjson_a
+0000a240: 7272 5f69 7465 725f 696e 6974 2028 6568  rr_iter_init (eh
+0000a250: 6172 722c 2026 6568 6974 6572 293b 0a0a  arr, &ehiter);..
+0000a260: 2020 2020 7768 696c 6520 2828 6568 6974      while ((ehit
+0000a270: 6572 7661 6c20 3d20 7979 6a73 6f6e 5f61  erval = yyjson_a
+0000a280: 7272 5f69 7465 725f 6e65 7874 2028 2665  rr_iter_next (&e
+0000a290: 6869 7465 7229 2929 0a20 2020 207b 0a20  hiter))).    {. 
+0000a2a0: 2020 2020 2069 6620 2821 7979 6a73 6f6e       if (!yyjson
+0000a2b0: 5f69 735f 6f62 6a20 2865 6869 7465 7276  _is_obj (ehiterv
+0000a2c0: 616c 2929 0a20 2020 2020 2020 2063 6f6e  al)).        con
+0000a2d0: 7469 6e75 653b 0a0a 2020 2020 2020 2f2a  tinue;..      /*
+0000a2e0: 2044 6574 6572 6d69 6e65 2077 6869 6368   Determine which
+0000a2f0: 2064 6574 6563 7469 6f6e 2074 7970 653a   detection type:
+0000a300: 204d 5552 444f 434b 2076 6572 7375 7320   MURDOCK versus 
+0000a310: 7468 6520 6765 6e65 7269 6320 7479 7065  the generic type
+0000a320: 202a 2f0a 2020 2020 2020 6966 2028 7979   */.      if (yy
+0000a330: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
+0000a340: 2028 6568 6974 6572 7661 6c2c 2022 2f54   (ehiterval, "/T
+0000a350: 7970 6522 2c20 2668 6561 6465 725f 7374  ype", &header_st
+0000a360: 7269 6e67 2920 2626 0a20 2020 2020 2020  ring) &&.       
+0000a370: 2020 2073 7472 6e63 6173 6563 6d70 2028     strncasecmp (
+0000a380: 6865 6164 6572 5f73 7472 696e 672c 2022  header_string, "
+0000a390: 4d55 5244 4f43 4b22 2c20 3729 203d 3d20  MURDOCK", 7) == 
+0000a3a0: 3029 0a20 2020 2020 207b 0a20 2020 2020  0).      {.     
+0000a3b0: 2020 2062 6c6f 636b 6574 7465 5f74 7970     blockette_typ
+0000a3c0: 6520 3d20 3230 313b 0a20 2020 2020 2020  e = 201;.       
+0000a3d0: 2062 6c6f 636b 6574 7465 5f6c 656e 6774   blockette_lengt
+0000a3e0: 6820 3d20 3630 3b0a 2020 2020 2020 7d0a  h = 60;.      }.
+0000a3f0: 2020 2020 2020 656c 7365 0a20 2020 2020        else.     
+0000a400: 207b 0a20 2020 2020 2020 2062 6c6f 636b   {.        block
+0000a410: 6574 7465 5f74 7970 6520 3d20 3230 303b  ette_type = 200;
+0000a420: 0a20 2020 2020 2020 2062 6c6f 636b 6574  .        blocket
+0000a430: 7465 5f6c 656e 6774 6820 3d20 3532 3b0a  te_length = 52;.
+0000a440: 2020 2020 2020 7d0a 0a20 2020 2020 2069        }..      i
+0000a450: 6620 2828 7265 6362 7566 6c65 6e20 2d20  f ((recbuflen - 
+0000a460: 7772 6974 7465 6e29 203c 2062 6c6f 636b  written) < block
+0000a470: 6574 7465 5f6c 656e 6774 6820 290a 2020  ette_length ).  
+0000a480: 2020 2020 7b0a 2020 2020 2020 2020 6d73      {.        ms
+0000a490: 5f6c 6f67 2028 322c 2022 2573 3a20 5265  _log (2, "%s: Re
+0000a4a0: 636f 7264 206c 656e 6774 6820 6e6f 7420  cord length not 
+0000a4b0: 6c61 7267 6520 656e 6f75 6768 2066 6f72  large enough for
+0000a4c0: 2042 2575 5c6e 222c 206d 7372 2d3e 7369   B%u\n", msr->si
+0000a4d0: 642c 2062 6c6f 636b 6574 7465 5f74 7970  d, blockette_typ
+0000a4e0: 6529 3b0a 2020 2020 2020 2020 7979 6a73  e);.        yyjs
+0000a4f0: 6f6e 5f64 6f63 5f66 7265 6520 2865 6864  on_doc_free (ehd
+0000a500: 6f63 293b 0a20 2020 2020 2020 2072 6574  oc);.        ret
+0000a510: 7572 6e20 2d31 3b0a 2020 2020 2020 7d0a  urn -1;.      }.
+0000a520: 0a20 2020 2020 202f 2a20 5468 6520 696e  .      /* The in
+0000a530: 6974 6961 6c20 6669 656c 6473 206f 6620  itial fields of 
+0000a540: 4232 3030 2061 6e64 2042 3230 3120 6172  B200 and B201 ar
+0000a550: 6520 7468 6520 7361 6d65 202a 2f0a 2020  e the same */.  
+0000a560: 2020 2020 2a6e 6578 745f 626c 6f63 6b65      *next_blocke
+0000a570: 7474 6520 3d20 484f 3275 2028 2875 696e  tte = HO2u ((uin
+0000a580: 7431 365f 7429 7772 6974 7465 6e2c 2073  t16_t)written, s
+0000a590: 7761 7066 6c61 6729 3b0a 2020 2020 2020  wapflag);.      
+0000a5a0: 6e65 7874 5f62 6c6f 636b 6574 7465 203d  next_blockette =
+0000a5b0: 2070 4d53 3242 3230 305f 4e45 5854 2028   pMS2B200_NEXT (
+0000a5c0: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000a5d0: 293b 0a20 2020 2020 202a 704d 5332 4653  );.      *pMS2FS
+0000a5e0: 4448 5f4e 554d 424c 4f43 4b45 5454 4553  DH_NUMBLOCKETTES
+0000a5f0: 2028 7265 636f 7264 2920 2b3d 2031 3b0a   (record) += 1;.
+0000a600: 0a20 2020 2020 206d 656d 7365 7420 2872  .      memset (r
+0000a610: 6563 6f72 6420 2b20 7772 6974 7465 6e2c  ecord + written,
+0000a620: 2030 2c20 626c 6f63 6b65 7474 655f 6c65   0, blockette_le
+0000a630: 6e67 7468 293b 0a20 2020 2020 202a 704d  ngth);.      *pM
+0000a640: 5332 4232 3030 5f54 5950 4520 2872 6563  S2B200_TYPE (rec
+0000a650: 6f72 6420 2b20 7772 6974 7465 6e29 203d  ord + written) =
+0000a660: 2048 4f32 7520 2862 6c6f 636b 6574 7465   HO2u (blockette
+0000a670: 5f74 7970 652c 2073 7761 7066 6c61 6729  _type, swapflag)
+0000a680: 3b0a 2020 2020 2020 2a70 4d53 3242 3230  ;.      *pMS2B20
+0000a690: 305f 4e45 5854 2028 7265 636f 7264 202b  0_NEXT (record +
+0000a6a0: 2077 7269 7474 656e 2920 3d20 303b 0a0a   written) = 0;..
+0000a6b0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+0000a6c0: 5f70 7472 5f67 6574 5f6e 756d 2028 6568  _ptr_get_num (eh
+0000a6d0: 6974 6572 7661 6c2c 2022 2f53 6967 6e61  iterval, "/Signa
+0000a6e0: 6c41 6d70 6c69 7475 6465 222c 2026 6865  lAmplitude", &he
+0000a6f0: 6164 6572 5f6e 756d 6265 7229 290a 2020  ader_number)).  
+0000a700: 2020 2020 2020 2a70 4d53 3242 3230 305f        *pMS2B200_
+0000a710: 414d 504c 4954 5544 4520 2872 6563 6f72  AMPLITUDE (recor
+0000a720: 6420 2b20 7772 6974 7465 6e29 203d 2048  d + written) = H
+0000a730: 4f34 6620 2828 666c 6f61 7429 6865 6164  O4f ((float)head
+0000a740: 6572 5f6e 756d 6265 722c 2073 7761 7066  er_number, swapf
+0000a750: 6c61 6729 3b0a 0a20 2020 2020 2069 6620  lag);..      if 
+0000a760: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
+0000a770: 6e75 6d20 2865 6869 7465 7276 616c 2c20  num (ehiterval, 
+0000a780: 222f 5369 676e 616c 5065 7269 6f64 222c  "/SignalPeriod",
+0000a790: 2026 6865 6164 6572 5f6e 756d 6265 7229   &header_number)
+0000a7a0: 290a 2020 2020 2020 2020 2a70 4d53 3242  ).        *pMS2B
+0000a7b0: 3230 305f 5045 5249 4f44 2028 7265 636f  200_PERIOD (reco
+0000a7c0: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
+0000a7d0: 484f 3466 2028 2866 6c6f 6174 2968 6561  HO4f ((float)hea
+0000a7e0: 6465 725f 6e75 6d62 6572 2c20 7377 6170  der_number, swap
+0000a7f0: 666c 6167 293b 0a0a 2020 2020 2020 6966  flag);..      if
+0000a800: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000a810: 5f6e 756d 2028 6568 6974 6572 7661 6c2c  _num (ehiterval,
+0000a820: 2022 2f42 6163 6b67 726f 756e 6445 7374   "/BackgroundEst
+0000a830: 696d 6174 6522 2c20 2668 6561 6465 725f  imate", &header_
+0000a840: 6e75 6d62 6572 2929 0a20 2020 2020 2020  number)).       
+0000a850: 202a 704d 5332 4232 3030 5f42 4143 4b47   *pMS2B200_BACKG
+0000a860: 524f 554e 4445 5354 2028 7265 636f 7264  ROUNDEST (record
+0000a870: 202b 2077 7269 7474 656e 2920 3d20 484f   + written) = HO
+0000a880: 3466 2028 2866 6c6f 6174 2968 6561 6465  4f ((float)heade
+0000a890: 725f 6e75 6d62 6572 2c20 7377 6170 666c  r_number, swapfl
+0000a8a0: 6167 293b 0a0a 2020 2020 2020 2f2a 2044  ag);..      /* D
+0000a8b0: 6574 6572 6d69 6e65 2077 6869 6368 2077  etermine which w
+0000a8c0: 6176 653a 2044 494c 4154 4154 494f 4e20  ave: DILATATION 
+0000a8d0: 7665 7273 7573 2028 6173 7375 6d65 6429  versus (assumed)
+0000a8e0: 2043 4f4d 5052 4553 5349 4f4e 202a 2f0a   COMPRESSION */.
+0000a8f0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+0000a900: 5f70 7472 5f67 6574 5f73 7472 2028 6568  _ptr_get_str (eh
+0000a910: 6974 6572 7661 6c2c 2022 2f57 6176 6522  iterval, "/Wave"
+0000a920: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
+0000a930: 2929 0a20 2020 2020 207b 0a20 2020 2020  )).      {.     
+0000a940: 2020 2069 6620 2873 7472 6e63 6173 6563     if (strncasec
+0000a950: 6d70 2028 6865 6164 6572 5f73 7472 696e  mp (header_strin
+0000a960: 672c 2022 4449 4c41 5441 5449 4f4e 222c  g, "DILATATION",
+0000a970: 2031 3029 203d 3d20 3029 0a20 2020 2020   10) == 0).     
+0000a980: 2020 2020 202a 704d 5332 4232 3030 5f46       *pMS2B200_F
+0000a990: 4c41 4753 2028 7265 636f 7264 202b 2077  LAGS (record + w
+0000a9a0: 7269 7474 656e 2920 7c3d 2030 7830 313b  ritten) |= 0x01;
+0000a9b0: 0a20 2020 2020 207d 0a20 2020 2020 2065  .      }.      e
+0000a9c0: 6c73 6520 6966 2028 626c 6f63 6b65 7474  lse if (blockett
+0000a9d0: 655f 7479 7065 203d 3d20 3230 3029 0a20  e_type == 200). 
+0000a9e0: 2020 2020 207b 0a20 2020 2020 2020 202a       {.        *
+0000a9f0: 704d 5332 4232 3030 5f46 4c41 4753 2028  pMS2B200_FLAGS (
+0000aa00: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000aa10: 2920 7c3d 2030 7830 343b 0a20 2020 2020  ) |= 0x04;.     
+0000aa20: 207d 0a0a 2020 2020 2020 6966 2028 626c   }..      if (bl
+0000aa30: 6f63 6b65 7474 655f 7479 7065 203d 3d20  ockette_type == 
+0000aa40: 3230 3020 2626 0a20 2020 2020 2020 2020  200 &&.         
+0000aa50: 2079 796a 736f 6e5f 7074 725f 6765 745f   yyjson_ptr_get_
+0000aa60: 7374 7220 2865 6869 7465 7276 616c 2c20  str (ehiterval, 
+0000aa70: 222f 556e 6974 7322 2c20 2668 6561 6465  "/Units", &heade
+0000aa80: 725f 7374 7269 6e67 2920 2626 0a20 2020  r_string) &&.   
+0000aa90: 2020 2020 2020 2073 7472 6e63 6173 6563         strncasec
+0000aaa0: 6d70 2028 6865 6164 6572 5f73 7472 696e  mp (header_strin
+0000aab0: 672c 2022 434f 554e 5422 2c20 3529 2021  g, "COUNT", 5) !
+0000aac0: 3d20 3029 0a20 2020 2020 2020 202a 704d  = 0).        *pM
+0000aad0: 5332 4232 3030 5f46 4c41 4753 2028 7265  S2B200_FLAGS (re
+0000aae0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+0000aaf0: 7c3d 2030 7830 323b 0a0a 2020 2020 2020  |= 0x02;..      
+0000ab00: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
+0000ab10: 6574 5f73 7472 2028 6568 6974 6572 7661  et_str (ehiterva
+0000ab20: 6c2c 2022 2f4f 6e73 6574 5469 6d65 222c  l, "/OnsetTime",
+0000ab30: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
+0000ab40: 290a 2020 2020 2020 7b0a 2020 2020 2020  ).      {.      
+0000ab50: 2020 6966 2028 6d73 5f74 696d 6573 7472    if (ms_timestr
+0000ab60: 3262 7469 6d65 2028 6865 6164 6572 5f73  2btime (header_s
+0000ab70: 7472 696e 672c 2028 7569 6e74 385f 7420  tring, (uint8_t 
+0000ab80: 2a29 704d 5332 4232 3030 5f59 4541 5220  *)pMS2B200_YEAR 
+0000ab90: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000aba0: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 6d73 722d 3e73 6964 2c20 7377 6170    msr->sid, swap
+0000abd0: 666c 6167 2920 3d3d 202d 3129 0a20 2020  flag) == -1).   
+0000abe0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+0000abf0: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
+0000ac00: 2043 616e 6e6f 7420 636f 6e76 6572 7420   Cannot convert 
+0000ac10: 4225 7520 7469 6d65 3a20 2573 5c6e 222c  B%u time: %s\n",
+0000ac20: 206d 7372 2d3e 7369 642c 2062 6c6f 636b   msr->sid, block
+0000ac30: 6574 7465 5f74 7970 652c 2068 6561 6465  ette_type, heade
+0000ac40: 725f 7374 7269 6e67 293b 0a20 2020 2020  r_string);.     
+0000ac50: 2020 2020 2079 796a 736f 6e5f 646f 635f       yyjson_doc_
+0000ac60: 6672 6565 2028 6568 646f 6329 3b0a 2020  free (ehdoc);.  
+0000ac70: 2020 2020 2020 2020 7265 7475 726e 202d          return -
+0000ac80: 313b 0a20 2020 2020 2020 207d 0a20 2020  1;.        }.   
+0000ac90: 2020 207d 0a0a 2020 2020 2020 6966 2028     }..      if (
+0000aca0: 626c 6f63 6b65 7474 655f 7479 7065 203d  blockette_type =
+0000acb0: 3d20 3230 3029 0a20 2020 2020 207b 0a20  = 200).      {. 
+0000acc0: 2020 2020 2020 2069 6620 2879 796a 736f         if (yyjso
+0000acd0: 6e5f 7074 725f 6765 745f 7374 7220 2865  n_ptr_get_str (e
+0000ace0: 6869 7465 7276 616c 2c20 222f 4465 7465  hiterval, "/Dete
+0000acf0: 6374 6f72 222c 2026 6865 6164 6572 5f73  ctor", &header_s
+0000ad00: 7472 696e 6729 290a 2020 2020 2020 2020  tring)).        
+0000ad10: 2020 6d73 5f73 7472 6e63 706f 7065 6e20    ms_strncpopen 
+0000ad20: 2870 4d53 3242 3230 305f 4445 5445 4354  (pMS2B200_DETECT
+0000ad30: 4f52 2028 7265 636f 7264 202b 2077 7269  OR (record + wri
+0000ad40: 7474 656e 292c 2068 6561 6465 725f 7374  tten), header_st
+0000ad50: 7269 6e67 2c20 3234 293b 0a20 2020 2020  ring, 24);.     
+0000ad60: 207d 0a20 2020 2020 2065 6c73 6520 2f2a   }.      else /*
+0000ad70: 2042 6c6f 636b 6574 7465 2032 3031 202a   Blockette 201 *
+0000ad80: 2f0a 2020 2020 2020 7b0a 2020 2020 2020  /.      {.      
+0000ad90: 2020 7979 6a73 6f6e 5f76 616c 202a 6568    yyjson_val *eh
+0000ada0: 7375 6261 7272 3b0a 2020 2020 2020 2020  subarr;.        
+0000adb0: 7979 6a73 6f6e 5f61 7272 5f69 7465 7220  yyjson_arr_iter 
+0000adc0: 6568 7375 6269 7465 723b 0a20 2020 2020  ehsubiter;.     
+0000add0: 2020 2079 796a 736f 6e5f 7661 6c20 2a65     yyjson_val *e
+0000ade0: 6873 7562 6974 6572 7661 6c3b 0a20 2020  hsubiterval;.   
+0000adf0: 2020 2020 2069 6e74 2069 6478 203d 2030       int idx = 0
+0000ae00: 3b0a 0a20 2020 2020 2020 2069 6620 2828  ;..        if ((
+0000ae10: 6568 7375 6261 7272 203d 2079 796a 736f  ehsubarr = yyjso
+0000ae20: 6e5f 7074 725f 6765 7420 2865 6869 7465  n_ptr_get (ehite
+0000ae30: 7276 616c 2c20 222f 4d45 4453 4e52 2229  rval, "/MEDSNR")
+0000ae40: 2920 2626 2079 796a 736f 6e5f 6973 5f61  ) && yyjson_is_a
+0000ae50: 7272 2028 6568 7375 6261 7272 2929 0a20  rr (ehsubarr)). 
+0000ae60: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000ae70: 2020 2079 796a 736f 6e5f 6172 725f 6974     yyjson_arr_it
+0000ae80: 6572 5f69 6e69 7420 2865 6873 7562 6172  er_init (ehsubar
+0000ae90: 722c 2026 6568 7375 6269 7465 7229 3b0a  r, &ehsubiter);.
+0000aea0: 0a20 2020 2020 2020 2020 2077 6869 6c65  .          while
+0000aeb0: 2028 2865 6873 7562 6974 6572 7661 6c20   ((ehsubiterval 
+0000aec0: 3d20 7979 6a73 6f6e 5f61 7272 5f69 7465  = yyjson_arr_ite
+0000aed0: 725f 6e65 7874 2028 2665 6873 7562 6974  r_next (&ehsubit
+0000aee0: 6572 2929 290a 2020 2020 2020 2020 2020  er))).          
+0000aef0: 7b0a 2020 2020 2020 2020 2020 2020 6966  {.            if
+0000af00: 2028 2179 796a 736f 6e5f 6973 5f6e 756d   (!yyjson_is_num
+0000af10: 2028 6568 7375 6269 7465 7276 616c 2929   (ehsubiterval))
+0000af20: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
+0000af30: 6f6e 7469 6e75 653b 0a0a 2020 2020 2020  ontinue;..      
+0000af40: 2020 2020 2020 704d 5332 4232 3031 5f4d        pMS2B201_M
+0000af50: 4544 534e 5220 2872 6563 6f72 6420 2b20  EDSNR (record + 
+0000af60: 7772 6974 7465 6e29 5b69 6478 2b2b 5d20  written)[idx++] 
+0000af70: 3d20 2875 696e 7438 5f74 2979 796a 736f  = (uint8_t)yyjso
+0000af80: 6e5f 6765 745f 6e75 6d20 2865 6873 7562  n_get_num (ehsub
+0000af90: 6974 6572 7661 6c29 3b0a 2020 2020 2020  iterval);.      
+0000afa0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+0000afb0: 0a20 2020 2020 2020 2069 6620 2879 796a  .        if (yyj
+0000afc0: 736f 6e5f 7074 725f 6765 745f 7569 6e74  son_ptr_get_uint
+0000afd0: 2028 6568 6974 6572 7661 6c2c 2022 2f4d   (ehiterval, "/M
+0000afe0: 4544 4c6f 6f6b 6261 636b 222c 2026 6865  EDLookback", &he
+0000aff0: 6164 6572 5f75 696e 7429 2026 2620 6865  ader_uint) && he
+0000b000: 6164 6572 5f75 696e 7420 3c20 5549 4e54  ader_uint < UINT
+0000b010: 385f 4d41 5829 0a20 2020 2020 2020 2020  8_MAX).         
+0000b020: 202a 704d 5332 4232 3031 5f4c 4f4f 5042   *pMS2B201_LOOPB
+0000b030: 4143 4b20 2872 6563 6f72 6420 2b20 7772  ACK (record + wr
+0000b040: 6974 7465 6e29 203d 2028 7569 6e74 385f  itten) = (uint8_
+0000b050: 7429 6865 6164 6572 5f75 696e 743b 0a0a  t)header_uint;..
+0000b060: 2020 2020 2020 2020 6966 2028 7979 6a73          if (yyjs
+0000b070: 6f6e 5f70 7472 5f67 6574 5f75 696e 7420  on_ptr_get_uint 
+0000b080: 2865 6869 7465 7276 616c 2c20 222f 4d45  (ehiterval, "/ME
+0000b090: 4450 6963 6b41 6c67 6f72 6974 686d 222c  DPickAlgorithm",
+0000b0a0: 2026 6865 6164 6572 5f75 696e 7429 2026   &header_uint) &
+0000b0b0: 2620 6865 6164 6572 5f75 696e 7420 3c20  & header_uint < 
+0000b0c0: 5549 4e54 385f 4d41 5829 0a20 2020 2020  UINT8_MAX).     
+0000b0d0: 2020 2020 202a 704d 5332 4232 3031 5f50       *pMS2B201_P
+0000b0e0: 4943 4b41 4c47 4f52 4954 484d 2028 7265  ICKALGORITHM (re
+0000b0f0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+0000b100: 3d20 2875 696e 7438 5f74 2968 6561 6465  = (uint8_t)heade
+0000b110: 725f 7569 6e74 3b0a 0a20 2020 2020 2020  r_uint;..       
+0000b120: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
+0000b130: 6765 745f 7374 7220 2865 6869 7465 7276  get_str (ehiterv
+0000b140: 616c 2c20 222f 4465 7465 6374 6f72 222c  al, "/Detector",
+0000b150: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
+0000b160: 290a 2020 2020 2020 2020 2020 6d73 5f73  ).          ms_s
+0000b170: 7472 6e63 706f 7065 6e20 2870 4d53 3242  trncpopen (pMS2B
+0000b180: 3230 315f 4445 5445 4354 4f52 2028 7265  201_DETECTOR (re
+0000b190: 636f 7264 202b 2077 7269 7474 656e 292c  cord + written),
+0000b1a0: 2068 6561 6465 725f 7374 7269 6e67 2c20   header_string, 
+0000b1b0: 3234 293b 0a20 2020 2020 207d 0a0a 2020  24);.      }..  
+0000b1c0: 2020 2020 7772 6974 7465 6e20 2b3d 2062      written += b
+0000b1d0: 6c6f 636b 6574 7465 5f6c 656e 6774 683b  lockette_length;
+0000b1e0: 0a20 2020 207d 0a20 207d 202f 2a20 456e  .    }.  } /* En
+0000b1f0: 6420 6966 202f 4644 534e 2f45 7665 6e74  d if /FDSN/Event
+0000b200: 2f44 6574 6563 7469 6f6e 202a 2f0a 0a20  /Detection */.. 
+0000b210: 202f 2a20 4164 6420 426c 6f63 6b65 7474   /* Add Blockett
+0000b220: 6520 4233 3030 2c20 3331 302c 2033 3230  e B300, 310, 320
+0000b230: 2c20 3339 302c 2033 3935 2066 6f72 2063  , 390, 395 for c
+0000b240: 616c 6962 7261 7469 6f6e 7320 2a2f 0a0a  alibrations */..
+0000b250: 2020 6966 2028 2865 6861 7272 203d 2079    if ((eharr = y
+0000b260: 796a 736f 6e5f 7074 725f 6765 7420 2865  yjson_ptr_get (e
+0000b270: 6872 6f6f 742c 2022 2f46 4453 4e2f 4361  hroot, "/FDSN/Ca
+0000b280: 6c69 6272 6174 696f 6e2f 5365 7175 656e  libration/Sequen
+0000b290: 6365 2229 2920 2626 2079 796a 736f 6e5f  ce")) && yyjson_
+0000b2a0: 6973 5f61 7272 2028 6568 6172 7229 290a  is_arr (eharr)).
+0000b2b0: 2020 7b0a 2020 2020 7979 6a73 6f6e 5f61    {.    yyjson_a
+0000b2c0: 7272 5f69 7465 725f 696e 6974 2028 6568  rr_iter_init (eh
+0000b2d0: 6172 722c 2026 6568 6974 6572 293b 0a0a  arr, &ehiter);..
+0000b2e0: 2020 2020 7768 696c 6520 2828 6568 6974      while ((ehit
+0000b2f0: 6572 7661 6c20 3d20 7979 6a73 6f6e 5f61  erval = yyjson_a
+0000b300: 7272 5f69 7465 725f 6e65 7874 2028 2665  rr_iter_next (&e
+0000b310: 6869 7465 7229 2929 0a20 2020 207b 0a20  hiter))).    {. 
+0000b320: 2020 2020 2069 6620 2821 7979 6a73 6f6e       if (!yyjson
+0000b330: 5f69 735f 6f62 6a20 2865 6869 7465 7276  _is_obj (ehiterv
+0000b340: 616c 2929 0a20 2020 2020 2020 2063 6f6e  al)).        con
+0000b350: 7469 6e75 653b 0a0a 2020 2020 2020 2f2a  tinue;..      /*
+0000b360: 2044 6574 6572 6d69 6e65 2077 6869 6368   Determine which
+0000b370: 2063 616c 6962 7261 7469 6f6e 2074 7970   calibration typ
+0000b380: 653a 2053 5445 502c 2053 494e 452c 2050  e: STEP, SINE, P
+0000b390: 5345 5544 4f52 414e 444f 4d2c 2047 454e  SEUDORANDOM, GEN
+0000b3a0: 4552 4943 202a 2f0a 2020 2020 2020 626c  ERIC */.      bl
+0000b3b0: 6f63 6b65 7474 655f 7479 7065 2020 203d  ockette_type   =
+0000b3c0: 2030 3b0a 2020 2020 2020 626c 6f63 6b65   0;.      blocke
+0000b3d0: 7474 655f 6c65 6e67 7468 203d 2030 3b0a  tte_length = 0;.
+0000b3e0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+0000b3f0: 5f70 7472 5f67 6574 5f73 7472 2028 6568  _ptr_get_str (eh
+0000b400: 6974 6572 7661 6c2c 2022 2f54 7970 6522  iterval, "/Type"
+0000b410: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
+0000b420: 2929 0a20 2020 2020 207b 0a20 2020 2020  )).      {.     
+0000b430: 2020 2069 6620 2873 7472 6e63 6173 6563     if (strncasec
+0000b440: 6d70 2028 6865 6164 6572 5f73 7472 696e  mp (header_strin
+0000b450: 672c 2022 5354 4550 222c 2034 2920 3d3d  g, "STEP", 4) ==
+0000b460: 2030 290a 2020 2020 2020 2020 7b0a 2020   0).        {.  
+0000b470: 2020 2020 2020 2020 626c 6f63 6b65 7474          blockett
+0000b480: 655f 7479 7065 2020 203d 2033 3030 3b0a  e_type   = 300;.
+0000b490: 2020 2020 2020 2020 2020 626c 6f63 6b65            blocke
+0000b4a0: 7474 655f 6c65 6e67 7468 203d 2036 303b  tte_length = 60;
+0000b4b0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0000b4c0: 2020 2065 6c73 6520 6966 2028 7374 726e     else if (strn
+0000b4d0: 6361 7365 636d 7020 2868 6561 6465 725f  casecmp (header_
+0000b4e0: 7374 7269 6e67 2c20 2253 494e 4522 2c20  string, "SINE", 
+0000b4f0: 3429 203d 3d20 3029 0a20 2020 2020 2020  4) == 0).       
+0000b500: 207b 0a20 2020 2020 2020 2020 2062 6c6f   {.          blo
+0000b510: 636b 6574 7465 5f74 7970 6520 2020 3d20  ckette_type   = 
+0000b520: 3331 303b 0a20 2020 2020 2020 2020 2062  310;.          b
+0000b530: 6c6f 636b 6574 7465 5f6c 656e 6774 6820  lockette_length 
+0000b540: 3d20 3630 3b0a 2020 2020 2020 2020 7d0a  = 60;.        }.
+0000b550: 2020 2020 2020 2020 656c 7365 2069 6620          else if 
+0000b560: 2873 7472 6e63 6173 6563 6d70 2028 6865  (strncasecmp (he
+0000b570: 6164 6572 5f73 7472 696e 672c 2022 5053  ader_string, "PS
+0000b580: 4555 444f 5241 4e44 4f4d 222c 2031 3229  EUDORANDOM", 12)
+0000b590: 203d 3d20 3029 0a20 2020 2020 2020 207b   == 0).        {
+0000b5a0: 0a20 2020 2020 2020 2020 2062 6c6f 636b  .          block
+0000b5b0: 6574 7465 5f74 7970 6520 2020 3d20 3332  ette_type   = 32
+0000b5c0: 303b 0a20 2020 2020 2020 2020 2062 6c6f  0;.          blo
+0000b5d0: 636b 6574 7465 5f6c 656e 6774 6820 3d20  ckette_length = 
+0000b5e0: 3634 3b0a 2020 2020 2020 2020 7d0a 2020  64;.        }.  
+0000b5f0: 2020 2020 2020 656c 7365 2069 6620 2873        else if (s
+0000b600: 7472 6e63 6173 6563 6d70 2028 6865 6164  trncasecmp (head
+0000b610: 6572 5f73 7472 696e 672c 2022 4745 4e45  er_string, "GENE
+0000b620: 5249 4322 2c20 3729 203d 3d20 3029 0a20  RIC", 7) == 0). 
+0000b630: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000b640: 2020 2062 6c6f 636b 6574 7465 5f74 7970     blockette_typ
+0000b650: 6520 2020 3d20 3339 303b 0a20 2020 2020  e   = 390;.     
+0000b660: 2020 2020 2062 6c6f 636b 6574 7465 5f6c       blockette_l
+0000b670: 656e 6774 6820 3d20 3238 3b0a 2020 2020  ength = 28;.    
+0000b680: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
+0000b690: 2020 2020 656c 7365 2069 6620 2879 796a      else if (yyj
+0000b6a0: 736f 6e5f 7074 725f 6765 7420 2865 6869  son_ptr_get (ehi
+0000b6b0: 7465 7276 616c 2c20 222f 456e 6454 696d  terval, "/EndTim
+0000b6c0: 6522 2929 0a20 2020 2020 207b 0a20 2020  e")).      {.   
+0000b6d0: 2020 2020 2062 6c6f 636b 6574 7465 5f74       blockette_t
+0000b6e0: 7970 6520 3d20 3339 353b 0a20 2020 2020  ype = 395;.     
+0000b6f0: 2020 2062 6c6f 636b 6574 7465 5f6c 656e     blockette_len
+0000b700: 6774 6820 3d20 3136 3b0a 2020 2020 2020  gth = 16;.      
+0000b710: 7d0a 0a20 2020 2020 2069 6620 2821 626c  }..      if (!bl
+0000b720: 6f63 6b65 7474 655f 7479 7065 207c 7c20  ockette_type || 
+0000b730: 2162 6c6f 636b 6574 7465 5f6c 656e 6774  !blockette_lengt
+0000b740: 6829 0a20 2020 2020 207b 0a20 2020 2020  h).      {.     
+0000b750: 2020 206d 735f 6c6f 6720 2832 2c20 2225     ms_log (2, "%
+0000b760: 733a 2055 6e6b 6e6f 776e 206f 7220 756e  s: Unknown or un
+0000b770: 7365 7420 2f46 4453 4e2f 4361 6c69 6272  set /FDSN/Calibr
+0000b780: 6174 696f 6e2f 5365 7175 656e 6365 2f54  ation/Sequence/T
+0000b790: 7970 6520 6f72 202f 456e 6454 696d 655c  ype or /EndTime\
+0000b7a0: 6e22 2c20 6d73 722d 3e73 6964 293b 0a20  n", msr->sid);. 
+0000b7b0: 2020 2020 2020 2079 796a 736f 6e5f 646f         yyjson_do
+0000b7c0: 635f 6672 6565 2028 6568 646f 6329 3b0a  c_free (ehdoc);.
+0000b7d0: 2020 2020 2020 2020 7265 7475 726e 202d          return -
+0000b7e0: 313b 0a20 2020 2020 207d 0a0a 2020 2020  1;.      }..    
+0000b7f0: 2020 6966 2028 2872 6563 6275 666c 656e    if ((recbuflen
+0000b800: 202d 2077 7269 7474 656e 2920 3c20 626c   - written) < bl
+0000b810: 6f63 6b65 7474 655f 6c65 6e67 7468 2029  ockette_length )
+0000b820: 0a20 2020 2020 207b 0a20 2020 2020 2020  .      {.       
+0000b830: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
+0000b840: 2052 6563 6f72 6420 6c65 6e67 7468 206e   Record length n
+0000b850: 6f74 206c 6172 6765 2065 6e6f 7567 6820  ot large enough 
+0000b860: 666f 7220 4225 755c 6e22 2c20 6d73 722d  for B%u\n", msr-
+0000b870: 3e73 6964 2c20 626c 6f63 6b65 7474 655f  >sid, blockette_
+0000b880: 7479 7065 293b 0a20 2020 2020 2020 2079  type);.        y
+0000b890: 796a 736f 6e5f 646f 635f 6672 6565 2028  yjson_doc_free (
+0000b8a0: 6568 646f 6329 3b0a 2020 2020 2020 2020  ehdoc);.        
+0000b8b0: 7265 7475 726e 202d 313b 0a20 2020 2020  return -1;.     
+0000b8c0: 207d 0a0a 2020 2020 2020 6966 2028 626c   }..      if (bl
+0000b8d0: 6f63 6b65 7474 655f 7479 7065 203d 3d20  ockette_type == 
+0000b8e0: 3330 3020 7c7c 2062 6c6f 636b 6574 7465  300 || blockette
+0000b8f0: 5f74 7970 6520 3d3d 2033 3130 207c 7c0a  _type == 310 ||.
+0000b900: 2020 2020 2020 2020 2020 626c 6f63 6b65            blocke
+0000b910: 7474 655f 7479 7065 203d 3d20 3332 3020  tte_type == 320 
+0000b920: 7c7c 2062 6c6f 636b 6574 7465 5f74 7970  || blockette_typ
+0000b930: 6520 3d3d 2033 3930 290a 2020 2020 2020  e == 390).      
+0000b940: 7b0a 2020 2020 2020 2020 2f2a 2054 6865  {.        /* The
+0000b950: 2069 6e69 7469 616c 2066 6965 6c64 7320   initial fields 
+0000b960: 6f66 2042 3330 302c 2033 3130 2c20 3332  of B300, 310, 32
+0000b970: 302c 2033 3930 2061 7265 2074 6865 2073  0, 390 are the s
+0000b980: 616d 6520 2a2f 0a20 2020 2020 2020 202a  ame */.        *
+0000b990: 6e65 7874 5f62 6c6f 636b 6574 7465 203d  next_blockette =
+0000b9a0: 2048 4f32 7520 2828 7569 6e74 3136 5f74   HO2u ((uint16_t
+0000b9b0: 2977 7269 7474 656e 2c20 7377 6170 666c  )written, swapfl
+0000b9c0: 6167 293b 0a20 2020 2020 2020 206e 6578  ag);.        nex
+0000b9d0: 745f 626c 6f63 6b65 7474 6520 203d 2070  t_blockette  = p
+0000b9e0: 4d53 3242 3330 305f 4e45 5854 2028 7265  MS2B300_NEXT (re
+0000b9f0: 636f 7264 202b 2077 7269 7474 656e 293b  cord + written);
+0000ba00: 0a20 2020 2020 2020 202a 704d 5332 4653  .        *pMS2FS
+0000ba10: 4448 5f4e 554d 424c 4f43 4b45 5454 4553  DH_NUMBLOCKETTES
+0000ba20: 2028 7265 636f 7264 2920 2b3d 2031 3b0a   (record) += 1;.
+0000ba30: 0a20 2020 2020 2020 206d 656d 7365 7420  .        memset 
+0000ba40: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000ba50: 6e2c 2030 2c20 626c 6f63 6b65 7474 655f  n, 0, blockette_
+0000ba60: 6c65 6e67 7468 293b 0a20 2020 2020 2020  length);.       
+0000ba70: 202a 704d 5332 4233 3030 5f54 5950 4520   *pMS2B300_TYPE 
+0000ba80: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000ba90: 6e29 203d 2048 4f32 7520 2862 6c6f 636b  n) = HO2u (block
+0000baa0: 6574 7465 5f74 7970 652c 2073 7761 7066  ette_type, swapf
+0000bab0: 6c61 6729 3b0a 2020 2020 2020 2020 2a70  lag);.        *p
+0000bac0: 4d53 3242 3330 305f 4e45 5854 2028 7265  MS2B300_NEXT (re
+0000bad0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+0000bae0: 3d20 303b 0a0a 2020 2020 2020 2020 6966  = 0;..        if
+0000baf0: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000bb00: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
+0000bb10: 2022 2f42 6567 696e 5469 6d65 222c 2026   "/BeginTime", &
+0000bb20: 6865 6164 6572 5f73 7472 696e 6729 290a  header_string)).
+0000bb30: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+0000bb40: 2020 2020 6966 2028 6d73 5f74 696d 6573      if (ms_times
+0000bb50: 7472 3262 7469 6d65 2028 6865 6164 6572  tr2btime (header
+0000bb60: 5f73 7472 696e 672c 2028 7569 6e74 385f  _string, (uint8_
+0000bb70: 7420 2a29 704d 5332 4233 3030 5f59 4541  t *)pMS2B300_YEA
+0000bb80: 5220 2872 6563 6f72 6420 2b20 7772 6974  R (record + writ
+0000bb90: 7465 6e29 2c0a 2020 2020 2020 2020 2020  ten),.          
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 2020 6d73 722d 3e73 6964 2c20        msr->sid, 
+0000bbc0: 7377 6170 666c 6167 2920 3d3d 202d 3129  swapflag) == -1)
+0000bbd0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
+0000bbe0: 2020 2020 2020 2020 206d 735f 6c6f 6720           ms_log 
+0000bbf0: 2832 2c20 2225 733a 2043 616e 6e6f 7420  (2, "%s: Cannot 
+0000bc00: 636f 6e76 6572 7420 4225 7520 7469 6d65  convert B%u time
+0000bc10: 3a20 2573 5c6e 222c 206d 7372 2d3e 7369  : %s\n", msr->si
+0000bc20: 642c 2062 6c6f 636b 6574 7465 5f74 7970  d, blockette_typ
+0000bc30: 652c 2068 6561 6465 725f 7374 7269 6e67  e, header_string
+0000bc40: 293b 0a20 2020 2020 2020 2020 2020 2079  );.            y
+0000bc50: 796a 736f 6e5f 646f 635f 6672 6565 2028  yjson_doc_free (
+0000bc60: 6568 646f 6329 3b0a 2020 2020 2020 2020  ehdoc);.        
+0000bc70: 2020 2020 7265 7475 726e 202d 313b 0a20      return -1;. 
+0000bc80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+0000bc90: 2020 207d 0a0a 2020 2020 2020 2020 6966     }..        if
+0000bca0: 2028 626c 6f63 6b65 7474 655f 7479 7065   (blockette_type
+0000bcb0: 203d 3d20 3330 3029 0a20 2020 2020 2020   == 300).       
+0000bcc0: 207b 0a20 2020 2020 2020 2020 2069 6620   {.          if 
+0000bcd0: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
+0000bce0: 7569 6e74 2028 6568 6974 6572 7661 6c2c  uint (ehiterval,
+0000bcf0: 2022 2f53 7465 7073 222c 2026 6865 6164   "/Steps", &head
+0000bd00: 6572 5f75 696e 7429 2026 2620 6865 6164  er_uint) && head
+0000bd10: 6572 5f75 696e 7420 3c3d 2055 494e 5438  er_uint <= UINT8
+0000bd20: 5f4d 4158 290a 2020 2020 2020 2020 2020  _MAX).          
+0000bd30: 2020 2a70 4d53 3242 3330 305f 4e55 4d43    *pMS2B300_NUMC
+0000bd40: 414c 4942 5241 5449 4f4e 5320 2872 6563  ALIBRATIONS (rec
+0000bd50: 6f72 6420 2b20 7772 6974 7465 6e29 203d  ord + written) =
+0000bd60: 2028 7569 6e74 385f 7429 6865 6164 6572   (uint8_t)header
+0000bd70: 5f75 696e 743b 0a0a 2020 2020 2020 2020  _uint;..        
+0000bd80: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+0000bd90: 5f67 6574 5f62 6f6f 6c20 2865 6869 7465  _get_bool (ehite
+0000bda0: 7276 616c 2c20 222f 5374 6570 4669 7273  rval, "/StepFirs
+0000bdb0: 7450 756c 7365 506f 7369 7469 7665 222c  tPulsePositive",
+0000bdc0: 2026 6865 6164 6572 5f62 6f6f 6c65 616e   &header_boolean
+0000bdd0: 2920 2626 2068 6561 6465 725f 626f 6f6c  ) && header_bool
+0000bde0: 6561 6e29 0a20 2020 2020 2020 2020 2020  ean).           
+0000bdf0: 202a 704d 5332 4233 3030 5f46 4c41 4753   *pMS2B300_FLAGS
+0000be00: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
+0000be10: 656e 2920 7c3d 2030 7830 313b 0a0a 2020  en) |= 0x01;..  
+0000be20: 2020 2020 2020 2020 6966 2028 7979 6a73          if (yyjs
+0000be30: 6f6e 5f70 7472 5f67 6574 5f62 6f6f 6c20  on_ptr_get_bool 
+0000be40: 2865 6869 7465 7276 616c 2c20 222f 5374  (ehiterval, "/St
+0000be50: 6570 416c 7465 726e 6174 6553 6967 6e22  epAlternateSign"
+0000be60: 2c20 2668 6561 6465 725f 626f 6f6c 6561  , &header_boolea
+0000be70: 6e29 2026 2620 6865 6164 6572 5f62 6f6f  n) && header_boo
+0000be80: 6c65 616e 290a 2020 2020 2020 2020 2020  lean).          
+0000be90: 2020 2a70 4d53 3242 3330 305f 464c 4147    *pMS2B300_FLAG
+0000bea0: 5320 2872 6563 6f72 6420 2b20 7772 6974  S (record + writ
+0000beb0: 7465 6e29 207c 3d20 3078 3032 3b0a 0a20  ten) |= 0x02;.. 
+0000bec0: 2020 2020 2020 2020 2069 6620 2879 796a           if (yyj
+0000bed0: 736f 6e5f 7074 725f 6765 745f 7374 7220  son_ptr_get_str 
+0000bee0: 2865 6869 7465 7276 616c 2c20 222f 5472  (ehiterval, "/Tr
+0000bef0: 6967 6765 7222 2c20 2668 6561 6465 725f  igger", &header_
+0000bf00: 7374 7269 6e67 2920 2626 0a20 2020 2020  string) &&.     
+0000bf10: 2020 2020 2020 2020 2073 7472 6e63 6173           strncas
+0000bf20: 6563 6d70 2028 6865 6164 6572 5f73 7472  ecmp (header_str
+0000bf30: 696e 672c 2022 4155 544f 4d41 5449 4322  ing, "AUTOMATIC"
+0000bf40: 2c20 3929 203d 3d20 3029 0a20 2020 2020  , 9) == 0).     
+0000bf50: 2020 2020 2020 202a 704d 5332 4233 3030         *pMS2B300
+0000bf60: 5f46 4c41 4753 2028 7265 636f 7264 202b  _FLAGS (record +
+0000bf70: 2077 7269 7474 656e 2920 7c3d 2030 7830   written) |= 0x0
+0000bf80: 343b 0a0a 2020 2020 2020 2020 2020 6966  4;..          if
+0000bf90: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000bfa0: 5f62 6f6f 6c20 2865 6869 7465 7276 616c  _bool (ehiterval
+0000bfb0: 2c20 222f 436f 6e74 696e 7565 6422 2c20  , "/Continued", 
+0000bfc0: 2668 6561 6465 725f 626f 6f6c 6561 6e29  &header_boolean)
+0000bfd0: 2026 2620 6865 6164 6572 5f62 6f6f 6c65   && header_boole
+0000bfe0: 616e 290a 2020 2020 2020 2020 2020 2020  an).            
+0000bff0: 2a70 4d53 3242 3330 305f 464c 4147 5320  *pMS2B300_FLAGS 
+0000c000: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000c010: 6e29 207c 3d20 3078 3038 3b0a 0a20 2020  n) |= 0x08;..   
+0000c020: 2020 2020 2020 2069 6620 2879 796a 736f         if (yyjso
+0000c030: 6e5f 7074 725f 6765 745f 6e75 6d20 2865  n_ptr_get_num (e
+0000c040: 6869 7465 7276 616c 2c20 222f 4475 7261  hiterval, "/Dura
+0000c050: 7469 6f6e 222c 2026 6865 6164 6572 5f6e  tion", &header_n
+0000c060: 756d 6265 7229 290a 2020 2020 2020 2020  umber)).        
+0000c070: 2020 2020 2a70 4d53 3242 3330 305f 5354      *pMS2B300_ST
+0000c080: 4550 4455 5241 5449 4f4e 2028 7265 636f  EPDURATION (reco
+0000c090: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
+0000c0a0: 484f 3475 2028 2875 696e 7433 325f 7429  HO4u ((uint32_t)
+0000c0b0: 2868 6561 6465 725f 6e75 6d62 6572 202a  (header_number *
+0000c0c0: 2031 3030 3030 202b 2030 2e35 292c 2073   10000 + 0.5), s
+0000c0d0: 7761 7066 6c61 6729 3b0a 0a20 2020 2020  wapflag);..     
+0000c0e0: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
+0000c0f0: 7074 725f 6765 745f 6e75 6d20 2865 6869  ptr_get_num (ehi
+0000c100: 7465 7276 616c 2c20 222f 5374 6570 4265  terval, "/StepBe
+0000c110: 7477 6565 6e22 2c20 2668 6561 6465 725f  tween", &header_
+0000c120: 6e75 6d62 6572 2929 0a20 2020 2020 2020  number)).       
+0000c130: 2020 2020 202a 704d 5332 4233 3030 5f49       *pMS2B300_I
+0000c140: 4e54 4552 5641 4c44 5552 4154 494f 4e20  NTERVALDURATION 
+0000c150: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000c160: 6e29 203d 2048 4f34 7520 2828 7569 6e74  n) = HO4u ((uint
+0000c170: 3332 5f74 2928 6865 6164 6572 5f6e 756d  32_t)(header_num
+0000c180: 6265 7220 2a20 3130 3030 3020 2b20 302e  ber * 10000 + 0.
+0000c190: 3529 2c20 7377 6170 666c 6167 293b 0a0a  5), swapflag);..
+0000c1a0: 2020 2020 2020 2020 2020 6966 2028 7979            if (yy
+0000c1b0: 6a73 6f6e 5f70 7472 5f67 6574 5f6e 756d  json_ptr_get_num
+0000c1c0: 2028 6568 6974 6572 7661 6c2c 2022 2f41   (ehiterval, "/A
+0000c1d0: 6d70 6c69 7475 6465 222c 2026 6865 6164  mplitude", &head
+0000c1e0: 6572 5f6e 756d 6265 7229 290a 2020 2020  er_number)).    
+0000c1f0: 2020 2020 2020 2020 2a70 4d53 3242 3330          *pMS2B30
+0000c200: 305f 414d 504c 4954 5544 4520 2872 6563  0_AMPLITUDE (rec
+0000c210: 6f72 6420 2b20 7772 6974 7465 6e29 203d  ord + written) =
+0000c220: 2048 4f34 6620 2828 666c 6f61 7429 6865   HO4f ((float)he
+0000c230: 6164 6572 5f6e 756d 6265 722c 2073 7761  ader_number, swa
+0000c240: 7066 6c61 6729 3b0a 0a20 2020 2020 2020  pflag);..       
+0000c250: 2020 2069 6620 2879 796a 736f 6e5f 7074     if (yyjson_pt
+0000c260: 725f 6765 745f 7374 7220 2865 6869 7465  r_get_str (ehite
+0000c270: 7276 616c 2c20 222f 496e 7075 7443 6861  rval, "/InputCha
+0000c280: 6e6e 656c 222c 2026 6865 6164 6572 5f73  nnel", &header_s
+0000c290: 7472 696e 6729 290a 2020 2020 2020 2020  tring)).        
+0000c2a0: 2020 2020 6d73 5f73 7472 6e63 706f 7065      ms_strncpope
+0000c2b0: 6e20 2870 4d53 3242 3330 305f 494e 5055  n (pMS2B300_INPU
+0000c2c0: 5443 4841 4e4e 454c 2028 7265 636f 7264  TCHANNEL (record
+0000c2d0: 202b 2077 7269 7474 656e 292c 2068 6561   + written), hea
+0000c2e0: 6465 725f 7374 7269 6e67 2c20 3329 3b0a  der_string, 3);.
+0000c2f0: 0a20 2020 2020 2020 2020 2069 6620 2879  .          if (y
+0000c300: 796a 736f 6e5f 7074 725f 6765 745f 6e75  yjson_ptr_get_nu
+0000c310: 6d20 2865 6869 7465 7276 616c 2c20 222f  m (ehiterval, "/
+0000c320: 5265 6665 7265 6e63 6541 6d70 6c69 7475  ReferenceAmplitu
+0000c330: 6465 222c 2026 6865 6164 6572 5f6e 756d  de", &header_num
+0000c340: 6265 7229 290a 2020 2020 2020 2020 2020  ber)).          
+0000c350: 2020 2a70 4d53 3242 3330 305f 5245 4645    *pMS2B300_REFE
+0000c360: 5245 4e43 4541 4d50 4c49 5455 4445 2028  RENCEAMPLITUDE (
+0000c370: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000c380: 2920 3d20 484f 3475 2028 2875 696e 7433  ) = HO4u ((uint3
+0000c390: 325f 7429 2868 6561 6465 725f 6e75 6d62  2_t)(header_numb
+0000c3a0: 6572 202b 2030 2e35 292c 2073 7761 7066  er + 0.5), swapf
+0000c3b0: 6c61 6729 3b0a 0a20 2020 2020 2020 2020  lag);..         
+0000c3c0: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
+0000c3d0: 6765 745f 7374 7220 2865 6869 7465 7276  get_str (ehiterv
+0000c3e0: 616c 2c20 222f 436f 7570 6c69 6e67 222c  al, "/Coupling",
+0000c3f0: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
+0000c400: 290a 2020 2020 2020 2020 2020 2020 6d73  ).            ms
+0000c410: 5f73 7472 6e63 706f 7065 6e20 2870 4d53  _strncpopen (pMS
+0000c420: 3242 3330 305f 434f 5550 4c49 4e47 2028  2B300_COUPLING (
+0000c430: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000c440: 292c 2068 6561 6465 725f 7374 7269 6e67  ), header_string
+0000c450: 2c20 3132 293b 0a0a 2020 2020 2020 2020  , 12);..        
+0000c460: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+0000c470: 5f67 6574 5f73 7472 2028 6568 6974 6572  _get_str (ehiter
+0000c480: 7661 6c2c 2022 2f52 6f6c 6c6f 6666 222c  val, "/Rolloff",
+0000c490: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
+0000c4a0: 290a 2020 2020 2020 2020 2020 2020 6d73  ).            ms
+0000c4b0: 5f73 7472 6e63 706f 7065 6e20 2870 4d53  _strncpopen (pMS
+0000c4c0: 3242 3330 305f 524f 4c4c 4f46 4620 2872  2B300_ROLLOFF (r
+0000c4d0: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
+0000c4e0: 2c20 6865 6164 6572 5f73 7472 696e 672c  , header_string,
+0000c4f0: 2031 3229 3b0a 2020 2020 2020 2020 7d0a   12);.        }.
+0000c500: 2020 2020 2020 2020 656c 7365 2069 6620          else if 
+0000c510: 2862 6c6f 636b 6574 7465 5f74 7970 6520  (blockette_type 
+0000c520: 3d3d 2033 3130 290a 2020 2020 2020 2020  == 310).        
+0000c530: 7b0a 2020 2020 2020 2020 2020 6966 2028  {.          if (
+0000c540: 7979 6a73 6f6e 5f70 7472 5f67 6574 5f73  yyjson_ptr_get_s
+0000c550: 7472 2028 6568 6974 6572 7661 6c2c 2022  tr (ehiterval, "
+0000c560: 2f54 7269 6767 6572 222c 2026 6865 6164  /Trigger", &head
+0000c570: 6572 5f73 7472 696e 6729 2026 260a 2020  er_string) &&.  
+0000c580: 2020 2020 2020 2020 2020 2020 7374 726e              strn
+0000c590: 6361 7365 636d 7020 2868 6561 6465 725f  casecmp (header_
+0000c5a0: 7374 7269 6e67 2c20 2241 5554 4f4d 4154  string, "AUTOMAT
+0000c5b0: 4943 222c 2039 2920 3d3d 2030 290a 2020  IC", 9) == 0).  
+0000c5c0: 2020 2020 2020 2020 2020 2a70 4d53 3242            *pMS2B
+0000c5d0: 3331 305f 464c 4147 5320 2872 6563 6f72  310_FLAGS (recor
+0000c5e0: 6420 2b20 7772 6974 7465 6e29 207c 3d20  d + written) |= 
+0000c5f0: 3078 3034 3b0a 0a20 2020 2020 2020 2020  0x04;..         
+0000c600: 2069 6620 2879 796a 736f 6e5f 7074 725f   if (yyjson_ptr_
+0000c610: 6765 745f 626f 6f6c 2028 6568 6974 6572  get_bool (ehiter
+0000c620: 7661 6c2c 2022 2f43 6f6e 7469 6e75 6564  val, "/Continued
+0000c630: 222c 2026 6865 6164 6572 5f62 6f6f 6c65  ", &header_boole
+0000c640: 616e 2920 2626 2068 6561 6465 725f 626f  an) && header_bo
+0000c650: 6f6c 6561 6e29 0a20 2020 2020 2020 2020  olean).         
+0000c660: 2020 202a 704d 5332 4233 3130 5f46 4c41     *pMS2B310_FLA
+0000c670: 4753 2028 7265 636f 7264 202b 2077 7269  GS (record + wri
+0000c680: 7474 656e 2920 7c3d 2030 7830 383b 0a0a  tten) |= 0x08;..
+0000c690: 2020 2020 2020 2020 2020 6966 2028 7979            if (yy
+0000c6a0: 6a73 6f6e 5f70 7472 5f67 6574 5f73 7472  json_ptr_get_str
+0000c6b0: 2028 6568 6974 6572 7661 6c2c 2022 2f41   (ehiterval, "/A
+0000c6c0: 6d70 6c69 7475 6465 5261 6e67 6522 2c20  mplitudeRange", 
+0000c6d0: 2668 6561 6465 725f 7374 7269 6e67 2929  &header_string))
+0000c6e0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
+0000c6f0: 2020 2020 2020 2020 2069 6620 2873 7472           if (str
+0000c700: 6e63 6173 6563 6d70 2028 6865 6164 6572  ncasecmp (header
+0000c710: 5f73 7472 696e 672c 2022 5045 414b 544f  _string, "PEAKTO
+0000c720: 5045 414b 222c 2031 3029 203d 3d20 3029  PEAK", 10) == 0)
+0000c730: 0a20 2020 2020 2020 2020 2020 2020 202a  .              *
+0000c740: 704d 5332 4233 3130 5f46 4c41 4753 2028  pMS2B310_FLAGS (
+0000c750: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000c760: 2920 7c3d 2030 7831 303b 0a20 2020 2020  ) |= 0x10;.     
+0000c770: 2020 2020 2020 2069 6620 2873 7472 6e63         if (strnc
+0000c780: 6173 6563 6d70 2028 6865 6164 6572 5f73  asecmp (header_s
+0000c790: 7472 696e 672c 2022 5a45 524f 544f 5045  tring, "ZEROTOPE
+0000c7a0: 414b 222c 2031 3029 203d 3d20 3029 0a20  AK", 10) == 0). 
+0000c7b0: 2020 2020 2020 2020 2020 2020 202a 704d               *pM
+0000c7c0: 5332 4233 3130 5f46 4c41 4753 2028 7265  S2B310_FLAGS (re
+0000c7d0: 636f 7264 202b 2077 7269 7474 656e 2920  cord + written) 
+0000c7e0: 7c3d 2030 7832 303b 0a20 2020 2020 2020  |= 0x20;.       
+0000c7f0: 2020 2020 2069 6620 2873 7472 6e63 6173       if (strncas
+0000c800: 6563 6d70 2028 6865 6164 6572 5f73 7472  ecmp (header_str
+0000c810: 696e 672c 2022 524d 5322 2c20 3329 203d  ing, "RMS", 3) =
+0000c820: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
+0000c830: 2020 202a 704d 5332 4233 3130 5f46 4c41     *pMS2B310_FLA
+0000c840: 4753 2028 7265 636f 7264 202b 2077 7269  GS (record + wri
+0000c850: 7474 656e 2920 7c3d 2030 7834 303b 0a20  tten) |= 0x40;. 
+0000c860: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+0000c870: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+0000c880: 5f70 7472 5f67 6574 5f6e 756d 2028 6568  _ptr_get_num (eh
+0000c890: 6974 6572 7661 6c2c 2022 2f44 7572 6174  iterval, "/Durat
+0000c8a0: 696f 6e22 2c20 2668 6561 6465 725f 6e75  ion", &header_nu
+0000c8b0: 6d62 6572 2929 0a20 2020 2020 2020 2020  mber)).         
+0000c8c0: 2020 202a 704d 5332 4233 3130 5f44 5552     *pMS2B310_DUR
+0000c8d0: 4154 494f 4e20 2872 6563 6f72 6420 2b20  ATION (record + 
+0000c8e0: 7772 6974 7465 6e29 203d 2048 4f34 7520  written) = HO4u 
+0000c8f0: 2828 7569 6e74 3332 5f74 2928 6865 6164  ((uint32_t)(head
+0000c900: 6572 5f6e 756d 6265 7220 2a20 3130 3030  er_number * 1000
+0000c910: 3020 2b20 302e 3529 2c20 7377 6170 666c  0 + 0.5), swapfl
+0000c920: 6167 293b 0a0a 2020 2020 2020 2020 2020  ag);..          
+0000c930: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
+0000c940: 6574 5f6e 756d 2028 6568 6974 6572 7661  et_num (ehiterva
+0000c950: 6c2c 2022 2f53 696e 6550 6572 696f 6422  l, "/SinePeriod"
+0000c960: 2c20 2668 6561 6465 725f 6e75 6d62 6572  , &header_number
+0000c970: 2929 0a20 2020 2020 2020 2020 2020 202a  )).            *
+0000c980: 704d 5332 4233 3130 5f50 4552 494f 4420  pMS2B310_PERIOD 
+0000c990: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000c9a0: 6e29 203d 2048 4f34 6620 2828 666c 6f61  n) = HO4f ((floa
+0000c9b0: 7429 6865 6164 6572 5f6e 756d 6265 722c  t)header_number,
+0000c9c0: 2073 7761 7066 6c61 6729 3b0a 0a20 2020   swapflag);..   
+0000c9d0: 2020 2020 2020 2069 6620 2879 796a 736f         if (yyjso
+0000c9e0: 6e5f 7074 725f 6765 745f 6e75 6d20 2865  n_ptr_get_num (e
+0000c9f0: 6869 7465 7276 616c 2c20 222f 416d 706c  hiterval, "/Ampl
+0000ca00: 6974 7564 6522 2c20 2668 6561 6465 725f  itude", &header_
+0000ca10: 6e75 6d62 6572 2929 0a20 2020 2020 2020  number)).       
+0000ca20: 2020 2020 202a 704d 5332 4233 3130 5f41       *pMS2B310_A
+0000ca30: 4d50 4c49 5455 4445 2028 7265 636f 7264  MPLITUDE (record
+0000ca40: 202b 2077 7269 7474 656e 2920 3d20 484f   + written) = HO
+0000ca50: 3466 2028 2866 6c6f 6174 2968 6561 6465  4f ((float)heade
+0000ca60: 725f 6e75 6d62 6572 2c20 7377 6170 666c  r_number, swapfl
+0000ca70: 6167 293b 0a0a 2020 2020 2020 2020 2020  ag);..          
+0000ca80: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
+0000ca90: 6574 5f73 7472 2028 6568 6974 6572 7661  et_str (ehiterva
+0000caa0: 6c2c 2022 2f49 6e70 7574 4368 616e 6e65  l, "/InputChanne
+0000cab0: 6c22 2c20 2668 6561 6465 725f 7374 7269  l", &header_stri
+0000cac0: 6e67 2929 0a20 2020 2020 2020 2020 2020  ng)).           
+0000cad0: 206d 735f 7374 726e 6370 6f70 656e 2028   ms_strncpopen (
+0000cae0: 704d 5332 4233 3130 5f49 4e50 5554 4348  pMS2B310_INPUTCH
+0000caf0: 414e 4e45 4c20 2872 6563 6f72 6420 2b20  ANNEL (record + 
+0000cb00: 7772 6974 7465 6e29 2c20 6865 6164 6572  written), header
+0000cb10: 5f73 7472 696e 672c 2033 293b 0a0a 2020  _string, 3);..  
+0000cb20: 2020 2020 2020 2020 6966 2028 7979 6a73          if (yyjs
+0000cb30: 6f6e 5f70 7472 5f67 6574 5f6e 756d 2028  on_ptr_get_num (
+0000cb40: 6568 6974 6572 7661 6c2c 2022 2f52 6566  ehiterval, "/Ref
+0000cb50: 6572 656e 6365 416d 706c 6974 7564 6522  erenceAmplitude"
+0000cb60: 2c20 2668 6561 6465 725f 6e75 6d62 6572  , &header_number
+0000cb70: 2929 0a20 2020 2020 2020 2020 2020 202a  )).            *
+0000cb80: 704d 5332 4233 3130 5f52 4546 4552 454e  pMS2B310_REFEREN
+0000cb90: 4345 414d 504c 4954 5544 4520 2872 6563  CEAMPLITUDE (rec
+0000cba0: 6f72 6420 2b20 7772 6974 7465 6e29 203d  ord + written) =
+0000cbb0: 2048 4f34 7520 2828 7569 6e74 3332 5f74   HO4u ((uint32_t
+0000cbc0: 2928 6865 6164 6572 5f6e 756d 6265 7220  )(header_number 
+0000cbd0: 2b20 302e 3529 2c20 7377 6170 666c 6167  + 0.5), swapflag
+0000cbe0: 293b 0a0a 2020 2020 2020 2020 2020 6966  );..          if
+0000cbf0: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000cc00: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
+0000cc10: 2022 2f43 6f75 706c 696e 6722 2c20 2668   "/Coupling", &h
+0000cc20: 6561 6465 725f 7374 7269 6e67 2929 0a20  eader_string)). 
+0000cc30: 2020 2020 2020 2020 2020 206d 735f 7374             ms_st
+0000cc40: 726e 6370 6f70 656e 2028 704d 5332 4233  rncpopen (pMS2B3
+0000cc50: 3130 5f43 4f55 504c 494e 4720 2872 6563  10_COUPLING (rec
+0000cc60: 6f72 6420 2b20 7772 6974 7465 6e29 2c20  ord + written), 
+0000cc70: 6865 6164 6572 5f73 7472 696e 672c 2031  header_string, 1
+0000cc80: 3229 3b0a 0a20 2020 2020 2020 2020 2069  2);..          i
+0000cc90: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
+0000cca0: 745f 7374 7220 2865 6869 7465 7276 616c  t_str (ehiterval
+0000ccb0: 2c20 222f 526f 6c6c 6f66 6622 2c20 2668  , "/Rolloff", &h
+0000ccc0: 6561 6465 725f 7374 7269 6e67 2929 0a20  eader_string)). 
+0000ccd0: 2020 2020 2020 2020 2020 206d 735f 7374             ms_st
+0000cce0: 726e 6370 6f70 656e 2028 704d 5332 4233  rncpopen (pMS2B3
+0000ccf0: 3130 5f52 4f4c 4c4f 4646 2028 7265 636f  10_ROLLOFF (reco
+0000cd00: 7264 202b 2077 7269 7474 656e 292c 2068  rd + written), h
+0000cd10: 6561 6465 725f 7374 7269 6e67 2c20 3132  eader_string, 12
+0000cd20: 293b 0a20 2020 2020 2020 207d 0a20 2020  );.        }.   
+0000cd30: 2020 2020 2065 6c73 6520 6966 2028 626c       else if (bl
+0000cd40: 6f63 6b65 7474 655f 7479 7065 203d 3d20  ockette_type == 
+0000cd50: 3332 3029 0a20 2020 2020 2020 207b 0a20  320).        {. 
+0000cd60: 2020 2020 2020 2020 2069 6620 2879 796a           if (yyj
+0000cd70: 736f 6e5f 7074 725f 6765 745f 7374 7220  son_ptr_get_str 
+0000cd80: 2865 6869 7465 7276 616c 2c20 222f 5472  (ehiterval, "/Tr
+0000cd90: 6967 6765 7222 2c20 2668 6561 6465 725f  igger", &header_
+0000cda0: 7374 7269 6e67 2920 2626 0a20 2020 2020  string) &&.     
+0000cdb0: 2020 2020 2020 2020 2073 7472 6e63 6173           strncas
+0000cdc0: 6563 6d70 2028 6865 6164 6572 5f73 7472  ecmp (header_str
+0000cdd0: 696e 672c 2022 4155 544f 4d41 5449 4322  ing, "AUTOMATIC"
+0000cde0: 2c20 3929 203d 3d20 3029 0a20 2020 2020  , 9) == 0).     
+0000cdf0: 2020 2020 2020 202a 704d 5332 4233 3230         *pMS2B320
+0000ce00: 5f46 4c41 4753 2028 7265 636f 7264 202b  _FLAGS (record +
+0000ce10: 2077 7269 7474 656e 2920 7c3d 2030 7830   written) |= 0x0
+0000ce20: 343b 0a0a 2020 2020 2020 2020 2020 6966  4;..          if
+0000ce30: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000ce40: 5f62 6f6f 6c20 2865 6869 7465 7276 616c  _bool (ehiterval
+0000ce50: 2c20 222f 436f 6e74 696e 7565 6422 2c20  , "/Continued", 
+0000ce60: 2668 6561 6465 725f 626f 6f6c 6561 6e29  &header_boolean)
+0000ce70: 2026 2620 6865 6164 6572 5f62 6f6f 6c65   && header_boole
+0000ce80: 616e 290a 2020 2020 2020 2020 2020 2020  an).            
+0000ce90: 2a70 4d53 3242 3332 305f 464c 4147 5320  *pMS2B320_FLAGS 
+0000cea0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000ceb0: 6e29 207c 3d20 3078 3038 3b0a 0a20 2020  n) |= 0x08;..   
+0000cec0: 2020 2020 2020 2069 6620 2879 796a 736f         if (yyjso
+0000ced0: 6e5f 7074 725f 6765 745f 7374 7220 2865  n_ptr_get_str (e
+0000cee0: 6869 7465 7276 616c 2c20 222f 416d 706c  hiterval, "/Ampl
+0000cef0: 6974 7564 6552 616e 6765 222c 2026 6865  itudeRange", &he
+0000cf00: 6164 6572 5f73 7472 696e 6729 2026 260a  ader_string) &&.
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000cf20: 726e 6361 7365 636d 7020 2868 6561 6465  rncasecmp (heade
+0000cf30: 725f 7374 7269 6e67 2c20 2252 414e 444f  r_string, "RANDO
+0000cf40: 4d22 2c20 3629 203d 3d20 3029 0a20 2020  M", 6) == 0).   
+0000cf50: 2020 2020 2020 2020 202a 704d 5332 4233           *pMS2B3
+0000cf60: 3230 5f46 4c41 4753 2028 7265 636f 7264  20_FLAGS (record
+0000cf70: 202b 2077 7269 7474 656e 2920 7c3d 2030   + written) |= 0
+0000cf80: 7831 303b 0a0a 2020 2020 2020 2020 2020  x10;..          
+0000cf90: 6966 2028 7979 6a73 6f6e 5f70 7472 5f67  if (yyjson_ptr_g
+0000cfa0: 6574 5f6e 756d 2028 6568 6974 6572 7661  et_num (ehiterva
+0000cfb0: 6c2c 2022 2f44 7572 6174 696f 6e22 2c20  l, "/Duration", 
+0000cfc0: 2668 6561 6465 725f 6e75 6d62 6572 2929  &header_number))
+0000cfd0: 0a20 2020 2020 2020 2020 2020 202a 704d  .            *pM
+0000cfe0: 5332 4233 3230 5f44 5552 4154 494f 4e20  S2B320_DURATION 
+0000cff0: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000d000: 6e29 203d 2048 4f34 7520 2828 7569 6e74  n) = HO4u ((uint
+0000d010: 3332 5f74 2928 6865 6164 6572 5f6e 756d  32_t)(header_num
+0000d020: 6265 7220 2a20 3130 3030 3020 2b20 302e  ber * 10000 + 0.
+0000d030: 3529 2c20 7377 6170 666c 6167 293b 0a0a  5), swapflag);..
+0000d040: 2020 2020 2020 2020 2020 6966 2028 7979            if (yy
+0000d050: 6a73 6f6e 5f70 7472 5f67 6574 5f6e 756d  json_ptr_get_num
+0000d060: 2028 6568 6974 6572 7661 6c2c 2022 2f41   (ehiterval, "/A
+0000d070: 6d70 6c69 7475 6465 222c 2026 6865 6164  mplitude", &head
+0000d080: 6572 5f6e 756d 6265 7229 290a 2020 2020  er_number)).    
+0000d090: 2020 2020 2020 2020 2a70 4d53 3242 3332          *pMS2B32
+0000d0a0: 305f 5054 5041 4d50 4c49 5455 4445 2028  0_PTPAMPLITUDE (
+0000d0b0: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000d0c0: 2920 3d20 484f 3466 2028 2866 6c6f 6174  ) = HO4f ((float
+0000d0d0: 2968 6561 6465 725f 6e75 6d62 6572 2c20  )header_number, 
+0000d0e0: 7377 6170 666c 6167 293b 0a0a 2020 2020  swapflag);..    
+0000d0f0: 2020 2020 2020 6966 2028 7979 6a73 6f6e        if (yyjson
+0000d100: 5f70 7472 5f67 6574 5f73 7472 2028 6568  _ptr_get_str (eh
+0000d110: 6974 6572 7661 6c2c 2022 2f49 6e70 7574  iterval, "/Input
+0000d120: 4368 616e 6e65 6c22 2c20 2668 6561 6465  Channel", &heade
+0000d130: 725f 7374 7269 6e67 2929 0a20 2020 2020  r_string)).     
+0000d140: 2020 2020 2020 206d 735f 7374 726e 6370         ms_strncp
+0000d150: 6f70 656e 2028 704d 5332 4233 3230 5f49  open (pMS2B320_I
+0000d160: 4e50 5554 4348 414e 4e45 4c20 2872 6563  NPUTCHANNEL (rec
+0000d170: 6f72 6420 2b20 7772 6974 7465 6e29 2c20  ord + written), 
+0000d180: 6865 6164 6572 5f73 7472 696e 672c 2033  header_string, 3
+0000d190: 293b 0a0a 2020 2020 2020 2020 2020 6966  );..          if
+0000d1a0: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000d1b0: 5f6e 756d 2028 6568 6974 6572 7661 6c2c  _num (ehiterval,
+0000d1c0: 2022 2f52 6566 6572 656e 6365 416d 706c   "/ReferenceAmpl
+0000d1d0: 6974 7564 6522 2c20 2668 6561 6465 725f  itude", &header_
+0000d1e0: 6e75 6d62 6572 2929 0a20 2020 2020 2020  number)).       
+0000d1f0: 2020 2020 202a 704d 5332 4233 3230 5f52       *pMS2B320_R
+0000d200: 4546 4552 454e 4345 414d 504c 4954 5544  EFERENCEAMPLITUD
+0000d210: 4520 2872 6563 6f72 6420 2b20 7772 6974  E (record + writ
+0000d220: 7465 6e29 203d 2048 4f34 7520 2828 7569  ten) = HO4u ((ui
+0000d230: 6e74 3332 5f74 2928 6865 6164 6572 5f6e  nt32_t)(header_n
+0000d240: 756d 6265 7220 2b20 302e 3529 2c20 7377  umber + 0.5), sw
+0000d250: 6170 666c 6167 293b 0a0a 2020 2020 2020  apflag);..      
+0000d260: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
+0000d270: 7472 5f67 6574 5f73 7472 2028 6568 6974  tr_get_str (ehit
+0000d280: 6572 7661 6c2c 2022 2f43 6f75 706c 696e  erval, "/Couplin
+0000d290: 6722 2c20 2668 6561 6465 725f 7374 7269  g", &header_stri
+0000d2a0: 6e67 2929 0a20 2020 2020 2020 2020 2020  ng)).           
+0000d2b0: 206d 735f 7374 726e 6370 6f70 656e 2028   ms_strncpopen (
+0000d2c0: 704d 5332 4233 3230 5f43 4f55 504c 494e  pMS2B320_COUPLIN
+0000d2d0: 4720 2872 6563 6f72 6420 2b20 7772 6974  G (record + writ
+0000d2e0: 7465 6e29 2c20 6865 6164 6572 5f73 7472  ten), header_str
+0000d2f0: 696e 672c 2031 3229 3b0a 0a20 2020 2020  ing, 12);..     
+0000d300: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
+0000d310: 7074 725f 6765 745f 7374 7220 2865 6869  ptr_get_str (ehi
+0000d320: 7465 7276 616c 2c20 222f 526f 6c6c 6f66  terval, "/Rollof
+0000d330: 6622 2c20 2668 6561 6465 725f 7374 7269  f", &header_stri
+0000d340: 6e67 2929 0a20 2020 2020 2020 2020 2020  ng)).           
+0000d350: 206d 735f 7374 726e 6370 6f70 656e 2028   ms_strncpopen (
+0000d360: 704d 5332 4233 3230 5f52 4f4c 4c4f 4646  pMS2B320_ROLLOFF
+0000d370: 2028 7265 636f 7264 202b 2077 7269 7474   (record + writt
+0000d380: 656e 292c 2068 6561 6465 725f 7374 7269  en), header_stri
+0000d390: 6e67 2c20 3132 293b 0a0a 2020 2020 2020  ng, 12);..      
+0000d3a0: 2020 2020 6966 2028 7979 6a73 6f6e 5f70      if (yyjson_p
+0000d3b0: 7472 5f67 6574 5f73 7472 2028 6568 6974  tr_get_str (ehit
+0000d3c0: 6572 7661 6c2c 2022 2f4e 6f69 7365 222c  erval, "/Noise",
+0000d3d0: 2026 6865 6164 6572 5f73 7472 696e 6729   &header_string)
+0000d3e0: 290a 2020 2020 2020 2020 2020 2020 6d73  ).            ms
+0000d3f0: 5f73 7472 6e63 706f 7065 6e20 2870 4d53  _strncpopen (pMS
+0000d400: 3242 3332 305f 4e4f 4953 4554 5950 4520  2B320_NOISETYPE 
+0000d410: 2872 6563 6f72 6420 2b20 7772 6974 7465  (record + writte
+0000d420: 6e29 2c20 6865 6164 6572 5f73 7472 696e  n), header_strin
+0000d430: 672c 2038 293b 0a20 2020 2020 2020 207d  g, 8);.        }
+0000d440: 0a20 2020 2020 2020 2065 6c73 6520 6966  .        else if
+0000d450: 2028 626c 6f63 6b65 7474 655f 7479 7065   (blockette_type
+0000d460: 203d 3d20 3339 3029 0a20 2020 2020 2020   == 390).       
+0000d470: 207b 0a20 2020 2020 2020 2020 2069 6620   {.          if 
+0000d480: 2879 796a 736f 6e5f 7074 725f 6765 745f  (yyjson_ptr_get_
+0000d490: 7374 7220 2865 6869 7465 7276 616c 2c20  str (ehiterval, 
+0000d4a0: 222f 5472 6967 6765 7222 2c20 2668 6561  "/Trigger", &hea
+0000d4b0: 6465 725f 7374 7269 6e67 2920 2626 0a20  der_string) &&. 
+0000d4c0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000d4d0: 6e63 6173 6563 6d70 2028 6865 6164 6572  ncasecmp (header
+0000d4e0: 5f73 7472 696e 672c 2022 4155 544f 4d41  _string, "AUTOMA
+0000d4f0: 5449 4322 2c20 3929 203d 3d20 3029 0a20  TIC", 9) == 0). 
+0000d500: 2020 2020 2020 2020 2020 202a 704d 5332             *pMS2
+0000d510: 4233 3930 5f46 4c41 4753 2028 7265 636f  B390_FLAGS (reco
+0000d520: 7264 202b 2077 7269 7474 656e 2920 7c3d  rd + written) |=
+0000d530: 2030 7830 343b 0a0a 2020 2020 2020 2020   0x04;..        
+0000d540: 2020 6966 2028 7979 6a73 6f6e 5f70 7472    if (yyjson_ptr
+0000d550: 5f67 6574 5f62 6f6f 6c20 2865 6869 7465  _get_bool (ehite
+0000d560: 7276 616c 2c20 222f 436f 6e74 696e 7565  rval, "/Continue
+0000d570: 6422 2c20 2668 6561 6465 725f 626f 6f6c  d", &header_bool
+0000d580: 6561 6e29 2026 2620 6865 6164 6572 5f62  ean) && header_b
+0000d590: 6f6f 6c65 616e 290a 2020 2020 2020 2020  oolean).        
+0000d5a0: 2020 2020 2a70 4d53 3242 3339 305f 464c      *pMS2B390_FL
+0000d5b0: 4147 5320 2872 6563 6f72 6420 2b20 7772  AGS (record + wr
+0000d5c0: 6974 7465 6e29 207c 3d20 3078 3038 3b0a  itten) |= 0x08;.
+0000d5d0: 0a20 2020 2020 2020 2020 2069 6620 2879  .          if (y
+0000d5e0: 796a 736f 6e5f 7074 725f 6765 745f 6e75  yjson_ptr_get_nu
+0000d5f0: 6d20 2865 6869 7465 7276 616c 2c20 222f  m (ehiterval, "/
+0000d600: 4475 7261 7469 6f6e 222c 2026 6865 6164  Duration", &head
+0000d610: 6572 5f6e 756d 6265 7229 290a 2020 2020  er_number)).    
+0000d620: 2020 2020 2020 2020 2a70 4d53 3242 3339          *pMS2B39
+0000d630: 305f 4455 5241 5449 4f4e 2028 7265 636f  0_DURATION (reco
+0000d640: 7264 202b 2077 7269 7474 656e 2920 3d20  rd + written) = 
+0000d650: 484f 3475 2028 2875 696e 7433 325f 7429  HO4u ((uint32_t)
+0000d660: 2868 6561 6465 725f 6e75 6d62 6572 202a  (header_number *
+0000d670: 2031 3030 3030 202b 2030 2e35 292c 2073   10000 + 0.5), s
+0000d680: 7761 7066 6c61 6729 3b0a 0a20 2020 2020  wapflag);..     
+0000d690: 2020 2020 2069 6620 2879 796a 736f 6e5f       if (yyjson_
+0000d6a0: 7074 725f 6765 745f 6e75 6d20 2865 6869  ptr_get_num (ehi
+0000d6b0: 7465 7276 616c 2c20 222f 416d 706c 6974  terval, "/Amplit
+0000d6c0: 7564 6522 2c20 2668 6561 6465 725f 6e75  ude", &header_nu
+0000d6d0: 6d62 6572 2929 0a20 2020 2020 2020 2020  mber)).         
+0000d6e0: 2020 202a 704d 5332 4233 3930 5f41 4d50     *pMS2B390_AMP
+0000d6f0: 4c49 5455 4445 2028 7265 636f 7264 202b  LITUDE (record +
+0000d700: 2077 7269 7474 656e 2920 3d20 484f 3466   written) = HO4f
+0000d710: 2028 2866 6c6f 6174 2968 6561 6465 725f   ((float)header_
+0000d720: 6e75 6d62 6572 2c20 7377 6170 666c 6167  number, swapflag
+0000d730: 293b 0a0a 2020 2020 2020 2020 2020 6966  );..          if
+0000d740: 2028 7979 6a73 6f6e 5f70 7472 5f67 6574   (yyjson_ptr_get
+0000d750: 5f73 7472 2028 6568 6974 6572 7661 6c2c  _str (ehiterval,
+0000d760: 2022 2f49 6e70 7574 4368 616e 6e65 6c22   "/InputChannel"
+0000d770: 2c20 2668 6561 6465 725f 7374 7269 6e67  , &header_string
+0000d780: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
+0000d790: 735f 7374 726e 6370 6f70 656e 2028 704d  s_strncpopen (pM
+0000d7a0: 5332 4233 3930 5f49 4e50 5554 4348 414e  S2B390_INPUTCHAN
+0000d7b0: 4e45 4c20 2872 6563 6f72 6420 2b20 7772  NEL (record + wr
+0000d7c0: 6974 7465 6e29 2c20 6865 6164 6572 5f73  itten), header_s
+0000d7d0: 7472 696e 672c 2033 293b 0a20 2020 2020  tring, 3);.     
+0000d7e0: 2020 207d 0a0a 2020 2020 2020 2020 7772     }..        wr
+0000d7f0: 6974 7465 6e20 2b3d 2062 6c6f 636b 6574  itten += blocket
+0000d800: 7465 5f6c 656e 6774 683b 0a20 2020 2020  te_length;.     
+0000d810: 207d 0a0a 2020 2020 2020 2f2a 2041 6464   }..      /* Add
+0000d820: 2042 6c6f 636b 6574 7465 2033 3935 2069   Blockette 395 i
+0000d830: 6620 456e 6454 696d 6520 6973 2069 6e63  f EndTime is inc
+0000d840: 6c75 6465 6420 2a2f 0a20 2020 2020 2069  luded */.      i
+0000d850: 6620 2879 796a 736f 6e5f 7074 725f 6765  f (yyjson_ptr_ge
+0000d860: 745f 7374 7220 2865 6869 7465 7276 616c  t_str (ehiterval
+0000d870: 2c20 222f 456e 6454 696d 6522 2c20 2668  , "/EndTime", &h
+0000d880: 6561 6465 725f 7374 7269 6e67 2929 0a20  eader_string)). 
+0000d890: 2020 2020 207b 0a20 2020 2020 2020 2062       {.        b
+0000d8a0: 6c6f 636b 6574 7465 5f74 7970 6520 203d  lockette_type  =
+0000d8b0: 2033 3935 3b0a 2020 2020 2020 2020 626c   395;.        bl
+0000d8c0: 6f63 6b65 7474 655f 6c65 6e67 7468 203d  ockette_length =
+0000d8d0: 2031 363b 0a0a 2020 2020 2020 2020 6966   16;..        if
+0000d8e0: 2028 2872 6563 6275 666c 656e 202d 2077   ((recbuflen - w
+0000d8f0: 7269 7474 656e 2920 3c20 626c 6f63 6b65  ritten) < blocke
+0000d900: 7474 655f 6c65 6e67 7468 290a 2020 2020  tte_length).    
+0000d910: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000d920: 6d73 5f6c 6f67 2028 322c 2022 2573 3a20  ms_log (2, "%s: 
+0000d930: 5265 636f 7264 206c 656e 6774 6820 6e6f  Record length no
+0000d940: 7420 6c61 7267 6520 656e 6f75 6768 2066  t large enough f
+0000d950: 6f72 2042 2575 5c6e 222c 206d 7372 2d3e  or B%u\n", msr->
+0000d960: 7369 642c 2062 6c6f 636b 6574 7465 5f74  sid, blockette_t
+0000d970: 7970 6529 3b0a 2020 2020 2020 2020 2020  ype);.          
+0000d980: 7979 6a73 6f6e 5f64 6f63 5f66 7265 6520  yyjson_doc_free 
+0000d990: 2865 6864 6f63 293b 0a20 2020 2020 2020  (ehdoc);.       
+0000d9a0: 2020 2072 6574 7572 6e20 2d31 3b0a 2020     return -1;.  
+0000d9b0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+0000d9c0: 202a 6e65 7874 5f62 6c6f 636b 6574 7465   *next_blockette
+0000d9d0: 203d 2048 4f32 7520 2828 7569 6e74 3136   = HO2u ((uint16
+0000d9e0: 5f74 2977 7269 7474 656e 2c20 7377 6170  _t)written, swap
+0000d9f0: 666c 6167 293b 0a20 2020 2020 2020 206e  flag);.        n
+0000da00: 6578 745f 626c 6f63 6b65 7474 6520 203d  ext_blockette  =
+0000da10: 2070 4d53 3242 3339 355f 4e45 5854 2028   pMS2B395_NEXT (
+0000da20: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000da30: 293b 0a20 2020 2020 2020 202a 704d 5332  );.        *pMS2
+0000da40: 4653 4448 5f4e 554d 424c 4f43 4b45 5454  FSDH_NUMBLOCKETT
+0000da50: 4553 2028 7265 636f 7264 2920 2b3d 2031  ES (record) += 1
+0000da60: 3b0a 0a20 2020 2020 2020 206d 656d 7365  ;..        memse
+0000da70: 7420 2872 6563 6f72 6420 2b20 7772 6974  t (record + writ
+0000da80: 7465 6e2c 2030 2c20 626c 6f63 6b65 7474  ten, 0, blockett
+0000da90: 655f 6c65 6e67 7468 293b 0a20 2020 2020  e_length);.     
+0000daa0: 2020 202a 704d 5332 4233 3935 5f54 5950     *pMS2B395_TYP
+0000dab0: 4520 2872 6563 6f72 6420 2b20 7772 6974  E (record + writ
+0000dac0: 7465 6e29 203d 2048 4f32 7520 2862 6c6f  ten) = HO2u (blo
+0000dad0: 636b 6574 7465 5f74 7970 652c 2073 7761  ckette_type, swa
+0000dae0: 7066 6c61 6729 3b0a 2020 2020 2020 2020  pflag);.        
+0000daf0: 2a70 4d53 3242 3339 355f 4e45 5854 2028  *pMS2B395_NEXT (
+0000db00: 7265 636f 7264 202b 2077 7269 7474 656e  record + written
+0000db10: 2920 3d20 303b 0a0a 2020 2020 2020 2020  ) = 0;..        
+0000db20: 6966 2028 6d73 5f74 696d 6573 7472 3262  if (ms_timestr2b
+0000db30: 7469 6d65 2028 6865 6164 6572 5f73 7472  time (header_str
+0000db40: 696e 672c 2028 7569 6e74 385f 7420 2a29  ing, (uint8_t *)
+0000db50: 704d 5332 4233 3935 5f59 4541 5220 2872  pMS2B395_YEAR (r
+0000db60: 6563 6f72 6420 2b20 7772 6974 7465 6e29  ecord + written)
+0000db70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db90: 6d73 722d 3e73 6964 2c20 7377 6170 666c  msr->sid, swapfl
+0000dba0: 6167 2920 3d3d 202d 3129 0a20 2020 2020  ag) == -1).     
+0000dbb0: 2020 207b 0a20 2020 2020 2020 2020 206d     {.          m
+0000dbc0: 735f 6c6f 6720 2832 2c20 2225 733a 2043  s_log (2, "%s: C
+0000dbd0: 616e 6e6f 7420 636f 6e76 6572 7420 4225  annot convert B%
+0000dbe0: 7520 7469 6d65 3a20 2573 5c6e 222c 206d  u time: %s\n", m
+0000dbf0: 7372 2d3e 7369 642c 2062 6c6f 636b 6574  sr->sid, blocket
+0000dc00: 7465 5f74 7970 652c 2068 6561 6465 725f  te_type, header_
+0000dc10: 7374 7269 6e67 293b 0a20 2020 2020 2020  string);.       
+0000dc20: 2020 2079 796a 736f 6e5f 646f 635f 6672     yyjson_doc_fr
+0000dc30: 6565 2028 6568 646f 6329 3b0a 2020 2020  ee (ehdoc);.    
+0000dc40: 2020 2020 2020 7265 7475 726e 202d 313b        return -1;
+0000dc50: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+0000dc60: 2020 2020 7772 6974 7465 6e20 2b3d 2062      written += b
+0000dc70: 6c6f 636b 6574 7465 5f6c 656e 6774 683b  lockette_length;
+0000dc80: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
+0000dc90: 207d 202f 2a20 456e 6420 6966 202f 4644   } /* End if /FD
+0000dca0: 534e 2f45 7665 6e74 2f44 6574 6563 7469  SN/Event/Detecti
+0000dcb0: 6f6e 202a 2f0a 0a20 2069 6620 2865 6864  on */..  if (ehd
+0000dcc0: 6f63 290a 2020 7b0a 2020 2020 7979 6a73  oc).  {.    yyjs
+0000dcd0: 6f6e 5f64 6f63 5f66 7265 6520 2865 6864  on_doc_free (ehd
+0000dce0: 6f63 293b 0a20 207d 0a0a 2020 7265 7475  oc);.  }..  retu
+0000dcf0: 726e 2077 7269 7474 656e 3b0a 7d20 2f2a  rn written;.} /*
+0000dd00: 2045 6e64 206f 6620 6d73 7233 5f70 6163   End of msr3_pac
+0000dd10: 6b5f 6865 6164 6572 3228 2920 2a2f 0a0a  k_header2() */..
+0000dd20: 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  /***************
+0000dd30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000dd40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000dd50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000dd60: 2a2a 2a2a 2a2a 2a2a 2a0a 202a 2020 5061  *********. *  Pa
+0000dd70: 636b 2064 6174 6120 7361 6d70 6c65 732e  ck data samples.
+0000dd80: 2020 5468 6520 696e 7075 7420 6461 7461    The input data
+0000dd90: 2073 616d 706c 6573 2073 7065 6369 6669   samples specifi
+0000dda0: 6564 2061 7320 2773 7263 2720 7769 6c6c  ed as 'src' will
+0000ddb0: 0a20 2a20 2062 6520 7061 636b 6564 2077  . *  be packed w
+0000ddc0: 6974 6820 2765 6e63 6f64 696e 6727 2066  ith 'encoding' f
+0000ddd0: 6f72 6d61 7420 616e 6420 706c 6163 6564  ormat and placed
+0000dde0: 2069 6e20 2764 6573 7427 2e0a 202a 0a20   in 'dest'.. *. 
+0000ddf0: 2a20 2052 6574 7572 6e20 6e75 6d62 6572  *  Return number
+0000de00: 206f 6620 7361 6d70 6c65 7320 7061 636b   of samples pack
+0000de10: 6564 206f 6e20 7375 6363 6573 7320 616e  ed on success an
+0000de20: 6420 6120 6e65 6761 7469 7665 206f 6e20  d a negative on 
+0000de30: 6572 726f 722e 0a20 2a0a 202a 205c 7265  error.. *. * \re
+0000de40: 6620 4d65 7373 6167 654f 6e45 7272 6f72  f MessageOnError
+0000de50: 202d 2074 6869 7320 6675 6e63 7469 6f6e   - this function
+0000de60: 206c 6f67 7320 6120 6d65 7373 6167 6520   logs a message 
+0000de70: 6f6e 2065 7272 6f72 0a20 2a2a 2a2a 2a2a  on error. ******
+0000de80: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000de90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000dea0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000deb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000dec0: 2a2a 2f0a 7374 6174 6963 2069 6e74 3634  **/.static int64
+0000ded0: 5f74 0a6d 7372 5f70 6163 6b5f 6461 7461  _t.msr_pack_data
+0000dee0: 2028 766f 6964 202a 6465 7374 2c20 766f   (void *dest, vo
+0000def0: 6964 202a 7372 632c 2075 696e 7436 345f  id *src, uint64_
+0000df00: 7420 6d61 7873 616d 706c 6573 2c20 7569  t maxsamples, ui
+0000df10: 6e74 3634 5f74 206d 6178 6461 7461 6279  nt64_t maxdataby
+0000df20: 7465 732c 0a20 2020 2020 2020 2020 2020  tes,.           
+0000df30: 2020 2020 6368 6172 2073 616d 706c 6574      char samplet
+0000df40: 7970 652c 2069 6e74 385f 7420 656e 636f  ype, int8_t enco
+0000df50: 6469 6e67 2c20 696e 7438 5f74 2073 7761  ding, int8_t swa
+0000df60: 7066 6c61 672c 0a20 2020 2020 2020 2020  pflag,.         
+0000df70: 2020 2020 2020 7569 6e74 3332 5f74 202a        uint32_t *
+0000df80: 6279 7465 7377 7269 7474 656e 2c20 636f  byteswritten, co
+0000df90: 6e73 7420 6368 6172 202a 7369 642c 2069  nst char *sid, i
+0000dfa0: 6e74 385f 7420 7665 7262 6f73 6529 0a7b  nt8_t verbose).{
+0000dfb0: 0a20 2069 6e74 3634 5f74 206e 7361 6d70  .  int64_t nsamp
+0000dfc0: 6c65 733b 0a0a 2020 6966 2028 6279 7465  les;..  if (byte
+0000dfd0: 7377 7269 7474 656e 290a 2020 2020 2a62  swritten).    *b
+0000dfe0: 7974 6573 7772 6974 7465 6e20 3d20 303b  yteswritten = 0;
+0000dff0: 0a0a 2020 2f2a 2044 6563 6964 6520 6966  ..  /* Decide if
+0000e000: 2074 6869 7320 6973 2061 2066 6f72 6d61   this is a forma
+0000e010: 7420 7468 6174 2077 6520 6361 6e20 656e  t that we can en
+0000e020: 636f 6465 202a 2f0a 2020 7377 6974 6368  code */.  switch
+0000e030: 2028 656e 636f 6469 6e67 290a 2020 7b0a   (encoding).  {.
+0000e040: 2020 6361 7365 2044 455f 5445 5854 3a0a    case DE_TEXT:.
+0000e050: 2020 2020 6966 2028 7361 6d70 6c65 7479      if (samplety
+0000e060: 7065 2021 3d20 2774 2720 2626 2073 616d  pe != 't' && sam
+0000e070: 706c 6574 7970 6520 213d 2027 6127 290a  pletype != 'a').
+0000e080: 2020 2020 7b0a 2020 2020 2020 6d73 5f6c      {.      ms_l
+0000e090: 6f67 2028 322c 2022 2573 3a20 5361 6d70  og (2, "%s: Samp
+0000e0a0: 6c65 2074 7970 6520 6d75 7374 2062 6520  le type must be 
+0000e0b0: 7465 7874 2028 7429 2066 6f72 2074 6578  text (t) for tex
+0000e0c0: 7420 656e 636f 6469 6e67 206e 6f74 2027  t encoding not '
+0000e0d0: 2563 275c 6e22 2c0a 2020 2020 2020 2020  %c'\n",.        
+0000e0e0: 2020 2020 2020 7369 642c 2073 616d 706c        sid, sampl
+0000e0f0: 6574 7970 6529 3b0a 2020 2020 2020 7265  etype);.      re
+0000e100: 7475 726e 202d 313b 0a20 2020 207d 0a0a  turn -1;.    }..
+0000e110: 2020 2020 6966 2028 7665 7262 6f73 6520      if (verbose 
+0000e120: 3e20 3129 0a20 2020 2020 206d 735f 6c6f  > 1).      ms_lo
+0000e130: 6720 2830 2c20 2225 733a 2050 6163 6b69  g (0, "%s: Packi
+0000e140: 6e67 2074 6578 7420 6461 7461 5c6e 222c  ng text data\n",
+0000e150: 2073 6964 293b 0a0a 2020 2020 6e73 616d   sid);..    nsam
+0000e160: 706c 6573 203d 206d 7372 5f65 6e63 6f64  ples = msr_encod
+0000e170: 655f 7465 7874 2028 2863 6861 7220 2a29  e_text ((char *)
+0000e180: 7372 632c 206d 6178 7361 6d70 6c65 732c  src, maxsamples,
+0000e190: 2028 6368 6172 202a 2964 6573 742c 206d   (char *)dest, m
+0000e1a0: 6178 6461 7461 6279 7465 7329 3b0a 0a20  axdatabytes);.. 
+0000e1b0: 2020 2069 6620 2862 7974 6573 7772 6974     if (byteswrit
+0000e1c0: 7465 6e20 2626 206e 7361 6d70 6c65 7320  ten && nsamples 
+0000e1d0: 3e20 3029 0a20 2020 2020 202a 6279 7465  > 0).      *byte
+0000e1e0: 7377 7269 7474 656e 203d 2028 7569 6e74  swritten = (uint
+0000e1f0: 3332 5f74 296e 7361 6d70 6c65 733b 0a0a  32_t)nsamples;..
+0000e200: 2020 2020 6272 6561 6b3b 0a0a 2020 6361      break;..  ca
+0000e210: 7365 2044 455f 494e 5431 363a 0a20 2020  se DE_INT16:.   
+0000e220: 2069 6620 2873 616d 706c 6574 7970 6520   if (sampletype 
+0000e230: 213d 2027 6927 290a 2020 2020 7b0a 2020  != 'i').    {.  
+0000e240: 2020 2020 6d73 5f6c 6f67 2028 322c 2022      ms_log (2, "
+0000e250: 2573 3a20 5361 6d70 6c65 2074 7970 6520  %s: Sample type 
+0000e260: 6d75 7374 2062 6520 696e 7465 6765 7220  must be integer 
+0000e270: 2869 2920 666f 7220 494e 5431 3620 656e  (i) for INT16 en
+0000e280: 636f 6469 6e67 206e 6f74 2027 2563 275c  coding not '%c'\
+0000e290: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+0000e2a0: 2020 7369 642c 2073 616d 706c 6574 7970    sid, sampletyp
+0000e2b0: 6529 3b0a 2020 2020 2020 7265 7475 726e  e);.      return
+0000e2c0: 202d 313b 0a20 2020 207d 0a0a 2020 2020   -1;.    }..    
+0000e2d0: 6966 2028 6d61 7864 6174 6162 7974 6573  if (maxdatabytes
+0000e2e0: 203c 2073 697a 656f 6628 696e 7431 365f   < sizeof(int16_
+0000e2f0: 7429 290a 2020 2020 7b0a 2020 2020 2020  t)).    {.      
+0000e300: 6d73 5f6c 6f67 2028 322c 2022 2573 3a20  ms_log (2, "%s: 
+0000e310: 4e6f 7420 656e 6f75 6768 2073 7061 6365  Not enough space
+0000e320: 2069 6e20 7265 636f 7264 2028 2522 2050   in record (%" P
+0000e330: 5249 7536 3420 2229 2066 6f72 2049 4e54  RIu64 ") for INT
+0000e340: 3136 2065 6e63 6f64 696e 672c 206e 6565  16 encoding, nee
+0000e350: 6420 6174 206c 6561 7374 2025 2250 5249  d at least %"PRI
+0000e360: 7369 7a65 5f74 2220 6279 7465 735c 6e22  size_t" bytes\n"
+0000e370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e380: 7369 642c 206d 6178 6461 7461 6279 7465  sid, maxdatabyte
+0000e390: 732c 2073 697a 656f 6628 696e 7431 365f  s, sizeof(int16_
+0000e3a0: 7429 293b 0a20 2020 2020 2072 6574 7572  t));.      retur
+0000e3b0: 6e20 2d31 3b0a 2020 2020 7d0a 0a20 2020  n -1;.    }..   
+0000e3c0: 2069 6620 2876 6572 626f 7365 203e 2031   if (verbose > 1
+0000e3d0: 290a 2020 2020 2020 6d73 5f6c 6f67 2028  ).      ms_log (
+0000e3e0: 302c 2022 2573 3a20 5061 636b 696e 6720  0, "%s: Packing 
+0000e3f0: 494e 5431 3620 6461 7461 2073 616d 706c  INT16 data sampl
+0000e400: 6573 5c6e 222c 2073 6964 293b 0a0a 2020  es\n", sid);..  
+0000e410: 2020 6e73 616d 706c 6573 203d 206d 7372    nsamples = msr
+0000e420: 5f65 6e63 6f64 655f 696e 7431 3620 2828  _encode_int16 ((
+0000e430: 696e 7433 325f 7420 2a29 7372 632c 206d  int32_t *)src, m
+0000e440: 6178 7361 6d70 6c65 732c 2028 696e 7431  axsamples, (int1
+0000e450: 365f 7420 2a29 6465 7374 2c20 6d61 7864  6_t *)dest, maxd
+0000e460: 6174 6162 7974 6573 2c20 7377 6170 666c  atabytes, swapfl
+0000e470: 6167 293b 0a0a 2020 2020 6966 2028 6279  ag);..    if (by
+0000e480: 7465 7377 7269 7474 656e 2026 2620 6e73  teswritten && ns
+0000e490: 616d 706c 6573 203e 2030 290a 2020 2020  amples > 0).    
+0000e4a0: 2020 2a62 7974 6573 7772 6974 7465 6e20    *byteswritten 
+0000e4b0: 3d20 2875 696e 7433 325f 7429 286e 7361  = (uint32_t)(nsa
+0000e4c0: 6d70 6c65 7320 2a20 3229 3b0a 0a20 2020  mples * 2);..   
+0000e4d0: 2062 7265 616b 3b0a 0a20 2063 6173 6520   break;..  case 
+0000e4e0: 4445 5f49 4e54 3332 3a0a 2020 2020 6966  DE_INT32:.    if
+0000e4f0: 2028 7361 6d70 6c65 7479 7065 2021 3d20   (sampletype != 
+0000e500: 2769 2729 0a20 2020 207b 0a20 2020 2020  'i').    {.     
+0000e510: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
+0000e520: 2053 616d 706c 6520 7479 7065 206d 7573   Sample type mus
+0000e530: 7420 6265 2069 6e74 6567 6572 2028 6929  t be integer (i)
+0000e540: 2066 6f72 2049 4e54 3332 2065 6e63 6f64   for INT32 encod
+0000e550: 696e 6720 6e6f 7420 2725 6327 5c6e 222c  ing not '%c'\n",
+0000e560: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
+0000e570: 6964 2c20 7361 6d70 6c65 7479 7065 293b  id, sampletype);
+0000e580: 0a20 2020 2020 2072 6574 7572 6e20 2d31  .      return -1
+0000e590: 3b0a 2020 2020 7d0a 0a20 2020 2069 6620  ;.    }..    if 
+0000e5a0: 286d 6178 6461 7461 6279 7465 7320 3c20  (maxdatabytes < 
+0000e5b0: 7369 7a65 6f66 2869 6e74 3332 5f74 2929  sizeof(int32_t))
+0000e5c0: 0a20 2020 207b 0a20 2020 2020 206d 735f  .    {.      ms_
+0000e5d0: 6c6f 6720 2832 2c20 2225 733a 204e 6f74  log (2, "%s: Not
+0000e5e0: 2065 6e6f 7567 6820 7370 6163 6520 696e   enough space in
+0000e5f0: 2072 6563 6f72 6420 2825 2220 5052 4975   record (%" PRIu
+0000e600: 3634 2022 2920 666f 7220 494e 5433 3220  64 ") for INT32 
+0000e610: 656e 636f 6469 6e67 2c20 6e65 6564 2061  encoding, need a
+0000e620: 7420 6c65 6173 7420 2522 5052 4973 697a  t least %"PRIsiz
+0000e630: 655f 7422 2062 7974 6573 5c6e 222c 0a20  e_t" bytes\n",. 
+0000e640: 2020 2020 2020 2020 2020 2020 2073 6964               sid
+0000e650: 2c20 6d61 7864 6174 6162 7974 6573 2c20  , maxdatabytes, 
+0000e660: 7369 7a65 6f66 2869 6e74 3332 5f74 2929  sizeof(int32_t))
+0000e670: 3b0a 2020 2020 2020 7265 7475 726e 202d  ;.      return -
+0000e680: 313b 0a20 2020 207d 0a0a 2020 2020 6966  1;.    }..    if
+0000e690: 2028 7665 7262 6f73 6520 3e20 3129 0a20   (verbose > 1). 
+0000e6a0: 2020 2020 206d 735f 6c6f 6720 2830 2c20       ms_log (0, 
+0000e6b0: 2225 733a 2050 6163 6b69 6e67 2049 4e54  "%s: Packing INT
+0000e6c0: 3332 2064 6174 6120 7361 6d70 6c65 735c  32 data samples\
+0000e6d0: 6e22 2c20 7369 6429 3b0a 0a20 2020 206e  n", sid);..    n
+0000e6e0: 7361 6d70 6c65 7320 3d20 6d73 725f 656e  samples = msr_en
+0000e6f0: 636f 6465 5f69 6e74 3332 2028 2869 6e74  code_int32 ((int
+0000e700: 3332 5f74 202a 2973 7263 2c20 6d61 7873  32_t *)src, maxs
+0000e710: 616d 706c 6573 2c20 2869 6e74 3332 5f74  amples, (int32_t
+0000e720: 202a 2964 6573 742c 206d 6178 6461 7461   *)dest, maxdata
+0000e730: 6279 7465 732c 2073 7761 7066 6c61 6729  bytes, swapflag)
+0000e740: 3b0a 0a20 2020 2069 6620 2862 7974 6573  ;..    if (bytes
+0000e750: 7772 6974 7465 6e20 2626 206e 7361 6d70  written && nsamp
+0000e760: 6c65 7320 3e20 3029 0a20 2020 2020 202a  les > 0).      *
+0000e770: 6279 7465 7377 7269 7474 656e 203d 2028  byteswritten = (
+0000e780: 7569 6e74 3332 5f74 2928 6e73 616d 706c  uint32_t)(nsampl
+0000e790: 6573 202a 2034 293b 0a0a 2020 2020 6272  es * 4);..    br
+0000e7a0: 6561 6b3b 0a0a 2020 6361 7365 2044 455f  eak;..  case DE_
+0000e7b0: 464c 4f41 5433 323a 0a20 2020 2069 6620  FLOAT32:.    if 
+0000e7c0: 2873 616d 706c 6574 7970 6520 213d 2027  (sampletype != '
+0000e7d0: 6627 290a 2020 2020 7b0a 2020 2020 2020  f').    {.      
+0000e7e0: 6d73 5f6c 6f67 2028 322c 2022 2573 3a20  ms_log (2, "%s: 
+0000e7f0: 5361 6d70 6c65 2074 7970 6520 6d75 7374  Sample type must
+0000e800: 2062 6520 666c 6f61 7420 2866 2920 666f   be float (f) fo
+0000e810: 7220 464c 4f41 5433 3220 656e 636f 6469  r FLOAT32 encodi
+0000e820: 6e67 206e 6f74 2027 2563 275c 6e22 2c0a  ng not '%c'\n",.
+0000e830: 2020 2020 2020 2020 2020 2020 2020 7369                si
+0000e840: 642c 2073 616d 706c 6574 7970 6529 3b0a  d, sampletype);.
+0000e850: 2020 2020 2020 7265 7475 726e 202d 313b        return -1;
+0000e860: 0a20 2020 207d 0a0a 2020 2020 6966 2028  .    }..    if (
+0000e870: 6d61 7864 6174 6162 7974 6573 203c 2073  maxdatabytes < s
+0000e880: 697a 656f 6628 666c 6f61 7429 290a 2020  izeof(float)).  
+0000e890: 2020 7b0a 2020 2020 2020 6d73 5f6c 6f67    {.      ms_log
+0000e8a0: 2028 322c 2022 2573 3a20 4e6f 7420 656e   (2, "%s: Not en
+0000e8b0: 6f75 6768 2073 7061 6365 2069 6e20 7265  ough space in re
+0000e8c0: 636f 7264 2028 2522 2050 5249 7536 3420  cord (%" PRIu64 
+0000e8d0: 2229 2066 6f72 2046 4c4f 4154 3332 2065  ") for FLOAT32 e
+0000e8e0: 6e63 6f64 696e 672c 206e 6565 6420 6174  ncoding, need at
+0000e8f0: 206c 6561 7374 2025 2250 5249 7369 7a65   least %"PRIsize
+0000e900: 5f74 2220 6279 7465 735c 6e22 2c0a 2020  _t" bytes\n",.  
+0000e910: 2020 2020 2020 2020 2020 2020 7369 642c              sid,
+0000e920: 206d 6178 6461 7461 6279 7465 732c 2073   maxdatabytes, s
+0000e930: 697a 656f 6628 666c 6f61 7429 293b 0a20  izeof(float));. 
+0000e940: 2020 2020 2072 6574 7572 6e20 2d31 3b0a       return -1;.
+0000e950: 2020 2020 7d0a 0a20 2020 2069 6620 2876      }..    if (v
+0000e960: 6572 626f 7365 203e 2031 290a 2020 2020  erbose > 1).    
+0000e970: 2020 6d73 5f6c 6f67 2028 302c 2022 2573    ms_log (0, "%s
+0000e980: 3a20 5061 636b 696e 6720 464c 4f41 5433  : Packing FLOAT3
+0000e990: 3220 6461 7461 2073 616d 706c 6573 5c6e  2 data samples\n
+0000e9a0: 222c 2073 6964 293b 0a0a 2020 2020 6e73  ", sid);..    ns
+0000e9b0: 616d 706c 6573 203d 206d 7372 5f65 6e63  amples = msr_enc
+0000e9c0: 6f64 655f 666c 6f61 7433 3220 2828 666c  ode_float32 ((fl
+0000e9d0: 6f61 7420 2a29 7372 632c 206d 6178 7361  oat *)src, maxsa
+0000e9e0: 6d70 6c65 732c 2028 666c 6f61 7420 2a29  mples, (float *)
+0000e9f0: 6465 7374 2c20 6d61 7864 6174 6162 7974  dest, maxdatabyt
+0000ea00: 6573 2c20 7377 6170 666c 6167 293b 0a0a  es, swapflag);..
+0000ea10: 2020 2020 6966 2028 6279 7465 7377 7269      if (byteswri
+0000ea20: 7474 656e 2026 2620 6e73 616d 706c 6573  tten && nsamples
+0000ea30: 203e 2030 290a 2020 2020 2020 2a62 7974   > 0).      *byt
+0000ea40: 6573 7772 6974 7465 6e20 3d20 2875 696e  eswritten = (uin
+0000ea50: 7433 325f 7429 286e 7361 6d70 6c65 7320  t32_t)(nsamples 
+0000ea60: 2a20 3429 3b0a 0a20 2020 2062 7265 616b  * 4);..    break
+0000ea70: 3b0a 0a20 2063 6173 6520 4445 5f46 4c4f  ;..  case DE_FLO
+0000ea80: 4154 3634 3a0a 2020 2020 6966 2028 7361  AT64:.    if (sa
+0000ea90: 6d70 6c65 7479 7065 2021 3d20 2764 2729  mpletype != 'd')
+0000eaa0: 0a20 2020 207b 0a20 2020 2020 206d 735f  .    {.      ms_
+0000eab0: 6c6f 6720 2832 2c20 2225 733a 2053 616d  log (2, "%s: Sam
+0000eac0: 706c 6520 7479 7065 206d 7573 7420 6265  ple type must be
+0000ead0: 2064 6f75 626c 6520 2864 2920 666f 7220   double (d) for 
+0000eae0: 464c 4f41 5436 3420 656e 636f 6469 6e67  FLOAT64 encoding
+0000eaf0: 206e 6f74 2027 2563 275c 6e22 2c0a 2020   not '%c'\n",.  
+0000eb00: 2020 2020 2020 2020 2020 2020 7369 642c              sid,
+0000eb10: 2073 616d 706c 6574 7970 6529 3b0a 2020   sampletype);.  
+0000eb20: 2020 2020 7265 7475 726e 202d 313b 0a20      return -1;. 
+0000eb30: 2020 207d 0a0a 2020 2020 6966 2028 6d61     }..    if (ma
+0000eb40: 7864 6174 6162 7974 6573 203c 2073 697a  xdatabytes < siz
+0000eb50: 656f 6628 646f 7562 6c65 2929 0a20 2020  eof(double)).   
+0000eb60: 207b 0a20 2020 2020 206d 735f 6c6f 6720   {.      ms_log 
+0000eb70: 2832 2c20 2225 733a 204e 6f74 2065 6e6f  (2, "%s: Not eno
+0000eb80: 7567 6820 7370 6163 6520 696e 2072 6563  ugh space in rec
+0000eb90: 6f72 6420 2825 2220 5052 4975 3634 2022  ord (%" PRIu64 "
+0000eba0: 2920 666f 7220 464c 4f41 5436 3420 656e  ) for FLOAT64 en
+0000ebb0: 636f 6469 6e67 2c20 6e65 6564 2061 7420  coding, need at 
+0000ebc0: 6c65 6173 7420 2522 5052 4973 697a 655f  least %"PRIsize_
+0000ebd0: 7422 2062 7974 6573 5c6e 222c 0a20 2020  t" bytes\n",.   
+0000ebe0: 2020 2020 2020 2020 2020 2073 6964 2c20             sid, 
+0000ebf0: 6d61 7864 6174 6162 7974 6573 2c20 7369  maxdatabytes, si
+0000ec00: 7a65 6f66 2864 6f75 626c 6529 293b 0a20  zeof(double));. 
+0000ec10: 2020 2020 2072 6574 7572 6e20 2d31 3b0a       return -1;.
+0000ec20: 2020 2020 7d0a 0a20 2020 2069 6620 2876      }..    if (v
+0000ec30: 6572 626f 7365 203e 2031 290a 2020 2020  erbose > 1).    
+0000ec40: 2020 6d73 5f6c 6f67 2028 302c 2022 2573    ms_log (0, "%s
+0000ec50: 3a20 5061 636b 696e 6720 464c 4f41 5436  : Packing FLOAT6
+0000ec60: 3420 6461 7461 2073 616d 706c 6573 5c6e  4 data samples\n
+0000ec70: 222c 2073 6964 293b 0a0a 2020 2020 6e73  ", sid);..    ns
+0000ec80: 616d 706c 6573 203d 206d 7372 5f65 6e63  amples = msr_enc
+0000ec90: 6f64 655f 666c 6f61 7436 3420 2828 646f  ode_float64 ((do
+0000eca0: 7562 6c65 202a 2973 7263 2c20 6d61 7873  uble *)src, maxs
+0000ecb0: 616d 706c 6573 2c20 2864 6f75 626c 6520  amples, (double 
+0000ecc0: 2a29 6465 7374 2c20 6d61 7864 6174 6162  *)dest, maxdatab
+0000ecd0: 7974 6573 2c20 7377 6170 666c 6167 293b  ytes, swapflag);
+0000ece0: 0a0a 2020 2020 6966 2028 6279 7465 7377  ..    if (bytesw
+0000ecf0: 7269 7474 656e 2026 2620 6e73 616d 706c  ritten && nsampl
+0000ed00: 6573 203e 2030 290a 2020 2020 2020 2a62  es > 0).      *b
+0000ed10: 7974 6573 7772 6974 7465 6e20 3d20 2875  yteswritten = (u
+0000ed20: 696e 7433 325f 7429 286e 7361 6d70 6c65  int32_t)(nsample
+0000ed30: 7320 2a20 3829 3b0a 0a20 2020 2062 7265  s * 8);..    bre
+0000ed40: 616b 3b0a 0a20 2063 6173 6520 4445 5f53  ak;..  case DE_S
+0000ed50: 5445 494d 313a 0a20 2020 2069 6620 2873  TEIM1:.    if (s
+0000ed60: 616d 706c 6574 7970 6520 213d 2027 6927  ampletype != 'i'
+0000ed70: 290a 2020 2020 7b0a 2020 2020 2020 6d73  ).    {.      ms
+0000ed80: 5f6c 6f67 2028 322c 2022 2573 3a20 5361  _log (2, "%s: Sa
+0000ed90: 6d70 6c65 2074 7970 6520 6d75 7374 2062  mple type must b
+0000eda0: 6520 696e 7465 6765 7220 2869 2920 666f  e integer (i) fo
+0000edb0: 7220 5374 6569 6d31 2063 6f6d 7072 6573  r Steim1 compres
+0000edc0: 7369 6f6e 206e 6f74 2027 2563 275c 6e22  sion not '%c'\n"
+0000edd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ede0: 7369 642c 2073 616d 706c 6574 7970 6529  sid, sampletype)
+0000edf0: 3b0a 2020 2020 2020 7265 7475 726e 202d  ;.      return -
+0000ee00: 313b 0a20 2020 207d 0a0a 2020 2020 6966  1;.    }..    if
+0000ee10: 2028 6d61 7864 6174 6162 7974 6573 203c   (maxdatabytes <
+0000ee20: 2036 3429 0a20 2020 207b 0a20 2020 2020   64).    {.     
+0000ee30: 206d 735f 6c6f 6720 2832 2c20 2225 733a   ms_log (2, "%s:
+0000ee40: 204e 6f74 2065 6e6f 7567 6820 7370 6163   Not enough spac
+0000ee50: 6520 696e 2072 6563 6f72 6420 2825 2220  e in record (%" 
+0000ee60: 5052 4975 3634 2022 2920 666f 7220 5354  PRIu64 ") for ST
+0000ee70: 4549 4d31 2065 6e63 6f64 696e 672c 206e  EIM1 encoding, n
+0000ee80: 6565 6420 6174 206c 6561 7374 2036 3420  eed at least 64 
+0000ee90: 6279 7465 735c 6e22 2c0a 2020 2020 2020  bytes\n",.      
+0000eea0: 2020 2020 2020 2020 7369 642c 206d 6178          sid, max
+0000eeb0: 6461 7461 6279 7465 7329 3b0a 2020 2020  databytes);.    
+0000eec0: 2020 7265 7475 726e 202d 313b 0a20 2020    return -1;.   
+0000eed0: 207d 0a0a 2020 2020 6966 2028 7665 7262   }..    if (verb
+0000eee0: 6f73 6520 3e20 3129 0a20 2020 2020 206d  ose > 1).      m
+0000eef0: 735f 6c6f 6720 2830 2c20 2225 733a 2050  s_log (0, "%s: P
+0000ef00: 6163 6b69 6e67 2053 7465 696d 3120 6461  acking Steim1 da
+0000ef10: 7461 2066 7261 6d65 735c 6e22 2c20 7369  ta frames\n", si
+0000ef20: 6429 3b0a 0a20 2020 202f 2a20 416c 7761  d);..    /* Alwa
+0000ef30: 7973 2062 6967 2065 6e64 6961 6e20 5374  ys big endian St
+0000ef40: 6569 6d31 202a 2f0a 2020 2020 7377 6170  eim1 */.    swap
+0000ef50: 666c 6167 203d 2028 6d73 5f62 6967 656e  flag = (ms_bigen
+0000ef60: 6469 616e 686f 7374 2829 2920 3f20 3020  dianhost()) ? 0 
+0000ef70: 3a20 313b 0a0a 2020 2020 6e73 616d 706c  : 1;..    nsampl
+0000ef80: 6573 203d 206d 7372 5f65 6e63 6f64 655f  es = msr_encode_
+0000ef90: 7374 6569 6d31 2028 2869 6e74 3332 5f74  steim1 ((int32_t
+0000efa0: 202a 2973 7263 2c20 6d61 7873 616d 706c   *)src, maxsampl
+0000efb0: 6573 2c20 2869 6e74 3332 5f74 202a 2964  es, (int32_t *)d
+0000efc0: 6573 742c 206d 6178 6461 7461 6279 7465  est, maxdatabyte
+0000efd0: 732c 2030 2c20 6279 7465 7377 7269 7474  s, 0, byteswritt
+0000efe0: 656e 2c20 7377 6170 666c 6167 293b 0a0a  en, swapflag);..
+0000eff0: 2020 2020 6272 6561 6b3b 0a0a 2020 6361      break;..  ca
+0000f000: 7365 2044 455f 5354 4549 4d32 3a0a 2020  se DE_STEIM2:.  
+0000f010: 2020 6966 2028 7361 6d70 6c65 7479 7065    if (sampletype
+0000f020: 2021 3d20 2769 2729 0a20 2020 207b 0a20   != 'i').    {. 
+0000f030: 2020 2020 206d 735f 6c6f 6720 2832 2c20       ms_log (2, 
+0000f040: 2225 733a 2053 616d 706c 6520 7479 7065  "%s: Sample type
+0000f050: 206d 7573 7420 6265 2069 6e74 6567 6572   must be integer
+0000f060: 2028 6929 2066 6f72 2053 7465 696d 3220   (i) for Steim2 
+0000f070: 636f 6d70 7265 7373 696f 6e20 6e6f 7420  compression not 
+0000f080: 2725 6327 5c6e 222c 0a20 2020 2020 2020  '%c'\n",.       
+0000f090: 2020 2020 2020 2073 6964 2c20 7361 6d70         sid, samp
+0000f0a0: 6c65 7479 7065 293b 0a20 2020 2020 2072  letype);.      r
+0000f0b0: 6574 7572 6e20 2d31 3b0a 2020 2020 7d0a  eturn -1;.    }.
+0000f0c0: 0a20 2020 2069 6620 286d 6178 6461 7461  .    if (maxdata
+0000f0d0: 6279 7465 7320 3c20 3634 290a 2020 2020  bytes < 64).    
+0000f0e0: 7b0a 2020 2020 2020 6d73 5f6c 6f67 2028  {.      ms_log (
+0000f0f0: 322c 2022 2573 3a20 4e6f 7420 656e 6f75  2, "%s: Not enou
+0000f100: 6768 2073 7061 6365 2069 6e20 7265 636f  gh space in reco
+0000f110: 7264 2028 2522 2050 5249 7536 3420 2229  rd (%" PRIu64 ")
+0000f120: 2066 6f72 2053 5445 494d 3220 656e 636f   for STEIM2 enco
+0000f130: 6469 6e67 2c20 6e65 6564 2061 7420 6c65  ding, need at le
+0000f140: 6173 7420 3634 2062 7974 6573 5c6e 222c  ast 64 bytes\n",
+0000f150: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
+0000f160: 6964 2c20 6d61 7864 6174 6162 7974 6573  id, maxdatabytes
+0000f170: 293b 0a20 2020 2020 2072 6574 7572 6e20  );.      return 
+0000f180: 2d31 3b0a 2020 2020 7d0a 0a20 2020 2069  -1;.    }..    i
+0000f190: 6620 2876 6572 626f 7365 203e 2031 290a  f (verbose > 1).
+0000f1a0: 2020 2020 2020 6d73 5f6c 6f67 2028 302c        ms_log (0,
+0000f1b0: 2022 2573 3a20 5061 636b 696e 6720 5374   "%s: Packing St
+0000f1c0: 6569 6d32 2064 6174 6120 6672 616d 6573  eim2 data frames
+0000f1d0: 5c6e 222c 2073 6964 293b 0a0a 2020 2020  \n", sid);..    
+0000f1e0: 2f2a 2041 6c77 6179 7320 6269 6720 656e  /* Always big en
+0000f1f0: 6469 616e 2053 7465 696d 3220 2a2f 0a20  dian Steim2 */. 
+0000f200: 2020 2073 7761 7066 6c61 6720 3d20 286d     swapflag = (m
+0000f210: 735f 6269 6765 6e64 6961 6e68 6f73 7428  s_bigendianhost(
+0000f220: 2929 203f 2030 203a 2031 3b0a 0a20 2020  )) ? 0 : 1;..   
+0000f230: 206e 7361 6d70 6c65 7320 3d20 6d73 725f   nsamples = msr_
+0000f240: 656e 636f 6465 5f73 7465 696d 3220 2828  encode_steim2 ((
+0000f250: 696e 7433 325f 7420 2a29 7372 632c 206d  int32_t *)src, m
+0000f260: 6178 7361 6d70 6c65 732c 2028 696e 7433  axsamples, (int3
+0000f270: 325f 7420 2a29 6465 7374 2c20 6d61 7864  2_t *)dest, maxd
+0000f280: 6174 6162 7974 6573 2c20 302c 2062 7974  atabytes, 0, byt
+0000f290: 6573 7772 6974 7465 6e2c 2073 6964 2c20  eswritten, sid, 
+0000f2a0: 7377 6170 666c 6167 293b 0a0a 2020 2020  swapflag);..    
+0000f2b0: 6272 6561 6b3b 0a0a 2020 6465 6661 756c  break;..  defaul
+0000f2c0: 743a 0a20 2020 206d 735f 6c6f 6720 2832  t:.    ms_log (2
+0000f2d0: 2c20 2225 733a 2055 6e61 626c 6520 746f  , "%s: Unable to
+0000f2e0: 2070 6163 6b20 666f 726d 6174 2025 645c   pack format %d\
+0000f2f0: 6e22 2c20 7369 642c 2065 6e63 6f64 696e  n", sid, encodin
+0000f300: 6729 3b0a 0a20 2020 2072 6574 7572 6e20  g);..    return 
+0000f310: 2d31 3b0a 2020 7d0a 0a20 2072 6574 7572  -1;.  }..  retur
+0000f320: 6e20 6e73 616d 706c 6573 3b0a 7d20 2f2a  n nsamples;.} /*
+0000f330: 2045 6e64 206f 6620 6d73 725f 7061 636b   End of msr_pack
+0000f340: 5f64 6174 6128 2920 2a2f 0a0a 2f2a 2a2a  _data() */../***
+0000f350: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 0000f360: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 0000f370: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 0000f380: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f390: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f  ***************/
-0000f3a0: 0a73 7461 7469 6320 696e 740a 6d73 5f72  .static int.ms_r
-0000f3b0: 6174 6170 7072 6f78 2028 646f 7562 6c65  atapprox (double
-0000f3c0: 2072 6561 6c2c 2069 6e74 202a 6e75 6d2c   real, int *num,
-0000f3d0: 2069 6e74 202a 6465 6e2c 2069 6e74 206d   int *den, int m
-0000f3e0: 6178 7661 6c2c 2064 6f75 626c 6520 7072  axval, double pr
-0000f3f0: 6563 6973 696f 6e29 0a7b 0a20 2064 6f75  ecision).{.  dou
-0000f400: 626c 6520 7265 616c 6a2c 2070 7265 616c  ble realj, preal
-0000f410: 3b0a 2020 6368 6172 2070 6f73 3b0a 2020  ;.  char pos;.  
-0000f420: 696e 7420 706e 756d 2c20 7064 656e 3b0a  int pnum, pden;.
-0000f430: 2020 696e 7420 6974 6572 6174 696f 6e73    int iterations
-0000f440: 203d 2031 3b0a 2020 696e 7420 416a 312c   = 1;.  int Aj1,
-0000f450: 2041 6a32 2c20 426a 312c 2042 6a32 3b0a   Aj2, Bj1, Bj2;.
-0000f460: 2020 696e 7420 626a 203d 2030 3b0a 2020    int bj = 0;.  
-0000f470: 696e 7420 416a 203d 2030 3b0a 2020 696e  int Aj = 0;.  in
-0000f480: 7420 426a 203d 2031 3b0a 0a20 2069 6620  t Bj = 1;..  if 
-0000f490: 2872 6561 6c20 3e3d 2030 2e30 290a 2020  (real >= 0.0).  
-0000f4a0: 7b0a 2020 2020 706f 7320 2020 3d20 313b  {.    pos   = 1;
-0000f4b0: 0a20 2020 2072 6561 6c6a 203d 2072 6561  .    realj = rea
-0000f4c0: 6c3b 0a20 207d 0a20 2065 6c73 650a 2020  l;.  }.  else.  
-0000f4d0: 7b0a 2020 2020 706f 7320 2020 3d20 303b  {.    pos   = 0;
-0000f4e0: 0a20 2020 2072 6561 6c6a 203d 202d 7265  .    realj = -re
-0000f4f0: 616c 3b0a 2020 7d0a 0a20 2070 7265 616c  al;.  }..  preal
-0000f500: 203d 2072 6561 6c6a 3b0a 0a20 2062 6a20   = realj;..  bj 
-0000f510: 2020 203d 2028 696e 7429 2872 6561 6c6a     = (int)(realj
-0000f520: 202b 2070 7265 6369 7369 6f6e 293b 0a20   + precision);. 
-0000f530: 2072 6561 6c6a 203d 2031 202f 2028 7265   realj = 1 / (re
-0000f540: 616c 6a20 2d20 626a 293b 0a20 2041 6a20  alj - bj);.  Aj 
-0000f550: 2020 203d 2062 6a3b 0a20 2041 6a31 2020     = bj;.  Aj1  
-0000f560: 203d 2031 3b0a 2020 426a 2020 2020 3d20   = 1;.  Bj    = 
-0000f570: 313b 0a20 2042 6a31 2020 203d 2030 3b0a  1;.  Bj1   = 0;.
-0000f580: 2020 2a6e 756d 203d 2070 6e75 6d20 3d20    *num = pnum = 
-0000f590: 416a 3b0a 2020 2a64 656e 203d 2070 6465  Aj;.  *den = pde
-0000f5a0: 6e20 3d20 426a 3b0a 2020 6966 2028 2170  n = Bj;.  if (!p
-0000f5b0: 6f73 290a 2020 2020 2a6e 756d 203d 202d  os).    *num = -
-0000f5c0: 2a6e 756d 3b0a 0a20 2077 6869 6c65 2028  *num;..  while (
-0000f5d0: 6d73 5f64 6162 7320 2870 7265 616c 202d  ms_dabs (preal -
-0000f5e0: 2028 646f 7562 6c65 2941 6a20 2f20 2864   (double)Aj / (d
-0000f5f0: 6f75 626c 6529 426a 2920 3e20 7072 6563  ouble)Bj) > prec
-0000f600: 6973 696f 6e20 2626 0a20 2020 2020 2020  ision &&.       
-0000f610: 2020 416a 203c 206d 6178 7661 6c20 2626    Aj < maxval &&
-0000f620: 2042 6a20 3c20 6d61 7876 616c 290a 2020   Bj < maxval).  
-0000f630: 7b0a 2020 2020 416a 3220 2020 3d20 416a  {.    Aj2   = Aj
-0000f640: 313b 0a20 2020 2041 6a31 2020 203d 2041  1;.    Aj1   = A
-0000f650: 6a3b 0a20 2020 2042 6a32 2020 203d 2042  j;.    Bj2   = B
-0000f660: 6a31 3b0a 2020 2020 426a 3120 2020 3d20  j1;.    Bj1   = 
-0000f670: 426a 3b0a 2020 2020 626a 2020 2020 3d20  Bj;.    bj    = 
-0000f680: 2869 6e74 2928 7265 616c 6a20 2b20 7072  (int)(realj + pr
-0000f690: 6563 6973 696f 6e29 3b0a 2020 2020 7265  ecision);.    re
-0000f6a0: 616c 6a20 3d20 3120 2f20 2872 6561 6c6a  alj = 1 / (realj
-0000f6b0: 202d 2062 6a29 3b0a 2020 2020 416a 2020   - bj);.    Aj  
-0000f6c0: 2020 3d20 626a 202a 2041 6a31 202b 2041    = bj * Aj1 + A
-0000f6d0: 6a32 3b0a 2020 2020 426a 2020 2020 3d20  j2;.    Bj    = 
-0000f6e0: 626a 202a 2042 6a31 202b 2042 6a32 3b0a  bj * Bj1 + Bj2;.
-0000f6f0: 2020 2020 2a6e 756d 2020 3d20 706e 756d      *num  = pnum
-0000f700: 3b0a 2020 2020 2a64 656e 2020 3d20 7064  ;.    *den  = pd
-0000f710: 656e 3b0a 2020 2020 6966 2028 2170 6f73  en;.    if (!pos
-0000f720: 290a 2020 2020 2020 2a6e 756d 203d 202d  ).      *num = -
-0000f730: 2a6e 756d 3b0a 2020 2020 706e 756d 203d  *num;.    pnum =
-0000f740: 2041 6a3b 0a20 2020 2070 6465 6e20 3d20   Aj;.    pden = 
-0000f750: 426a 3b0a 0a20 2020 2069 7465 7261 7469  Bj;..    iterati
-0000f760: 6f6e 732b 2b3b 0a20 207d 0a0a 2020 6966  ons++;.  }..  if
-0000f770: 2028 706e 756d 203c 206d 6178 7661 6c20   (pnum < maxval 
-0000f780: 2626 2070 6465 6e20 3c20 6d61 7876 616c  && pden < maxval
-0000f790: 290a 2020 7b0a 2020 2020 2a6e 756d 203d  ).  {.    *num =
-0000f7a0: 2070 6e75 6d3b 0a20 2020 202a 6465 6e20   pnum;.    *den 
-0000f7b0: 3d20 7064 656e 3b0a 2020 2020 6966 2028  = pden;.    if (
-0000f7c0: 2170 6f73 290a 2020 2020 2020 2a6e 756d  !pos).      *num
-0000f7d0: 203d 202d 2a6e 756d 3b0a 2020 7d0a 0a20   = -*num;.  }.. 
-0000f7e0: 2072 6574 7572 6e20 6974 6572 6174 696f   return iteratio
-0000f7f0: 6e73 3b0a 7d0a 0a2f 2a2a 2a2a 2a2a 2a2a  ns;.}../********
-0000f800: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f810: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f820: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f830: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000f840: 2a2a 2a0a 202a 206d 735f 7273 7172 7436  ***. * ms_rsqrt6
-0000f850: 343a 0a20 2a0a 202a 2041 6e20 6f70 7469  4:. *. * An opti
-0000f860: 6d69 7a65 6420 7265 6369 7072 6f63 616c  mized reciprocal
-0000f870: 2073 7175 6172 6520 726f 6f74 2063 616c   square root cal
-0000f880: 6375 6c61 7469 6f6e 2066 726f 6d3a 0a20  culation from:. 
-0000f890: 2a20 2020 4d61 7474 6865 7720 526f 6265  *   Matthew Robe
-0000f8a0: 7274 736f 6e20 2832 3031 3229 2e20 2241  rtson (2012). "A
-0000f8b0: 2042 7269 6566 2048 6973 746f 7279 206f   Brief History o
-0000f8c0: 6620 496e 7653 7172 7422 0a20 2a20 2020  f InvSqrt". *   
-0000f8d0: 6874 7470 733a 2f2f 6373 2e75 7761 7465  https://cs.uwate
-0000f8e0: 726c 6f6f 2e63 612f 7e6d 3332 726f 6265  rloo.ca/~m32robe
-0000f8f0: 722f 7273 7172 742e 7064 660a 202a 0a20  r/rsqrt.pdf. *. 
-0000f900: 2a20 4675 7274 6865 7220 7265 6665 7265  * Further refere
-0000f910: 6e63 6520 616e 6420 6465 7363 7269 7074  nce and descript
-0000f920: 696f 6e3a 0a20 2a20 2020 6874 7470 733a  ion:. *   https:
-0000f930: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-0000f940: 7267 2f77 696b 692f 4661 7374 5f69 6e76  rg/wiki/Fast_inv
-0000f950: 6572 7365 5f73 7175 6172 655f 726f 6f74  erse_square_root
-0000f960: 0a20 2a0a 202a 204d 6f64 6966 6963 6174  . *. * Modificat
-0000f970: 696f 6e73 3a0a 202a 2041 6464 2032 206d  ions:. * Add 2 m
-0000f980: 6f72 6520 6974 6572 6174 696f 6e73 206f  ore iterations o
-0000f990: 6620 4e65 7774 6f6e 2773 206d 6574 686f  f Newton's metho
-0000f9a0: 6420 746f 2069 6e63 7265 6173 6520 6163  d to increase ac
-0000f9b0: 6375 7261 6379 2c0a 202a 2073 7065 6369  curacy,. * speci
-0000f9c0: 6669 6361 6c6c 7920 666f 7220 6c61 7267  fically for larg
-0000f9d0: 6520 7661 6c75 6573 2e0a 202a 2055 7365  e values.. * Use
-0000f9e0: 206d 656d 6370 7920 696e 7374 6561 6420   memcpy instead 
-0000f9f0: 6f66 2061 7373 6967 6e6d 656e 7420 7468  of assignment th
-0000fa00: 726f 7567 6820 6469 6666 6572 696e 6720  rough differing 
-0000fa10: 706f 696e 7465 7220 7479 7065 732e 0a20  pointer types.. 
-0000fa20: 2a0a 202a 2052 6574 7572 6e73 2030 2069  *. * Returns 0 i
-0000fa30: 6620 7468 6520 686f 7374 2069 7320 6c69  f the host is li
-0000fa40: 7474 6c65 2065 6e64 6961 6e2c 206f 7468  ttle endian, oth
-0000fa50: 6572 7769 7365 2031 2e0a 202a 2a2a 2a2a  erwise 1.. *****
-0000fa60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fa70: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fa80: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fa90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000faa0: 2a2a 2a2a 2a2a 2f0a 7374 6174 6963 2064  ******/.static d
-0000fab0: 6f75 626c 650a 6d73 5f72 7371 7274 3634  ouble.ms_rsqrt64
-0000fac0: 2028 646f 7562 6c65 2076 616c 290a 7b0a   (double val).{.
-0000fad0: 2020 7569 6e74 3634 5f74 2069 3b0a 2020    uint64_t i;.  
-0000fae0: 646f 7562 6c65 2078 323b 0a20 2064 6f75  double x2;.  dou
-0000faf0: 626c 6520 793b 0a0a 2020 7832 203d 2076  ble y;..  x2 = v
-0000fb00: 616c 202a 2030 2e35 3b0a 2020 7920 203d  al * 0.5;.  y  =
-0000fb10: 2076 616c 3b0a 2020 6d65 6d63 7079 2028   val;.  memcpy (
-0000fb20: 2669 2c20 2679 2c20 7369 7a65 6f66 2028  &i, &y, sizeof (
-0000fb30: 6929 293b 0a20 2069 203d 2030 7835 6665  i));.  i = 0x5fe
-0000fb40: 3665 6235 3063 3762 3533 3761 3955 4c4c  6eb50c7b537a9ULL
-0000fb50: 202d 2028 6920 3e3e 2031 293b 0a20 206d   - (i >> 1);.  m
-0000fb60: 656d 6370 7920 2826 792c 2026 692c 2073  emcpy (&y, &i, s
-0000fb70: 697a 656f 6620 2879 2929 3b0a 2020 7920  izeof (y));.  y 
-0000fb80: 3d20 7920 2a20 2831 2e35 202d 2028 7832  = y * (1.5 - (x2
-0000fb90: 202a 2079 202a 2079 2929 3b0a 2020 7920   * y * y));.  y 
-0000fba0: 3d20 7920 2a20 2831 2e35 202d 2028 7832  = y * (1.5 - (x2
-0000fbb0: 202a 2079 202a 2079 2929 3b0a 2020 7920   * y * y));.  y 
-0000fbc0: 3d20 7920 2a20 2831 2e35 202d 2028 7832  = y * (1.5 - (x2
-0000fbd0: 202a 2079 202a 2079 2929 3b0a 0a20 2072   * y * y));..  r
-0000fbe0: 6574 7572 6e20 793b 0a7d 202f 2a20 456e  eturn y;.} /* En
-0000fbf0: 6420 6f66 206d 735f 7273 7172 7436 3428  d of ms_rsqrt64(
-0000fc00: 2920 2a2f 0a0a 2f2a 2a2a 2a2a 2a2a 2a2a  ) */../*********
+0000f390: 2a2a 2a2a 2a2a 2a2a 0a20 2a20 6d73 5f72  ********. * ms_r
+0000f3a0: 6174 6170 7072 6f78 3a0a 202a 0a20 2a20  atapprox:. *. * 
+0000f3b0: 4669 6e64 2061 6e20 6170 7072 6f78 696d  Find an approxim
+0000f3c0: 6174 6520 7261 7469 6f6e 616c 206e 756d  ate rational num
+0000f3d0: 6265 7220 666f 7220 6120 7265 616c 2074  ber for a real t
+0000f3e0: 6872 6f75 6768 2063 6f6e 7469 6e75 6564  hrough continued
+0000f3f0: 0a20 2a20 6672 6163 7469 6f6e 2065 7870  . * fraction exp
+0000f400: 616e 7369 6f6e 2e20 2047 6976 656e 2061  ansion.  Given a
+0000f410: 2064 6f75 626c 6520 7072 6563 7369 6f6e   double precsion
+0000f420: 2027 7265 616c 2720 6669 6e64 2061 0a20   'real' find a. 
+0000f430: 2a20 6e75 6d65 7261 746f 7220 286e 756d  * numerator (num
+0000f440: 2920 616e 6420 6465 6e6f 6d69 6e61 746f  ) and denominato
+0000f450: 7220 2864 656e 2920 7768 6f73 6520 6162  r (den) whose ab
+0000f460: 736f 6c75 7465 2076 616c 7565 7320 6172  solute values ar
+0000f470: 6520 6e6f 740a 202a 206c 6172 6765 7220  e not. * larger 
+0000f480: 7468 616e 2027 6d61 7876 616c 2720 7768  than 'maxval' wh
+0000f490: 696c 6520 7472 7969 6e67 2074 6f20 7265  ile trying to re
+0000f4a0: 6163 6820 6120 7370 6563 6966 6965 6420  ach a specified 
+0000f4b0: 2770 7265 6369 7369 6f6e 272e 0a20 2a0a  'precision'.. *.
+0000f4c0: 202a 2052 6574 7572 6e73 2074 6865 206e   * Returns the n
+0000f4d0: 756d 6265 7220 6f66 2069 7465 7261 7469  umber of iterati
+0000f4e0: 6f6e 7320 7065 7266 6f72 6d65 642e 0a20  ons performed.. 
+0000f4f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f500: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f510: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f520: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f530: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f 0a73 7461  ***********/.sta
+0000f540: 7469 6320 696e 740a 6d73 5f72 6174 6170  tic int.ms_ratap
+0000f550: 7072 6f78 2028 646f 7562 6c65 2072 6561  prox (double rea
+0000f560: 6c2c 2069 6e74 202a 6e75 6d2c 2069 6e74  l, int *num, int
+0000f570: 202a 6465 6e2c 2069 6e74 206d 6178 7661   *den, int maxva
+0000f580: 6c2c 2064 6f75 626c 6520 7072 6563 6973  l, double precis
+0000f590: 696f 6e29 0a7b 0a20 2064 6f75 626c 6520  ion).{.  double 
+0000f5a0: 7265 616c 6a2c 2070 7265 616c 3b0a 2020  realj, preal;.  
+0000f5b0: 6368 6172 2070 6f73 3b0a 2020 696e 7420  char pos;.  int 
+0000f5c0: 706e 756d 2c20 7064 656e 3b0a 2020 696e  pnum, pden;.  in
+0000f5d0: 7420 6974 6572 6174 696f 6e73 203d 2031  t iterations = 1
+0000f5e0: 3b0a 2020 696e 7420 416a 312c 2041 6a32  ;.  int Aj1, Aj2
+0000f5f0: 2c20 426a 312c 2042 6a32 3b0a 2020 696e  , Bj1, Bj2;.  in
+0000f600: 7420 626a 203d 2030 3b0a 2020 696e 7420  t bj = 0;.  int 
+0000f610: 416a 203d 2030 3b0a 2020 696e 7420 426a  Aj = 0;.  int Bj
+0000f620: 203d 2031 3b0a 0a20 2069 6620 2872 6561   = 1;..  if (rea
+0000f630: 6c20 3e3d 2030 2e30 290a 2020 7b0a 2020  l >= 0.0).  {.  
+0000f640: 2020 706f 7320 2020 3d20 313b 0a20 2020    pos   = 1;.   
+0000f650: 2072 6561 6c6a 203d 2072 6561 6c3b 0a20   realj = real;. 
+0000f660: 207d 0a20 2065 6c73 650a 2020 7b0a 2020   }.  else.  {.  
+0000f670: 2020 706f 7320 2020 3d20 303b 0a20 2020    pos   = 0;.   
+0000f680: 2072 6561 6c6a 203d 202d 7265 616c 3b0a   realj = -real;.
+0000f690: 2020 7d0a 0a20 2070 7265 616c 203d 2072    }..  preal = r
+0000f6a0: 6561 6c6a 3b0a 0a20 2062 6a20 2020 203d  ealj;..  bj    =
+0000f6b0: 2028 696e 7429 2872 6561 6c6a 202b 2070   (int)(realj + p
+0000f6c0: 7265 6369 7369 6f6e 293b 0a20 2072 6561  recision);.  rea
+0000f6d0: 6c6a 203d 2031 202f 2028 7265 616c 6a20  lj = 1 / (realj 
+0000f6e0: 2d20 626a 293b 0a20 2041 6a20 2020 203d  - bj);.  Aj    =
+0000f6f0: 2062 6a3b 0a20 2041 6a31 2020 203d 2031   bj;.  Aj1   = 1
+0000f700: 3b0a 2020 426a 2020 2020 3d20 313b 0a20  ;.  Bj    = 1;. 
+0000f710: 2042 6a31 2020 203d 2030 3b0a 2020 2a6e   Bj1   = 0;.  *n
+0000f720: 756d 203d 2070 6e75 6d20 3d20 416a 3b0a  um = pnum = Aj;.
+0000f730: 2020 2a64 656e 203d 2070 6465 6e20 3d20    *den = pden = 
+0000f740: 426a 3b0a 2020 6966 2028 2170 6f73 290a  Bj;.  if (!pos).
+0000f750: 2020 2020 2a6e 756d 203d 202d 2a6e 756d      *num = -*num
+0000f760: 3b0a 0a20 2077 6869 6c65 2028 6661 6273  ;..  while (fabs
+0000f770: 2028 7072 6561 6c20 2d20 2864 6f75 626c   (preal - (doubl
+0000f780: 6529 416a 202f 2028 646f 7562 6c65 2942  e)Aj / (double)B
+0000f790: 6a29 203e 2070 7265 6369 7369 6f6e 2026  j) > precision &
+0000f7a0: 260a 2020 2020 2020 2020 2041 6a20 3c20  &.         Aj < 
+0000f7b0: 6d61 7876 616c 2026 2620 426a 203c 206d  maxval && Bj < m
+0000f7c0: 6178 7661 6c29 0a20 207b 0a20 2020 2041  axval).  {.    A
+0000f7d0: 6a32 2020 203d 2041 6a31 3b0a 2020 2020  j2   = Aj1;.    
+0000f7e0: 416a 3120 2020 3d20 416a 3b0a 2020 2020  Aj1   = Aj;.    
+0000f7f0: 426a 3220 2020 3d20 426a 313b 0a20 2020  Bj2   = Bj1;.   
+0000f800: 2042 6a31 2020 203d 2042 6a3b 0a20 2020   Bj1   = Bj;.   
+0000f810: 2062 6a20 2020 203d 2028 696e 7429 2872   bj    = (int)(r
+0000f820: 6561 6c6a 202b 2070 7265 6369 7369 6f6e  ealj + precision
+0000f830: 293b 0a20 2020 2072 6561 6c6a 203d 2031  );.    realj = 1
+0000f840: 202f 2028 7265 616c 6a20 2d20 626a 293b   / (realj - bj);
+0000f850: 0a20 2020 2041 6a20 2020 203d 2062 6a20  .    Aj    = bj 
+0000f860: 2a20 416a 3120 2b20 416a 323b 0a20 2020  * Aj1 + Aj2;.   
+0000f870: 2042 6a20 2020 203d 2062 6a20 2a20 426a   Bj    = bj * Bj
+0000f880: 3120 2b20 426a 323b 0a20 2020 202a 6e75  1 + Bj2;.    *nu
+0000f890: 6d20 203d 2070 6e75 6d3b 0a20 2020 202a  m  = pnum;.    *
+0000f8a0: 6465 6e20 203d 2070 6465 6e3b 0a20 2020  den  = pden;.   
+0000f8b0: 2069 6620 2821 706f 7329 0a20 2020 2020   if (!pos).     
+0000f8c0: 202a 6e75 6d20 3d20 2d2a 6e75 6d3b 0a20   *num = -*num;. 
+0000f8d0: 2020 2070 6e75 6d20 3d20 416a 3b0a 2020     pnum = Aj;.  
+0000f8e0: 2020 7064 656e 203d 2042 6a3b 0a0a 2020    pden = Bj;..  
+0000f8f0: 2020 6974 6572 6174 696f 6e73 2b2b 3b0a    iterations++;.
+0000f900: 2020 7d0a 0a20 2069 6620 2870 6e75 6d20    }..  if (pnum 
+0000f910: 3c20 6d61 7876 616c 2026 2620 7064 656e  < maxval && pden
+0000f920: 203c 206d 6178 7661 6c29 0a20 207b 0a20   < maxval).  {. 
+0000f930: 2020 202a 6e75 6d20 3d20 706e 756d 3b0a     *num = pnum;.
+0000f940: 2020 2020 2a64 656e 203d 2070 6465 6e3b      *den = pden;
+0000f950: 0a20 2020 2069 6620 2821 706f 7329 0a20  .    if (!pos). 
+0000f960: 2020 2020 202a 6e75 6d20 3d20 2d2a 6e75       *num = -*nu
+0000f970: 6d3b 0a20 207d 0a0a 2020 7265 7475 726e  m;.  }..  return
+0000f980: 2069 7465 7261 7469 6f6e 733b 0a7d 0a0a   iterations;.}..
+0000f990: 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  /***************
+0000f9a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f9b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f9c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000f9d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a20 2a20  ************. * 
+0000f9e0: 6d73 5f72 7371 7274 3634 3a0a 202a 0a20  ms_rsqrt64:. *. 
+0000f9f0: 2a20 416e 206f 7074 696d 697a 6564 2072  * An optimized r
+0000fa00: 6563 6970 726f 6361 6c20 7371 7561 7265  eciprocal square
+0000fa10: 2072 6f6f 7420 6361 6c63 756c 6174 696f   root calculatio
+0000fa20: 6e20 6672 6f6d 3a0a 202a 2020 204d 6174  n from:. *   Mat
+0000fa30: 7468 6577 2052 6f62 6572 7473 6f6e 2028  thew Robertson (
+0000fa40: 3230 3132 292e 2022 4120 4272 6965 6620  2012). "A Brief 
+0000fa50: 4869 7374 6f72 7920 6f66 2049 6e76 5371  History of InvSq
+0000fa60: 7274 220a 202a 2020 2068 7474 7073 3a2f  rt". *   https:/
+0000fa70: 2f63 732e 7577 6174 6572 6c6f 6f2e 6361  /cs.uwaterloo.ca
+0000fa80: 2f7e 6d33 3272 6f62 6572 2f72 7371 7274  /~m32rober/rsqrt
+0000fa90: 2e70 6466 0a20 2a0a 202a 2046 7572 7468  .pdf. *. * Furth
+0000faa0: 6572 2072 6566 6572 656e 6365 2061 6e64  er reference and
+0000fab0: 2064 6573 6372 6970 7469 6f6e 3a0a 202a   description:. *
+0000fac0: 2020 2068 7474 7073 3a2f 2f65 6e2e 7769     https://en.wi
+0000fad0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+0000fae0: 2f46 6173 745f 696e 7665 7273 655f 7371  /Fast_inverse_sq
+0000faf0: 7561 7265 5f72 6f6f 740a 202a 0a20 2a20  uare_root. *. * 
+0000fb00: 4d6f 6469 6669 6361 7469 6f6e 733a 0a20  Modifications:. 
+0000fb10: 2a20 4164 6420 3220 6d6f 7265 2069 7465  * Add 2 more ite
+0000fb20: 7261 7469 6f6e 7320 6f66 204e 6577 746f  rations of Newto
+0000fb30: 6e27 7320 6d65 7468 6f64 2074 6f20 696e  n's method to in
+0000fb40: 6372 6561 7365 2061 6363 7572 6163 792c  crease accuracy,
+0000fb50: 0a20 2a20 7370 6563 6966 6963 616c 6c79  . * specifically
+0000fb60: 2066 6f72 206c 6172 6765 2076 616c 7565   for large value
+0000fb70: 732e 0a20 2a20 5573 6520 6d65 6d63 7079  s.. * Use memcpy
+0000fb80: 2069 6e73 7465 6164 206f 6620 6173 7369   instead of assi
+0000fb90: 676e 6d65 6e74 2074 6872 6f75 6768 2064  gnment through d
+0000fba0: 6966 6665 7269 6e67 2070 6f69 6e74 6572  iffering pointer
+0000fbb0: 2074 7970 6573 2e0a 202a 0a20 2a20 5265   types.. *. * Re
+0000fbc0: 7475 726e 7320 3020 6966 2074 6865 2068  turns 0 if the h
+0000fbd0: 6f73 7420 6973 206c 6974 746c 6520 656e  ost is little en
+0000fbe0: 6469 616e 2c20 6f74 6865 7277 6973 6520  dian, otherwise 
+0000fbf0: 312e 0a20 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  1.. ************
+0000fc00: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 0000fc10: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 0000fc20: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fc30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fc40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fc50: 2a2a 0a20 2a20 6d73 5f72 6564 7563 655f  **. * ms_reduce_
-0000fc60: 7261 7465 3a0a 202a 0a20 2a20 5265 6475  rate:. *. * Redu
-0000fc70: 6365 2074 6865 2073 7065 6369 6669 6564  ce the specified
-0000fc80: 2073 616d 706c 6520 7261 7465 2069 6e74   sample rate int
-0000fc90: 6f20 7477 6f20 2266 6163 746f 7273 2220  o two "factors" 
-0000fca0: 2869 6e20 736f 6d65 2063 6173 6573 0a20  (in some cases. 
-0000fcb0: 2a20 7468 6520 7365 636f 6e64 2066 6163  * the second fac
-0000fcc0: 746f 7220 6973 2061 6374 7561 6c6c 7920  tor is actually 
-0000fcd0: 6120 6469 7669 736f 7229 2e0a 202a 0a20  a divisor).. *. 
-0000fce0: 2a20 496e 7465 6765 7220 7261 7465 7320  * Integer rates 
-0000fcf0: 6265 7477 6565 6e20 3120 616e 6420 3332  between 1 and 32
-0000fd00: 3736 3720 6361 6e20 6265 2072 6570 7265  767 can be repre
-0000fd10: 7365 6e74 6564 2065 7861 6374 6c79 2e0a  sented exactly..
-0000fd20: 202a 0a20 2a20 496e 7465 6765 7220 7261   *. * Integer ra
-0000fd30: 7465 7320 6869 6768 6572 2074 6861 6e20  tes higher than 
-0000fd40: 3332 3736 3720 7769 6c6c 2062 6520 6d61  32767 will be ma
-0000fd50: 7463 6865 6420 6173 2063 6c6f 7365 6c79  tched as closely
-0000fd60: 2061 730a 202a 2070 6f73 7369 626c 6520   as. * possible 
-0000fd70: 7769 7468 2074 6865 2064 6576 6961 7469  with the deviati
-0000fd80: 6f6e 2062 6563 6f6d 696e 6720 6c61 7267  on becoming larg
-0000fd90: 6572 2061 7320 7468 6520 696e 7465 6765  er as the intege
-0000fda0: 7273 2072 6561 6368 0a20 2a20 2833 3237  rs reach. * (327
-0000fdb0: 3637 202a 2033 3237 3637 292e 0a20 2a0a  67 * 32767).. *.
-0000fdc0: 202a 204e 6f6e 2d69 6e74 6567 6572 2072   * Non-integer r
-0000fdd0: 6174 6573 2062 6574 7765 656e 2033 3237  ates between 327
-0000fde0: 3637 2e30 2061 6e64 2031 2e30 2f33 3237  67.0 and 1.0/327
-0000fdf0: 3637 2e30 2061 7265 2072 6570 7265 7365  67.0 are represe
-0000fe00: 6e74 6564 0a20 2a20 6578 6163 746c 7920  nted. * exactly 
-0000fe10: 7768 656e 2070 6f73 7369 626c 6520 616e  when possible an
-0000fe20: 6420 6170 7072 6f78 696d 6174 6564 206f  d approximated o
-0000fe30: 7468 6572 7769 7365 2e0a 202a 0a20 2a20  therwise.. *. * 
-0000fe40: 4e6f 6e2d 696e 7465 6765 7220 7261 7465  Non-integer rate
-0000fe50: 7320 6772 6561 7465 7220 7468 616e 2033  s greater than 3
-0000fe60: 3237 3637 206f 7220 6c65 7373 2074 6861  2767 or less tha
-0000fe70: 6e20 312f 3332 3736 3720 6172 6520 6e6f  n 1/32767 are no
-0000fe80: 7420 7375 7070 6f72 7465 642e 0a20 2a0a  t supported.. *.
-0000fe90: 202a 2052 6574 7572 6e73 2030 206f 6e20   * Returns 0 on 
-0000fea0: 7375 6363 6573 7320 616e 6420 2d31 206f  success and -1 o
-0000feb0: 6e20 6572 726f 722e 0a20 2a2a 2a2a 2a2a  n error.. ******
-0000fec0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fed0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fee0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000fef0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0000ff00: 2a2a 2a2a 2a2f 0a73 7461 7469 6320 696e  *****/.static in
-0000ff10: 740a 6d73 5f72 6564 7563 655f 7261 7465  t.ms_reduce_rate
-0000ff20: 2028 646f 7562 6c65 2073 616d 7072 6174   (double samprat
-0000ff30: 652c 2069 6e74 3136 5f74 202a 6661 6374  e, int16_t *fact
-0000ff40: 6f72 312c 2069 6e74 3136 5f74 202a 6661  or1, int16_t *fa
-0000ff50: 6374 6f72 3229 0a7b 0a20 2069 6e74 206e  ctor2).{.  int n
-0000ff60: 756d 3b0a 2020 696e 7420 6465 6e3b 0a20  um;.  int den;. 
-0000ff70: 2069 6e74 3332 5f74 2069 6e74 7361 6d70   int32_t intsamp
-0000ff80: 7261 7465 203d 2028 696e 7433 325f 7429  rate = (int32_t)
-0000ff90: 2028 7361 6d70 7261 7465 202b 2030 2e35   (samprate + 0.5
-0000ffa0: 293b 0a0a 2020 696e 7433 325f 7420 7365  );..  int32_t se
-0000ffb0: 6172 6368 6661 6374 6f72 313b 0a20 2069  archfactor1;.  i
-0000ffc0: 6e74 3332 5f74 2073 6561 7263 6866 6163  nt32_t searchfac
-0000ffd0: 746f 7232 3b0a 2020 696e 7433 325f 7420  tor2;.  int32_t 
-0000ffe0: 636c 6f73 6573 7466 6163 746f 723b 0a20  closestfactor;. 
-0000fff0: 2069 6e74 3332 5f74 2063 6c6f 7365 7374   int32_t closest
-00010000: 6469 6666 3b0a 2020 696e 7433 325f 7420  diff;.  int32_t 
-00010010: 6469 6666 3b0a 0a20 202f 2a20 4861 6e64  diff;..  /* Hand
-00010020: 6c65 2063 6173 6520 6f66 2069 6e74 6567  le case of integ
-00010030: 6572 2073 616d 706c 6520 7661 6c75 6573  er sample values
-00010040: 2e20 2a2f 0a20 2069 6620 286d 735f 6461  . */.  if (ms_da
-00010050: 6273 2028 7361 6d70 7261 7465 202d 2069  bs (samprate - i
-00010060: 6e74 7361 6d70 7261 7465 2920 3c20 302e  ntsamprate) < 0.
-00010070: 3030 3030 3030 3129 0a20 207b 0a20 2020  0000001).  {.   
-00010080: 202f 2a20 4966 2069 6e74 6567 6572 2073   /* If integer s
-00010090: 616d 706c 6520 7261 7465 2069 7320 6c65  ample rate is le
-000100a0: 7373 2074 6861 6e20 7261 6e67 6520 6f66  ss than range of
-000100b0: 2031 362d 6269 7420 696e 7420 7365 7420   16-bit int set 
-000100c0: 6974 2064 6972 6563 746c 7920 2a2f 0a20  it directly */. 
-000100d0: 2020 2069 6620 2869 6e74 7361 6d70 7261     if (intsampra
-000100e0: 7465 203c 3d20 3332 3736 3729 0a20 2020  te <= 32767).   
-000100f0: 207b 0a20 2020 2020 202a 6661 6374 6f72   {.      *factor
-00010100: 3120 3d20 696e 7473 616d 7072 6174 653b  1 = intsamprate;
-00010110: 0a20 2020 2020 202a 6661 6374 6f72 3220  .      *factor2 
-00010120: 3d20 313b 0a20 2020 2020 2072 6574 7572  = 1;.      retur
-00010130: 6e20 303b 0a20 2020 207d 0a20 2020 202f  n 0;.    }.    /
-00010140: 2a20 4966 2069 6e74 6567 6572 2073 616d  * If integer sam
-00010150: 706c 6520 7261 7465 2069 7320 7769 7468  ple rate is with
-00010160: 696e 2074 6865 206d 6178 696d 756d 2070  in the maximum p
-00010170: 6f73 7369 626c 6520 6e6f 6d69 6e61 6c20  ossible nominal 
-00010180: 7261 7465 202a 2f0a 2020 2020 656c 7365  rate */.    else
-00010190: 2069 6620 2869 6e74 7361 6d70 7261 7465   if (intsamprate
-000101a0: 203c 3d20 2833 3237 3637 202a 2033 3237   <= (32767 * 327
-000101b0: 3637 2929 0a20 2020 207b 0a20 2020 2020  67)).    {.     
-000101c0: 202f 2a20 4465 7465 726d 696e 6520 7468   /* Determine th
-000101d0: 6520 636c 6f73 6573 7420 6661 6374 6f72  e closest factor
-000101e0: 7320 7468 6174 2072 6570 7265 7365 6e74  s that represent
-000101f0: 2074 6865 2073 616d 706c 6520 7261 7465   the sample rate
-00010200: 2e0a 2020 2020 2020 202a 2054 6865 2061  ..       * The a
-00010210: 7070 726f 7869 6d61 7469 6f6e 2067 6574  pproximation get
-00010220: 7320 776f 7273 6520 6173 2074 6865 2076  s worse as the v
-00010230: 616c 7565 7320 696e 6372 6561 7365 2e20  alues increase. 
-00010240: 2a2f 0a20 2020 2020 2073 6561 7263 6866  */.      searchf
-00010250: 6163 746f 7231 203d 2028 696e 7429 2831  actor1 = (int)(1
-00010260: 2e30 202f 206d 735f 7273 7172 7436 3420  .0 / ms_rsqrt64 
-00010270: 2873 616d 7072 6174 6529 293b 0a20 2020  (samprate));.   
-00010280: 2020 2063 6c6f 7365 7374 6469 6666 2020     closestdiff  
-00010290: 203d 2073 6561 7263 6866 6163 746f 7231   = searchfactor1
-000102a0: 3b0a 2020 2020 2020 636c 6f73 6573 7466  ;.      closestf
-000102b0: 6163 746f 7220 3d20 7365 6172 6368 6661  actor = searchfa
-000102c0: 6374 6f72 313b 0a0a 2020 2020 2020 7768  ctor1;..      wh
-000102d0: 696c 6520 2828 696e 7473 616d 7072 6174  ile ((intsamprat
-000102e0: 6520 2520 7365 6172 6368 6661 6374 6f72  e % searchfactor
-000102f0: 3129 2021 3d20 3029 0a20 2020 2020 207b  1) != 0).      {
-00010300: 0a20 2020 2020 2020 2073 6561 7263 6866  .        searchf
-00010310: 6163 746f 7231 202d 3d20 313b 0a0a 2020  actor1 -= 1;..  
-00010320: 2020 2020 2020 2f2a 2054 7261 636b 2074        /* Track t
-00010330: 6865 2066 6163 746f 7220 7468 6174 2067  he factor that g
-00010340: 656e 6572 6174 6573 2074 6865 2063 6c6f  enerates the clo
-00010350: 7365 7374 206d 6174 6368 202a 2f0a 2020  sest match */.  
-00010360: 2020 2020 2020 7365 6172 6368 6661 6374        searchfact
-00010370: 6f72 3220 3d20 696e 7473 616d 7072 6174  or2 = intsamprat
-00010380: 6520 2f20 7365 6172 6368 6661 6374 6f72  e / searchfactor
-00010390: 313b 0a20 2020 2020 2020 2064 6966 6620  1;.        diff 
-000103a0: 2020 2020 2020 2020 203d 2069 6e74 7361           = intsa
-000103b0: 6d70 7261 7465 202d 2028 7365 6172 6368  mprate - (search
-000103c0: 6661 6374 6f72 3120 2a20 7365 6172 6368  factor1 * search
-000103d0: 6661 6374 6f72 3229 3b0a 2020 2020 2020  factor2);.      
-000103e0: 2020 6966 2028 6469 6666 203c 2063 6c6f    if (diff < clo
-000103f0: 7365 7374 6469 6666 290a 2020 2020 2020  sestdiff).      
-00010400: 2020 7b0a 2020 2020 2020 2020 2020 636c    {.          cl
-00010410: 6f73 6573 7464 6966 6620 2020 3d20 6469  osestdiff   = di
-00010420: 6666 3b0a 2020 2020 2020 2020 2020 636c  ff;.          cl
-00010430: 6f73 6573 7466 6163 746f 7220 3d20 7365  osestfactor = se
-00010440: 6172 6368 6661 6374 6f72 313b 0a20 2020  archfactor1;.   
-00010450: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00010460: 2f2a 2049 6620 7468 6520 6e65 7874 2069  /* If the next i
-00010470: 7465 7261 7469 6f6e 2077 6f75 6c64 2063  teration would c
-00010480: 7265 6174 6520 6120 6661 6374 6f72 2062  reate a factor b
-00010490: 6579 6f6e 6420 7468 6520 6c69 6d69 740a  eyond the limit.
-000104a0: 2020 2020 2020 2020 202a 2077 6520 6163           * we ac
-000104b0: 6365 7074 2074 6865 2063 6c6f 7365 7374  cept the closest
-000104c0: 2066 6163 746f 7220 2a2f 0a20 2020 2020   factor */.     
-000104d0: 2020 2069 6620 2828 696e 7473 616d 7072     if ((intsampr
-000104e0: 6174 6520 2f20 2873 6561 7263 6866 6163  ate / (searchfac
-000104f0: 746f 7231 202d 2031 2929 203e 2033 3237  tor1 - 1)) > 327
-00010500: 3637 290a 2020 2020 2020 2020 7b0a 2020  67).        {.  
-00010510: 2020 2020 2020 2020 7365 6172 6368 6661          searchfa
-00010520: 6374 6f72 3120 3d20 636c 6f73 6573 7466  ctor1 = closestf
-00010530: 6163 746f 723b 0a20 2020 2020 2020 2020  actor;.         
-00010540: 2062 7265 616b 3b0a 2020 2020 2020 2020   break;.        
-00010550: 7d0a 2020 2020 2020 7d0a 0a20 2020 2020  }.      }..     
-00010560: 2073 6561 7263 6866 6163 746f 7232 203d   searchfactor2 =
-00010570: 2069 6e74 7361 6d70 7261 7465 202f 2073   intsamprate / s
-00010580: 6561 7263 6866 6163 746f 7231 3b0a 0a20  earchfactor1;.. 
-00010590: 2020 2020 2069 6620 2873 6561 7263 6866       if (searchf
-000105a0: 6163 746f 7231 203c 3d20 3332 3736 3720  actor1 <= 32767 
-000105b0: 2626 2073 6561 7263 6866 6163 746f 7232  && searchfactor2
-000105c0: 203c 3d20 3332 3736 3729 0a20 2020 2020   <= 32767).     
-000105d0: 207b 0a20 2020 2020 2020 202a 6661 6374   {.        *fact
-000105e0: 6f72 3120 3d20 7365 6172 6368 6661 6374  or1 = searchfact
-000105f0: 6f72 313b 0a20 2020 2020 2020 202a 6661  or1;.        *fa
-00010600: 6374 6f72 3220 3d20 7365 6172 6368 6661  ctor2 = searchfa
-00010610: 6374 6f72 323b 0a20 2020 2020 2020 2072  ctor2;.        r
-00010620: 6574 7572 6e20 303b 0a20 2020 2020 207d  eturn 0;.      }
-00010630: 0a20 2020 207d 0a20 207d 0a20 202f 2a20  .    }.  }.  /* 
-00010640: 4861 6e64 6c65 2063 6173 6520 6f66 206e  Handle case of n
-00010650: 6f6e 2d69 6e74 6567 6572 206c 6573 7320  on-integer less 
-00010660: 7468 616e 2031 362d 6269 7420 696e 7420  than 16-bit int 
-00010670: 7261 6e67 6520 2a2f 0a20 2065 6c73 6520  range */.  else 
-00010680: 6966 2028 7361 6d70 7261 7465 203c 3d20  if (samprate <= 
-00010690: 3332 3736 372e 3029 0a20 207b 0a20 2020  32767.0).  {.   
-000106a0: 202f 2a20 466f 7220 7361 6d70 6c65 732f   /* For samples/
-000106b0: 7365 636f 6e64 732c 2064 6574 6572 6d69  seconds, determi
-000106c0: 6e65 2c20 706f 7465 6e74 6961 6c6c 7920  ne, potentially 
-000106d0: 6170 7072 6f78 696d 6174 652c 206e 756d  approximate, num
-000106e0: 6572 6174 6f72 2061 6e64 2064 656e 6f6d  erator and denom
-000106f0: 6961 746f 7220 2a2f 0a20 2020 206d 735f  iator */.    ms_
-00010700: 7261 7461 7070 726f 7820 2873 616d 7072  ratapprox (sampr
-00010710: 6174 652c 2026 6e75 6d2c 2026 6465 6e2c  ate, &num, &den,
-00010720: 2033 3237 3637 2c20 3165 2d38 293b 0a0a   32767, 1e-8);..
-00010730: 2020 2020 2f2a 204e 6567 6174 6520 7468      /* Negate th
-00010740: 6520 6661 6374 6f72 3220 746f 2064 656e  e factor2 to den
-00010750: 6f74 6520 6120 6469 7669 7369 6f6e 206f  ote a division o
-00010760: 7065 7261 7469 6f6e 202a 2f0a 2020 2020  peration */.    
-00010770: 2a66 6163 746f 7231 203d 2028 696e 7431  *factor1 = (int1
-00010780: 365f 7429 6e75 6d3b 0a20 2020 202a 6661  6_t)num;.    *fa
-00010790: 6374 6f72 3220 3d20 2869 6e74 3136 5f74  ctor2 = (int16_t
-000107a0: 292d 6465 6e3b 0a20 2020 2072 6574 7572  )-den;.    retur
-000107b0: 6e20 303b 0a20 207d 0a0a 2020 7265 7475  n 0;.  }..  retu
-000107c0: 726e 202d 313b 0a7d 202f 2a20 456e 6420  rn -1;.} /* End 
-000107d0: 6f66 206d 735f 7265 6475 6365 5f72 6174  of ms_reduce_rat
-000107e0: 6528 2920 2a2f 0a0a 2f2a 2a2a 2a2a 2a2a  e() */../*******
-000107f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010800: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010810: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010820: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010830: 2a2a 2a2a 0a20 2a20 6d73 5f67 656e 6661  ****. * ms_genfa
-00010840: 6374 6d75 6c74 3a0a 202a 0a20 2a20 4765  ctmult:. *. * Ge
-00010850: 6e65 7261 7465 2061 6e20 6170 7072 6f70  nerate an approp
-00010860: 7269 6174 6520 5345 4544 2073 616d 706c  riate SEED sampl
-00010870: 6520 7261 7465 2066 6163 746f 7220 616e  e rate factor an
-00010880: 6420 6d75 6c74 6970 6c69 6572 2066 726f  d multiplier fro
-00010890: 6d0a 202a 2061 2064 6f75 626c 6520 7072  m. * a double pr
-000108a0: 6563 6973 696f 6e20 7361 6d70 6c65 2072  ecision sample r
-000108b0: 6174 652e 0a20 2a0a 202a 2049 6620 7468  ate.. *. * If th
-000108c0: 6520 7361 6d70 6c65 7261 7465 203e 2030  e samplerate > 0
-000108d0: 2e30 2069 7420 6973 2065 7870 6563 7465  .0 it is expecte
-000108e0: 6420 746f 2062 6520 6120 7261 7465 2069  d to be a rate i
-000108f0: 6e20 5341 4d50 4c45 532f 5345 434f 4e44  n SAMPLES/SECOND
-00010900: 2e0a 202a 2049 6620 7468 6520 7361 6d70  .. * If the samp
-00010910: 6c65 7261 7465 203c 2030 2e30 2069 7420  lerate < 0.0 it 
-00010920: 6973 2065 7870 6563 7465 6420 746f 2062  is expected to b
-00010930: 6520 6120 7065 7269 6f64 2069 6e20 5345  e a period in SE
-00010940: 434f 4e44 532f 5341 4d50 4c45 2e0a 202a  CONDS/SAMPLE.. *
-00010950: 0a20 2a20 5265 7375 6c74 7320 7573 6520  . * Results use 
-00010960: 5341 4d50 4c45 532f 5345 434f 4e44 206e  SAMPLES/SECOND n
-00010970: 6f74 6174 696f 6e20 7768 656e 2073 616d  otation when sam
-00010980: 706c 6520 7261 7465 203e 3d20 312e 300a  ple rate >= 1.0.
-00010990: 202a 2052 6573 756c 7473 2075 7365 2053   * Results use S
-000109a0: 4543 4f4e 4453 2f53 414d 504c 4520 6e6f  ECONDS/SAMPLE no
-000109b0: 7461 7469 6f6e 2077 6865 6e20 7361 6d6c  tation when saml
-000109c0: 6573 2072 6174 6573 203c 2031 2e30 0a20  es rates < 1.0. 
-000109d0: 2a0a 202a 2052 6574 7572 6e73 2030 206f  *. * Returns 0 o
-000109e0: 6e20 7375 6363 6573 7320 616e 6420 2d31  n success and -1
-000109f0: 206f 6e20 6572 726f 7220 6f72 2063 616c   on error or cal
-00010a00: 6375 6c61 7469 6f6e 206e 6f74 2070 6f73  culation not pos
-00010a10: 7369 626c 652e 0a20 2a2a 2a2a 2a2a 2a2a  sible.. ********
-00010a20: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010a30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010a40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010a50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010a60: 2a2a 2a2f 0a73 7461 7469 6320 696e 740a  ***/.static int.
-00010a70: 6d73 5f67 656e 6661 6374 6d75 6c74 2028  ms_genfactmult (
-00010a80: 646f 7562 6c65 2073 616d 7072 6174 652c  double samprate,
-00010a90: 2069 6e74 3136 5f74 202a 6661 6374 6f72   int16_t *factor
-00010aa0: 2c20 696e 7431 365f 7420 2a6d 756c 7469  , int16_t *multi
-00010ab0: 706c 6965 7229 0a7b 0a20 2069 6e74 3136  plier).{.  int16
-00010ac0: 5f74 2066 6163 746f 7231 3b0a 2020 696e  _t factor1;.  in
-00010ad0: 7431 365f 7420 6661 6374 6f72 323b 0a0a  t16_t factor2;..
-00010ae0: 2020 6966 2028 2166 6163 746f 7220 7c7c    if (!factor ||
-00010af0: 2021 6d75 6c74 6970 6c69 6572 290a 2020   !multiplier).  
-00010b00: 2020 7265 7475 726e 202d 313b 0a0a 2020    return -1;..  
-00010b10: 2f2a 2043 6f6e 7665 7274 2073 616d 706c  /* Convert sampl
-00010b20: 6520 7065 7269 6f64 2074 6f20 7361 6d70  e period to samp
-00010b30: 6c65 2072 6174 6520 2a2f 0a20 2069 6620  le rate */.  if 
-00010b40: 2873 616d 7072 6174 6520 3c20 302e 3029  (samprate < 0.0)
-00010b50: 0a20 2020 2073 616d 7072 6174 6520 3d20  .    samprate = 
-00010b60: 2d31 2e30 202f 2073 616d 7072 6174 653b  -1.0 / samprate;
-00010b70: 0a0a 2020 2f2a 2048 616e 646c 6520 7370  ..  /* Handle sp
-00010b80: 6563 6961 6c20 6361 7365 206f 6620 7a65  ecial case of ze
-00010b90: 726f 202a 2f0a 2020 6966 2028 7361 6d70  ro */.  if (samp
-00010ba0: 7261 7465 203d 3d20 302e 3029 0a20 207b  rate == 0.0).  {
-00010bb0: 0a20 2020 202a 6661 6374 6f72 2020 2020  .    *factor    
-00010bc0: 203d 2030 3b0a 2020 2020 2a6d 756c 7469   = 0;.    *multi
-00010bd0: 706c 6965 7220 3d20 303b 0a20 2020 2072  plier = 0;.    r
-00010be0: 6574 7572 6e20 303b 0a20 207d 0a20 202f  eturn 0;.  }.  /
-00010bf0: 2a20 4861 6e64 6c65 2073 616d 706c 6520  * Handle sample 
-00010c00: 7261 7465 7320 3e3d 2031 2e30 2077 6974  rates >= 1.0 wit
-00010c10: 6820 7468 6520 5341 4d50 4c45 532f 5345  h the SAMPLES/SE
-00010c20: 434f 4e44 2072 6570 7265 7365 6e74 6174  COND representat
-00010c30: 696f 6e20 2a2f 0a20 2065 6c73 6520 6966  ion */.  else if
-00010c40: 2028 7361 6d70 7261 7465 203e 3d20 312e   (samprate >= 1.
-00010c50: 3029 0a20 207b 0a20 2020 2069 6620 286d  0).  {.    if (m
-00010c60: 735f 7265 6475 6365 5f72 6174 6520 2873  s_reduce_rate (s
-00010c70: 616d 7072 6174 652c 2026 6661 6374 6f72  amprate, &factor
-00010c80: 312c 2026 6661 6374 6f72 3229 203d 3d20  1, &factor2) == 
-00010c90: 3029 0a20 2020 207b 0a20 2020 2020 202a  0).    {.      *
-00010ca0: 6661 6374 6f72 2020 2020 203d 2066 6163  factor     = fac
-00010cb0: 746f 7231 3b0a 2020 2020 2020 2a6d 756c  tor1;.      *mul
-00010cc0: 7469 706c 6965 7220 3d20 6661 6374 6f72  tiplier = factor
-00010cd0: 323b 0a20 2020 2020 2072 6574 7572 6e20  2;.      return 
-00010ce0: 303b 0a20 2020 207d 0a20 207d 0a20 202f  0;.    }.  }.  /
-00010cf0: 2a20 4861 6e64 6c65 2073 616d 706c 6520  * Handle sample 
-00010d00: 7261 7465 7320 3c20 3120 7769 7468 2074  rates < 1 with t
-00010d10: 6865 2053 4543 4f4e 4453 2f53 414d 504c  he SECONDS/SAMPL
-00010d20: 4520 7265 7072 6573 656e 7461 7469 6f6e  E representation
-00010d30: 202a 2f0a 2020 656c 7365 0a20 207b 0a20   */.  else.  {. 
-00010d40: 2020 202f 2a20 5265 6475 6365 2072 6174     /* Reduce rat
-00010d50: 6520 6173 2061 2073 616d 706c 6520 7065  e as a sample pe
-00010d60: 7269 6f64 2061 6e64 2069 6e76 6572 7420  riod and invert 
-00010d70: 6661 6374 6f72 2f6d 756c 7469 706c 6965  factor/multiplie
-00010d80: 7220 2a2f 0a20 2020 2069 6620 286d 735f  r */.    if (ms_
-00010d90: 7265 6475 6365 5f72 6174 6520 2831 2e30  reduce_rate (1.0
-00010da0: 202f 2073 616d 7072 6174 652c 2026 6661   / samprate, &fa
-00010db0: 6374 6f72 312c 2026 6661 6374 6f72 3229  ctor1, &factor2)
-00010dc0: 203d 3d20 3029 0a20 2020 207b 0a20 2020   == 0).    {.   
-00010dd0: 2020 202a 6661 6374 6f72 2020 2020 203d     *factor     =
-00010de0: 202d 6661 6374 6f72 313b 0a20 2020 2020   -factor1;.     
-00010df0: 202a 6d75 6c74 6970 6c69 6572 203d 202d   *multiplier = -
-00010e00: 6661 6374 6f72 323b 0a20 2020 2020 2072  factor2;.      r
-00010e10: 6574 7572 6e20 303b 0a20 2020 207d 0a20  eturn 0;.    }. 
-00010e20: 207d 0a0a 2020 7265 7475 726e 202d 313b   }..  return -1;
-00010e30: 0a7d 202f 2a20 456e 6420 6f66 206d 735f  .} /* End of ms_
-00010e40: 6765 6e66 6163 746d 756c 7428 2920 2a2f  genfactmult() */
-00010e50: 0a0a 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ../*************
-00010e60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e70: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e80: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a20  **************. 
-00010ea0: 2a20 436f 6e76 656e 6965 6e63 6520 6675  * Convenience fu
-00010eb0: 6e63 7469 6f6e 2074 6f20 636f 6e76 6572  nction to conver
-00010ec0: 7420 6120 6d6f 6e74 682d 6461 7920 7469  t a month-day ti
-00010ed0: 6d65 2073 7472 696e 6720 746f 2061 2053  me string to a S
-00010ee0: 4545 440a 202a 2032 2e78 2022 4254 494d  EED. * 2.x "BTIM
-00010ef0: 4522 2073 7472 7563 7475 7265 2e0a 202a  E" structure.. *
-00010f00: 0a20 2a20 5468 6520 3130 2d62 7974 6520  . * The 10-byte 
-00010f10: 4254 494d 4520 7374 7275 6374 7572 6520  BTIME structure 
-00010f20: 6c61 796f 7574 3a0a 202a 0a20 2a20 5661  layout:. *. * Va
-00010f30: 6c75 6520 2054 7970 6520 2020 2020 204f  lue  Type      O
-00010f40: 6666 7365 7420 2044 6573 6372 6970 7469  ffset  Descripti
-00010f50: 6f6e 0a20 2a20 7965 6172 2020 2075 696e  on. * year   uin
-00010f60: 7431 365f 7420 2030 2020 2020 2020 2046  t16_t  0       F
-00010f70: 6f75 7220 6469 6769 7420 7965 6172 2028  our digit year (
-00010f80: 652e 672e 2031 3938 3729 0a20 2a20 6461  e.g. 1987). * da
-00010f90: 7920 2020 2075 696e 7431 365f 7420 2032  y    uint16_t  2
-00010fa0: 2020 2020 2020 2044 6179 206f 6620 7965         Day of ye
-00010fb0: 6172 2028 4a61 6e20 3173 7420 6973 2031  ar (Jan 1st is 1
-00010fc0: 290a 202a 2068 6f75 7220 2020 7569 6e74  ). * hour   uint
-00010fd0: 385f 7420 2020 3420 2020 2020 2020 486f  8_t   4       Ho
-00010fe0: 7572 2028 3020 2d20 3233 290a 202a 206d  ur (0 - 23). * m
-00010ff0: 696e 2020 2020 7569 6e74 385f 7420 2020  in    uint8_t   
-00011000: 3520 2020 2020 2020 4d69 6e75 7465 2028  5       Minute (
-00011010: 3020 2d20 3539 290a 202a 2073 6563 2020  0 - 59). * sec  
-00011020: 2020 7569 6e74 385f 7420 2020 3620 2020    uint8_t   6   
-00011030: 2020 2020 5365 636f 6e64 2028 3020 2d20      Second (0 - 
-00011040: 3539 2c20 3630 2066 6f72 206c 6561 7020  59, 60 for leap 
-00011050: 7365 636f 6e64 7329 0a20 2a20 756e 7573  seconds). * unus
-00011060: 6564 2075 696e 7438 5f74 2020 2037 2020  ed uint8_t   7  
-00011070: 2020 2020 2055 6e75 7365 642c 2069 6e63       Unused, inc
-00011080: 6c75 6465 6420 666f 7220 616c 6967 6e6d  luded for alignm
-00011090: 656e 740a 202a 2066 7261 6374 2020 7569  ent. * fract  ui
-000110a0: 6e74 3136 5f74 2020 3820 2020 2020 2020  nt16_t  8       
-000110b0: 302e 3030 3031 2073 6563 6f6e 6473 2c20  0.0001 seconds, 
-000110c0: 692e 652e 2031 2f31 3074 6873 206f 6620  i.e. 1/10ths of 
-000110d0: 6d69 6c6c 6973 6563 6f6e 6473 2028 30e2  milliseconds (0.
-000110e0: 8094 3939 3939 290a 202a 0a20 2a20 5265  ..9999). *. * Re
-000110f0: 7475 726e 206e 616e 6f73 6563 6f6e 6473  turn nanoseconds
-00011100: 206f 6e20 7375 6363 6573 7320 616e 6420   on success and 
-00011110: 2d31 206f 6e20 6572 726f 722e 0a20 2a0a  -1 on error.. *.
-00011120: 202a 205c 7265 6620 4d65 7373 6167 654f   * \ref MessageO
-00011130: 6e45 7272 6f72 202d 2074 6869 7320 6675  nError - this fu
-00011140: 6e63 7469 6f6e 206c 6f67 7320 6120 6d65  nction logs a me
-00011150: 7373 6167 6520 6f6e 2065 7272 6f72 0a20  ssage on error. 
-00011160: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00011170: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00011180: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00011190: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000111a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f 0a73 7461  ***********/.sta
-000111b0: 7469 6320 696e 6c69 6e65 2069 6e74 3634  tic inline int64
-000111c0: 5f74 0a6d 735f 7469 6d65 7374 7232 6274  _t.ms_timestr2bt
-000111d0: 696d 6520 2863 6f6e 7374 2063 6861 7220  ime (const char 
-000111e0: 2a74 696d 6573 7472 2c20 7569 6e74 385f  *timestr, uint8_
-000111f0: 7420 2a62 7469 6d65 2c20 636f 6e73 7420  t *btime, const 
-00011200: 6368 6172 202a 7369 642c 2069 6e74 385f  char *sid, int8_
-00011210: 7420 7377 6170 666c 6167 290a 7b0a 2020  t swapflag).{.  
-00011220: 7569 6e74 3136 5f74 2079 6561 723b 0a20  uint16_t year;. 
-00011230: 2075 696e 7431 365f 7420 6461 793b 0a20   uint16_t day;. 
-00011240: 2075 696e 7438 5f74 2068 6f75 723b 0a20   uint8_t hour;. 
-00011250: 2075 696e 7438 5f74 206d 696e 3b0a 2020   uint8_t min;.  
-00011260: 7569 6e74 385f 7420 7365 633b 0a20 2075  uint8_t sec;.  u
-00011270: 696e 7433 325f 7420 6e73 6563 3b0a 2020  int32_t nsec;.  
-00011280: 6e73 7469 6d65 5f74 206e 7374 696d 653b  nstime_t nstime;
-00011290: 0a0a 2020 6966 2028 2174 696d 6573 7472  ..  if (!timestr
-000112a0: 207c 7c20 2162 7469 6d65 290a 2020 7b0a   || !btime).  {.
-000112b0: 2020 2020 6d73 5f6c 6f67 2028 322c 2022      ms_log (2, "
-000112c0: 2573 2825 7329 3a20 5265 7175 6972 6564  %s(%s): Required
-000112d0: 2069 6e70 7574 206e 6f74 2064 6566 696e   input not defin
-000112e0: 6564 3a20 2774 696d 6573 7472 2720 6f72  ed: 'timestr' or
-000112f0: 2027 6274 696d 6527 5c6e 222c 0a20 2020   'btime'\n",.   
-00011300: 2020 2020 2020 2020 2073 6964 2c20 5f5f           sid, __
-00011310: 6675 6e63 5f5f 293b 0a20 2020 2072 6574  func__);.    ret
-00011320: 7572 6e20 2d31 3b0a 2020 7d0a 0a20 2069  urn -1;.  }..  i
-00011330: 6620 2828 6e73 7469 6d65 203d 206d 735f  f ((nstime = ms_
-00011340: 7469 6d65 7374 7232 6e73 7469 6d65 2028  timestr2nstime (
-00011350: 7469 6d65 7374 7229 2920 3d3d 204e 5354  timestr)) == NST
-00011360: 4552 524f 5229 0a20 2020 2072 6574 7572  ERROR).    retur
-00011370: 6e20 2d31 3b0a 0a20 2069 6620 286d 735f  n -1;..  if (ms_
-00011380: 6e73 7469 6d65 3274 696d 6520 286e 7374  nstime2time (nst
-00011390: 696d 652c 2026 7965 6172 2c20 2664 6179  ime, &year, &day
-000113a0: 2c20 2668 6f75 722c 2026 6d69 6e2c 2026  , &hour, &min, &
-000113b0: 7365 632c 2026 6e73 6563 2929 0a20 2020  sec, &nsec)).   
-000113c0: 2072 6574 7572 6e20 2d31 3b0a 0a20 202a   return -1;..  *
-000113d0: 2828 7569 6e74 3136 5f74 202a 2928 6274  ((uint16_t *)(bt
-000113e0: 696d 6529 2920 2020 2020 3d20 484f 3275  ime))     = HO2u
-000113f0: 2028 7965 6172 2c20 7377 6170 666c 6167   (year, swapflag
-00011400: 293b 0a20 202a 2828 7569 6e74 3136 5f74  );.  *((uint16_t
-00011410: 202a 2928 6274 696d 6520 2b20 3229 2920   *)(btime + 2)) 
-00011420: 3d20 484f 3275 2028 6461 792c 2073 7761  = HO2u (day, swa
-00011430: 7066 6c61 6729 3b0a 2020 2a28 2875 696e  pflag);.  *((uin
-00011440: 7438 5f74 202a 2928 6274 696d 6520 2b20  t8_t *)(btime + 
-00011450: 3429 2920 203d 2068 6f75 723b 0a20 202a  4))  = hour;.  *
-00011460: 2828 7569 6e74 385f 7420 2a29 2862 7469  ((uint8_t *)(bti
-00011470: 6d65 202b 2035 2929 2020 3d20 6d69 6e3b  me + 5))  = min;
-00011480: 0a20 202a 2828 7569 6e74 385f 7420 2a29  .  *((uint8_t *)
-00011490: 2862 7469 6d65 202b 2036 2929 2020 3d20  (btime + 6))  = 
-000114a0: 7365 633b 0a20 202a 2828 7569 6e74 385f  sec;.  *((uint8_
-000114b0: 7420 2a29 2862 7469 6d65 202b 2037 2929  t *)(btime + 7))
-000114c0: 2020 3d20 303b 0a20 202a 2828 7569 6e74    = 0;.  *((uint
-000114d0: 3136 5f74 202a 2928 6274 696d 6520 2b20  16_t *)(btime + 
-000114e0: 3829 2920 3d20 484f 3275 2028 6e73 6563  8)) = HO2u (nsec
-000114f0: 202f 2031 3030 3030 302c 2073 7761 7066   / 100000, swapf
-00011500: 6c61 6729 3b0a 0a20 2072 6574 7572 6e20  lag);..  return 
-00011510: 6e73 6563 3b0a 7d20 2f2a 2045 6e64 206f  nsec;.} /* End o
-00011520: 6620 7469 6d65 7374 7232 6274 696d 6528  f timestr2btime(
-00011530: 2920 2a2f 0a                             ) */.
+0000fc30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f  ***************/
+0000fc40: 0a73 7461 7469 6320 646f 7562 6c65 0a6d  .static double.m
+0000fc50: 735f 7273 7172 7436 3420 2864 6f75 626c  s_rsqrt64 (doubl
+0000fc60: 6520 7661 6c29 0a7b 0a20 2075 696e 7436  e val).{.  uint6
+0000fc70: 345f 7420 693b 0a20 2064 6f75 626c 6520  4_t i;.  double 
+0000fc80: 7832 3b0a 2020 646f 7562 6c65 2079 3b0a  x2;.  double y;.
+0000fc90: 0a20 2078 3220 3d20 7661 6c20 2a20 302e  .  x2 = val * 0.
+0000fca0: 353b 0a20 2079 2020 3d20 7661 6c3b 0a20  5;.  y  = val;. 
+0000fcb0: 206d 656d 6370 7920 2826 692c 2026 792c   memcpy (&i, &y,
+0000fcc0: 2073 697a 656f 6620 2869 2929 3b0a 2020   sizeof (i));.  
+0000fcd0: 6920 3d20 3078 3566 6536 6562 3530 6337  i = 0x5fe6eb50c7
+0000fce0: 6235 3337 6139 554c 4c20 2d20 2869 203e  b537a9ULL - (i >
+0000fcf0: 3e20 3129 3b0a 2020 6d65 6d63 7079 2028  > 1);.  memcpy (
+0000fd00: 2679 2c20 2669 2c20 7369 7a65 6f66 2028  &y, &i, sizeof (
+0000fd10: 7929 293b 0a20 2079 203d 2079 202a 2028  y));.  y = y * (
+0000fd20: 312e 3520 2d20 2878 3220 2a20 7920 2a20  1.5 - (x2 * y * 
+0000fd30: 7929 293b 0a20 2079 203d 2079 202a 2028  y));.  y = y * (
+0000fd40: 312e 3520 2d20 2878 3220 2a20 7920 2a20  1.5 - (x2 * y * 
+0000fd50: 7929 293b 0a20 2079 203d 2079 202a 2028  y));.  y = y * (
+0000fd60: 312e 3520 2d20 2878 3220 2a20 7920 2a20  1.5 - (x2 * y * 
+0000fd70: 7929 293b 0a0a 2020 7265 7475 726e 2079  y));..  return y
+0000fd80: 3b0a 7d20 2f2a 2045 6e64 206f 6620 6d73  ;.} /* End of ms
+0000fd90: 5f72 7371 7274 3634 2829 202a 2f0a 0a2f  _rsqrt64() */../
+0000fda0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000fdb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000fdc0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000fdd0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0000fde0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 202a 206d  ***********. * m
+0000fdf0: 735f 7265 6475 6365 5f72 6174 653a 0a20  s_reduce_rate:. 
+0000fe00: 2a0a 202a 2052 6564 7563 6520 7468 6520  *. * Reduce the 
+0000fe10: 7370 6563 6966 6965 6420 7361 6d70 6c65  specified sample
+0000fe20: 2072 6174 6520 696e 746f 2074 776f 2022   rate into two "
+0000fe30: 6661 6374 6f72 7322 2028 696e 2073 6f6d  factors" (in som
+0000fe40: 6520 6361 7365 730a 202a 2074 6865 2073  e cases. * the s
+0000fe50: 6563 6f6e 6420 6661 6374 6f72 2069 7320  econd factor is 
+0000fe60: 6163 7475 616c 6c79 2061 2064 6976 6973  actually a divis
+0000fe70: 6f72 292e 0a20 2a0a 202a 2049 6e74 6567  or).. *. * Integ
+0000fe80: 6572 2072 6174 6573 2062 6574 7765 656e  er rates between
+0000fe90: 2031 2061 6e64 2033 3237 3637 2063 616e   1 and 32767 can
+0000fea0: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
+0000feb0: 6578 6163 746c 792e 0a20 2a0a 202a 2049  exactly.. *. * I
+0000fec0: 6e74 6567 6572 2072 6174 6573 2068 6967  nteger rates hig
+0000fed0: 6865 7220 7468 616e 2033 3237 3637 2077  her than 32767 w
+0000fee0: 696c 6c20 6265 206d 6174 6368 6564 2061  ill be matched a
+0000fef0: 7320 636c 6f73 656c 7920 6173 0a20 2a20  s closely as. * 
+0000ff00: 706f 7373 6962 6c65 2077 6974 6820 7468  possible with th
+0000ff10: 6520 6465 7669 6174 696f 6e20 6265 636f  e deviation beco
+0000ff20: 6d69 6e67 206c 6172 6765 7220 6173 2074  ming larger as t
+0000ff30: 6865 2069 6e74 6567 6572 7320 7265 6163  he integers reac
+0000ff40: 680a 202a 2028 3332 3736 3720 2a20 3332  h. * (32767 * 32
+0000ff50: 3736 3729 2e0a 202a 0a20 2a20 4e6f 6e2d  767).. *. * Non-
+0000ff60: 696e 7465 6765 7220 7261 7465 7320 6265  integer rates be
+0000ff70: 7477 6565 6e20 3332 3736 372e 3020 616e  tween 32767.0 an
+0000ff80: 6420 312e 302f 3332 3736 372e 3020 6172  d 1.0/32767.0 ar
+0000ff90: 6520 7265 7072 6573 656e 7465 640a 202a  e represented. *
+0000ffa0: 2065 7861 6374 6c79 2077 6865 6e20 706f   exactly when po
+0000ffb0: 7373 6962 6c65 2061 6e64 2061 7070 726f  ssible and appro
+0000ffc0: 7869 6d61 7465 6420 6f74 6865 7277 6973  ximated otherwis
+0000ffd0: 652e 0a20 2a0a 202a 204e 6f6e 2d69 6e74  e.. *. * Non-int
+0000ffe0: 6567 6572 2072 6174 6573 2067 7265 6174  eger rates great
+0000fff0: 6572 2074 6861 6e20 3332 3736 3720 6f72  er than 32767 or
+00010000: 206c 6573 7320 7468 616e 2031 2f33 3237   less than 1/327
+00010010: 3637 2061 7265 206e 6f74 2073 7570 706f  67 are not suppo
+00010020: 7274 6564 2e0a 202a 0a20 2a20 5265 7475  rted.. *. * Retu
+00010030: 726e 7320 3020 6f6e 2073 7563 6365 7373  rns 0 on success
+00010040: 2061 6e64 202d 3120 6f6e 2065 7272 6f72   and -1 on error
+00010050: 2e0a 202a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  .. *************
+00010060: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010070: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010080: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010090: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2f0a  **************/.
+000100a0: 7374 6174 6963 2069 6e74 0a6d 735f 7265  static int.ms_re
+000100b0: 6475 6365 5f72 6174 6520 2864 6f75 626c  duce_rate (doubl
+000100c0: 6520 7361 6d70 7261 7465 2c20 696e 7431  e samprate, int1
+000100d0: 365f 7420 2a66 6163 746f 7231 2c20 696e  6_t *factor1, in
+000100e0: 7431 365f 7420 2a66 6163 746f 7232 290a  t16_t *factor2).
+000100f0: 7b0a 2020 696e 7420 6e75 6d3b 0a20 2069  {.  int num;.  i
+00010100: 6e74 2064 656e 3b0a 2020 696e 7433 325f  nt den;.  int32_
+00010110: 7420 696e 7473 616d 7072 6174 6520 3d20  t intsamprate = 
+00010120: 2869 6e74 3332 5f74 2920 2873 616d 7072  (int32_t) (sampr
+00010130: 6174 6520 2b20 302e 3529 3b0a 0a20 2069  ate + 0.5);..  i
+00010140: 6e74 3332 5f74 2073 6561 7263 6866 6163  nt32_t searchfac
+00010150: 746f 7231 3b0a 2020 696e 7433 325f 7420  tor1;.  int32_t 
+00010160: 7365 6172 6368 6661 6374 6f72 323b 0a20  searchfactor2;. 
+00010170: 2069 6e74 3332 5f74 2063 6c6f 7365 7374   int32_t closest
+00010180: 6661 6374 6f72 3b0a 2020 696e 7433 325f  factor;.  int32_
+00010190: 7420 636c 6f73 6573 7464 6966 663b 0a20  t closestdiff;. 
+000101a0: 2069 6e74 3332 5f74 2064 6966 663b 0a0a   int32_t diff;..
+000101b0: 2020 2f2a 2048 616e 646c 6520 6361 7365    /* Handle case
+000101c0: 206f 6620 696e 7465 6765 7220 7361 6d70   of integer samp
+000101d0: 6c65 2076 616c 7565 732e 202a 2f0a 2020  le values. */.  
+000101e0: 6966 2028 6661 6273 2028 7361 6d70 7261  if (fabs (sampra
+000101f0: 7465 202d 2069 6e74 7361 6d70 7261 7465  te - intsamprate
+00010200: 2920 3c20 302e 3030 3030 3030 3129 0a20  ) < 0.0000001). 
+00010210: 207b 0a20 2020 202f 2a20 4966 2069 6e74   {.    /* If int
+00010220: 6567 6572 2073 616d 706c 6520 7261 7465  eger sample rate
+00010230: 2069 7320 6c65 7373 2074 6861 6e20 7261   is less than ra
+00010240: 6e67 6520 6f66 2031 362d 6269 7420 696e  nge of 16-bit in
+00010250: 7420 7365 7420 6974 2064 6972 6563 746c  t set it directl
+00010260: 7920 2a2f 0a20 2020 2069 6620 2869 6e74  y */.    if (int
+00010270: 7361 6d70 7261 7465 203c 3d20 3332 3736  samprate <= 3276
+00010280: 3729 0a20 2020 207b 0a20 2020 2020 202a  7).    {.      *
+00010290: 6661 6374 6f72 3120 3d20 696e 7473 616d  factor1 = intsam
+000102a0: 7072 6174 653b 0a20 2020 2020 202a 6661  prate;.      *fa
+000102b0: 6374 6f72 3220 3d20 313b 0a20 2020 2020  ctor2 = 1;.     
+000102c0: 2072 6574 7572 6e20 303b 0a20 2020 207d   return 0;.    }
+000102d0: 0a20 2020 202f 2a20 4966 2069 6e74 6567  .    /* If integ
+000102e0: 6572 2073 616d 706c 6520 7261 7465 2069  er sample rate i
+000102f0: 7320 7769 7468 696e 2074 6865 206d 6178  s within the max
+00010300: 696d 756d 2070 6f73 7369 626c 6520 6e6f  imum possible no
+00010310: 6d69 6e61 6c20 7261 7465 202a 2f0a 2020  minal rate */.  
+00010320: 2020 656c 7365 2069 6620 2869 6e74 7361    else if (intsa
+00010330: 6d70 7261 7465 203c 3d20 2833 3237 3637  mprate <= (32767
+00010340: 202a 2033 3237 3637 2929 0a20 2020 207b   * 32767)).    {
+00010350: 0a20 2020 2020 202f 2a20 4465 7465 726d  .      /* Determ
+00010360: 696e 6520 7468 6520 636c 6f73 6573 7420  ine the closest 
+00010370: 6661 6374 6f72 7320 7468 6174 2072 6570  factors that rep
+00010380: 7265 7365 6e74 2074 6865 2073 616d 706c  resent the sampl
+00010390: 6520 7261 7465 2e0a 2020 2020 2020 202a  e rate..       *
+000103a0: 2054 6865 2061 7070 726f 7869 6d61 7469   The approximati
+000103b0: 6f6e 2067 6574 7320 776f 7273 6520 6173  on gets worse as
+000103c0: 2074 6865 2076 616c 7565 7320 696e 6372   the values incr
+000103d0: 6561 7365 2e20 2a2f 0a20 2020 2020 2073  ease. */.      s
+000103e0: 6561 7263 6866 6163 746f 7231 203d 2028  earchfactor1 = (
+000103f0: 696e 7429 2831 2e30 202f 206d 735f 7273  int)(1.0 / ms_rs
+00010400: 7172 7436 3420 2873 616d 7072 6174 6529  qrt64 (samprate)
+00010410: 293b 0a20 2020 2020 2063 6c6f 7365 7374  );.      closest
+00010420: 6469 6666 2020 203d 2073 6561 7263 6866  diff   = searchf
+00010430: 6163 746f 7231 3b0a 2020 2020 2020 636c  actor1;.      cl
+00010440: 6f73 6573 7466 6163 746f 7220 3d20 7365  osestfactor = se
+00010450: 6172 6368 6661 6374 6f72 313b 0a0a 2020  archfactor1;..  
+00010460: 2020 2020 7768 696c 6520 2828 696e 7473      while ((ints
+00010470: 616d 7072 6174 6520 2520 7365 6172 6368  amprate % search
+00010480: 6661 6374 6f72 3129 2021 3d20 3029 0a20  factor1) != 0). 
+00010490: 2020 2020 207b 0a20 2020 2020 2020 2073       {.        s
+000104a0: 6561 7263 6866 6163 746f 7231 202d 3d20  earchfactor1 -= 
+000104b0: 313b 0a0a 2020 2020 2020 2020 2f2a 2054  1;..        /* T
+000104c0: 7261 636b 2074 6865 2066 6163 746f 7220  rack the factor 
+000104d0: 7468 6174 2067 656e 6572 6174 6573 2074  that generates t
+000104e0: 6865 2063 6c6f 7365 7374 206d 6174 6368  he closest match
+000104f0: 202a 2f0a 2020 2020 2020 2020 7365 6172   */.        sear
+00010500: 6368 6661 6374 6f72 3220 3d20 696e 7473  chfactor2 = ints
+00010510: 616d 7072 6174 6520 2f20 7365 6172 6368  amprate / search
+00010520: 6661 6374 6f72 313b 0a20 2020 2020 2020  factor1;.       
+00010530: 2064 6966 6620 2020 2020 2020 2020 203d   diff          =
+00010540: 2069 6e74 7361 6d70 7261 7465 202d 2028   intsamprate - (
+00010550: 7365 6172 6368 6661 6374 6f72 3120 2a20  searchfactor1 * 
+00010560: 7365 6172 6368 6661 6374 6f72 3229 3b0a  searchfactor2);.
+00010570: 2020 2020 2020 2020 6966 2028 6469 6666          if (diff
+00010580: 203c 2063 6c6f 7365 7374 6469 6666 290a   < closestdiff).
+00010590: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000105a0: 2020 2020 636c 6f73 6573 7464 6966 6620      closestdiff 
+000105b0: 2020 3d20 6469 6666 3b0a 2020 2020 2020    = diff;.      
+000105c0: 2020 2020 636c 6f73 6573 7466 6163 746f      closestfacto
+000105d0: 7220 3d20 7365 6172 6368 6661 6374 6f72  r = searchfactor
+000105e0: 313b 0a20 2020 2020 2020 207d 0a0a 2020  1;.        }..  
+000105f0: 2020 2020 2020 2f2a 2049 6620 7468 6520        /* If the 
+00010600: 6e65 7874 2069 7465 7261 7469 6f6e 2077  next iteration w
+00010610: 6f75 6c64 2063 7265 6174 6520 6120 6661  ould create a fa
+00010620: 6374 6f72 2062 6579 6f6e 6420 7468 6520  ctor beyond the 
+00010630: 6c69 6d69 740a 2020 2020 2020 2020 202a  limit.         *
+00010640: 2077 6520 6163 6365 7074 2074 6865 2063   we accept the c
+00010650: 6c6f 7365 7374 2066 6163 746f 7220 2a2f  losest factor */
+00010660: 0a20 2020 2020 2020 2069 6620 2828 696e  .        if ((in
+00010670: 7473 616d 7072 6174 6520 2f20 2873 6561  tsamprate / (sea
+00010680: 7263 6866 6163 746f 7231 202d 2031 2929  rchfactor1 - 1))
+00010690: 203e 2033 3237 3637 290a 2020 2020 2020   > 32767).      
+000106a0: 2020 7b0a 2020 2020 2020 2020 2020 7365    {.          se
+000106b0: 6172 6368 6661 6374 6f72 3120 3d20 636c  archfactor1 = cl
+000106c0: 6f73 6573 7466 6163 746f 723b 0a20 2020  osestfactor;.   
+000106d0: 2020 2020 2020 2062 7265 616b 3b0a 2020         break;.  
+000106e0: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+000106f0: 0a20 2020 2020 2073 6561 7263 6866 6163  .      searchfac
+00010700: 746f 7232 203d 2069 6e74 7361 6d70 7261  tor2 = intsampra
+00010710: 7465 202f 2073 6561 7263 6866 6163 746f  te / searchfacto
+00010720: 7231 3b0a 0a20 2020 2020 2069 6620 2873  r1;..      if (s
+00010730: 6561 7263 6866 6163 746f 7231 203c 3d20  earchfactor1 <= 
+00010740: 3332 3736 3720 2626 2073 6561 7263 6866  32767 && searchf
+00010750: 6163 746f 7232 203c 3d20 3332 3736 3729  actor2 <= 32767)
+00010760: 0a20 2020 2020 207b 0a20 2020 2020 2020  .      {.       
+00010770: 202a 6661 6374 6f72 3120 3d20 7365 6172   *factor1 = sear
+00010780: 6368 6661 6374 6f72 313b 0a20 2020 2020  chfactor1;.     
+00010790: 2020 202a 6661 6374 6f72 3220 3d20 7365     *factor2 = se
+000107a0: 6172 6368 6661 6374 6f72 323b 0a20 2020  archfactor2;.   
+000107b0: 2020 2020 2072 6574 7572 6e20 303b 0a20       return 0;. 
+000107c0: 2020 2020 207d 0a20 2020 207d 0a20 207d       }.    }.  }
+000107d0: 0a20 202f 2a20 4861 6e64 6c65 2063 6173  .  /* Handle cas
+000107e0: 6520 6f66 206e 6f6e 2d69 6e74 6567 6572  e of non-integer
+000107f0: 206c 6573 7320 7468 616e 2031 362d 6269   less than 16-bi
+00010800: 7420 696e 7420 7261 6e67 6520 2a2f 0a20  t int range */. 
+00010810: 2065 6c73 6520 6966 2028 7361 6d70 7261   else if (sampra
+00010820: 7465 203c 3d20 3332 3736 372e 3029 0a20  te <= 32767.0). 
+00010830: 207b 0a20 2020 202f 2a20 466f 7220 7361   {.    /* For sa
+00010840: 6d70 6c65 732f 7365 636f 6e64 732c 2064  mples/seconds, d
+00010850: 6574 6572 6d69 6e65 2c20 706f 7465 6e74  etermine, potent
+00010860: 6961 6c6c 7920 6170 7072 6f78 696d 6174  ially approximat
+00010870: 652c 206e 756d 6572 6174 6f72 2061 6e64  e, numerator and
+00010880: 2064 656e 6f6d 6961 746f 7220 2a2f 0a20   denomiator */. 
+00010890: 2020 206d 735f 7261 7461 7070 726f 7820     ms_ratapprox 
+000108a0: 2873 616d 7072 6174 652c 2026 6e75 6d2c  (samprate, &num,
+000108b0: 2026 6465 6e2c 2033 3237 3637 2c20 3165   &den, 32767, 1e
+000108c0: 2d38 293b 0a0a 2020 2020 2f2a 204e 6567  -8);..    /* Neg
+000108d0: 6174 6520 7468 6520 6661 6374 6f72 3220  ate the factor2 
+000108e0: 746f 2064 656e 6f74 6520 6120 6469 7669  to denote a divi
+000108f0: 7369 6f6e 206f 7065 7261 7469 6f6e 202a  sion operation *
+00010900: 2f0a 2020 2020 2a66 6163 746f 7231 203d  /.    *factor1 =
+00010910: 2028 696e 7431 365f 7429 6e75 6d3b 0a20   (int16_t)num;. 
+00010920: 2020 202a 6661 6374 6f72 3220 3d20 2869     *factor2 = (i
+00010930: 6e74 3136 5f74 292d 6465 6e3b 0a20 2020  nt16_t)-den;.   
+00010940: 2072 6574 7572 6e20 303b 0a20 207d 0a0a   return 0;.  }..
+00010950: 2020 7265 7475 726e 202d 313b 0a7d 202f    return -1;.} /
+00010960: 2a20 456e 6420 6f66 206d 735f 7265 6475  * End of ms_redu
+00010970: 6365 5f72 6174 6528 2920 2a2f 0a0a 2f2a  ce_rate() */../*
+00010980: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010990: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000109a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000109b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000109c0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a20 2a20 6d73  **********. * ms
+000109d0: 5f67 656e 6661 6374 6d75 6c74 3a0a 202a  _genfactmult:. *
+000109e0: 0a20 2a20 4765 6e65 7261 7465 2061 6e20  . * Generate an 
+000109f0: 6170 7072 6f70 7269 6174 6520 5345 4544  appropriate SEED
+00010a00: 2073 616d 706c 6520 7261 7465 2066 6163   sample rate fac
+00010a10: 746f 7220 616e 6420 6d75 6c74 6970 6c69  tor and multipli
+00010a20: 6572 2066 726f 6d0a 202a 2061 2064 6f75  er from. * a dou
+00010a30: 626c 6520 7072 6563 6973 696f 6e20 7361  ble precision sa
+00010a40: 6d70 6c65 2072 6174 652e 0a20 2a0a 202a  mple rate.. *. *
+00010a50: 2049 6620 7468 6520 7361 6d70 6c65 7261   If the samplera
+00010a60: 7465 203e 2030 2e30 2069 7420 6973 2065  te > 0.0 it is e
+00010a70: 7870 6563 7465 6420 746f 2062 6520 6120  xpected to be a 
+00010a80: 7261 7465 2069 6e20 5341 4d50 4c45 532f  rate in SAMPLES/
+00010a90: 5345 434f 4e44 2e0a 202a 2049 6620 7468  SECOND.. * If th
+00010aa0: 6520 7361 6d70 6c65 7261 7465 203c 2030  e samplerate < 0
+00010ab0: 2e30 2069 7420 6973 2065 7870 6563 7465  .0 it is expecte
+00010ac0: 6420 746f 2062 6520 6120 7065 7269 6f64  d to be a period
+00010ad0: 2069 6e20 5345 434f 4e44 532f 5341 4d50   in SECONDS/SAMP
+00010ae0: 4c45 2e0a 202a 0a20 2a20 5265 7375 6c74  LE.. *. * Result
+00010af0: 7320 7573 6520 5341 4d50 4c45 532f 5345  s use SAMPLES/SE
+00010b00: 434f 4e44 206e 6f74 6174 696f 6e20 7768  COND notation wh
+00010b10: 656e 2073 616d 706c 6520 7261 7465 203e  en sample rate >
+00010b20: 3d20 312e 300a 202a 2052 6573 756c 7473  = 1.0. * Results
+00010b30: 2075 7365 2053 4543 4f4e 4453 2f53 414d   use SECONDS/SAM
+00010b40: 504c 4520 6e6f 7461 7469 6f6e 2077 6865  PLE notation whe
+00010b50: 6e20 7361 6d6c 6573 2072 6174 6573 203c  n samles rates <
+00010b60: 2031 2e30 0a20 2a0a 202a 2052 6574 7572   1.0. *. * Retur
+00010b70: 6e73 2030 206f 6e20 7375 6363 6573 7320  ns 0 on success 
+00010b80: 616e 6420 2d31 206f 6e20 6572 726f 7220  and -1 on error 
+00010b90: 6f72 2063 616c 6375 6c61 7469 6f6e 206e  or calculation n
+00010ba0: 6f74 2070 6f73 7369 626c 652e 0a20 2a2a  ot possible.. **
+00010bb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010bc0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010bd0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010be0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010bf0: 2a2a 2a2a 2a2a 2a2a 2a2f 0a73 7461 7469  *********/.stati
+00010c00: 6320 696e 740a 6d73 5f67 656e 6661 6374  c int.ms_genfact
+00010c10: 6d75 6c74 2028 646f 7562 6c65 2073 616d  mult (double sam
+00010c20: 7072 6174 652c 2069 6e74 3136 5f74 202a  prate, int16_t *
+00010c30: 6661 6374 6f72 2c20 696e 7431 365f 7420  factor, int16_t 
+00010c40: 2a6d 756c 7469 706c 6965 7229 0a7b 0a20  *multiplier).{. 
+00010c50: 2069 6e74 3136 5f74 2066 6163 746f 7231   int16_t factor1
+00010c60: 3b0a 2020 696e 7431 365f 7420 6661 6374  ;.  int16_t fact
+00010c70: 6f72 323b 0a0a 2020 6966 2028 2166 6163  or2;..  if (!fac
+00010c80: 746f 7220 7c7c 2021 6d75 6c74 6970 6c69  tor || !multipli
+00010c90: 6572 290a 2020 2020 7265 7475 726e 202d  er).    return -
+00010ca0: 313b 0a0a 2020 2f2a 2043 6f6e 7665 7274  1;..  /* Convert
+00010cb0: 2073 616d 706c 6520 7065 7269 6f64 2074   sample period t
+00010cc0: 6f20 7361 6d70 6c65 2072 6174 6520 2a2f  o sample rate */
+00010cd0: 0a20 2069 6620 2873 616d 7072 6174 6520  .  if (samprate 
+00010ce0: 3c20 302e 3029 0a20 2020 2073 616d 7072  < 0.0).    sampr
+00010cf0: 6174 6520 3d20 2d31 2e30 202f 2073 616d  ate = -1.0 / sam
+00010d00: 7072 6174 653b 0a0a 2020 2f2a 2048 616e  prate;..  /* Han
+00010d10: 646c 6520 7370 6563 6961 6c20 6361 7365  dle special case
+00010d20: 206f 6620 7a65 726f 202a 2f0a 2020 6966   of zero */.  if
+00010d30: 2028 7361 6d70 7261 7465 203d 3d20 302e   (samprate == 0.
+00010d40: 3029 0a20 207b 0a20 2020 202a 6661 6374  0).  {.    *fact
+00010d50: 6f72 2020 2020 203d 2030 3b0a 2020 2020  or     = 0;.    
+00010d60: 2a6d 756c 7469 706c 6965 7220 3d20 303b  *multiplier = 0;
+00010d70: 0a20 2020 2072 6574 7572 6e20 303b 0a20  .    return 0;. 
+00010d80: 207d 0a20 202f 2a20 4861 6e64 6c65 2073   }.  /* Handle s
+00010d90: 616d 706c 6520 7261 7465 7320 3e3d 2031  ample rates >= 1
+00010da0: 2e30 2077 6974 6820 7468 6520 5341 4d50  .0 with the SAMP
+00010db0: 4c45 532f 5345 434f 4e44 2072 6570 7265  LES/SECOND repre
+00010dc0: 7365 6e74 6174 696f 6e20 2a2f 0a20 2065  sentation */.  e
+00010dd0: 6c73 6520 6966 2028 7361 6d70 7261 7465  lse if (samprate
+00010de0: 203e 3d20 312e 3029 0a20 207b 0a20 2020   >= 1.0).  {.   
+00010df0: 2069 6620 286d 735f 7265 6475 6365 5f72   if (ms_reduce_r
+00010e00: 6174 6520 2873 616d 7072 6174 652c 2026  ate (samprate, &
+00010e10: 6661 6374 6f72 312c 2026 6661 6374 6f72  factor1, &factor
+00010e20: 3229 203d 3d20 3029 0a20 2020 207b 0a20  2) == 0).    {. 
+00010e30: 2020 2020 202a 6661 6374 6f72 2020 2020       *factor    
+00010e40: 203d 2066 6163 746f 7231 3b0a 2020 2020   = factor1;.    
+00010e50: 2020 2a6d 756c 7469 706c 6965 7220 3d20    *multiplier = 
+00010e60: 6661 6374 6f72 323b 0a20 2020 2020 2072  factor2;.      r
+00010e70: 6574 7572 6e20 303b 0a20 2020 207d 0a20  eturn 0;.    }. 
+00010e80: 207d 0a20 202f 2a20 4861 6e64 6c65 2073   }.  /* Handle s
+00010e90: 616d 706c 6520 7261 7465 7320 3c20 3120  ample rates < 1 
+00010ea0: 7769 7468 2074 6865 2053 4543 4f4e 4453  with the SECONDS
+00010eb0: 2f53 414d 504c 4520 7265 7072 6573 656e  /SAMPLE represen
+00010ec0: 7461 7469 6f6e 202a 2f0a 2020 656c 7365  tation */.  else
+00010ed0: 0a20 207b 0a20 2020 202f 2a20 5265 6475  .  {.    /* Redu
+00010ee0: 6365 2072 6174 6520 6173 2061 2073 616d  ce rate as a sam
+00010ef0: 706c 6520 7065 7269 6f64 2061 6e64 2069  ple period and i
+00010f00: 6e76 6572 7420 6661 6374 6f72 2f6d 756c  nvert factor/mul
+00010f10: 7469 706c 6965 7220 2a2f 0a20 2020 2069  tiplier */.    i
+00010f20: 6620 286d 735f 7265 6475 6365 5f72 6174  f (ms_reduce_rat
+00010f30: 6520 2831 2e30 202f 2073 616d 7072 6174  e (1.0 / samprat
+00010f40: 652c 2026 6661 6374 6f72 312c 2026 6661  e, &factor1, &fa
+00010f50: 6374 6f72 3229 203d 3d20 3029 0a20 2020  ctor2) == 0).   
+00010f60: 207b 0a20 2020 2020 202a 6661 6374 6f72   {.      *factor
+00010f70: 2020 2020 203d 202d 6661 6374 6f72 313b       = -factor1;
+00010f80: 0a20 2020 2020 202a 6d75 6c74 6970 6c69  .      *multipli
+00010f90: 6572 203d 202d 6661 6374 6f72 323b 0a20  er = -factor2;. 
+00010fa0: 2020 2020 2072 6574 7572 6e20 303b 0a20       return 0;. 
+00010fb0: 2020 207d 0a20 207d 0a0a 2020 7265 7475     }.  }..  retu
+00010fc0: 726e 202d 313b 0a7d 202f 2a20 456e 6420  rn -1;.} /* End 
+00010fd0: 6f66 206d 735f 6765 6e66 6163 746d 756c  of ms_genfactmul
+00010fe0: 7428 2920 2a2f 0a0a 2f2a 2a2a 2a2a 2a2a  t() */../*******
+00010ff0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011000: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011010: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011020: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011030: 2a2a 2a2a 0a20 2a20 436f 6e76 656e 6965  ****. * Convenie
+00011040: 6e63 6520 6675 6e63 7469 6f6e 2074 6f20  nce function to 
+00011050: 636f 6e76 6572 7420 6120 6d6f 6e74 682d  convert a month-
+00011060: 6461 7920 7469 6d65 2073 7472 696e 6720  day time string 
+00011070: 746f 2061 2053 4545 440a 202a 2032 2e78  to a SEED. * 2.x
+00011080: 2022 4254 494d 4522 2073 7472 7563 7475   "BTIME" structu
+00011090: 7265 2e0a 202a 0a20 2a20 5468 6520 3130  re.. *. * The 10
+000110a0: 2d62 7974 6520 4254 494d 4520 7374 7275  -byte BTIME stru
+000110b0: 6374 7572 6520 6c61 796f 7574 3a0a 202a  cture layout:. *
+000110c0: 0a20 2a20 5661 6c75 6520 2054 7970 6520  . * Value  Type 
+000110d0: 2020 2020 204f 6666 7365 7420 2044 6573       Offset  Des
+000110e0: 6372 6970 7469 6f6e 0a20 2a20 7965 6172  cription. * year
+000110f0: 2020 2075 696e 7431 365f 7420 2030 2020     uint16_t  0  
+00011100: 2020 2020 2046 6f75 7220 6469 6769 7420       Four digit 
+00011110: 7965 6172 2028 652e 672e 2031 3938 3729  year (e.g. 1987)
+00011120: 0a20 2a20 6461 7920 2020 2075 696e 7431  . * day    uint1
+00011130: 365f 7420 2032 2020 2020 2020 2044 6179  6_t  2       Day
+00011140: 206f 6620 7965 6172 2028 4a61 6e20 3173   of year (Jan 1s
+00011150: 7420 6973 2031 290a 202a 2068 6f75 7220  t is 1). * hour 
+00011160: 2020 7569 6e74 385f 7420 2020 3420 2020    uint8_t   4   
+00011170: 2020 2020 486f 7572 2028 3020 2d20 3233      Hour (0 - 23
+00011180: 290a 202a 206d 696e 2020 2020 7569 6e74  ). * min    uint
+00011190: 385f 7420 2020 3520 2020 2020 2020 4d69  8_t   5       Mi
+000111a0: 6e75 7465 2028 3020 2d20 3539 290a 202a  nute (0 - 59). *
+000111b0: 2073 6563 2020 2020 7569 6e74 385f 7420   sec    uint8_t 
+000111c0: 2020 3620 2020 2020 2020 5365 636f 6e64    6       Second
+000111d0: 2028 3020 2d20 3539 2c20 3630 2066 6f72   (0 - 59, 60 for
+000111e0: 206c 6561 7020 7365 636f 6e64 7329 0a20   leap seconds). 
+000111f0: 2a20 756e 7573 6564 2075 696e 7438 5f74  * unused uint8_t
+00011200: 2020 2037 2020 2020 2020 2055 6e75 7365     7       Unuse
+00011210: 642c 2069 6e63 6c75 6465 6420 666f 7220  d, included for 
+00011220: 616c 6967 6e6d 656e 740a 202a 2066 7261  alignment. * fra
+00011230: 6374 2020 7569 6e74 3136 5f74 2020 3820  ct  uint16_t  8 
+00011240: 2020 2020 2020 302e 3030 3031 2073 6563        0.0001 sec
+00011250: 6f6e 6473 2c20 692e 652e 2031 2f31 3074  onds, i.e. 1/10t
+00011260: 6873 206f 6620 6d69 6c6c 6973 6563 6f6e  hs of millisecon
+00011270: 6473 2028 30e2 8094 3939 3939 290a 202a  ds (0...9999). *
+00011280: 0a20 2a20 5265 7475 726e 206e 616e 6f73  . * Return nanos
+00011290: 6563 6f6e 6473 206f 6e20 7375 6363 6573  econds on succes
+000112a0: 7320 616e 6420 2d31 206f 6e20 6572 726f  s and -1 on erro
+000112b0: 722e 0a20 2a0a 202a 205c 7265 6620 4d65  r.. *. * \ref Me
+000112c0: 7373 6167 654f 6e45 7272 6f72 202d 2074  ssageOnError - t
+000112d0: 6869 7320 6675 6e63 7469 6f6e 206c 6f67  his function log
+000112e0: 7320 6120 6d65 7373 6167 6520 6f6e 2065  s a message on e
+000112f0: 7272 6f72 0a20 2a2a 2a2a 2a2a 2a2a 2a2a  rror. **********
+00011300: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011310: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011320: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011330: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011340: 2a2f 0a73 7461 7469 6320 696e 6c69 6e65  */.static inline
+00011350: 2069 6e74 3634 5f74 0a6d 735f 7469 6d65   int64_t.ms_time
+00011360: 7374 7232 6274 696d 6520 2863 6f6e 7374  str2btime (const
+00011370: 2063 6861 7220 2a74 696d 6573 7472 2c20   char *timestr, 
+00011380: 7569 6e74 385f 7420 2a62 7469 6d65 2c20  uint8_t *btime, 
+00011390: 636f 6e73 7420 6368 6172 202a 7369 642c  const char *sid,
+000113a0: 2069 6e74 385f 7420 7377 6170 666c 6167   int8_t swapflag
+000113b0: 290a 7b0a 2020 7569 6e74 3136 5f74 2079  ).{.  uint16_t y
+000113c0: 6561 723b 0a20 2075 696e 7431 365f 7420  ear;.  uint16_t 
+000113d0: 6461 793b 0a20 2075 696e 7438 5f74 2068  day;.  uint8_t h
+000113e0: 6f75 723b 0a20 2075 696e 7438 5f74 206d  our;.  uint8_t m
+000113f0: 696e 3b0a 2020 7569 6e74 385f 7420 7365  in;.  uint8_t se
+00011400: 633b 0a20 2075 696e 7433 325f 7420 6e73  c;.  uint32_t ns
+00011410: 6563 3b0a 2020 6e73 7469 6d65 5f74 206e  ec;.  nstime_t n
+00011420: 7374 696d 653b 0a0a 2020 6966 2028 2174  stime;..  if (!t
+00011430: 696d 6573 7472 207c 7c20 2162 7469 6d65  imestr || !btime
+00011440: 290a 2020 7b0a 2020 2020 6d73 5f6c 6f67  ).  {.    ms_log
+00011450: 2028 322c 2022 2573 2825 7329 3a20 5265   (2, "%s(%s): Re
+00011460: 7175 6972 6564 2069 6e70 7574 206e 6f74  quired input not
+00011470: 2064 6566 696e 6564 3a20 2774 696d 6573   defined: 'times
+00011480: 7472 2720 6f72 2027 6274 696d 6527 5c6e  tr' or 'btime'\n
+00011490: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+000114a0: 6964 2c20 5f5f 6675 6e63 5f5f 293b 0a20  id, __func__);. 
+000114b0: 2020 2072 6574 7572 6e20 2d31 3b0a 2020     return -1;.  
+000114c0: 7d0a 0a20 2069 6620 2828 6e73 7469 6d65  }..  if ((nstime
+000114d0: 203d 206d 735f 7469 6d65 7374 7232 6e73   = ms_timestr2ns
+000114e0: 7469 6d65 2028 7469 6d65 7374 7229 2920  time (timestr)) 
+000114f0: 3d3d 204e 5354 4552 524f 5229 0a20 2020  == NSTERROR).   
+00011500: 2072 6574 7572 6e20 2d31 3b0a 0a20 2069   return -1;..  i
+00011510: 6620 286d 735f 6e73 7469 6d65 3274 696d  f (ms_nstime2tim
+00011520: 6520 286e 7374 696d 652c 2026 7965 6172  e (nstime, &year
+00011530: 2c20 2664 6179 2c20 2668 6f75 722c 2026  , &day, &hour, &
+00011540: 6d69 6e2c 2026 7365 632c 2026 6e73 6563  min, &sec, &nsec
+00011550: 2929 0a20 2020 2072 6574 7572 6e20 2d31  )).    return -1
+00011560: 3b0a 0a20 202a 2828 7569 6e74 3136 5f74  ;..  *((uint16_t
+00011570: 202a 2928 6274 696d 6529 2920 2020 2020   *)(btime))     
+00011580: 3d20 484f 3275 2028 7965 6172 2c20 7377  = HO2u (year, sw
+00011590: 6170 666c 6167 293b 0a20 202a 2828 7569  apflag);.  *((ui
+000115a0: 6e74 3136 5f74 202a 2928 6274 696d 6520  nt16_t *)(btime 
+000115b0: 2b20 3229 2920 3d20 484f 3275 2028 6461  + 2)) = HO2u (da
+000115c0: 792c 2073 7761 7066 6c61 6729 3b0a 2020  y, swapflag);.  
+000115d0: 2a28 2875 696e 7438 5f74 202a 2928 6274  *((uint8_t *)(bt
+000115e0: 696d 6520 2b20 3429 2920 203d 2068 6f75  ime + 4))  = hou
+000115f0: 723b 0a20 202a 2828 7569 6e74 385f 7420  r;.  *((uint8_t 
+00011600: 2a29 2862 7469 6d65 202b 2035 2929 2020  *)(btime + 5))  
+00011610: 3d20 6d69 6e3b 0a20 202a 2828 7569 6e74  = min;.  *((uint
+00011620: 385f 7420 2a29 2862 7469 6d65 202b 2036  8_t *)(btime + 6
+00011630: 2929 2020 3d20 7365 633b 0a20 202a 2828  ))  = sec;.  *((
+00011640: 7569 6e74 385f 7420 2a29 2862 7469 6d65  uint8_t *)(btime
+00011650: 202b 2037 2929 2020 3d20 303b 0a20 202a   + 7))  = 0;.  *
+00011660: 2828 7569 6e74 3136 5f74 202a 2928 6274  ((uint16_t *)(bt
+00011670: 696d 6520 2b20 3829 2920 3d20 484f 3275  ime + 8)) = HO2u
+00011680: 2028 6e73 6563 202f 2031 3030 3030 302c   (nsec / 100000,
+00011690: 2073 7761 7066 6c61 6729 3b0a 0a20 2072   swapflag);..  r
+000116a0: 6574 7572 6e20 6e73 6563 3b0a 7d20 2f2a  eturn nsec;.} /*
+000116b0: 2045 6e64 206f 6620 7469 6d65 7374 7232   End of timestr2
+000116c0: 6274 696d 6528 2920 2a2f 0a              btime() */.
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/packdata.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/packdata.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/packdata.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/packdata.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/parseutils.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/parseutils.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/selection.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/selection.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/tracelist.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/tracelist.c`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 MS3TraceSeg *mstl3_addmsrtoseg (MS3TraceSeg *seg, const MS3Record *msr, nstime_t endtime, int8_t whence);
 MS3TraceSeg *mstl3_addsegtoseg (MS3TraceSeg *seg1, MS3TraceSeg *seg2);
 MS3RecordPtr *mstl3_add_recordptr (MS3TraceSeg *seg, const MS3Record *msr, nstime_t endtime, int8_t whence);
 
 static uint32_t lm_lcg_r (uint64_t *state);
 static uint8_t lm_random_height (uint8_t maximum, uint64_t *state);
 
+/* Test if two sample rates are similar using either specified tolerance (if positive) or default tolerance */
+#define IS_SAMPRATE_SIMILAR(SR1, SR2, SRT) ((SRT > 0.0) ? fabs (SR1 - SR2) > SRT : MS_ISRATETOLERABLE (SR1, SR2))
+
 /**********************************************************************/ /**
  * @brief Initialize a ::MS3TraceList container
  *
  * A new ::MS3TraceList is allocated if needed. If the supplied
  * ::MS3TraceList is not NULL it will be re-initialized and any
  * associated memory will be freed including data at \a prvtptr pointers.
  *
@@ -373,23 +376,20 @@
   MS3TraceSeg *followseg = 0;
 
   nstime_t endtime;
   nstime_t pregap;
   nstime_t postgap;
   nstime_t lastgap;
   nstime_t firstgap;
-  nstime_t nsdelta;
+  nstime_t nsperiod;
   nstime_t nstimetol = 0;
   nstime_t nnstimetol = 0;
 
   double sampratehz;
   double sampratetol = -1.0;
-  int8_t whence;
-  int8_t lastratecheck;
-  int8_t firstratecheck;
 
   if (!mstl || !msr)
   {
     ms_log (2, "%s(): Required input not defined: 'mstl' or 'msr'\n", __func__);
     return NULL;
   }
 
@@ -441,83 +441,67 @@
       ms_log (2, "Error adding new ID to trace list\n");
       return NULL;
     }
   }
   /* Add data coverage to the matching MS3TraceID */
   else
   {
-    /* Calculate high-precision sample period, handling different rate notations */
-    if (msr->samprate > 0.0)
-      nsdelta = (nstime_t) (NSTMODULUS / msr->samprate); /* samples/second */
-    else if (msr->samprate < 0.0)
-      nsdelta = (nstime_t) (NSTMODULUS * -msr->samprate); /* period */
-    else
-      nsdelta = 0;
+    /* Calculate nanosecond sample period */
+    nsperiod = msr3_nsperiod (msr);
 
     /* Calculate high-precision time tolerance */
     if (tolerance && tolerance->time)
       nstimetol = (nstime_t) (NSTMODULUS * tolerance->time (msr));
     else
-      nstimetol = (nstime_t) (0.5 * nsdelta); /* Default time tolerance is 1/2 sample period */
+      nstimetol = (nstime_t) (0.5 * nsperiod); /* Default time tolerance is 1/2 sample period */
 
     nnstimetol = (nstimetol) ? -nstimetol : 0;
 
     /* Calculate sample rate tolerance */
     if (tolerance && tolerance->samprate)
       sampratetol = tolerance->samprate (msr);
 
     sampratehz = msr3_sampratehz(msr);
 
     /* last/firstgap are negative when the record overlaps the trace
      * segment and positive when there is a time gap. */
 
     /* Gap relative to the last segment */
-    lastgap = msr->starttime - id->last->endtime - nsdelta;
+    lastgap = msr->starttime - id->last->endtime - nsperiod;
 
     /* Gap relative to the first segment */
-    firstgap = id->first->starttime - endtime - nsdelta;
-
-    /* Sample rate tolerance checks for first and last segments */
-    if (tolerance && tolerance->samprate)
-    {
-      lastratecheck = (sampratetol < 0.0 || ms_dabs (sampratehz - id->last->samprate) > sampratetol) ? 0 : 1;
-      firstratecheck = (sampratetol < 0.0 || ms_dabs (sampratehz - id->first->samprate) > sampratetol) ? 0 : 1;
-    }
-    else
-    {
-      lastratecheck = MS_ISRATETOLERABLE (sampratehz, id->last->samprate);
-      firstratecheck = MS_ISRATETOLERABLE (sampratehz, id->first->samprate);
-    }
+    firstgap = id->first->starttime - endtime - nsperiod;
 
     /* Search first for the simple scenarios in order of likelihood:
      * - Record fits at end of last segment
      * - Record fits after all coverage
      * - Record fits before all coverage
      * - Record fits at beginning of first segment
      *
      * If none of those scenarios are true search the complete segment list.
      */
 
     /* Record coverage fits at end of last segment */
-    if (lastgap <= nstimetol && lastgap >= nnstimetol && lastratecheck)
+    if (lastgap <= nstimetol && lastgap >= nnstimetol &&
+        IS_SAMPRATE_SIMILAR (sampratehz, id->last->samprate, sampratetol))
     {
       if (!mstl3_addmsrtoseg (id->last, msr, endtime, 1))
         return NULL;
 
       seg = id->last;
 
       if (endtime > id->latest)
         id->latest = endtime;
 
       /* Add MS3RecordPtr if requested */
       if (pprecptr && !(*pprecptr = mstl3_add_recordptr (seg, msr, endtime, 1)))
         return NULL;
     }
     /* Record coverage is after all other coverage */
-    else if ((msr->starttime - nsdelta - nstimetol) > id->latest)
+    else if ((msr->starttime - nsperiod - nstimetol) > id->latest)
     {
       if (!(seg = mstl3_msr2seg (msr, endtime)))
         return NULL;
 
       /* Add to end of list */
       id->last->next = seg;
       seg->prev = id->last;
@@ -528,15 +512,15 @@
         id->latest = endtime;
 
       /* Add MS3RecordPtr if requested */
       if (pprecptr && !(*pprecptr = mstl3_add_recordptr (seg, msr, endtime, 0)))
         return NULL;
     }
     /* Record coverage is before all other coverage */
-    else if ((endtime + nsdelta + nstimetol) < id->earliest)
+    else if ((endtime + nsperiod + nstimetol) < id->earliest)
     {
       if (!(seg = mstl3_msr2seg (msr, endtime)))
         return NULL;
 
       /* Add to beginning of list */
       id->first->prev = seg;
       seg->next = id->first;
@@ -547,15 +531,16 @@
         id->earliest = msr->starttime;
 
       /* Add MS3RecordPtr if requested */
       if (pprecptr && !(*pprecptr = mstl3_add_recordptr (seg, msr, endtime, 0)))
         return NULL;
     }
     /* Record coverage fits at beginning of first segment */
-    else if (firstgap <= nstimetol && firstgap >= nnstimetol && firstratecheck)
+    else if (firstgap <= nstimetol && firstgap >= nnstimetol &&
+             IS_SAMPRATE_SIMILAR (sampratehz, id->first->samprate, sampratetol))
     {
       if (!mstl3_addmsrtoseg (id->first, msr, endtime, 2))
         return NULL;
 
       seg = id->first;
 
       if (msr->starttime < id->earliest)
@@ -564,23 +549,22 @@
       /* Add MS3RecordPtr if requested */
       if (pprecptr && !(*pprecptr = mstl3_add_recordptr (seg, msr, endtime, 2)))
         return NULL;
     }
     /* Search complete segment list for matches */
     else
     {
+      /* This search finds the following values if they exist: */
+      segbefore = NULL; /* The first segment end that matches the record start (within tolerance) */
+      segafter  = NULL; /* The first segment start that matches the record end (within tolerance) */
+      followseg = NULL; /* The segment with latest start time before the record start */
       searchseg = id->first;
-      segbefore = NULL; /* Find segment that record fits before */
-      segafter  = NULL; /* Find segment that record fits after */
-      followseg = NULL; /* Track segment that record follows in time order */
-
       while (searchseg)
       {
-        /* Done searching if autohealing and record exactly matches
-         * a segment.
+        /* Done searching if autohealing and record exactly matches a segment.
          *
          * Rationale: autohealing would have combined this segment
          * with another if that were possible, so this record will
          * also not fit with any other segment. */
         if (autoheal &&
             msr->starttime == searchseg->starttime &&
             endtime == searchseg->endtime)
@@ -588,59 +572,38 @@
           followseg = searchseg;
           break;
         }
 
         if (msr->starttime > searchseg->starttime)
           followseg = searchseg;
 
-        whence = 0;
-
-        postgap = msr->starttime - searchseg->endtime - nsdelta;
-        if (!segbefore && postgap <= nstimetol && postgap >= nnstimetol)
-          whence = 1;
-
-        pregap = searchseg->starttime - endtime - nsdelta;
-        if (!segafter && pregap <= nstimetol && pregap >= nnstimetol)
-          whence = 2;
-
-        if (!whence)
+        if (!segbefore)
         {
-          searchseg = searchseg->next;
-          continue;
-        }
+          postgap = msr->starttime - searchseg->endtime - nsperiod;
 
-        if (tolerance && tolerance->samprate)
-        {
-          if (sampratetol >= 0 && ms_dabs (sampratehz - searchseg->samprate) > sampratetol)
-          {
-            searchseg = searchseg->next;
-            continue;
-          }
-        }
-        else
-        {
-          if (!MS_ISRATETOLERABLE (sampratehz, searchseg->samprate))
-          {
-            searchseg = searchseg->next;
-            continue;
-          }
+          if (postgap <= nstimetol && postgap >= nnstimetol &&
+              IS_SAMPRATE_SIMILAR (sampratehz, searchseg->samprate, sampratetol))
+            segbefore = searchseg;
         }
 
-        if (whence == 1)
-          segbefore = searchseg;
-        else
-          segafter = searchseg;
+        if (!segafter)
+        {
+          pregap = searchseg->starttime - endtime - nsperiod;
 
-        /* Done searching if not autohealing */
-        if (!autoheal)
-          break;
+          if (pregap <= nstimetol && pregap >= nnstimetol &&
+              IS_SAMPRATE_SIMILAR (sampratehz, searchseg->samprate, sampratetol))
+            segafter = searchseg;
+        }
 
         /* Done searching if both before and after segments are found */
         if (segbefore && segafter)
           break;
+        /* Done searching if not autohealing and one match found */
+        else if (!autoheal && (segbefore || segafter))
+          break;
 
         searchseg = searchseg->next;
       } /* Done looping through segments */
 
       /* Add MS3Record coverage to end of segment before */
       if (segbefore)
       {
@@ -2413,15 +2376,15 @@
 
       if (maxgap)
         if (gap > *maxgap)
           printflag = 0;
 
       if (printflag)
       {
-        nsamples = ms_dabs (gap) * seg->samprate;
+        nsamples = fabs (gap) * seg->samprate;
 
         if (gap > 0.0)
           nsamples -= 1.0;
         else
           nsamples += 1.0;
 
         /* Fix up gap display */
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/unpack.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/unpack.c`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
  * limitations under the License.
  ***************************************************************************/
 #include <ctype.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <time.h>
-#include <math.h>
 
 #include "libmseed.h"
 #include "mseedformat.h"
 #include "unpack.h"
 #include "unpackdata.h"
 
 /* Function(s) internal to this file */
@@ -131,16 +130,16 @@
     header_crc = HO4u (*pMS3FSDH_CRC (record), swapflag);
     memset (pMS3FSDH_CRC(record), 0, sizeof(uint32_t));
     calculated_crc = ms_crc32c ((const uint8_t*)record, reclen, 0);
     *pMS3FSDH_CRC(record) = HO4u (header_crc, swapflag);
 
     if (header_crc != calculated_crc)
     {
-      ms_log (2, "%.*s: CRC is invalid, miniSEED record may be corrupt\n",
-              sidlength, pMS3FSDH_SID (record));
+      ms_log (2, "%.*s: CRC is invalid, miniSEED record may be corrupt, header: 0x%X calculated: 0x%X\n",
+              sidlength, pMS3FSDH_SID (record), header_crc, calculated_crc);
       return MS_INVALIDCRC;
     }
   }
 
   /* Initialize the MS3Record */
   if (!(*ppmsr = msr3_init (*ppmsr)))
     return MS_GENERROR;
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/unpack.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/unpack.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/unpackdata.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/unpackdata.c`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/unpackdata.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/unpackdata.h`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/yyjson.c` & `mseedlib-0.0.5/src/mseedlib/libmseed/yyjson.c`

 * *Files 0% similar despite different names*

```diff
@@ -1403,14 +1403,15 @@
     doc->val_pool.chunk_size = (count + 1) * sizeof(yyjson_mut_val);
     return true;
 }
 
 void yyjson_mut_doc_free(yyjson_mut_doc *doc) {
     if (doc) {
         yyjson_alc alc = doc->alc;
+        memset(&doc->alc, 0, sizeof(alc));
         unsafe_yyjson_str_pool_release(&doc->str_pool, &alc);
         unsafe_yyjson_val_pool_release(&doc->val_pool, &alc);
         alc.free(alc.ctx, doc);
     }
 }
 
 yyjson_mut_doc *yyjson_mut_doc_new(const yyjson_alc *alc) {
```

### Comparing `mseedlib-0.0.2/src/mseedlib/libmseed/yyjson.h` & `mseedlib-0.0.5/src/mseedlib/libmseed/yyjson.h`

 * *Files 1% similar despite different names*

```diff
@@ -523,24 +523,24 @@
  * Version
  *============================================================================*/
 
 /** The major version of yyjson. */
 #define YYJSON_VERSION_MAJOR  0
 
 /** The minor version of yyjson. */
-#define YYJSON_VERSION_MINOR  8
+#define YYJSON_VERSION_MINOR  9
 
 /** The patch version of yyjson. */
 #define YYJSON_VERSION_PATCH  0
 
 /** The version of yyjson in hex: `(major << 16) | (minor << 8) | (patch)`. */
-#define YYJSON_VERSION_HEX    0x000800
+#define YYJSON_VERSION_HEX    0x000900
 
 /** The version string of yyjson. */
-#define YYJSON_VERSION_STRING "0.8.0"
+#define YYJSON_VERSION_STRING "0.9.0"
 
 /** The version of yyjson in hex, same as `YYJSON_VERSION_HEX`. */
 yyjson_api uint32_t yyjson_version(void);
 
 
 
 /*==============================================================================
@@ -3695,15 +3695,15 @@
 
 /** Adds a string value at the end of the object.
     The `key` should be a null-terminated UTF-8 string.
     The `val` should be a UTF-8 string, null-terminator is not required.
     The `len` should be the length of the `val`, in bytes.
     This function allows duplicated key in one object.
     
-    @warning The key/value strings are not copied, you should keep these strings
+    @warning The key strings are not copied, you should keep these strings
         unmodified for the lifetime of this JSON document. */
 yyjson_api_inline bool yyjson_mut_obj_add_strncpy(yyjson_mut_doc *doc,
                                                   yyjson_mut_val *obj,
                                                   const char *key,
                                                   const char *val, size_t len);
 
 /**
@@ -4829,14 +4829,15 @@
 yyjson_api_inline size_t yyjson_doc_get_val_count(yyjson_doc *doc) {
     return doc ? doc->val_read : 0;
 }
 
 yyjson_api_inline void yyjson_doc_free(yyjson_doc *doc) {
     if (doc) {
         yyjson_alc alc = doc->alc;
+        memset(&doc->alc, 0, sizeof(alc));
         if (doc->str_pool) alc.free(alc.ctx, doc->str_pool);
         alc.free(alc.ctx, doc);
     }
 }
 
 
 
@@ -5668,14 +5669,15 @@
 }
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_bool(yyjson_mut_doc *doc,
                                                   bool _val) {
     if (yyjson_likely(doc)) {
         yyjson_mut_val *val = unsafe_yyjson_mut_val(doc, 1);
         if (yyjson_likely(val)) {
+            _val = !!_val;
             val->tag = YYJSON_TYPE_BOOL | (uint8_t)((uint8_t)_val << 3);
             return val;
         }
     }
     return NULL;
 }
 
@@ -5920,15 +5922,16 @@
         } \
     } \
     return NULL
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_arr_with_bool(
     yyjson_mut_doc *doc, const bool *vals, size_t count) {
     yyjson_mut_arr_with_func({
-        val->tag = YYJSON_TYPE_BOOL | (uint8_t)((uint8_t)vals[i] << 3);
+        bool _val = !!vals[i];
+        val->tag = YYJSON_TYPE_BOOL | (uint8_t)((uint8_t)_val << 3);
     });
 }
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_arr_with_sint(
     yyjson_mut_doc *doc, const int64_t *vals, size_t count) {
     return yyjson_mut_arr_with_sint64(doc, vals, count);
 }
@@ -6872,14 +6875,15 @@
 }
 
 yyjson_api_inline bool yyjson_mut_obj_add_bool(yyjson_mut_doc *doc,
                                                yyjson_mut_val *obj,
                                                const char *_key,
                                                bool _val) {
     yyjson_mut_obj_add_func({
+        _val = !!_val;
         val->tag = YYJSON_TYPE_BOOL | (uint8_t)((uint8_t)(_val) << 3);
     });
 }
 
 yyjson_api_inline bool yyjson_mut_obj_add_uint(yyjson_mut_doc *doc,
                                                yyjson_mut_val *obj,
                                                const char *_key,
@@ -7730,41 +7734,47 @@
         return true;
     } else {
         return false;
     }
 }
 
 /**
- Set provided `value` if the JSON Pointer (RFC 6901) exists and is type uint.
- Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is an integer
+ that fits in `uint64_t`. Returns true if successful, otherwise false.
  */
 yyjson_api_inline bool yyjson_ptr_get_uint(
     yyjson_val *root, const char *ptr, uint64_t *value) {
     yyjson_val *val = yyjson_ptr_get(root, ptr);
-    if (value && yyjson_is_uint(val)) {
-        *value = unsafe_yyjson_get_uint(val);
-        return true;
-    } else {
-        return false;
+    if (value && val) {
+        uint64_t ret = val->uni.u64;
+        if (unsafe_yyjson_is_uint(val) ||
+            (unsafe_yyjson_is_sint(val) && !(ret >> 63))) {
+            *value = ret;
+            return true;
+        }
     }
+    return false;
 }
 
 /**
- Set provided `value` if the JSON Pointer (RFC 6901) exists and is type sint.
- Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is an integer
+ that fits in `int64_t`. Returns true if successful, otherwise false.
  */
 yyjson_api_inline bool yyjson_ptr_get_sint(
     yyjson_val *root, const char *ptr, int64_t *value) {
     yyjson_val *val = yyjson_ptr_get(root, ptr);
-    if (value && yyjson_is_sint(val)) {
-        *value = unsafe_yyjson_get_sint(val);
-        return true;
-    } else {
-        return false;
+    if (value && val) {
+        int64_t ret = val->uni.i64;
+        if (unsafe_yyjson_is_sint(val) ||
+            (unsafe_yyjson_is_uint(val) && ret >= 0)) {
+            *value = ret;
+            return true;
+        }
     }
+    return false;
 }
 
 /**
  Set provided `value` if the JSON Pointer (RFC 6901) exists and is type real.
  Returns true if value at `ptr` exists and is the correct type, otherwise false.
  */
 yyjson_api_inline bool yyjson_ptr_get_real(
```

### Comparing `mseedlib-0.0.2/tests/test_msrecord.py` & `mseedlib-0.0.5/tests/test_msrecord.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/test_msrecord_buffer_reader.py` & `mseedlib-0.0.5/tests/test_msrecord_buffer_reader.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/test_msrecord_reader.py` & `mseedlib-0.0.5/tests/test_msrecord_reader.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/test_mstracelist.py` & `mseedlib-0.0.5/tests/test_mstracelist.py`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/data/packtest_sine2000.mseed3` & `mseedlib-0.0.5/tests/data/packtest_sine2000.mseed3`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/data/packtest_sine500.mseed2` & `mseedlib-0.0.5/tests/data/packtest_sine500.mseed2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 3030 3030 3030 4420 5445 5354 2020 2042  000000D TEST   B
+00000000: 3030 3030 3030 5220 5445 5354 2020 2042  000000R TEST   B
 00000010: 5358 5858 07e7 0002 0102 0300 04d2 01f4  SXXX............
 00000020: 0032 0001 0020 0002 0000 0000 0040 0030  .2... .......@.0
 00000030: 03e8 0038 0b01 0900 03e9 0000 5038 0000  ...8........P8..
 00000040: 03ff ffff 0000 0000 0000 0148 4084 a509  ...........H@...
 00000050: 5284 a509 5094 2509 5084 a108 5084 1d08  R...P.%.P...P...
 00000060: 4e83 a0e7 8777 7776 8676 6666 8656 5555  N....wwv.vff.VUU
 00000070: 8554 5444 8443 4333 8333 2232 8212 1211  .TTD.CC3.3"2....
```

### Comparing `mseedlib-0.0.2/tests/data/testdata-COLA-signal.mseed2` & `mseedlib-0.0.5/tests/data/testdata-COLA-signal.mseed2`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/tests/data/testdata-COLA-signal.mseed3` & `mseedlib-0.0.5/tests/data/testdata-COLA-signal.mseed3`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/LICENSE` & `mseedlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/README.md` & `mseedlib-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 a callback to consume, and do whatever you want, with generated records.
 
 Simple example of writing multiple channels of data:
 ```Python
 import math
 from mseedlib import MSTraceList, timestr2nstime
 
-# Generate synthetic sinusoid data, starting at 9, 45, and 90 degrees
+# Generate synthetic sinusoid data, starting at 0, 45, and 90 degrees
 data0 = list(map(lambda x: int(math.sin(math.radians(0)) * 500), range(0, 500)))
 data1 = list(map(lambda x: int(math.sin(math.radians(45)) * 500), range(45, 500 + 45)))
 data2 = list(map(lambda x: int(math.sin(math.radians(90)) * 500), range(90, 500 + 90)))
 
 mstl = MSTraceList()
 
 sample_rate = 40.0
@@ -119,8 +119,8 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
-Copyright (C) 2023 Chad Trabant, EarthScope Data Services
+Copyright (C) 2024 Chad Trabant, EarthScope Data Services
```

### Comparing `mseedlib-0.0.2/pyproject.toml` & `mseedlib-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mseedlib-0.0.2/PKG-INFO` & `mseedlib-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mseedlib
-Version: 0.0.2
+Version: 0.0.5
 Summary: A Python package for reading and writing miniSEED formatted data
 Project-URL: Homepage, https://github.com/EarthScope/mseedlib
 Project-URL: Issues, https://github.com/EarthScope/mseedlib/issues
 Author-email: EarthScope Data Services <software@earthscope.org>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: data,miniseed,mseed,seismic,seismology,waveform
@@ -81,15 +81,15 @@
 a callback to consume, and do whatever you want, with generated records.
 
 Simple example of writing multiple channels of data:
 ```Python
 import math
 from mseedlib import MSTraceList, timestr2nstime
 
-# Generate synthetic sinusoid data, starting at 9, 45, and 90 degrees
+# Generate synthetic sinusoid data, starting at 0, 45, and 90 degrees
 data0 = list(map(lambda x: int(math.sin(math.radians(0)) * 500), range(0, 500)))
 data1 = list(map(lambda x: int(math.sin(math.radians(45)) * 500), range(45, 500 + 45)))
 data2 = list(map(lambda x: int(math.sin(math.radians(90)) * 500), range(90, 500 + 90)))
 
 mstl = MSTraceList()
 
 sample_rate = 40.0
@@ -146,8 +146,8 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
-Copyright (C) 2023 Chad Trabant, EarthScope Data Services
+Copyright (C) 2024 Chad Trabant, EarthScope Data Services
```

