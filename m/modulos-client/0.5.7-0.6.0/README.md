# Comparing `tmp/modulos_client-0.5.7.tar.gz` & `tmp/modulos_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modulos_client-0.5.7.tar", last modified: Thu Apr 25 16:55:18 2024, max compression
+gzip compressed data, was "modulos_client-0.6.0.tar", last modified: Fri May 31 07:33:12 2024, max compression
```

## Comparing `modulos_client-0.5.7.tar` & `modulos_client-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.387778 modulos_client-0.5.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.387778 modulos_client-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/workflows/pr-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 16:55:11.000000 modulos_client-0.5.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-25 16:55:18.395778 modulos_client-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-25 16:55:11.000000 modulos_client-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 16:55:11.000000 modulos_client-0.5.7/dev_README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/registering/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/registering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/registering/register_on_modulos_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/services/users_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/modulos_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-25 16:55:11.000000 modulos_client-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:55:18.395778 modulos_client-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.476586 modulos_client-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.468586 modulos_client-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 07:33:02.000000 modulos_client-0.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-31 07:33:02.000000 modulos_client-0.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.468586 modulos_client-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-31 07:33:02.000000 modulos_client-0.6.0/.github/workflows/pr-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-31 07:33:02.000000 modulos_client-0.6.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 07:33:02.000000 modulos_client-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-31 07:33:02.000000 modulos_client-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-31 07:33:12.476586 modulos_client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-31 07:33:02.000000 modulos_client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 07:33:02.000000 modulos_client-0.6.0/dev_README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.472586 modulos_client-0.6.0/modulos_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.472586 modulos_client-0.6.0/modulos_client/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/monitoring/monitoring_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.472586 modulos_client-0.6.0/modulos_client/registering/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/registering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/registering/register_on_modulos_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.472586 modulos_client-0.6.0/modulos_client/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/services/users_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-31 07:33:02.000000 modulos_client-0.6.0/modulos_client/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.476586 modulos_client-0.6.0/modulos_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 07:33:12.000000 modulos_client-0.6.0/modulos_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-31 07:33:02.000000 modulos_client-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 07:33:12.476586 modulos_client-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:33:12.476586 modulos_client-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 07:33:02.000000 modulos_client-0.6.0/tox.ini
```

### Comparing `modulos_client-0.5.7/.github/workflows/pr-test.yml` & `modulos_client-0.6.0/.github/workflows/pr-test.yml`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/.github/workflows/publish_pypi.yml` & `modulos_client-0.6.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/.gitignore` & `modulos_client-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/Makefile` & `modulos_client-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/PKG-INFO` & `modulos_client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: modulos_client
-Version: 0.5.7
+Version: 0.6.0
 Summary: Package to interact with the Modulos Platform
 Author-email: Modulos AG <contact@modulos.ai>
 Project-URL: Homepage, https://github.com/Modulos/modulos_client
 Project-URL: Bug Reports, https://github.com/Modulos/modulos_client/issues
 Project-URL: Source, https://github.com/Modulos/modulos_client
 Keywords: modulos_client
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click<=8.1.7,>=8.1.7
-Requires-Dist: pandas<=2.2.1,>=1.5.3
-Requires-Dist: pydantic<=2.6.3,>=2.4.2
+Requires-Dist: pandas<=2.2.2,>=1.5.3
+Requires-Dist: pydantic<=2.7.1,>=2.4.2
 Requires-Dist: pyYAML<=6.0.1,>=6.0.1
-Requires-Dist: requests<=2.31.0,>=2.0.0
+Requires-Dist: requests<=2.32.2,>=2.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.9.0
 Provides-Extra: dev
-Requires-Dist: coverage<=7.4.3,>=7.2.7; extra == "dev"
-Requires-Dist: pytest<=8.0.2,>=7.3.1; extra == "dev"
-Requires-Dist: tox<=4.13.0,>=4.11.4; extra == "dev"
+Requires-Dist: coverage<=7.5.2,>=7.2.7; extra == "dev"
+Requires-Dist: pytest<=8.2.1,>=7.3.1; extra == "dev"
+Requires-Dist: tox<=4.15.0,>=4.11.4; extra == "dev"
 
 ## Modulos Client Tool
 
 This tool provides a command-line interface to interact with the Modulos platform.
 
 ### Prerequisites
```

### Comparing `modulos_client-0.5.7/README.md` & `modulos_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/dev_README.md` & `modulos_client-0.6.0/dev_README.md`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/cli.py` & `modulos_client-0.6.0/modulos_client/cli.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/config.py` & `modulos_client-0.6.0/modulos_client/config.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/configurations.py` & `modulos_client-0.6.0/modulos_client/configurations.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/organizations.py` & `modulos_client-0.6.0/modulos_client/organizations.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/profiles.py` & `modulos_client-0.6.0/modulos_client/profiles.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/projects.py` & `modulos_client-0.6.0/modulos_client/projects.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/registering/register_on_modulos_platform.py` & `modulos_client-0.6.0/modulos_client/registering/register_on_modulos_platform.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/services/users_services.py` & `modulos_client-0.6.0/modulos_client/services/users_services.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/templates.py` & `modulos_client-0.6.0/modulos_client/templates.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client/users.py` & `modulos_client-0.6.0/modulos_client/users.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/modulos_client.egg-info/PKG-INFO` & `modulos_client-0.6.0/modulos_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: modulos_client
-Version: 0.5.7
+Version: 0.6.0
 Summary: Package to interact with the Modulos Platform
 Author-email: Modulos AG <contact@modulos.ai>
 Project-URL: Homepage, https://github.com/Modulos/modulos_client
 Project-URL: Bug Reports, https://github.com/Modulos/modulos_client/issues
 Project-URL: Source, https://github.com/Modulos/modulos_client
 Keywords: modulos_client
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click<=8.1.7,>=8.1.7
-Requires-Dist: pandas<=2.2.1,>=1.5.3
-Requires-Dist: pydantic<=2.6.3,>=2.4.2
+Requires-Dist: pandas<=2.2.2,>=1.5.3
+Requires-Dist: pydantic<=2.7.1,>=2.4.2
 Requires-Dist: pyYAML<=6.0.1,>=6.0.1
-Requires-Dist: requests<=2.31.0,>=2.0.0
+Requires-Dist: requests<=2.32.2,>=2.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.9.0
 Provides-Extra: dev
-Requires-Dist: coverage<=7.4.3,>=7.2.7; extra == "dev"
-Requires-Dist: pytest<=8.0.2,>=7.3.1; extra == "dev"
-Requires-Dist: tox<=4.13.0,>=4.11.4; extra == "dev"
+Requires-Dist: coverage<=7.5.2,>=7.2.7; extra == "dev"
+Requires-Dist: pytest<=8.2.1,>=7.3.1; extra == "dev"
+Requires-Dist: tox<=4.15.0,>=4.11.4; extra == "dev"
 
 ## Modulos Client Tool
 
 This tool provides a command-line interface to interact with the Modulos platform.
 
 ### Prerequisites
```

### Comparing `modulos_client-0.5.7/modulos_client.egg-info/SOURCES.txt` & `modulos_client-0.6.0/modulos_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 modulos_client/users.py
 modulos_client.egg-info/PKG-INFO
 modulos_client.egg-info/SOURCES.txt
 modulos_client.egg-info/dependency_links.txt
 modulos_client.egg-info/entry_points.txt
 modulos_client.egg-info/requires.txt
 modulos_client.egg-info/top_level.txt
+modulos_client/monitoring/__init__.py
+modulos_client/monitoring/monitoring_datasource.py
 modulos_client/registering/__init__.py
 modulos_client/registering/register_on_modulos_platform.py
 modulos_client/services/__init__.py
 modulos_client/services/users_services.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_config.py
```

### Comparing `modulos_client-0.5.7/pyproject.toml` & `modulos_client-0.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -17,31 +17,31 @@
   "Natural Language :: English",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
     "click >= 8.1.7, <= 8.1.7",
-    "pandas >= 1.5.3, <= 2.2.1",
-    "pydantic >= 2.4.2, <= 2.6.3",
+    "pandas >= 1.5.3, <= 2.2.2",
+    "pydantic >= 2.4.2, <= 2.7.1",
     "pyYAML >= 6.0.1, <= 6.0.1",
-    "requests >= 2.0.0, <= 2.31.0",
+    "requests >= 2.0.0, <= 2.32.2",
     "tabulate >= 0.9.0, <= 0.9.0",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install modulos_client[dev]
 [project.optional-dependencies]
 dev = [
-    'coverage>= 7.2.7, <= 7.4.3',
-    'pytest >= 7.3.1, <= 8.0.2',
-    'tox >= 4.11.4, <= 4.13.0',
+    'coverage>= 7.2.7, <= 7.5.2',
+    'pytest >= 7.3.1, <= 8.2.1',
+    'tox >= 4.11.4, <= 4.15.0',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Modulos/modulos_client"
 "Bug Reports" = "https://github.com/Modulos/modulos_client/issues"
 "Source" = "https://github.com/Modulos/modulos_client"
```

### Comparing `modulos_client-0.5.7/tests/conftest.py` & `modulos_client-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_cli.py` & `modulos_client-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_config.py` & `modulos_client-0.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_configurations.py` & `modulos_client-0.6.0/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_organization.py` & `modulos_client-0.6.0/tests/test_organization.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_profiles.py` & `modulos_client-0.6.0/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_projects.py` & `modulos_client-0.6.0/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_services.py` & `modulos_client-0.6.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_templates.py` & `modulos_client-0.6.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tests/test_users.py` & `modulos_client-0.6.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.7/tox.ini` & `modulos_client-0.6.0/tox.ini`

 * *Files identical despite different names*

