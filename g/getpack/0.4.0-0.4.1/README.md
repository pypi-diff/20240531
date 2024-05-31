# Comparing `tmp/getpack-0.4.0.tar.gz` & `tmp/getpack-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpack-0.4.0.tar", last modified: Sat Feb 10 22:36:02 2024, max compression
+gzip compressed data, was "getpack-0.4.1.tar", last modified: Fri May 31 19:32:43 2024, max compression
```

## Comparing `getpack-0.4.0.tar` & `getpack-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:02.042496 getpack-0.4.0/
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2337 2024-02-10 22:36:02.043505 getpack-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1647 2023-08-09 22:24:08.000000 getpack-0.4.0/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2024-02-10 22:36:02.046508 getpack-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:01.898193 getpack-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:01.964181 getpack-0.4.0/src/getpack/
--rw-rw-rw-   0        0        0      618 2024-02-10 21:58:17.000000 getpack-0.4.0/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     3253 2024-02-10 21:58:04.000000 getpack-0.4.0/src/getpack/executable.py
--rw-rw-rw-   0        0        0     1926 2023-08-09 21:03:35.000000 getpack-0.4.0/src/getpack/extraction.py
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:02.006497 getpack-0.4.0/src/getpack/library/
--rw-rw-rw-   0        0        0     3024 2024-02-10 21:59:25.000000 getpack-0.4.0/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0    12275 2024-02-10 21:08:09.000000 getpack-0.4.0/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:02.003495 getpack-0.4.0/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2337 2024-02-10 22:36:01.000000 getpack-0.4.0/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-02-10 22:36:01.000000 getpack-0.4.0/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-10 22:36:01.000000 getpack-0.4.0/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2024-02-10 22:36:01.000000 getpack-0.4.0/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-10 22:36:01.000000 getpack-0.4.0/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-10 22:36:02.039497 getpack-0.4.0/tests/
--rw-rw-rw-   0        0        0     1733 2023-08-09 22:23:50.000000 getpack-0.4.0/tests/test_common.py
--rw-rw-rw-   0        0        0     1071 2023-05-10 21:29:25.000000 getpack-0.4.0/tests/test_concurrency.py
--rw-rw-rw-   0        0        0      444 2024-02-10 20:50:58.000000 getpack-0.4.0/tests/test_executable.py
--rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.4.0/tests/test_unicode.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.634082 getpack-0.4.1/
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2514 2024-05-31 19:32:43.635082 getpack-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1819 2024-05-31 15:45:07.000000 getpack-0.4.1/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1088 2024-05-31 19:32:43.638082 getpack-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.533082 getpack-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.549082 getpack-0.4.1/src/getpack/
+-rw-rw-rw-   0        0        0      618 2024-05-31 16:43:19.000000 getpack-0.4.1/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     3577 2024-05-31 15:10:51.000000 getpack-0.4.1/src/getpack/executable.py
+-rw-rw-rw-   0        0        0     1926 2023-08-09 21:03:35.000000 getpack-0.4.1/src/getpack/extraction.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.612082 getpack-0.4.1/src/getpack/library/
+-rw-rw-rw-   0        0        0     3024 2024-02-10 21:59:25.000000 getpack-0.4.1/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0    12828 2024-05-31 19:27:20.000000 getpack-0.4.1/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.608081 getpack-0.4.1/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2514 2024-05-31 19:32:43.000000 getpack-0.4.1/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-05-31 19:32:43.000000 getpack-0.4.1/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:32:43.000000 getpack-0.4.1/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2024-05-31 19:32:43.000000 getpack-0.4.1/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 19:32:43.000000 getpack-0.4.1/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 19:32:43.631089 getpack-0.4.1/tests/
+-rw-rw-rw-   0        0        0     1793 2024-05-31 15:34:54.000000 getpack-0.4.1/tests/test_common.py
+-rw-rw-rw-   0        0        0     1698 2024-05-31 19:31:34.000000 getpack-0.4.1/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      622 2024-05-31 15:10:51.000000 getpack-0.4.1/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2024-05-31 15:37:58.000000 getpack-0.4.1/tests/test_unicode.py
```

### Comparing `getpack-0.4.0/LICENSE` & `getpack-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.4.0/PKG-INFO` & `getpack-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.4.0
+Version: 0.4.1
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Platform: UNKNOWN
@@ -53,8 +53,13 @@
 
 - Utilize `requirements.txt` to reproduce both development and production
   environments.
 
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
 
+### Environs
+* `GETPACK_RETRIES` - int, number of general retries, used for renaming and
+    removing temporary folders
+* `GETPACK_BACKOFF` - float, delay between retires
+
```

### Comparing `getpack-0.4.0/README.md` & `getpack-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -34,7 +34,12 @@
 ### TODO
 
 - Utilize `requirements.txt` to reproduce both development and production
   environments.
 
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
+
+### Environs
+* `GETPACK_RETRIES` - int, number of general retries, used for renaming and
+    removing temporary folders
+* `GETPACK_BACKOFF` - float, delay between retires
```

### Comparing `getpack-0.4.0/setup.cfg` & `getpack-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `getpack-0.4.0/src/getpack/__init__.py` & `getpack-0.4.1/src/getpack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Copyright (c) 2022 Konstantin Maslyuk. All rights reserved.
 
 This work is licensed under the terms of the MIT license.
 For a copy, see <https://opensource.org/licenses/MIT>.
 """
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 from .executable import Executable, LocalExecutable  # noqa: F401
 from .resource import (  # noqa: F401
     LocalResource,
     PyPiPackage,
     PythonPackage,
     Resource,
```

### Comparing `getpack-0.4.0/src/getpack/executable.py` & `getpack-0.4.1/src/getpack/executable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-import subprocess
-import sys
-
-from .resource import Base, Resource
-
-
-class LocalExecutable(Base):
-    """
-    Wrapper for locally available executable.
-
-    So it is easier to add convenience methods and accomplish nitty-gritty
-    tasks.
-    """
-    executable = None
-    popen_class = subprocess.Popen
-
-    def __init__(self, executable=None, *args, **kwargs):
-        if executable:
-            self.executable = executable
-        super(LocalExecutable, self).__init__(*args, **kwargs)
-
-    def get_popen_params(self, args, kwargs):
-        assert self.executable, 'Property `executable` should be provided'
-        args = (self.executable, ) + args
-        args = tuple(str(i) for i in args)  # conform to string (pathlib.Path)
-        kwargs = dict((k, v) for k, v in kwargs.items() if k not in {
-            'check',
-        })
-        if kwargs.get('input') is None:
-            kwargs['stdin'] = subprocess.PIPE
-        kwargs.setdefault('stdout', subprocess.PIPE)
-        kwargs.setdefault('stderr', subprocess.PIPE)
-        if not kwargs.pop('show', None):
-            if sys.platform == 'win32':
-                # hide console window
-                startupinfo = subprocess.STARTUPINFO()
-                startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-                kwargs['startupinfo'] = startupinfo
-        kwargs['args'] = args
-        return kwargs
-
-    def __call__(self, *args, **kwargs):
-        """
-        Execute process provided by this resource.
-
-        Parameters
-        -----
-        input - `str`, `bytes` or Stream, process input data passed to
-            `Popen.communicate()`.
-        check - `bool`, whether exception should be raised if process returned
-                non zero exit code. Default is `True`.
-        """
-        input = kwargs.pop('input', None)
-        detach = kwargs.pop('detach', False)
-        proc = self.make_popen(*args, **kwargs)
-        if detach:
-            return
-        out, err = proc.communicate(input=input)
-        if kwargs.get('check', True) and proc.returncode:
-            raise Exception(
-                'Command {!r} returned non-zero exit status: {}, output:'
-                '\n{}'.format(args, proc.returncode,
-                              err.decode(errors='replace')))
-        return out
-
-    def make_popen(self, *args, **kwargs):
-        resolved_kwargs = self.get_popen_params(args, kwargs)
-        return self.popen_class(**resolved_kwargs)
-
-
-class Executable(LocalExecutable, Resource):
-    """Intended for executables provided by WebResource."""
-
-    executable_ext = ''
-    if sys.platform == 'win32':
-        executable_ext = '.exe'
-
-    @property
-    def executable(self):
-        return self.path / (self.executable_name + self.executable_ext)
-
-    @property
-    def executable_name(self):
-        try:
-            return self._executable_name
-        except AttributeError:
-            pass
-        return self.name
-
-    @executable_name.setter
-    def executable_name(self, value):
-        self._executable_name = value
-
-    def __call__(self, *args, **kwargs):
-        self.provide()
-        return super(Executable, self).__call__(*args, **kwargs)
+import subprocess
+import sys
+
+from .resource import Base, Resource
+
+
+class LocalExecutable(Base):
+    """
+    Wrapper for locally available executable.
+
+    So it is easier to add convenience methods and accomplish nitty-gritty
+    tasks.
+    """
+    executable = None  # type: str
+    popen_class = subprocess.Popen
+
+    __default_params__ = ('detach', 'show')
+
+    def __init__(self, executable=None, *args, **kwargs):
+        if executable:
+            self.executable = executable
+        super(LocalExecutable, self).__init__(*args, **kwargs)
+
+    def get_popen_params(self, args, kwargs):
+        assert self.executable, 'Property `executable` should be provided'
+        args = (self.executable, ) + args
+        args = tuple(str(i) for i in args)  # conform to string (pathlib.Path)
+        kwargs = dict(kwargs)
+        if kwargs.pop('input', None) is None:
+            kwargs['stdin'] = subprocess.PIPE
+        kwargs.setdefault('stdout', subprocess.PIPE)
+        kwargs.setdefault('stderr', subprocess.PIPE)
+        if not kwargs.pop('show', None):
+            if sys.platform == 'win32':
+                # hide console window
+                startupinfo = subprocess.STARTUPINFO()
+                startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+                kwargs['startupinfo'] = startupinfo
+        kwargs['args'] = args
+        return self._filter_non_popen_params(kwargs)
+
+    def __call__(self, *args, **kwargs):
+        """
+        Execute process provided by this resource.
+
+        Parameters
+        -----
+        input - `str`, `bytes` or Stream, process input data passed to
+            `Popen.communicate()`.
+        check - `bool`, whether exception should be raised if process returned
+            non zero exit code. Default is `True`.
+        show - `bool`, whether to show console or gui window for started
+            process. `False` by default.
+        detach - `bool`, do not wait for process termination, process instance
+            will be returned instead of output. `False` by default.
+        """
+        for k in self.__default_params__:
+            v = getattr(self, k, None)
+            if v is not None:
+                kwargs.setdefault(k, v)
+        popen_kwargs = self.get_popen_params(args, kwargs)
+        proc = self.popen_class(**popen_kwargs)
+        if kwargs.get('detach'):
+            return proc
+        out, err = proc.communicate(input=kwargs.get('input'))
+        if kwargs.get('check', True) and proc.returncode:
+            raise Exception(
+                'Command {!r} returned non-zero exit status: {}, output:'
+                '\n{}'.format(args, proc.returncode,
+                              err.decode(errors='replace')))
+        return self._format_output(out, err, proc)
+
+    def _filter_non_popen_params(self, kwargs):
+        return dict((k, v) for k, v in kwargs.items() if k not in {
+            'check', 'detach',
+        })
+
+    def _format_output(self, out, err, proc):
+        return out
+
+
+class Executable(LocalExecutable, Resource):
+    """Intended for executables provided by WebResource."""
+
+    executable_ext = ''
+    if sys.platform == 'win32':
+        executable_ext = '.exe'
+
+    def __init__(self, *args, **kwargs):
+        super(Executable, self).__init__(*args, **kwargs)
+        if self.executable is None:
+            name = getattr(self, 'executable_name', self.name)
+            self.executable = str(self.path / (name + self.executable_ext))
+
+    def __call__(self, *args, **kwargs):
+        self.provide()
+        return super(Executable, self).__call__(*args, **kwargs)
```

### Comparing `getpack-0.4.0/src/getpack/extraction.py` & `getpack-0.4.1/src/getpack/extraction.py`

 * *Files identical despite different names*

### Comparing `getpack-0.4.0/src/getpack/library/__init__.py` & `getpack-0.4.1/src/getpack/library/__init__.py`

 * *Files identical despite different names*

### Comparing `getpack-0.4.0/src/getpack/resource.py` & `getpack-0.4.1/src/getpack/resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,381 +1,411 @@
-"""
-Declarative external resources with implicit deployment.
-
-This file is suitable to bundle with projects so they would bootstrap *getpack*
-and install it from pypi, then use full set of functions.
-
-
-Copyright (c) 2022 Konstantin Maslyuk. All rights reserved.
-
-This work is licensed under the terms of the MIT license.
-For a copy, see <https://opensource.org/licenses/MIT>.
-"""
-
-import certifi
-import json
-import os
-from pathlib import Path
-import random
-import re
-import shutil
-import sys
-import threading
-import typing  # noqa: F401
-
-import fasteners
-from six.moves import urllib
-
-from .extraction import TarExtractor, ZipExtractor
-
-
-if sys.version_info.major >= 3:
-    __py_implementation__ = sys.implementation.name
-else:
-    __py_implementation__ = 'cpython'
-
-
-class HybridLock:
-    def __init__(self, key):
-        self.key = key.as_posix() + '.lock'
-        self.folder = os.path.dirname(self.key)
-        self.file_lock = fasteners.InterProcessLock(self.key)
-        self.lock = threading.RLock()
-        self.counter = 0
-
-    def __enter__(self):
-        self.lock.acquire()
-
-        # no more single thread now can access here
-        self.counter += 1
-        if self.counter == 1:
-            if not os.path.isdir(self.folder):
-                try:
-                    os.makedirs(self.folder)
-                except OSError:
-                    pass  # may fail because of race
-            try:
-                self.file_lock.acquire()
-            except Exception:
-                # attempt to fix rare PermissionError in multi process races,
-                # maybe timeout? Have no info on effectiveness of following
-                # code
-                self.file_lock.acquire()
-
-    def __exit__(self, *_):
-        self.counter -= 1
-        if not self.counter:
-            self.file_lock.release()
-            try:
-                os.unlink(self.key)
-            except Exception:
-                pass
-        self.lock.release()
-
-
-def lock(key, _locks={None: threading.Lock()}):
-    with _locks[None]:
-        if key not in _locks:
-            _locks[key] = HybridLock(key)
-    return _locks[key]
-
-
-def _logging(*args):
-    print(args[0] % args[1:])
-
-
-def _logging_off(*args):
-    pass
-
-
-info = _logging_off
-debug = info
-
-
-class Base(object):
-
-    def __init__(self, **kwargs):
-        """
-        Initialization is not heavy operation, feel free to construct a
-        Resource and query available versions.
-        """
-        for k, v in kwargs.items():
-            if v is not None:
-                setattr(self, k, v)
-
-
-class Resource(Base):
-    """Base resource."""
-    _available = False
-    name = ''
-    path = None  # type: Path
-    version = None  # type: str
-
-    @property
-    def lock(self):
-        return lock(self.path)
-
-    def get_available_versions(self):  # type: () -> typing.List[str]
-        """Get list of available versions."""
-        raise NotImplementedError()
-
-    def deploy(self):
-        """
-        This will produce all the hard work to make resource available, but
-        not necessary to make an effect from resource in current environment.
-        This method also will cleanup currently deployed data before the
-        deployment.
-        """
-        raise NotImplementedError
-
-    def provide(self):
-        """Make resource available so it would be immediately used."""
-        if self._available:
-            return
-        assert self.name, 'Resource should be named'
-        assert self.version, 'Resource should be versioned'
-        with self.lock:
-            if self.version in self.get_available_versions():
-                self._available = True
-                return
-            self.deploy()
-            self._available = True
-
-    def __call__(self):
-        self.provide()
-        return self
-
-    def cleanup(self):
-        raise NotImplementedError
-
-
-class LocalResource(Resource):
-    """Locally cached resource."""
-    if sys.platform == 'win32':
-        local_base = Path(os.getenv('APPDATA')) / 'getpack'
-    elif sys.platform == 'linux':
-        local_base = Path(os.environ['HOME']) / '.config' / 'getpack'
-    local_prefix = ''
-    _path = None
-
-    @property
-    def path(self):  # type: () -> Path
-        if self._path is None:
-            self._path = (
-                self.local_base / self.local_prefix / self.name / self.version)
-        return self._path
-
-    def get_available_versions(self):
-        if not self.path.parent.is_dir():
-            return []
-        return [
-            i.name for i in self.path.parent.iterdir()
-            if not i.name.endswith('.temp')
-        ]
-
-    def _deploy_to(self, path):
-        """Obtain resrouce and store in `path`"""
-        raise NotImplementedError
-
-    def deploy(self):
-        self.cleanup()
-        # extract to temporary folder then rename
-        temp_path = None
-        try:
-            for _ in range(100):
-                temp_path = self.path.parent / '{:020x}.temp'.format(
-                    random.randrange(16**20))
-                if not temp_path.is_dir():
-                    temp_path.mkdir(parents=True)
-                    break
-            else:
-                raise Exception(
-                    'Failed to find empty temp dir (last: {})'.format(
-                        temp_path))
-            self._deploy_to(temp_path)
-            if not self.path.parent.is_dir():
-                self.path.parent.mkdir(parents=True)
-            temp_path.rename(self.path)
-        except Exception:
-            if temp_path and temp_path.is_dir():
-                shutil.rmtree(str(temp_path))
-            raise
-
-    def cleanup(self):
-        with self.lock:
-            if self.path.is_dir():
-                info('Cleanup %s', self.path)
-                shutil.rmtree(str(self.path))
-            self._available = False
-
-
-class ArchivedResource(LocalResource):
-    archive_name = ''
-    archive_extraction = {'': {'path': ''}}
-    extractor_plugins = {
-        r'.+\.(whl|zip)$': ZipExtractor,
-        r'.+\.tar(.gz|.xz|.bz)?$': TarExtractor,
-    }
-
-    def get_archive_stream(self):
-        raise NotImplementedError
-
-    def _deploy_to(self, path):
-        assert self.archive_name, (
-            'Property *archive_name* should be defined for {}'.format(self))
-        for k, extractor_cls in self.extractor_plugins.items():
-            if re.match(k, self.archive_name):
-                break
-        else:
-            raise Exception('No extractor for {}'.format(self.archive_name))
-
-        with extractor_cls(self.get_archive_stream()) as extractor:
-            for filename in extractor.get_file_list():
-                dest_path = ''
-                for k, v in self.archive_extraction.items():
-                    k = k.format(self=self)
-                    # TODO add regex
-                    if filename.startswith(k):
-                        dest_path = v['path'] + filename[len(k):]
-                        break
-                else:
-                    continue
-                assert dest_path and dest_path[0] != '/'
-                dest_path = path / dest_path
-                if not dest_path.parent.is_dir():
-                    dest_path.parent.mkdir(parents=True)
-
-                # py2 pathlib.Path does not have write_bytes()
-                with open(str(dest_path), 'wb') as f:
-                    f.write(extractor.get_bytes(filename))
-
-
-class WebResource(ArchivedResource):
-    """Resource from the web."""
-
-    def get_archive_stream(self):
-        archive_url = self.archive_url.format(self=self)
-        info('Downloading %s', archive_url)
-        request = urllib.request.Request(
-            archive_url,
-            data=None,
-            headers={
-                # Blender web resource seems to disallow python user agent
-                'User-Agent': ('Mozilla/5.0 (Macintosh; Intel Mac OS X '
-                               '10_9_3) AppleWebKit/537.36 (KHTML, like '
-                               'Gecko) Chrome/35.0.1916.47 Safari/537.36'),
-            },
-        )
-        response = urllib.request.urlopen(request, cafile=certifi.where())
-        assert response.getcode() in {200}, (
-            'Unexpected status {} for {}'.format(
-                response.getcode(), archive_url))
-        return response
-
-    @property
-    def archive_name(self):
-        return urllib.parse.urlparse(self.archive_url).path.rsplit('/', 1)[1]
-
-
-class PythonPackage(LocalResource):
-    """Python package."""
-    local_prefix = 'python'
-    _activated = False
-    requirements = []  # type: typing.Iterable[Resource]
-    python_tag = '{}{}{}'.format(
-        {
-            'cpython': 'cp',
-        }.get(__py_implementation__, __py_implementation__),
-        sys.version_info.major,
-        sys.version_info.minor,
-    )
-
-    def __init__(self, name=None, version=None, **kwargs):
-        if name:
-            kwargs['name'] = name
-        if version:
-            kwargs['version'] = version
-        super(PythonPackage, self).__init__(**kwargs)
-        if self.python_tag:
-            self.local_prefix += '/' + self.python_tag
-
-    def provide(self):
-        for r in self.requirements:
-            r.provide()
-        super(PythonPackage, self).provide()
-        if str(self.path) not in sys.path:
-            sys.path.insert(0, str(self.path))
-
-    def activate(self):
-        if self._activated:
-            return
-        self.provide()
-        [r.activate() for r in self.requirements]
-        __import__(self.name)
-        self._activated = True
-
-    def get(self, name=None):
-        name = name or self.name
-        self.activate()
-        __import__(name)
-        return sys.modules[name]
-
-    def __call__(self, name=None):
-        return self.get(name=name)
-
-
-class WebPythonPackage(PythonPackage, WebResource):
-    """Python package from the web."""
-
-
-WebPackage = WebPythonPackage  # TODO deprecated
-
-
-class PyPiPackage(WebPythonPackage):
-    _archive_url = ''
-    _release_info = None
-
-    @property
-    def release_info(self):
-        if self._release_info is None:
-            request = urllib.request.urlopen(
-                'https://pypi.org/pypi/{}/json'.format(self.name))
-            data = json.loads(request.read())
-            releases = data['releases'][self.version]
-            debug('Available releases:\n\t%s', '\n\t'.join(
-                r['filename'] for r in data['releases'][self.version]))
-            platform = 'win_amd64'
-            if (len(releases) == 1
-                    and releases[0]['python_version'] == 'source'):
-                pass
-            else:
-                releases = [
-                    r for r in releases
-                    if platform in r['filename']
-                    or re.search(r'\Wany\W', r['filename'])
-                ]
-            if self.python_tag:
-                # python_version looks as `cp39.cp310.cp311` or `py2.py3`
-                supported_versions = {self.python_tag, 'source'}
-                if self.python_tag.startswith('cp3'):
-                    supported_versions.add('py3')
-                if self.python_tag.startswith('cp2'):
-                    supported_versions.add('py2')
-                releases = [
-                    r for r in releases if 'python_version' not in r
-                    or supported_versions & set(r['python_version'].split('.'))
-                ]
-            # TODO improve release selection
-            assert len(
-                releases) >= 1, 'No unique release available from {}'.format(
-                    ', '.join(r['filename'] +
-                              (' (selected)' if r in releases else '')
-                              for r in data['releases'][self.version]))
-            self._release_info = releases[0]
-        return self._release_info
-
-    @property
-    def archive_url(self):
-        if not self._archive_url:
-            # TODO save and check digest
-            self._archive_url = self.release_info['url']
-        return self._archive_url
+"""
+Declarative external resources with implicit deployment.
+
+This file is suitable to bundle with projects so they would bootstrap *getpack*
+and install it from pypi, then use full set of functions.
+
+
+Copyright (c) 2022 Konstantin Maslyuk. All rights reserved.
+
+This work is licensed under the terms of the MIT license.
+For a copy, see <https://opensource.org/licenses/MIT>.
+"""
+
+import json
+import os
+import random
+import re
+import shutil
+import sys
+import threading
+import time
+import typing  # noqa: F401
+from pathlib import Path
+
+import certifi
+import fasteners
+from six.moves import urllib
+
+from .extraction import TarExtractor, ZipExtractor
+
+if sys.version_info.major >= 3:
+    __py_implementation__ = sys.implementation.name
+else:
+    __py_implementation__ = 'cpython'
+
+
+class HybridLock:
+    def __init__(self, key):
+        self.key = key.as_posix() + '.lock'
+        self.folder = os.path.dirname(self.key)
+        self.file_lock = fasteners.InterProcessLock(self.key)
+        self.lock = threading.RLock()
+        self.counter = 0
+
+    def __enter__(self):
+        self.lock.acquire()
+
+        # no more single thread now can access here
+        self.counter += 1
+        if self.counter == 1:
+            if not os.path.isdir(self.folder):
+                try:
+                    os.makedirs(self.folder)
+                except OSError:
+                    pass  # may fail because of race
+            try:
+                self.file_lock.acquire()
+            except Exception:
+                # attempt to fix rare PermissionError in multi process races,
+                # maybe timeout? Have no info on effectiveness of following
+                # code
+                self.file_lock.acquire()
+
+    def __exit__(self, *_):
+        self.counter -= 1
+        if not self.counter:
+            self.file_lock.release()
+            try:
+                os.unlink(self.key)
+            except Exception:
+                pass
+        self.lock.release()
+
+
+def lock(key, _locks={None: threading.Lock()}):
+    with _locks[None]:
+        if key not in _locks:
+            _locks[key] = HybridLock(key)
+    return _locks[key]
+
+
+def _logging(*args):
+    print(args[0] % args[1:])
+
+
+def _logging_off(*args):
+    pass
+
+
+info = _logging_off
+debug = info
+
+
+def retry(func, retries=None, backoff=None, exceptions=(Exception, )):
+    if retries is None:
+        if 'GETPACK_RETRIES' in os.environ:
+            retries = int(os.getenv('GETPACK_RETRIES'))
+        else:
+            retries = 50
+    if backoff is None:
+        if 'GETPACK_BACKOFF' in os.environ:
+            backoff = float(os.getenv('GETPACK_BACKOFF'))
+        else:
+            backoff = 0.1
+
+    def wrapped(*args, **kwargs):
+        for i in reversed(range(retries)):
+            try:
+                return func(*args, **kwargs)
+            except exceptions:
+                if not i:
+                    raise
+                time.sleep(backoff)
+
+    return wrapped
+
+
+class Base(object):
+
+    def __init__(self, **kwargs):
+        """
+        Initialization is not heavy operation, feel free to construct a
+        Resource and query available versions.
+        """
+        for k, v in kwargs.items():
+            if v is not None:
+                setattr(self, k, v)
+
+
+class Resource(Base):
+    """Base resource."""
+    _available = False
+    name = ''
+    path = None  # type: Path
+    version = None  # type: str
+
+    @property
+    def lock(self):
+        return lock(self.path)
+
+    def get_available_versions(self):  # type: () -> typing.List[str]
+        """Get list of available versions."""
+        raise NotImplementedError()
+
+    def deploy(self):
+        """
+        This will produce all the hard work to make resource available, but
+        not necessary to make an effect from resource in current environment.
+        This method also will cleanup currently deployed data before the
+        deployment.
+        """
+        raise NotImplementedError
+
+    def provide(self):
+        """Make resource available so it would be immediately used."""
+        if self._available:
+            return
+        assert self.name, 'Resource should be named'
+        assert self.version, 'Resource should be versioned'
+        with self.lock:
+            if self.version in self.get_available_versions():
+                self._available = True
+                return
+            self.deploy()
+            self._available = True
+
+    def __call__(self):
+        self.provide()
+        return self
+
+    def cleanup(self):
+        raise NotImplementedError
+
+
+class LocalResource(Resource):
+    """Locally cached resource."""
+    if sys.platform == 'win32':
+        local_base = Path(os.getenv('APPDATA')) / 'getpack'
+    elif sys.platform == 'linux':
+        local_base = Path(os.environ['HOME']) / '.config' / 'getpack'
+    local_prefix = ''
+    _path = None
+
+    @property
+    def path(self):  # type: () -> Path
+        if self._path is None:
+            self._path = (self.local_base / self.local_prefix / self.name /
+                          self.version)
+        return self._path
+
+    @path.setter
+    def path(self, value):
+        self._path = value
+
+    def get_available_versions(self):
+        if not self.path.parent.is_dir():
+            return []
+        return [
+            i.name for i in self.path.parent.iterdir()
+            if not i.name.endswith('.temp')
+        ]
+
+    def _deploy_to(self, path):
+        """Obtain resrouce and store in `path`"""
+        raise NotImplementedError
+
+    def deploy(self):
+        self.cleanup()
+        # extract to temporary folder then rename
+        temp_path = None
+        try:
+            for _ in range(100):
+                temp_path = self.path.parent / '{:020x}.temp'.format(
+                    random.randrange(16**20))
+                if not temp_path.is_dir():
+                    temp_path.mkdir(parents=True)
+                    break
+            else:
+                raise Exception(
+                    'Failed to find empty temp dir (last: {})'.format(
+                        temp_path))
+            self._deploy_to(temp_path)
+            if not self.path.parent.is_dir():
+                self.path.parent.mkdir(parents=True)
+            retry(temp_path.rename, exceptions=(PermissionError, ))(self.path)
+        except Exception:
+            if temp_path and temp_path.is_dir():
+                retry(shutil.rmtree,
+                      exceptions=(PermissionError, ))(str(temp_path))
+            raise
+
+    def cleanup(self):
+        with self.lock:
+            if self.path.is_dir():
+                info('Cleanup %s', self.path)
+                retry(shutil.rmtree,
+                      exceptions=(PermissionError, ))(str(self.path))
+            self._available = False
+
+
+class ArchivedResource(LocalResource):
+    archive_name = ''
+    archive_extraction = {'': {'path': ''}}
+    extractor_plugins = {
+        r'.+\.(whl|zip)$': ZipExtractor,
+        r'.+\.tar(.gz|.xz|.bz)?$': TarExtractor,
+    }
+
+    def get_archive_stream(self):
+        raise NotImplementedError
+
+    def _deploy_to(self, path):
+        assert self.archive_name, (
+            'Property *archive_name* should be defined for {}'.format(self))
+        for k, extractor_cls in self.extractor_plugins.items():
+            if re.match(k, self.archive_name):
+                break
+        else:
+            raise Exception('No extractor for {}'.format(self.archive_name))
+
+        with extractor_cls(self.get_archive_stream()) as extractor:
+            for filename in extractor.get_file_list():
+                dest_path = ''
+                for k, v in self.archive_extraction.items():
+                    k = k.format(self=self)
+                    # TODO add regex
+                    if filename.startswith(k):
+                        dest_path = v['path'] + filename[len(k):]
+                        break
+                else:
+                    continue
+                assert dest_path and dest_path[0] != '/'
+                dest_path = path / dest_path
+                if not dest_path.parent.is_dir():
+                    dest_path.parent.mkdir(parents=True)
+
+                # py2 pathlib.Path does not have write_bytes()
+                with open(str(dest_path), 'wb') as f:
+                    f.write(extractor.get_bytes(filename))
+
+
+class WebResource(ArchivedResource):
+    """Resource from the web."""
+
+    def get_archive_stream(self):
+        archive_url = self.archive_url.format(self=self)
+        info('Downloading %s', archive_url)
+        request = urllib.request.Request(
+            archive_url,
+            data=None,
+            headers={
+                # Blender web resource seems to disallow python user agent
+                'User-Agent': ('Mozilla/5.0 (Macintosh; Intel Mac OS X '
+                               '10_9_3) AppleWebKit/537.36 (KHTML, like '
+                               'Gecko) Chrome/35.0.1916.47 Safari/537.36'),
+            },
+        )
+        response = urllib.request.urlopen(request, cafile=certifi.where())
+        assert response.getcode() in {200}, (
+            'Unexpected status {} for {}'.format(
+                response.getcode(), archive_url))
+        return response
+
+    @property
+    def archive_name(self):
+        return urllib.parse.urlparse(self.archive_url).path.rsplit('/', 1)[1]
+
+
+class PythonPackage(LocalResource):
+    """Python package."""
+    local_prefix = 'python'
+    _activated = False
+    requirements = []  # type: typing.Iterable[Resource]
+    python_tag = '{}{}{}'.format(
+        {
+            'cpython': 'cp',
+        }.get(__py_implementation__, __py_implementation__),
+        sys.version_info.major,
+        sys.version_info.minor,
+    )
+
+    def __init__(self, name=None, version=None, **kwargs):
+        if name:
+            kwargs['name'] = name
+        if version:
+            kwargs['version'] = version
+        super(PythonPackage, self).__init__(**kwargs)
+        if self.python_tag:
+            self.local_prefix += '/' + self.python_tag
+
+    def provide(self):
+        for r in self.requirements:
+            r.provide()
+        super(PythonPackage, self).provide()
+        if str(self.path) not in sys.path:
+            sys.path.insert(0, str(self.path))
+
+    def activate(self):
+        if self._activated:
+            return
+        self.provide()
+        [r.activate() for r in self.requirements]
+        __import__(self.name)
+        self._activated = True
+
+    def get(self, name=None):
+        name = name or self.name
+        self.activate()
+        __import__(name)
+        return sys.modules[name]
+
+    def __call__(self, name=None):
+        return self.get(name=name)
+
+
+class WebPythonPackage(PythonPackage, WebResource):
+    """Python package from the web."""
+
+
+WebPackage = WebPythonPackage  # TODO deprecated
+
+
+class PyPiPackage(WebPythonPackage):
+    _archive_url = ''
+    _release_info = None
+
+    @property
+    def release_info(self):
+        if self._release_info is None:
+            request = urllib.request.urlopen(
+                'https://pypi.org/pypi/{}/json'.format(self.name))
+            data = json.loads(request.read())
+            releases = data['releases'][self.version]
+            debug('Available releases:\n\t%s', '\n\t'.join(
+                r['filename'] for r in data['releases'][self.version]))
+            platform = 'win_amd64'
+            if (len(releases) == 1
+                    and releases[0]['python_version'] == 'source'):
+                pass
+            else:
+                releases = [
+                    r for r in releases
+                    if platform in r['filename']
+                    or re.search(r'\Wany\W', r['filename'])
+                ]
+            if self.python_tag:
+                # python_version looks as `cp39.cp310.cp311` or `py2.py3`
+                supported_versions = {self.python_tag, 'source'}
+                if self.python_tag.startswith('cp3'):
+                    supported_versions.add('py3')
+                if self.python_tag.startswith('cp2'):
+                    supported_versions.add('py2')
+                releases = [
+                    r for r in releases if 'python_version' not in r
+                    or supported_versions & set(r['python_version'].split('.'))
+                ]
+            # TODO improve release selection
+            assert len(
+                releases) >= 1, 'No unique release available from {}'.format(
+                    ', '.join(r['filename'] +
+                              (' (selected)' if r in releases else '')
+                              for r in data['releases'][self.version]))
+            self._release_info = releases[0]
+        return self._release_info
+
+    @property
+    def archive_url(self):
+        if not self._archive_url:
+            # TODO save and check digest
+            self._archive_url = self.release_info['url']
+        return self._archive_url
```

### Comparing `getpack-0.4.0/src/getpack.egg-info/PKG-INFO` & `getpack-0.4.1/src/getpack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.4.0
+Version: 0.4.1
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Platform: UNKNOWN
@@ -53,8 +53,13 @@
 
 - Utilize `requirements.txt` to reproduce both development and production
   environments.
 
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
 
+### Environs
+* `GETPACK_RETRIES` - int, number of general retries, used for renaming and
+    removing temporary folders
+* `GETPACK_BACKOFF` - float, delay between retires
+
```

### Comparing `getpack-0.4.0/tests/test_common.py` & `getpack-0.4.1/tests/test_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from getpack import library, resource
 import pytest
 
 
-def test_cefpython3(temp_folder):
+def test_cefpython3(temp_folder, background_scanner):
     cefpython3 = resource.WebPackage(
         name='cefpython3',
         archive_url=(
             'https://files.pythonhosted.org/packages/3b/d4/f313221a999e4d295'
             'cc8fcb15fc4ac9c98f6759e50735d6f6ce84fd3e98a/'
             'cefpython3-66.1-py2.py3-none-win_amd64.whl'),
         version='66.1',
@@ -22,15 +22,15 @@
         sys.version_info < (3,), reason='PySide2 available for Py3 only')
 def test_pyside2():
     PySide2 = library.PySide2()
     PySide2.cleanup()
     assert PySide2().__version__ == PySide2.version
 
 
-def test_cefpython3_pypi(temp_folder):
+def test_cefpython3_pypi(temp_folder, background_scanner):
     cefpython3 = library.CefPython3(local_base=temp_folder)
     assert not cefpython3._activated
     cefpython3.cleanup()
     assert not cefpython3._activated
     assert cefpython3().__version__ == cefpython3.version
     assert cefpython3._activated
 
@@ -43,15 +43,15 @@
         'flag set')
     blender.cleanup()
     blender.provide()
     output = blender('--version')
     assert version in output.decode()
 
 
-def test_parent_folders_exists(temp_folder):
+def test_parent_folders_exists(temp_folder, background_scanner):
     python = library.Python(local_base=temp_folder)
     assert python.version.encode() in python('--version')
 
 
 def test_numpy():
     package = resource.PyPiPackage(
         'numpy', '1.11.2' if sys.version_info < (3, ) else '1.23.1')
```

