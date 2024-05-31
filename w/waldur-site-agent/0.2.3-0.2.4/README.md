# Comparing `tmp/waldur_site_agent-0.2.3.tar.gz` & `tmp/waldur_site_agent-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waldur_site_agent-0.2.3.tar", max compression
+gzip compressed data, was "waldur_site_agent-0.2.4.tar", max compression
```

## Comparing `waldur_site_agent-0.2.3.tar` & `waldur_site_agent-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2024-05-06 18:36:27.393608 waldur_site_agent-0.2.3/LICENCE
--rw-r--r--   0        0        0    10138 2024-05-30 07:30:27.655660 waldur_site_agent-0.2.3/README.md
--rw-r--r--   0        0        0     1174 2024-05-30 07:30:44.151879 waldur_site_agent-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2836 2024-05-30 07:30:27.659661 waldur_site_agent-0.2.3/waldur_site_agent/__init__.py
--rw-r--r--   0        0        0     9460 2024-05-30 07:30:27.659661 waldur_site_agent-0.2.3/waldur_site_agent/common_utils.py
--rw-r--r--   0        0        0      597 2024-05-30 07:30:27.659661 waldur_site_agent-0.2.3/waldur_site_agent/main.py
--rw-r--r--   0        0        0     2125 2024-05-30 07:30:27.659661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/__init__.py
--rw-r--r--   0        0        0    11844 2024-05-30 07:30:27.659661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/backend.py
--rw-r--r--   0        0        0     1317 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/base.py
--rw-r--r--   0        0        0     5975 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/client.py
--rw-r--r--   0        0        0      128 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/exceptions.py
--rw-r--r--   0        0        0     3384 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/parser.py
--rw-r--r--   0        0        0      401 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/structures.py
--rw-r--r--   0        0        0     2006 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/utils.py
--rw-r--r--   0        0        0     8621 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/slurm_waldur_utils.py
--rw-r--r--   0        0        0    10039 2024-05-30 07:30:27.663661 waldur_site_agent-0.2.3/waldur_site_agent/waldur_slurm_utils.py
--rw-r--r--   0        0        0    11052 1970-01-01 00:00:00.000000 waldur_site_agent-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-06 18:55:25.076175 waldur_site_agent-0.2.4/LICENCE
+-rw-r--r--   0        0        0    10138 2024-05-31 09:22:18.116112 waldur_site_agent-0.2.4/README.md
+-rw-r--r--   0        0        0     1173 2024-05-31 09:22:33.260312 waldur_site_agent-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2836 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/__init__.py
+-rw-r--r--   0        0        0     9460 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/common_utils.py
+-rw-r--r--   0        0        0      597 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/main.py
+-rw-r--r--   0        0        0     2125 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/__init__.py
+-rw-r--r--   0        0        0    11844 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/backend.py
+-rw-r--r--   0        0        0     1317 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/base.py
+-rw-r--r--   0        0        0     5975 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/client.py
+-rw-r--r--   0        0        0      128 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/exceptions.py
+-rw-r--r--   0        0        0     3384 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/parser.py
+-rw-r--r--   0        0        0      401 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/structures.py
+-rw-r--r--   0        0        0     2006 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/utils.py
+-rw-r--r--   0        0        0     8621 2024-05-31 09:22:18.120112 waldur_site_agent-0.2.4/waldur_site_agent/slurm_waldur_utils.py
+-rw-r--r--   0        0        0    10039 2024-05-31 09:22:18.124112 waldur_site_agent-0.2.4/waldur_site_agent/waldur_slurm_utils.py
+-rw-r--r--   0        0        0    11051 1970-01-01 00:00:00.000000 waldur_site_agent-0.2.4/PKG-INFO
```

### Comparing `waldur_site_agent-0.2.3/LICENCE` & `waldur_site_agent-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/README.md` & `waldur_site_agent-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/pyproject.toml` & `waldur_site_agent-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "waldur-site-agent"
-version = "0.2.3"
+version = "0.2.4"
 description = "Agent for integrating service provider's site with Waldur Mastermind."
 authors = ["OpenNode Team <info@opennodecloud.com>"]
 license = "MIT"
 homepage = "https://waldur.com"
 documentation = "https://docs.waldur.com"
 readme = "README.md"
 classifiers=[
@@ -15,17 +15,17 @@
 packages = [
     {include = "waldur_site_agent"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-waldur-client = "^0.3.0"
-requests = "2.27.1"
+requests = "2.32.3"
 pyyaml = "6.0.1"
-sentry-sdk = "1.14.0"
+sentry-sdk = "2.3.1"
 
 
 [tool.poetry.group.dev.dependencies]
 freezegun = "0.3.4"
 coverage = "6.3.2"
 pytest = "7.1.2"
 pytest-cov = "3.0.0"
```

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/__init__.py` & `waldur_site_agent-0.2.4/waldur_site_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/common_utils.py` & `waldur_site_agent-0.2.4/waldur_site_agent/common_utils.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/main.py` & `waldur_site_agent-0.2.4/waldur_site_agent/main.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/__init__.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/backend.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/backend.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/base.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/base.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/client.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/client.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/parser.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/parser.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_client/utils.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_client/utils.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/slurm_waldur_utils.py` & `waldur_site_agent-0.2.4/waldur_site_agent/slurm_waldur_utils.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/waldur_site_agent/waldur_slurm_utils.py` & `waldur_site_agent-0.2.4/waldur_site_agent/waldur_slurm_utils.py`

 * *Files identical despite different names*

### Comparing `waldur_site_agent-0.2.3/PKG-INFO` & `waldur_site_agent-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waldur-site-agent
-Version: 0.2.3
+Version: 0.2.4
 Summary: Agent for integrating service provider's site with Waldur Mastermind.
 Home-page: https://waldur.com
 License: MIT
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-waldur-client (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (==6.0.1)
-Requires-Dist: requests (==2.27.1)
-Requires-Dist: sentry-sdk (==1.14.0)
+Requires-Dist: requests (==2.32.3)
+Requires-Dist: sentry-sdk (==2.3.1)
 Project-URL: Documentation, https://docs.waldur.com
 Description-Content-Type: text/markdown
 
 # Agent for Service Provider Integration
 
 Agent for Mastermind integration with a provider's site.
 The main purpose of the agent is data syncronization between Waldur instance and an application (for example SLURM or MOAB cluster).
```

