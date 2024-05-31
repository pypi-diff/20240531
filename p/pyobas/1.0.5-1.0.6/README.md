# Comparing `tmp/pyobas-1.0.5.tar.gz` & `tmp/pyobas-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.5.tar", last modified: Wed May 29 19:55:33 2024, max compression
+gzip compressed data, was "pyobas-1.0.6.tar", last modified: Thu May 30 13:58:34 2024, max compression
```

## Comparing `pyobas-1.0.5.tar` & `pyobas-1.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.364380 pyobas-1.0.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-29 19:55:21.000000 pyobas-1.0.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-29 19:55:33.364380 pyobas-1.0.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-29 19:55:21.000000 pyobas-1.0.5/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.356379 pyobas-1.0.5/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/inject_expectation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15283 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-29 19:55:33.364380 pyobas-1.0.5/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.299619 pyobas-1.0.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-30 13:58:20.000000 pyobas-1.0.6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-30 13:58:34.299619 pyobas-1.0.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-30 13:58:20.000000 pyobas-1.0.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.291618 pyobas-1.0.6/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.295618 pyobas-1.0.6/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/inject_expectation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.295618 pyobas-1.0.6/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.295618 pyobas-1.0.6/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15494 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 13:58:34.295618 pyobas-1.0.6/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-30 13:58:34.000000 pyobas-1.0.6/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-30 13:58:34.000000 pyobas-1.0.6/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-30 13:58:34.000000 pyobas-1.0.6/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-30 13:58:34.000000 pyobas-1.0.6/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-30 13:58:34.000000 pyobas-1.0.6/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-30 13:58:20.000000 pyobas-1.0.6/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-30 13:58:34.299619 pyobas-1.0.6/setup.cfg
```

### Comparing `pyobas-1.0.5/LICENSE` & `pyobas-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/PKG-INFO` & `pyobas-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobas-1.0.5/README.md` & `pyobas-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/__init__.py` & `pyobas-1.0.6/pyobas/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.5/pyobas/apis/__init__.py` & `pyobas-1.0.6/pyobas/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/attack_pattern.py` & `pyobas-1.0.6/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/collector.py` & `pyobas-1.0.6/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/document.py` & `pyobas-1.0.6/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/inject.py` & `pyobas-1.0.6/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/inject_expectation.py` & `pyobas-1.0.6/pyobas/apis/inject_expectation.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/injector.py` & `pyobas-1.0.6/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.6/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/team.py` & `pyobas-1.0.6/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/apis/user.py` & `pyobas-1.0.6/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/backends/backend.py` & `pyobas-1.0.6/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/backends/protocol.py` & `pyobas-1.0.6/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/base.py` & `pyobas-1.0.6/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/client.py` & `pyobas-1.0.6/pyobas/client.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/contracts/contract_builder.py` & `pyobas-1.0.6/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/contracts/contract_config.py` & `pyobas-1.0.6/pyobas/contracts/contract_config.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/contracts/variable_helper.py` & `pyobas-1.0.6/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/exceptions.py` & `pyobas-1.0.6/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/helpers.py` & `pyobas-1.0.6/pyobas/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,16 +260,16 @@
     def ping(self) -> None:
         while not self.exit_event.is_set():
             try:
                 if self.ping_type == "injector":
                     self.api.injector.create(self.config, False)
                 else:
                     self.api.collector.create(self.config, False)
-            except Exception as e:  # pylint: disable=broad-except
-                self.logger.error(str(e))
+            except Exception as err:  # pylint: disable=broad-except
+                self.logger.error("Error pinging the API: " + str(err))
             self.exit_event.wait(40)
 
     def run(self) -> None:
         self.logger.info("Starting PingAlive thread")
         self.ping()
 
     def stop(self) -> None:
@@ -338,29 +338,33 @@
                 self.api, self.config, self.collector_logger, "collector"
             )
             self.ping.start()
         self.listen_queue = None
 
     def _schedule(self, scheduler, message_callback, delay):
         # Execute
-        message_callback()
+        try:
+            message_callback()
+        except Exception as err:  # pylint: disable=broad-except
+            self.collector_logger.error("Error collecting: " + str(err))
+
         # Then schedule the next execution
         scheduler.enter(delay, 1, self._schedule, (scheduler, message_callback, delay))
 
     def schedule(self, message_callback, delay):
         # Start execution directly
         try:
             message_callback()
             now = datetime.now(timezone.utc).isoformat()
             self.api.collector.update(
                 self.config_helper.get_conf("collector_id"),
                 {"collector_last_execution": now},
             )
         except Exception as err:  # pylint: disable=broad-except
-            self.collector_logger.error(str(err))
+            self.collector_logger.error("Error collecting: " + str(err))
         # Then schedule the next execution
         self.scheduler.enter(
             delay, 1, self._schedule, (self.scheduler, message_callback, delay)
         )
         self.scheduler.run()
```

### Comparing `pyobas-1.0.5/pyobas/mixins.py` & `pyobas-1.0.6/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas/utils.py` & `pyobas-1.0.6/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.6/pyobas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobas-1.0.5/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.6/pyobas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyobas.egg-info/requires.txt` & `pyobas-1.0.6/pyobas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/pyproject.toml` & `pyobas-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.5/setup.cfg` & `pyobas-1.0.6/setup.cfg`

 * *Files identical despite different names*

