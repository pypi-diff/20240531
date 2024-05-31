# Comparing `tmp/foc-0.4.6.tar.gz` & `tmp/foc-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.4.6.tar", last modified: Tue Jan 16 06:24:23 2024, max compression
+gzip compressed data, was "foc-0.4.7.tar", last modified: Fri May 31 18:13:23 2024, max compression
```

## Comparing `foc-0.4.6.tar` & `foc-0.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-01-16 06:24:23.555066 foc-0.4.6/
--rw-r--r--   0 thyeem     (501) staff       (20)     2896 2024-01-16 06:01:33.000000 foc-0.4.6/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1055 2023-11-16 05:54:17.000000 foc-0.4.6/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)      190 2023-11-16 06:06:16.000000 foc-0.4.6/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)    28605 2024-01-16 06:24:23.554971 foc-0.4.6/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    28082 2024-01-16 04:14:52.000000 foc-0.4.6/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-01-16 06:24:23.553196 foc-0.4.6/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    52301 2024-01-16 06:02:00.000000 foc-0.4.6/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-01-16 06:24:23.554254 foc-0.4.6/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)    28605 2024-01-16 06:24:23.000000 foc-0.4.6/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2024-01-16 06:24:23.000000 foc-0.4.6/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2024-01-16 06:24:23.000000 foc-0.4.6/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2024-01-16 06:24:23.000000 foc-0.4.6/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       74 2024-01-16 06:24:23.555283 foc-0.4.6/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      835 2023-12-14 07:16:13.000000 foc-0.4.6/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-01-16 06:24:23.554468 foc-0.4.6/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-07-29 10:49:10.000000 foc-0.4.6/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     8153 2024-01-16 04:14:52.000000 foc-0.4.6/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-05-31 18:13:23.176477 foc-0.4.7/
+-rw-r--r--   0 thyeem     (501) staff       (20)     2977 2024-05-31 17:25:35.000000 foc-0.4.7/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1055 2023-11-16 05:54:17.000000 foc-0.4.7/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)      190 2023-11-16 06:06:16.000000 foc-0.4.7/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)    28736 2024-05-31 18:13:23.176401 foc-0.4.7/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    28213 2024-05-31 17:52:36.000000 foc-0.4.7/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-05-31 18:13:23.175310 foc-0.4.7/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    52592 2024-05-31 18:06:37.000000 foc-0.4.7/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-05-31 18:13:23.176190 foc-0.4.7/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)    28736 2024-05-31 18:13:23.000000 foc-0.4.7/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2024-05-31 18:13:23.000000 foc-0.4.7/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2024-05-31 18:13:23.000000 foc-0.4.7/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2024-05-31 18:13:23.000000 foc-0.4.7/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       74 2024-05-31 18:13:23.176675 foc-0.4.7/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      835 2023-12-14 07:16:13.000000 foc-0.4.7/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2024-05-31 18:13:23.176015 foc-0.4.7/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-07-29 10:49:10.000000 foc-0.4.7/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8153 2024-01-16 04:14:52.000000 foc-0.4.7/tests/test_foc.py
```

### Comparing `foc-0.4.6/ChangeLog.md` & `foc-0.4.7/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -137,7 +137,10 @@
 
 # 0.4.5
 - Fix `choice` and `chunks_of`
 
 # 0.4.6
 - Add `chunks_from`
 - Fix `neatly` and `nprint` (add sorting flags)
+
+# 0.4.7
+- Fix `ls`: don't list hidden files(dotfile) by default. add '-a' flag.
```

### Comparing `foc-0.4.6/LICENSE` & `foc-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.4.6/PKG-INFO` & `foc-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.4.6
+Version: 0.4.7
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 License: MIT
 Keywords: functional functools functional-python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -829,31 +829,34 @@
 >>> d.bach.chopin.beethoven
 {}
 ```
 ### Handy File Tools: `ls` and `grep` 
 Use `ls` and `grep` in the same way you use in your terminal every day.   
 _This is just a more intuitive alternative to_ `os.listdir` and `os.walk`. When applicable, use `shell` instead. 
 
-> `ls(*paths, grep=REGEX, i=BOOL, r=BOOL, f=BOOL, d=BOOL, g=BOOL)`
+> `ls(*paths, grep=REGEX, a=BOOL, r=BOOL, i=BOOL, f=BOOL, d=BOOL, g=BOOL)`
 ```python
 # couldn't be simpler!
->>> ls()       # the same as ls("."): get contents of the curruent dir
+>>> ls()         # the same as ls("."): get contents of the curruent dir
 
 # expands "~" automatically
->>> ls("~")    # the same as `ls -a1 ~`: returns a list of $HOME
+>>> ls("~")      # the same as `ls -1 ~`: returns a list of $HOME
+
+# list hidden files ('dotfiles' or files starting with ".")
+>>> ls(a=True)   # the same as `ls -a`
 
 # support glob patterns (*, ?, [)
 >>> ls("./*/*.py")
 
 # with multiple filepaths
 >>> ls(FILE, DIR, ...)
 ```
 ```python
-# list up recursively and filter hidden files out
->>> ls(".git", r=True, grep="^[^\.]")
+# list up `.git` directory recursively and pick files ending with digits
+>>> ls(".git", r=True, grep="\d$")
 ```
 ```python
 # only files in '.git' directory
 >>> ls(".git", r=True, f=True)
 
 # only directories in '.git' directory
 >>> ls(".git", r=True, d=True)
```

### Comparing `foc-0.4.6/README.md` & `foc-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -813,31 +813,34 @@
 >>> d.bach.chopin.beethoven
 {}
 ```
 ### Handy File Tools: `ls` and `grep` 
 Use `ls` and `grep` in the same way you use in your terminal every day.   
 _This is just a more intuitive alternative to_ `os.listdir` and `os.walk`. When applicable, use `shell` instead. 
 
-> `ls(*paths, grep=REGEX, i=BOOL, r=BOOL, f=BOOL, d=BOOL, g=BOOL)`
+> `ls(*paths, grep=REGEX, a=BOOL, r=BOOL, i=BOOL, f=BOOL, d=BOOL, g=BOOL)`
 ```python
 # couldn't be simpler!
->>> ls()       # the same as ls("."): get contents of the curruent dir
+>>> ls()         # the same as ls("."): get contents of the curruent dir
 
 # expands "~" automatically
->>> ls("~")    # the same as `ls -a1 ~`: returns a list of $HOME
+>>> ls("~")      # the same as `ls -1 ~`: returns a list of $HOME
+
+# list hidden files ('dotfiles' or files starting with ".")
+>>> ls(a=True)   # the same as `ls -a`
 
 # support glob patterns (*, ?, [)
 >>> ls("./*/*.py")
 
 # with multiple filepaths
 >>> ls(FILE, DIR, ...)
 ```
 ```python
-# list up recursively and filter hidden files out
->>> ls(".git", r=True, grep="^[^\.]")
+# list up `.git` directory recursively and pick files ending with digits
+>>> ls(".git", r=True, grep="\d$")
 ```
 ```python
 # only files in '.git' directory
 >>> ls(".git", r=True, f=True)
 
 # only directories in '.git' directory
 >>> ls(".git", r=True, d=True)
```

### Comparing `foc-0.4.6/foc/__init__.py` & `foc-0.4.7/foc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from itertools import takewhile
 from multiprocessing import Process
 from shutil import rmtree
 from subprocess import DEVNULL, PIPE, STDOUT, Popen
 from textwrap import fill
 from threading import Thread, Timer
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 __all__ = [
     "composable",
     "fx",
     "trap",
     "safe",
     "id",
@@ -1556,28 +1556,24 @@
 def reader(f=None, mode="r", zipf=False):
     """get ready to read stream from a file or stdin, then returns the handle."""
     if f is not None:
         guard(exists(f, "f"), f"reader: not found such a file: {f}")
     return (
         sys.stdin
         if f is None
-        else zipfile.ZipFile(normpath(f), mode)
-        if zipf
-        else open(normpath(f), mode)
+        else zipfile.ZipFile(normpath(f), mode) if zipf else open(normpath(f), mode)
     )
 
 
 def writer(f=None, mode="w", zipf=False):
     """get ready to write stream to a file or stout, then returns the handle."""
     return (
         sys.stdout
         if f is None
-        else zipfile.ZipFile(normpath(f), mode)
-        if zipf
-        else open(normpath(f), mode)
+        else zipfile.ZipFile(normpath(f), mode) if zipf else open(normpath(f), mode)
     )
 
 
 def split_at(ix, x):
     """split the given iterable 'x' at the given splitting-indices 'ix'."""
     s = flatl(0, ix, None)
     return ([*it.islice(x, begin, end)] for begin, end in zip(s, s[1:]))
@@ -1709,60 +1705,81 @@
     path = normpath(path)
     if rm_rf:
         rmtree(path)
     else:
         os.removedirs(path)
 
 
-def ls(*paths, grep=None, i=False, r=False, f=False, d=False, g=False, _root=True):
-    """list directory contents: just like 'ls -a1'.
+def ls(
+    *paths,
+    grep=None,
+    a=False,
+    r=False,
+    i=False,
+    f=False,
+    d=False,
+    g=False,
+    _root=True,
+):
+    """list directory contents: just like 'ls -1'.
 
     Note:
       - allowed glob patterns (*,?,[) in <path..>
-      - given 'grep=<regex>', it behaves like 'ls -a1 <path..> | grep <regex>'
-      - if i is set, it makes 'grep' case-insensitive (-i flag in grep)
+      - given 'grep=<regex>', it behaves like 'ls -1 <path..> | grep <regex>'
+      - if a is set, it also lists hidden files (dotfiles) (-a flag in ls)
       - if r is set, it behaves like 'find -s <path..>' (-R flag in ls)
+      - if i is set, it makes 'grep' case-insensitive (-i flag in grep)
       - if f is set, it lists only files like 'find <path..> -type f'
       - if d is set, it lists only directories like 'find <path..> -type d'
       - if g is set, it returns a generator instead of a sorted list
     """
     paths = paths or ["."]
     typef = f and f ^ d
     typed = d and f ^ d
 
     def fd(x):
         return (typef and exists(x, "f")) or (typed and exists(x, "d"))
 
+    def listdir(x):
+        return cf_(
+            id if a else filter(cf_(_not, ff_(str.startswith, "."))),
+            os.listdir,
+        )(x)
+
     def root(xs):
         return flat(
-            glob(normpath(x))
-            if re.search(r"[\*\+\?\[]", x)
-            else cf_(
-                guard_(exists, f"ls, no such file or directory: {x}"),
-                normpath,
-            )(x)
+            (
+                glob(normpath(x))
+                if re.search(r"[\*\+\?\[]", x)
+                else cf_(
+                    guard_(exists, f"ls, no such file or directory: {x}"),
+                    normpath,
+                )(x)
+            )
             for x in xs
         )
 
     def rflag(xs):
         return flat(
-            (x, ls(x, grep=grep, i=i, r=r, f=f, d=d, g=g, _root=False))
-            if exists(x, "d")
-            else x
+            (
+                (x, ls(x, grep=grep, a=a, r=r, i=i, f=f, d=d, g=g, _root=False))
+                if exists(x, "d")
+                else x
+            )
             for x in xs
         )
 
     return cf_(
         id if g else sort,  # return generator or sort by filepath
         filter(fd) if typef ^ typed else id,  # filetype filter: -f or -d flag
         globals()["grep"](grep, i=i) if grep else id,  # grep -i flag
         rflag if r else id,  # recursively listing: -R flag
     )(
         flat(
-            [normpath(f"{x}/{o}") for o in (os.listdir(x))] if exists(x, "d") else x
+            [normpath(f"{x}/{o}") for o in listdir(x)] if exists(x, "d") else x
             for x in (root(paths) if _root else paths)
         )
     )
 
 
 @safe
 def grep(regex, *, i=False):
@@ -1833,21 +1850,21 @@
 def randbytes(n):
     """generate cryptographically secure random bytes"""
     return os.urandom(n)
 
 
 def rand(x=None, high=None, size=None):
     return (
-        [rd.uniform(x, high) for _ in range(size)]  # #args == 3
+        [rd.uniform(x, high) for _ in range(size)]
         if size is not None
-        else rd.uniform(x, high)  # #args == 2
-        if high is not None
-        else rd.uniform(0, x)  # #args == 1
-        if x is not None
-        else rd.random()  # #args == 0
+        else (
+            rd.uniform(x, high)
+            if high is not None
+            else rd.uniform(0, x) if x is not None else rd.random()
+        )
     )
 
 
 def randn(mu=0, sigma=1, size=None):
     return (
         [rd.gauss(mu, sigma) for _ in range(size)]
         if size is not None
@@ -1862,21 +1879,21 @@
 
     def rint(high=1 << 256, low=0):
         guard(low < high, f"randint: low({low}) must be less than high({high})")
         x = high - low
         return low + (bytes_to_int(randbytes((x.bit_length() + 7) // 8)) % x)
 
     return (
-        [rint(high, x) for _ in range(size)]  # #args == 3
+        [rint(high, x) for _ in range(size)]
         if size is not None
-        else rint(high, x)  # #args == 2
-        if high is not None
-        else rint(x)  # #args == 1
-        if x is not None
-        else rint()  # #args == 0
+        else (
+            rint(high, x)
+            if high is not None
+            else (rint(x) if x is not None else rint())
+        )
     )
 
 
 @fx
 def shuffle(x):
     """Fisher-Yates shuffle in a cryptographically secure way"""
     for i in range(len(x) - 1, 0, -1):
@@ -2113,17 +2130,19 @@
     def indent(x, i):
         def u(c, j=0):
             return f"{c:3}{x[j:]}"
 
         return (
             (u("-", 3) if i else u("+", 3))
             if x and x[0] == "|"
-            else f"{x}"
-            if x and x[0] == ":"
-            else ((u("-") if x[0] == "+" else u("")) if i else u("+"))
+            else (
+                f"{x}"
+                if x and x[0] == ":"
+                else ((u("-") if x[0] == "+" else u("")) if i else u("+"))
+            )
         )
 
     def bullet(o, s):
         return (
             (indent(x, i) for i, x in enumerate(s))
             if isinstance(o, list)
             else (f":  {x}" if i else f"|  {x}" for i, x in enumerate(s))
```

### Comparing `foc-0.4.6/foc.egg-info/PKG-INFO` & `foc-0.4.7/foc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.4.6
+Version: 0.4.7
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 License: MIT
 Keywords: functional functools functional-python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -829,31 +829,34 @@
 >>> d.bach.chopin.beethoven
 {}
 ```
 ### Handy File Tools: `ls` and `grep` 
 Use `ls` and `grep` in the same way you use in your terminal every day.   
 _This is just a more intuitive alternative to_ `os.listdir` and `os.walk`. When applicable, use `shell` instead. 
 
-> `ls(*paths, grep=REGEX, i=BOOL, r=BOOL, f=BOOL, d=BOOL, g=BOOL)`
+> `ls(*paths, grep=REGEX, a=BOOL, r=BOOL, i=BOOL, f=BOOL, d=BOOL, g=BOOL)`
 ```python
 # couldn't be simpler!
->>> ls()       # the same as ls("."): get contents of the curruent dir
+>>> ls()         # the same as ls("."): get contents of the curruent dir
 
 # expands "~" automatically
->>> ls("~")    # the same as `ls -a1 ~`: returns a list of $HOME
+>>> ls("~")      # the same as `ls -1 ~`: returns a list of $HOME
+
+# list hidden files ('dotfiles' or files starting with ".")
+>>> ls(a=True)   # the same as `ls -a`
 
 # support glob patterns (*, ?, [)
 >>> ls("./*/*.py")
 
 # with multiple filepaths
 >>> ls(FILE, DIR, ...)
 ```
 ```python
-# list up recursively and filter hidden files out
->>> ls(".git", r=True, grep="^[^\.]")
+# list up `.git` directory recursively and pick files ending with digits
+>>> ls(".git", r=True, grep="\d$")
 ```
 ```python
 # only files in '.git' directory
 >>> ls(".git", r=True, f=True)
 
 # only directories in '.git' directory
 >>> ls(".git", r=True, d=True)
```

### Comparing `foc-0.4.6/setup.py` & `foc-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `foc-0.4.6/tests/test_foc.py` & `foc-0.4.7/tests/test_foc.py`

 * *Files identical despite different names*

