# Comparing `tmp/crc_bonfire-5.8.0.tar.gz` & `tmp/crc_bonfire-5.8.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc_bonfire-5.8.0.tar", last modified: Wed May 15 13:42:13 2024, max compression
+gzip compressed data, was "crc_bonfire-5.8.1b0.tar", last modified: Fri May 31 18:34:34 2024, max compression
```

## Comparing `crc_bonfire-5.8.0.tar` & `crc_bonfire-5.8.1b0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.259021 crc_bonfire-5.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/bonfire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48982 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/configmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/elastic_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/openshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/qontract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/bonfire/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/default-iqe-cji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/local-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/reservation-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/build_deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/cicd/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/cicd/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/cicd/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/crc_bonfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/entry_points.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/data/namespace_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/data/reservation_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_app_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/utils/search_replace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.185313 crc_bonfire-5.8.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/bonfire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48968 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/configmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/elastic_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/qontract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/bonfire/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/default-iqe-cji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/local-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/reservation-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/build_deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/cicd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/cicd/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/demo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/data/namespace_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/data/reservation_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_app_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/utils/search_replace.py
```

### Comparing `crc_bonfire-5.8.0/.github/workflows/release.yml` & `crc_bonfire-5.8.1b0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/.github/workflows/tests.yml` & `crc_bonfire-5.8.1b0/.github/workflows/tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 
 jobs:
   build:
     runs-on: ubuntu-20.04
     steps:
 
     - name: Checkout to master
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
+
+    - uses: chartboost/ruff-action@v1
 
     - name: Setup python
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
         architecture: 'x64'
 
+    - uses: pre-commit/action@v3.0.1
+
     - name: Install build dependencies
       run: |
         python -m pip install -U pip
         pip install -U wheel setuptools build
 
-    - name: run Flake8
-      uses: TrueBrain/actions-flake8@v2
-
     - name: Build
       run: python -m build -o dist/
 
     - uses: actions/upload-artifact@v3
       with:
         name: dist
         path: dist
```

### Comparing `crc_bonfire-5.8.0/.gitignore` & `crc_bonfire-5.8.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/CONTRIBUTING.md` & `crc_bonfire-5.8.1b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/Dockerfile` & `crc_bonfire-5.8.1b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/PKG-INFO` & `crc_bonfire-5.8.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.8.0
+Version: 5.8.1b0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
-Home-page: https://www.github.com/RedHatInsights/bonfire
-Author: Brandon Squizzato
-Author-email: bsquizza@redhat.com
-License: MIT
-Classifier: Topic :: Utilities
+Author-email: Brandon Squizzato <bsquizza@redhat.com>
+License: MIT License
+Project-URL: Homepage, https://www.github.com/RedHatInsights/bonfire
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: app-common-python>=0.1.6
 Requires-Dist: cached_property
 Requires-Dist: chardet<4.0,>=2.0
-Requires-Dist: multidict
 Requires-Dist: click>=7.1.2
 Requires-Dist: gql==3.0.0a6
+Requires-Dist: importlib-metadata>=0.12; python_version < "3.8"
+Requires-Dist: junitparser
+Requires-Dist: multidict
+Requires-Dist: ocviapy>=1.2.2
+Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: sh
-Requires-Dist: wait-for
 Requires-Dist: tabulate
-Requires-Dist: python-dotenv
-Requires-Dist: ocviapy>=1.2.2
-Requires-Dist: app-common-python>=0.1.6
-Requires-Dist: junitparser
-Requires-Dist: importlib-metadata>=0.12; python_version < "3.8"
+Requires-Dist: wait-for
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # bonfire <!-- omit in toc -->
```

### Comparing `crc_bonfire-5.8.0/README.md` & `crc_bonfire-5.8.1b0/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/bonfire.py` & `crc_bonfire-5.8.1b0/bonfire/bonfire.py`

 * *Files 0% similar despite different names*

```diff
@@ -1264,17 +1264,15 @@
     type=str,
     help="Directory to use for secrets import (default: $XDG_CONFIG_HOME/bonfire/secrets/)",
     default=conf.DEFAULT_SECRETS_DIR,
 )
 @click.option(
     "--configmaps-dir",
     type=str,
-    help=(
-        "Directory to use for configmaps import (default: $XDG_CONFIG_HOME/bonfire/configmaps/)"
-    ),
+    help=("Directory to use for configmaps import (default: $XDG_CONFIG_HOME/bonfire/configmaps/)"),
     default=conf.DEFAULT_CONFIGMAPS_DIR,
 )
 @click.option(
     "--no-release-on-fail",
     is_flag=True,
     help="Do not release namespace reservation if deployment fails",
 )
```

### Comparing `crc_bonfire-5.8.0/bonfire/config.py` & `crc_bonfire-5.8.1b0/bonfire/config.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/configmaps.py` & `crc_bonfire-5.8.1b0/bonfire/configmaps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Handles importing of configmaps from a local directory
 """
+
 import glob
 import json
 import logging
 import os
 
 from ocviapy import get_json, oc
 
@@ -67,15 +68,19 @@
         raise FatalError(f"invalid configmaps directory: {path}")
 
     files = _get_files_in_dir(path)
     configmaps = {}
     log.info("importing configmaps from local path: %s", path)
     for confmaps_file in files:
         confmaps_in_file = _parse_configmaps_file(confmaps_file)
-        log.info("loaded %d configmap(s) from file '%s'", len(confmaps_in_file), confmaps_file)
+        log.info(
+            "loaded %d configmap(s) from file '%s'",
+            len(confmaps_in_file),
+            confmaps_file,
+        )
         for confmaps_name in confmaps_in_file:
             if confmaps_name in configmaps:
                 raise FatalError(
                     f"configmap with name '{confmaps_name}' defined twice in configmaps dir"
                 )
         configmaps.update(confmaps_in_file)
```

### Comparing `crc_bonfire-5.8.0/bonfire/elastic_logging.py` & `crc_bonfire-5.8.1b0/bonfire/elastic_logging.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/local.py` & `crc_bonfire-5.8.1b0/bonfire/local.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/namespaces.py` & `crc_bonfire-5.8.1b0/bonfire/namespaces.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/openshift.py` & `crc_bonfire-5.8.1b0/bonfire/openshift.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/processor.py` & `crc_bonfire-5.8.1b0/bonfire/processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/qontract.py` & `crc_bonfire-5.8.1b0/bonfire/qontract.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/resources/default-iqe-cji.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/default-iqe-cji.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/resources/default_config.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/default_config.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/resources/local-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/local-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/bonfire/secrets.py` & `crc_bonfire-5.8.1b0/bonfire/secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Handles importing of secrets from a local directory
 """
+
 import glob
 import json
 import logging
 import os
 
 from ocviapy import get_json, oc
```

### Comparing `crc_bonfire-5.8.0/bonfire/utils.py` & `crc_bonfire-5.8.1b0/bonfire/utils.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/cicd/README.md` & `crc_bonfire-5.8.1b0/cicd/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/crc_bonfire.egg-info/PKG-INFO` & `crc_bonfire-5.8.1b0/crc_bonfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.8.0
+Version: 5.8.1b0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
-Home-page: https://www.github.com/RedHatInsights/bonfire
-Author: Brandon Squizzato
-Author-email: bsquizza@redhat.com
-License: MIT
-Classifier: Topic :: Utilities
+Author-email: Brandon Squizzato <bsquizza@redhat.com>
+License: MIT License
+Project-URL: Homepage, https://www.github.com/RedHatInsights/bonfire
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: app-common-python>=0.1.6
 Requires-Dist: cached_property
 Requires-Dist: chardet<4.0,>=2.0
-Requires-Dist: multidict
 Requires-Dist: click>=7.1.2
 Requires-Dist: gql==3.0.0a6
+Requires-Dist: importlib-metadata>=0.12; python_version < "3.8"
+Requires-Dist: junitparser
+Requires-Dist: multidict
+Requires-Dist: ocviapy>=1.2.2
+Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: sh
-Requires-Dist: wait-for
 Requires-Dist: tabulate
-Requires-Dist: python-dotenv
-Requires-Dist: ocviapy>=1.2.2
-Requires-Dist: app-common-python>=0.1.6
-Requires-Dist: junitparser
-Requires-Dist: importlib-metadata>=0.12; python_version < "3.8"
+Requires-Dist: wait-for
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # bonfire <!-- omit in toc -->
```

### Comparing `crc_bonfire-5.8.0/crc_bonfire.egg-info/SOURCES.txt` & `crc_bonfire-5.8.1b0/crc_bonfire.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+.flake8
 .gitignore
+.pre-commit-config.yaml
 CONTRIBUTING.md
 Dockerfile
 README.md
 build_deploy.sh
 demo.gif
-entry_points.txt
 entrypoint.sh
 pyproject.toml
 pytest.ini
-setup.cfg
 .github/workflows/release.yml
 .github/workflows/tests.yml
 bonfire/__init__.py
 bonfire/bonfire.py
 bonfire/config.py
 bonfire/configmaps.py
 bonfire/elastic_logging.py
```

### Comparing `crc_bonfire-5.8.0/demo.gif` & `crc_bonfire-5.8.1b0/demo.gif`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/entrypoint.sh` & `crc_bonfire-5.8.1b0/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/data/namespace_data.json` & `crc_bonfire-5.8.1b0/tests/data/namespace_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/data/reservation_data.json` & `crc_bonfire-5.8.1b0/tests/data/reservation_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/test_app_configs.py` & `crc_bonfire-5.8.1b0/tests/test_app_configs.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/test_bonfire.py` & `crc_bonfire-5.8.1b0/tests/test_bonfire.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/test_get_apps.py` & `crc_bonfire-5.8.1b0/tests/test_get_apps.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/test_processor.py` & `crc_bonfire-5.8.1b0/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/tests/test_utils.py` & `crc_bonfire-5.8.1b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.0/utils/search_replace.py` & `crc_bonfire-5.8.1b0/utils/search_replace.py`

 * *Files identical despite different names*

