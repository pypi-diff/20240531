# Comparing `tmp/pypath_common-0.2.0.tar.gz` & `tmp/pypath_common-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypath_common-0.2.0.tar", max compression
+gzip compressed data, was "pypath_common-0.2.2.tar", max compression
```

## Comparing `pypath_common-0.2.0.tar` & `pypath_common-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35141 2022-06-03 17:25:14.594620 pypath_common-0.2.0/LICENSE
--rw-r--r--   0        0        0      252 2022-06-03 00:06:10.880106 pypath_common-0.2.0/README.rst
--rw-r--r--   0        0        0      990 2023-11-30 09:26:44.143756 pypath_common-0.2.0/pypath_common/__init__.py
--rw-r--r--   0        0        0     1380 2023-11-30 09:25:10.093750 pypath_common-0.2.0/pypath_common/_constants.py
--rw-r--r--   0        0        0     7555 2023-11-24 16:54:30.917695 pypath_common-0.2.0/pypath_common/_logger.py
--rw-r--r--   0        0        0    73105 2023-11-24 23:21:25.749119 pypath_common-0.2.0/pypath_common/_misc.py
--rw-r--r--   0        0        0    11777 2023-11-25 00:45:26.122761 pypath_common-0.2.0/pypath_common/_session.py
--rw-r--r--   0        0        0    13712 2023-11-24 22:05:10.425505 pypath_common-0.2.0/pypath_common/_settings.py
--rw-r--r--   0        0        0      868 2023-11-24 21:27:49.352034 pypath_common-0.2.0/pypath_common/data/__init__.py
--rw-r--r--   0        0        0     4048 2023-11-25 00:47:56.866104 pypath_common-0.2.0/pypath_common/data/_data.py
--rw-r--r--   0        0        0      168 2022-06-05 00:03:34.184119 pypath_common-0.2.0/pypath_common/data/aacodes.yaml
--rw-r--r--   0        0        0      256 2022-06-05 00:05:23.303603 pypath_common-0.2.0/pypath_common/data/aanames.yaml
--rw-r--r--   0        0        0     1300 2022-06-05 16:38:10.443912 pypath_common-0.2.0/pypath_common/data/amino_acids.yaml
--rw-r--r--   0        0        0       74 2023-11-25 22:36:02.368818 pypath_common-0.2.0/pypath_common/data/idtypes/array.yaml
--rw-r--r--   0        0        0      657 2023-11-25 16:48:36.214207 pypath_common-0.2.0/pypath_common/data/idtypes/biomart.yaml
--rw-r--r--   0        0        0      275 2023-11-25 16:52:19.030887 pypath_common-0.2.0/pypath_common/data/idtypes/hmdb.yaml
--rw-r--r--   0        0        0      436 2023-11-25 16:49:15.717543 pypath_common-0.2.0/pypath_common/data/idtypes/pro.yaml
--rw-r--r--   0        0        0      147 2023-11-25 16:41:51.730849 pypath_common-0.2.0/pypath_common/data/idtypes/ramp.yaml
--rw-r--r--   0        0        0      278 2023-11-25 16:46:48.937534 pypath_common-0.2.0/pypath_common/data/idtypes/uniprot.yaml
--rw-r--r--   0        0        0      386 2023-11-25 16:47:51.197537 pypath_common-0.2.0/pypath_common/data/idtypes/uniprot_idmapping.yaml
--rw-r--r--   0        0        0      209 2022-06-05 15:04:26.367850 pypath_common-0.2.0/pypath_common/data/igraph_graphics_attrs.yaml
--rw-r--r--   0        0        0     3997 2022-06-05 15:04:26.407848 pypath_common-0.2.0/pypath_common/data/mod_keywords.yaml
--rw-r--r--   0        0        0     2110 2022-06-05 16:38:10.453912 pypath_common-0.2.0/pypath_common/data/pmod_bel.yaml
--rw-r--r--   0        0        0      348 2022-06-05 16:38:10.433913 pypath_common-0.2.0/pypath_common/data/psite_mod_types.yaml
--rw-r--r--   0        0        0      856 2022-06-05 16:38:10.457245 pypath_common-0.2.0/pypath_common/data/psite_mod_types2.yaml
--rw-r--r--   0        0        0     6454 2023-11-20 22:31:55.702641 pypath_common-0.2.0/pypath_common/data/settings.yaml
--rw-r--r--   0        0        0     3812 2023-11-30 09:26:44.143756 pypath_common-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pypath_common-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2022-06-03 17:25:14.594620 pypath_common-0.2.2/LICENSE
+-rw-r--r--   0        0        0      252 2022-06-03 00:06:10.880106 pypath_common-0.2.2/README.rst
+-rw-r--r--   0        0        0      990 2024-05-31 08:19:00.620058 pypath_common-0.2.2/pypath_common/__init__.py
+-rw-r--r--   0        0        0     1380 2023-11-30 09:25:10.093750 pypath_common-0.2.2/pypath_common/_constants.py
+-rw-r--r--   0        0        0     7760 2024-05-31 00:41:45.306879 pypath_common-0.2.2/pypath_common/_logger.py
+-rw-r--r--   0        0        0    73105 2023-11-24 23:21:25.749119 pypath_common-0.2.2/pypath_common/_misc.py
+-rw-r--r--   0        0        0    11868 2024-05-30 23:43:05.393329 pypath_common-0.2.2/pypath_common/_session.py
+-rw-r--r--   0        0        0    13712 2023-11-24 22:05:10.425505 pypath_common-0.2.2/pypath_common/_settings.py
+-rw-r--r--   0        0        0      868 2023-11-24 21:27:49.352034 pypath_common-0.2.2/pypath_common/data/__init__.py
+-rw-r--r--   0        0        0     4048 2023-11-25 00:47:56.866104 pypath_common-0.2.2/pypath_common/data/_data.py
+-rw-r--r--   0        0        0      168 2022-06-05 00:03:34.184119 pypath_common-0.2.2/pypath_common/data/aacodes.yaml
+-rw-r--r--   0        0        0      256 2022-06-05 00:05:23.303603 pypath_common-0.2.2/pypath_common/data/aanames.yaml
+-rw-r--r--   0        0        0     1300 2022-06-05 16:38:10.443912 pypath_common-0.2.2/pypath_common/data/amino_acids.yaml
+-rw-r--r--   0        0        0       74 2023-11-25 22:36:02.368818 pypath_common-0.2.2/pypath_common/data/idtypes/array.yaml
+-rw-r--r--   0        0        0      657 2023-11-25 16:48:36.214207 pypath_common-0.2.2/pypath_common/data/idtypes/biomart.yaml
+-rw-r--r--   0        0        0      275 2023-11-25 16:52:19.030887 pypath_common-0.2.2/pypath_common/data/idtypes/hmdb.yaml
+-rw-r--r--   0        0        0      436 2023-11-25 16:49:15.717543 pypath_common-0.2.2/pypath_common/data/idtypes/pro.yaml
+-rw-r--r--   0        0        0      147 2023-11-25 16:41:51.730849 pypath_common-0.2.2/pypath_common/data/idtypes/ramp.yaml
+-rw-r--r--   0        0        0      278 2023-11-25 16:46:48.937534 pypath_common-0.2.2/pypath_common/data/idtypes/uniprot.yaml
+-rw-r--r--   0        0        0      386 2023-11-25 16:47:51.197537 pypath_common-0.2.2/pypath_common/data/idtypes/uniprot_idmapping.yaml
+-rw-r--r--   0        0        0      209 2022-06-05 15:04:26.367850 pypath_common-0.2.2/pypath_common/data/igraph_graphics_attrs.yaml
+-rw-r--r--   0        0        0     3997 2022-06-05 15:04:26.407848 pypath_common-0.2.2/pypath_common/data/mod_keywords.yaml
+-rw-r--r--   0        0        0     2110 2022-06-05 16:38:10.453912 pypath_common-0.2.2/pypath_common/data/pmod_bel.yaml
+-rw-r--r--   0        0        0      348 2022-06-05 16:38:10.433913 pypath_common-0.2.2/pypath_common/data/psite_mod_types.yaml
+-rw-r--r--   0        0        0      856 2022-06-05 16:38:10.457245 pypath_common-0.2.2/pypath_common/data/psite_mod_types2.yaml
+-rw-r--r--   0        0        0     6454 2024-03-22 14:31:31.160585 pypath_common-0.2.2/pypath_common/data/settings.yaml
+-rw-r--r--   0        0        0     3797 2024-05-31 08:19:00.616725 pypath_common-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1493 1970-01-01 00:00:00.000000 pypath_common-0.2.2/PKG-INFO
```

### Comparing `pypath_common-0.2.0/LICENSE` & `pypath_common-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/__init__.py` & `pypath_common-0.2.2/pypath_common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """
 Code shared across pypath modules.
 """
 
 __author__ = ', '.join(['Dénes Türei'])
 __maintainer__ = ', '.join(['Dénes Türei'])
-__version__ = '0.2.0'
+__version__ = '0.2.2'
 __email__ = 'turei.denes@gmail.com'
 
 from pypath_common import data
 from pypath_common import _misc as misc  # noqa: F401
 from pypath_common import _constants as const
 from pypath_common._session import Logger, log, logger, session  # noqa: F401
```

### Comparing `pypath_common-0.2.0/pypath_common/_constants.py` & `pypath_common-0.2.2/pypath_common/_constants.py`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/_logger.py` & `pypath_common-0.2.2/pypath_common/_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,25 +22,21 @@
 #
 
 from typing import TYPE_CHECKING, Optional
 import os
 import sys
 import time
 import pydoc
-import datetime
 import textwrap
+import threading
 
-import timeloop
+from . import _misc
 
 __all__ = ['new_logger', 'Logger']
 
-
-_log_flush_timeloop = timeloop.Timeloop()
-_log_flush_timeloop.logger.setLevel(9999)
-
 if TYPE_CHECKING:
 
     from ._settings import Settings
 
 
 def new_logger(
     name: str,
@@ -116,45 +112,51 @@
             console_level:
                 Messages below this log level will be printed not only into
                 logfile but also to the console.
             max_width:
                 Maximum line width (longer lines will be wrapped).
         """
 
-        @_log_flush_timeloop.job(
-            interval = datetime.timedelta(
-                seconds = settings.get('log_flush_interval'),
-            ),
-        )
-        def _flush():
-
-            self.flush()
-
-        _log_flush_timeloop.start(block = False)
-
         self.settings = settings
         self.wrapper = textwrap.TextWrapper(
             width = max_width,
             subsequent_indent = ' ' * 22,
             break_long_words = False,
         )
         self.logdir = self.get_logdir(logdir)
         self.fname = os.path.join(self.logdir, fname)
         self.verbosity = (
             verbosity
             if verbosity is not None
-            else self.settings.get('log_verbosity')
+            else self.settings.get('log_verbosity') or 0
         )
         self.console_level = (
             console_level
             if console_level is not None
-            else self.settings.get('console_verbosity')
+            else self.settings.get('console_verbosity') or -1
         )
         self.open_logfile()
 
+        flush_interval = settings.get('log_flush_interval') or 1
+
+        def _flush(stop):
+
+            while not stop.wait(flush_interval):
+
+                self.flush()
+
+
+        self._flush_thread_kill = threading.Event()
+        self._flush_thread = threading.Thread(
+            target = _flush,
+            args = (self._flush_thread_kill,),
+            daemon = True,
+        )
+        self._flush_thread.start()
+
         # sending some greetings
         self.msg('Welcome!')
         self.msg('Logger started, logging into `%s`.' % self.fname)
 
     def msg(
         self,
         msg: str = '',
@@ -234,34 +236,34 @@
 
         return cls.strftime('%Y-%m-%d %H:%M:%S')
 
     def __del__(self):
         """
         Clean up before destroying this instance.
 
-        Especially, shut down the timeloop and close the logfile.
+        Especially, shut down the flushing thread and close the logfile.
         """
 
-        if hasattr(_log_flush_timeloop, 'stop'):
-
-            _log_flush_timeloop.stop()
-
         self.msg('Logger shut down, logfile `%s` closed.' % self.fname)
         self.msg('Bye.')
         self.close_logfile()
 
     def get_logdir(self, dirname = None):
         """
         Path to the log directory.
 
         Returns the path to log directory, creates the directory if it does
         not exist.
         """
 
-        dirname = dirname or '%s_log' % self.settings.get('module_name')
+        dirname = (
+            dirname or
+            '%s_log' % self.settings.get('module_name') or
+            _misc.caller_module()
+        )
 
         if not os.path.exists(dirname):
             os.makedirs(dirname)
 
         return os.path.abspath(dirname)
 
     def open_logfile(self):
@@ -274,14 +276,19 @@
         self.fp = open(self.fname, 'wb')
 
     def close_logfile(self):
         """
         Closes the log file.
         """
 
+        if kill := getattr(self, '_flush_thread_kill', False):
+
+            kill.set()
+            self._flush_thread.join()
+
         if hasattr(self, 'fp') and not self.fp.closed:
 
             self.fp.close()
 
     def flush(self):
         """
         Flushes the log file.
```

### Comparing `pypath_common-0.2.0/pypath_common/_misc.py` & `pypath_common-0.2.2/pypath_common/_misc.py`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/_session.py` & `pypath_common-0.2.2/pypath_common/_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,25 +126,28 @@
     def start_logger(self):
         """
         Start the logger.
 
         Creates a logger for this session which will be served to all modules.
         """
 
+        env_var = f'{self.module.upper()}_LOG'
+
         self.logfile = str(
-            os.getenv('PYPATH_LOG') or
-            getattr(builtins, 'PYPATH_LOG', None) or
-            'pypath-%s.log' % self.label,
+            os.getenv(env_var) or
+            getattr(builtins, env_var, None) or
+            f'{self.module}-{self.label}.log',
         )
+        logdir = os.path.dirname(self.logfile) or f'{self.module}_log'
 
         self._logger = _logger.Logger(
             fname = os.path.basename(self.logfile),
             settings = self.config,
             verbosity = self.log_verbosity,
-            logdir = os.path.dirname(self.logfile),
+            logdir = logdir,
         )
         self._managed_loggers = {}
 
 
     def finish_logger(self):
         """
         Close the logger.
```

### Comparing `pypath_common-0.2.0/pypath_common/_settings.py` & `pypath_common-0.2.2/pypath_common/_settings.py`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/__init__.py` & `pypath_common-0.2.2/pypath_common/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/_data.py` & `pypath_common-0.2.2/pypath_common/data/_data.py`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/amino_acids.yaml` & `pypath_common-0.2.2/pypath_common/data/amino_acids.yaml`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/idtypes/biomart.yaml` & `pypath_common-0.2.2/pypath_common/data/idtypes/biomart.yaml`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/mod_keywords.yaml` & `pypath_common-0.2.2/pypath_common/data/mod_keywords.yaml`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/pmod_bel.yaml` & `pypath_common-0.2.2/pypath_common/data/pmod_bel.yaml`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/psite_mod_types2.yaml` & `pypath_common-0.2.2/pypath_common/data/psite_mod_types2.yaml`

 * *Files identical despite different names*

### Comparing `pypath_common-0.2.0/pypath_common/data/settings.yaml` & `pypath_common-0.2.2/pypath_common/data/settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 genecards_datasheet_timeout: 20
 curl_connect_timeout: 10
 curl_timeout: 120
 curl_extended_timeout: 1200
 curl_retries: 3
 user_agent: 'User-Agent: Mozilla/5.0 (X11; U; Linux i686; en-US; rv:54.0) Gecko/20110304 Firefox/54.0'
 msigdb_email: omnipathdb@gmail.com
-msigdb_version: '2023.1'
+msigdb_version: '2023.2'
 
 # Module settings
 network_expand_complexes: false
 network_allow_loops: false
 network_keep_original_names: true
 network_pickle_cache: true
 network_load_resource_attempts: 3
```

### Comparing `pypath_common-0.2.0/pyproject.toml` & `pypath_common-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pypath_common"
-version = "0.2.0"
+version = "0.2.2"
 description = "Code shared across pypath modules"
 license = "GPL-3.0-only"
 authors = [
     "Denes Turei <turei.denes@gmail.com>"
 ]
 packages = [
     { include = "pypath_common" }
@@ -28,15 +28,14 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "*"
 platformdirs = "*"
 psutil = "*"
 tabulate = "*"
-timeloop = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0"
 tox = ">=3.20.1"
 pre-commit = ">=2.17.0"
 bump2version = "*"
 coverage = ">=6.0"
```

### Comparing `pypath_common-0.2.0/PKG-INFO` & `pypath_common-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pypath-common
-Version: 0.2.0
+Name: pypath_common
+Version: 0.2.2
 Summary: Code shared across pypath modules
 Home-page: https://github.com/saezlab/pypath-common
 License: GPL-3.0-only
 Author: Denes Turei
 Author-email: turei.denes@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: psutil
 Requires-Dist: tabulate
-Requires-Dist: timeloop
 Project-URL: Bug Tracker, https://github.com/saezlab/pypath-common/issues
 Project-URL: Repository, https://github.com/saezlab/pypath-common
 Description-Content-Type: text/x-rst
 
 #################################
 Code shared across pypath modules
 #################################
```

