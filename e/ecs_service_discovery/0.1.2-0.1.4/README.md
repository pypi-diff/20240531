# Comparing `tmp/ecs_service_discovery-0.1.2.tar.gz` & `tmp/ecs_service_discovery-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_service_discovery-0.1.2.tar", max compression
+gzip compressed data, was "ecs_service_discovery-0.1.4.tar", max compression
```

## Comparing `ecs_service_discovery-0.1.2.tar` & `ecs_service_discovery-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    16725 2023-03-12 12:50:13.531742 ecs_service_discovery-0.1.2/LICENSE
--rw-r--r--   0        0        0     3214 2023-03-31 07:22:14.894858 ecs_service_discovery-0.1.2/README.rst
--rw-r--r--   0        0        0      225 2023-04-16 14:14:44.969920 ecs_service_discovery-0.1.2/ecs_service_discovery/__init__.py
--rw-r--r--   0        0        0     1923 2023-03-12 12:50:13.532742 ecs_service_discovery-0.1.2/ecs_service_discovery/cli.py
--rw-r--r--   0        0        0     4001 2023-03-31 05:09:27.319912 ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_sd_common.py
--rw-r--r--   0        0        0     3806 2023-03-31 10:14:55.557618 ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_service_discovery.py
--rw-r--r--   0        0        0     8786 2023-04-16 09:16:17.633828 ecs_service_discovery-0.1.2/ecs_service_discovery/prometheus_sd.py
--rw-r--r--   0        0        0      723 2023-03-31 10:14:22.583225 ecs_service_discovery-0.1.2/ecs_service_discovery/stats.py
--rw-r--r--   0        0        0     2289 2023-04-16 14:14:44.969920 ecs_service_discovery-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.2/setup.py
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-03-12 12:50:13.531742 ecs_service_discovery-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3214 2023-03-31 07:22:14.894858 ecs_service_discovery-0.1.4/README.rst
+-rw-r--r--   0        0        0      225 2024-05-31 04:28:23.113201 ecs_service_discovery-0.1.4/ecs_service_discovery/__init__.py
+-rw-r--r--   0        0        0     1923 2023-03-12 12:50:13.532742 ecs_service_discovery-0.1.4/ecs_service_discovery/cli.py
+-rw-r--r--   0        0        0     4001 2023-03-31 05:09:27.319912 ecs_service_discovery-0.1.4/ecs_service_discovery/ecs_sd_common.py
+-rw-r--r--   0        0        0     3806 2023-03-31 10:14:55.557618 ecs_service_discovery-0.1.4/ecs_service_discovery/ecs_service_discovery.py
+-rw-r--r--   0        0        0     9289 2024-05-26 12:36:29.589876 ecs_service_discovery-0.1.4/ecs_service_discovery/prometheus_sd.py
+-rw-r--r--   0        0        0      723 2023-03-31 10:14:22.583225 ecs_service_discovery-0.1.4/ecs_service_discovery/stats.py
+-rw-r--r--   0        0        0     2282 2024-05-31 04:28:23.113201 ecs_service_discovery-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.4/PKG-INFO
```

### Comparing `ecs_service_discovery-0.1.2/LICENSE` & `ecs_service_discovery-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/README.rst` & `ecs_service_discovery-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/ecs_service_discovery/cli.py` & `ecs_service_discovery-0.1.4/ecs_service_discovery/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_sd_common.py` & `ecs_service_discovery-0.1.4/ecs_service_discovery/ecs_sd_common.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_service_discovery.py` & `ecs_service_discovery-0.1.4/ecs_service_discovery/ecs_service_discovery.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/ecs_service_discovery/prometheus_sd.py` & `ecs_service_discovery-0.1.4/ecs_service_discovery/prometheus_sd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #  SPDX-License-Identifier: MPL-2.0
 #  Copyright 2020-2022 John Mille <john@compose-x.io>
 
 from __future__ import annotations
 
 import json
-import pathlib
+import shutil
 from os import path
+from pathlib import Path
+from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Union
 
 import yaml
 
 try:
     from yaml import CDumper as Dumper
     from yaml import CSafeDumper as SafeDumper
@@ -99,36 +101,43 @@
     targets = identify_prometheus_enabled_targets(cluster_targets)
     if not targets:
         return
     cluster_prometheus_targets = targets[1]
     PROMETHEUS_TARGETS.labels(cluster.arn).set(
         sum(len(_t["targets"]) for _t in cluster_prometheus_targets)
     )
+    temp_dir = TemporaryDirectory()
     file_format = set_else_none("prometheus_output_format", kwargs, alt_value="json")
     file_path = f"{output_dir}/{cluster.name}.{file_format}"
+    temp_file_path = "{}/{}.{}".format(temp_dir.name, cluster.name, file_format)
     if file_format == "yaml":
-        with open(file_path, "w") as targets_fd:
+        with open(temp_file_path, "w") as targets_fd:
             targets_fd.write(yaml.dump(cluster_prometheus_targets, Dumper=SafeDumper))
     else:
-        with open(file_path, "w") as targets_fd:
+        with open(temp_file_path, "w") as targets_fd:
             targets_fd.write(
                 json.dumps(cluster_prometheus_targets, separators=(",", ":"), indent=1)
             )
+    shutil.move(temp_file_path, file_path)
     cluster_path_dir = f"{output_dir}/{cluster.name}/per_job"
-    cluster_jobs_dir = pathlib.Path(path.abspath(cluster_path_dir))
+    cluster_jobs_dir = Path(path.abspath(cluster_path_dir))
+    temp_cluster_jobs_dir = Path("{}/{}".format(temp_dir.name, cluster_path_dir))
     cluster_jobs_dir.mkdir(parents=True, exist_ok=True)
+    temp_cluster_jobs_dir.mkdir(parents=True, exist_ok=True)
     for job_name, job_targets in targets[0].items():
         job_file_name = f"{cluster_path_dir}/{job_name}.{file_format}"
-        with open(job_file_name, "w") as cluster_job_fd:
+        temp_job_file_name = "{}/{}".format(temp_dir.name, job_file_name)
+        with open(temp_job_file_name, "w") as cluster_job_fd:
             if file_format == "yaml":
                 cluster_job_fd.write(yaml.dump([job_targets], Dumper=SafeDumper))
             else:
                 cluster_job_fd.write(
                     json.dumps([job_targets], separators=(",", ":"), indent=1)
                 )
+        shutil.move(temp_job_file_name, job_file_name)
 
 
 def set_labels(task: dict, container_name, job_name: str) -> dict:
     task_def = task["_taskDefinition"]
     for container_def in task_def["containerDefinitions"]:
         if container_name == container_def["name"]:
             break
```

### Comparing `ecs_service_discovery-0.1.2/ecs_service_discovery/stats.py` & `ecs_service_discovery-0.1.4/ecs_service_discovery/stats.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.2/pyproject.toml` & `ecs_service_discovery-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_service_discovery"
-version = "0.1.2"
+version = "0.1.4"
 description = "ECS Service Discovery"
 authors = ["John Preston <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["ecs", "service discovery", "observability"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -24,37 +24,37 @@
 "Source" = "https://github.com/compose-x/ecs-service-discovery/"
 "Bug Tracker" = "https://github.com/compose-x/ecs-service-discovery/issues"
 "Labs" = "https://labs.compose-x.io/"
 "Blog" = "https://blog.compose-x.io/"
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 compose-x-common = "^1.2"
-prometheus-client = "^0.16"
+prometheus-client = "^0.20"
 PyYAML = "^6.0"
 
 [tool.poetry.scripts]
 ecs-service-discovery = "ecs_service_discovery.cli:main"
 ecs-sd = "ecs_service_discovery.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 tbump = "^6.9.0"
-black = "^23.1"
+black = "^24.1"
 isort = "^5.10"
 pre-commit = "^3.1"
 mypy-boto3-sts = "^1.24"
 mypy-boto3-ecs = "^1.24"
 mypy-boto3-ssm = "^1.24"
 Sphinx = "^5.1.1"
 sphinx-material = "^0.0.35"
 sphinx-sitemap = "^2.2.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
@@ -71,15 +71,15 @@
 
 [tool.coverage.run]
 omit = [
   "*/cli.py"
 ]
 
 [tool.tbump.version]
-current = "0.1.2"
+current = "0.1.4"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `ecs_service_discovery-0.1.2/PKG-INFO` & `ecs_service_discovery-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
-Name: ecs-service-discovery
-Version: 0.1.2
+Name: ecs_service_discovery
+Version: 0.1.4
 Summary: ECS Service Discovery
 License: MPL-2.0
 Keywords: ecs,service discovery,observability
 Author: John Preston
 Author-email: john@ews-network.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: compose-x-common (>=1.2,<2.0)
-Requires-Dist: prometheus-client (>=0.16,<0.17)
+Requires-Dist: prometheus-client (>=0.20,<0.21)
 Project-URL: Bug Tracker, https://github.com/compose-x/ecs-service-discovery/issues
 Project-URL: Blog, https://blog.compose-x.io/
 Project-URL: Labs, https://labs.compose-x.io/
 Project-URL: Source, https://github.com/compose-x/ecs-service-discovery/
 Description-Content-Type: text/x-rst
 
 =====================
```

