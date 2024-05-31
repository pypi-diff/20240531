# Comparing `tmp/prefect_slack-0.2.5.tar.gz` & `tmp/prefect_slack-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_slack-0.2.5.tar", last modified: Fri May  3 16:56:48 2024, max compression
+gzip compressed data, was "prefect_slack-0.2.6.tar", last modified: Thu May 16 20:56:01 2024, max compression
```

## Comparing `prefect_slack-0.2.5.tar` & `prefect_slack-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/prefect_slack/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/prefect_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_notification_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:01.207636 prefect_slack-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 20:56:01.207636 prefect_slack-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:01.203636 prefect_slack-0.2.6/prefect_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/prefect_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/prefect_slack/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/prefect_slack/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:01.207636 prefect_slack-0.2.6/prefect_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 20:56:01.000000 prefect_slack-0.2.6/prefect_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:56:00.000000 prefect_slack-0.2.6/prefect_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:56:01.207636 prefect_slack-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:01.207636 prefect_slack-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/test_notification_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 20:55:48.000000 prefect_slack-0.2.6/tests/test_version.py
```

### Comparing `prefect_slack-0.2.5/LICENSE` & `prefect_slack-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/PKG-INFO` & `prefect_slack-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: slack_sdk>=3.15.1
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_slack-0.2.5/README.md` & `prefect_slack-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/prefect_slack/credentials.py` & `prefect_slack-0.2.6/prefect_slack/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/prefect_slack/messages.py` & `prefect_slack-0.2.6/prefect_slack/messages.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/prefect_slack.egg-info/PKG-INFO` & `prefect_slack-0.2.6/prefect_slack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: slack_sdk>=3.15.1
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_slack-0.2.5/prefect_slack.egg-info/SOURCES.txt` & `prefect_slack-0.2.6/prefect_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/pyproject.toml` & `prefect_slack-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,37 +3,31 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-slack"
 description = "Prefect integrations with Slack"
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "Apache License 2.0"}
+license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
-authors = [
-  {name = "Prefect Technologies, Inc.", email = "help@prefect.io"}
-]
+authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = [
-  "aiohttp",
-  "slack_sdk>=3.15.1",
-  "prefect>=2.14.10",
-]
+dependencies = ["aiohttp", "slack_sdk>=3.15.1", "prefect>=2.14.10, < 3.0.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
@@ -73,8 +67,8 @@
 omit = ["tests/*", "prefect_slack/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_slack-0.2.5/tests/conftest.py` & `prefect_slack-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/tests/test_block_standards.py` & `prefect_slack-0.2.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/tests/test_credentials.py` & `prefect_slack-0.2.6/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/tests/test_messages.py` & `prefect_slack-0.2.6/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.5/tests/test_notification_block.py` & `prefect_slack-0.2.6/tests/test_notification_block.py`

 * *Files identical despite different names*

