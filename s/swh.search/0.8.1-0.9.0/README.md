# Comparing `tmp/swh.search-0.8.1.tar.gz` & `tmp/swh.search-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.search-0.8.1.tar", last modified: Thu Apr 29 12:41:00 2021, max compression
+gzip compressed data, was "dist/swh.search-0.9.0.tar", last modified: Thu Jun 17 15:01:23 2021, max compression
```

## Comparing `swh.search-0.8.1.tar` & `swh.search-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-04-29 12:40:59.000000 swh.search-0.8.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1021 2021-04-29 12:40:59.000000 swh.search-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-04-29 12:40:59.000000 swh.search-0.8.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2021-04-29 12:40:59.000000 swh.search-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-04-29 12:40:59.000000 swh.search-0.8.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2021-04-29 12:40:59.000000 swh.search-0.8.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-04-29 12:40:59.000000 swh.search-0.8.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2021-04-29 12:40:59.000000 swh.search-0.8.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2250 2021-04-29 12:41:00.000000 swh.search-0.8.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1100 2021-04-29 12:40:59.000000 swh.search-0.8.1/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      147 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      979 2021-04-29 12:40:59.000000 swh.search-0.8.1/docs/index.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/es_config/
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2021-04-29 12:40:59.000000 swh.search-0.8.1/es_config/elasticsearch.keystore
--rw-r--r--   0 jenkins    (115) docker     (999)     2857 2021-04-29 12:40:59.000000 swh.search-0.8.1/es_config/elasticsearch.yml
--rw-r--r--   0 jenkins    (115) docker     (999)     3203 2021-04-29 12:40:59.000000 swh.search-0.8.1/es_config/jvm.options
--rw-r--r--   0 jenkins    (115) docker     (999)    17222 2021-04-29 12:40:59.000000 swh.search-0.8.1/es_config/log4j2.properties
--rw-r--r--   0 jenkins    (115) docker     (999)      363 2021-04-29 12:40:59.000000 swh.search-0.8.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2021-04-29 12:40:59.000000 swh.search-0.8.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       33 2021-04-29 12:40:59.000000 swh.search-0.8.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      133 2021-04-29 12:40:59.000000 swh.search-0.8.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       35 2021-04-29 12:40:59.000000 swh.search-0.8.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      277 2021-04-29 12:40:59.000000 swh.search-0.8.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       93 2021-04-29 12:41:00.000000 swh.search-0.8.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2355 2021-04-29 12:40:59.000000 swh.search-0.8.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)      371 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh/search/
--rw-r--r--   0 jenkins    (115) docker     (999)     1726 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh/search/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      437 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2559 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3116 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11886 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/elasticsearch.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4916 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2373 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2363 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1679 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh/search/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3489 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1901 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14048 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2780 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_elasticsearch.py
--rw-r--r--   0 jenkins    (115) docker     (999)      671 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3058 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2895 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23768 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4917 2021-04-29 12:40:59.000000 swh.search-0.8.1/swh/search/tests/test_server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2250 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1290 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       65 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      161 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2021-04-29 12:41:00.000000 swh.search-0.8.1/swh.search.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1395 2021-04-29 12:40:59.000000 swh.search-0.8.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-06-17 15:01:22.000000 swh.search-0.9.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1021 2021-06-17 15:01:22.000000 swh.search-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-06-17 15:01:22.000000 swh.search-0.9.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2021-06-17 15:01:22.000000 swh.search-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:22.000000 swh.search-0.9.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2021-06-17 15:01:22.000000 swh.search-0.9.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2021-06-17 15:01:22.000000 swh.search-0.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2021-06-17 15:01:22.000000 swh.search-0.9.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2043 2021-06-17 15:01:23.000000 swh.search-0.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1100 2021-06-17 15:01:22.000000 swh.search-0.9.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      147 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      979 2021-06-17 15:01:22.000000 swh.search-0.9.0/docs/index.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/es_config/
+-rw-r--r--   0 jenkins    (115) docker     (999)      199 2021-06-17 15:01:22.000000 swh.search-0.9.0/es_config/elasticsearch.keystore
+-rw-r--r--   0 jenkins    (115) docker     (999)     2857 2021-06-17 15:01:22.000000 swh.search-0.9.0/es_config/elasticsearch.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)     3203 2021-06-17 15:01:22.000000 swh.search-0.9.0/es_config/jvm.options
+-rw-r--r--   0 jenkins    (115) docker     (999)    17222 2021-06-17 15:01:22.000000 swh.search-0.9.0/es_config/log4j2.properties
+-rw-r--r--   0 jenkins    (115) docker     (999)      363 2021-06-17 15:01:22.000000 swh.search-0.9.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2021-06-17 15:01:22.000000 swh.search-0.9.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       33 2021-06-17 15:01:22.000000 swh.search-0.9.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      133 2021-06-17 15:01:22.000000 swh.search-0.9.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       86 2021-06-17 15:01:22.000000 swh.search-0.9.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      277 2021-06-17 15:01:22.000000 swh.search-0.9.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       93 2021-06-17 15:01:23.000000 swh.search-0.9.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2355 2021-06-17 15:01:22.000000 swh.search-0.9.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)      363 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh/search/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1726 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh/search/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      437 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2559 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3116 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14096 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/elasticsearch.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5986 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2683 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2510 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1679 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh/search/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3489 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1901 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14139 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4097 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_elasticsearch.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      671 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3058 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3480 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27420 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4917 2021-06-17 15:01:22.000000 swh.search-0.9.0/swh/search/tests/test_server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2043 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1290 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       65 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      212 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2021-06-17 15:01:23.000000 swh.search-0.9.0/swh.search.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1395 2021-06-17 15:01:22.000000 swh.search-0.9.0/tox.ini
```

### Comparing `swh.search-0.8.1/.pre-commit-config.yaml` & `swh.search-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/CODE_OF_CONDUCT.md` & `swh.search-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/LICENSE` & `swh.search-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/PKG-INFO` & `swh.search-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: swh.search
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software Heritage search service
 Home-page: https://forge.softwareheritage.org/diffusion/DSEA
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-search
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-search/
-Description: swh-search
-        ==========
-        
-        Search service for the Software Heritage archive.
-        
-        It is similar to swh-storage in what it contains,
-        but provides different ways to query it: while swh-storage is mostly
-        a key-value store that returns an object from a primary key,
-        swh-search is focused on reverse indices, to allow finding objects that
-        match some criteria; for example full-text search.
-        
-        Currently uses ElasticSearch, and provides only origin search (by URL and metadata)
-        
-        # Dependencies
-        
-        Python tests for this module include tests that cannot be run without a local
-        ElasticSearch instance, so you need the ElasticSearch server executable on your
-        machine (no need to have a running ElasticSearch server).
-        
-        ## Debian-like host
-        
-        The elasticsearch package is required. As it's not part of debian-stable,
-        [another debian repository is required to be
-        configured](https://www.elastic.co/guide/en/elasticsearch/reference/current/deb.html#deb-repo)
-        
-        ## Non Debian-like host
-        
-        The tests expect:
-        - `/usr/share/elasticsearch/jdk/bin/java` to exist.
-        - `org.elasticsearch.bootstrap.Elasticsearch` to be in java's classpath.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+License-File: AUTHORS
+
+swh-search
+==========
+
+Search service for the Software Heritage archive.
+
+It is similar to swh-storage in what it contains,
+but provides different ways to query it: while swh-storage is mostly
+a key-value store that returns an object from a primary key,
+swh-search is focused on reverse indices, to allow finding objects that
+match some criteria; for example full-text search.
+
+Currently uses ElasticSearch, and provides only origin search (by URL and metadata)
+
+# Dependencies
+
+Python tests for this module include tests that cannot be run without a local
+ElasticSearch instance, so you need the ElasticSearch server executable on your
+machine (no need to have a running ElasticSearch server).
+
+## Debian-like host
+
+The elasticsearch package is required. As it's not part of debian-stable,
+[another debian repository is required to be
+configured](https://www.elastic.co/guide/en/elasticsearch/reference/current/deb.html#deb-repo)
+
+## Non Debian-like host
+
+The tests expect:
+- `/usr/share/elasticsearch/jdk/bin/java` to exist.
+- `org.elasticsearch.bootstrap.Elasticsearch` to be in java's classpath.
+
+
```

### Comparing `swh.search-0.8.1/README.md` & `swh.search-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/docs/index.rst` & `swh.search-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/es_config/elasticsearch.yml` & `swh.search-0.9.0/es_config/elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/es_config/jvm.options` & `swh.search-0.9.0/es_config/jvm.options`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/es_config/log4j2.properties` & `swh.search-0.9.0/es_config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/setup.py` & `swh.search-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/__init__.py` & `swh.search-0.9.0/swh/search/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/api/server.py` & `swh.search-0.9.0/swh/search/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/cli.py` & `swh.search-0.9.0/swh/search/cli.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/in_memory.py` & `swh.search-0.9.0/swh/search/in_memory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2019-2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
+from datetime import datetime
 import itertools
 import re
 from typing import Any, Dict, Iterable, Iterator, List, Optional
 
 from swh.model.identifiers import origin_identifier
 from swh.search.interface import MinimalOriginDict, OriginDict, PagedResult
 
@@ -61,27 +62,42 @@
                 document["_url_tokens"] = set(
                     self._url_splitter.split(source_document["url"])
                 )
             if "visit_types" in document:
                 document["visit_types"] = set(source_document["visit_types"])
                 if "visit_types" in self._origins[id_]:
                     document["visit_types"].update(self._origins[id_]["visit_types"])
+            if "nb_visits" in document:
+                document["nb_visits"] = max(
+                    document["nb_visits"], self._origins[id_].get("nb_visits", 0)
+                )
+            if "last_visit_date" in document:
+                document["last_visit_date"] = max(
+                    datetime.fromisoformat(document["last_visit_date"]),
+                    datetime.fromisoformat(
+                        self._origins[id_]
+                        .get("last_visit_date", "0001-01-01T00:00:00.000000Z",)
+                        .replace("Z", "+00:00")
+                    ),
+                ).isoformat()
             self._origins[id_].update(document)
 
             if id_ not in self._origin_ids:
                 self._origin_ids.append(id_)
 
     def origin_search(
         self,
         *,
         url_pattern: Optional[str] = None,
         metadata_pattern: Optional[str] = None,
         with_visit: bool = False,
         visit_types: Optional[List[str]] = None,
         page_token: Optional[str] = None,
+        min_nb_visits: int = 0,
+        min_last_visit_date: str = "",
         limit: int = 50,
     ) -> PagedResult[MinimalOriginDict]:
         hits: Iterator[Dict[str, Any]] = (
             self._origins[id_]
             for id_ in self._origin_ids
             if not self._origins[id_].get("blocklisted")
         )
@@ -125,14 +141,22 @@
                 "At least one of url_pattern and metadata_pattern must be provided."
             )
 
         next_page_token: Optional[str] = None
 
         if with_visit:
             hits = filter(lambda o: o.get("has_visits"), hits)
+        if min_nb_visits:
+            hits = filter(lambda o: o.get("nb_visits", 0) >= min_nb_visits, hits)
+        if min_last_visit_date:
+            hits = filter(
+                lambda o: datetime.fromisoformat(o.get("last_visit_date", ""))
+                >= datetime.fromisoformat(min_last_visit_date),
+                hits,
+            )
 
         if visit_types is not None:
             visit_types_set = set(visit_types)
             hits = filter(
                 lambda o: visit_types_set.intersection(o.get("visit_types", set())),
                 hits,
             )
```

### Comparing `swh.search-0.8.1/swh/search/interface.py` & `swh.search-0.9.0/swh/search/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,25 +55,31 @@
         self,
         *,
         url_pattern: Optional[str] = None,
         metadata_pattern: Optional[str] = None,
         with_visit: bool = False,
         visit_types: Optional[List[str]] = None,
         page_token: Optional[str] = None,
+        min_nb_visits: int = 0,
+        min_last_visit_date: str = "",
         limit: int = 50,
     ) -> PagedResult[MinimalOriginDict]:
         """Searches for origins matching the `url_pattern`.
 
         Args:
             url_pattern: Part of the URL to search for
             with_visit: Whether origins with no visit are to be
               filtered out
             visit_types: Only origins having any of the provided visit types
                 (e.g. git, svn, pypi) will be returned
             page_token: Opaque value used for pagination
+            min_nb_visits: Filter origins that have number of visits >=
+                the provided value
+            min_last_visit_date: Filter origins that have
+                last_visit_date on or after the provided date(ISO format)
             limit: number of results to return
 
         Returns:
             PagedResult of origin dicts matching the search criteria. If next_page_token
             is None, there is no longer data to retrieve.
 
         """
```

### Comparing `swh.search-0.8.1/swh/search/journal_client.py` & `swh.search-0.9.0/swh/search/journal_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,20 @@
     )
 
 
 def process_origin_visit_statuses(visit_statuses, search):
     logging.debug("processing origin visit statuses %r", visit_statuses)
 
     full_visit_status = [
-        {"url": (visit_status["origin"]), "has_visits": True,}
+        {
+            "url": (visit_status["origin"]),
+            "has_visits": True,
+            "nb_visits": visit_status["visit"],
+            "last_visit_date": visit_status["date"].isoformat(),
+        }
         for visit_status in visit_statuses
         if visit_status["status"] == "full"
     ]
 
     if full_visit_status:
         search.origin_update(full_visit_status)
```

### Comparing `swh.search-0.8.1/swh/search/metrics.py` & `swh.search-0.9.0/swh/search/metrics.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/tests/conftest.py` & `swh.search-0.9.0/swh/search/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/tests/test_api_client.py` & `swh.search-0.9.0/swh/search/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/tests/test_cli.py` & `swh.search-0.9.0/swh/search/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2019-2020  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import copy
+from datetime import datetime, timezone
 import tempfile
 
 from click.testing import CliRunner
 from confluent_kafka import Producer
 import pytest
 import yaml
 
@@ -175,14 +176,15 @@
         }
     )
     topic = f"{kafka_prefix}.origin_visit_status"
     value = value_to_kafka(
         {
             "origin": origin_foobar["url"],
             "visit": 1,
+            "date": datetime.now(tz=timezone.utc),
             "snapshot": None,
             "status": "full",
         }
     )
     producer.produce(topic=topic, key=b"bogus-origin-visit-status", value=value)
 
     journal_objects_config = JOURNAL_OBJECTS_CONFIG_TEMPLATE.format(
```

### Comparing `swh.search-0.8.1/swh/search/tests/test_elasticsearch.py` & `swh.search-0.9.0/swh/search/tests/test_elasticsearch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,60 @@
-# Copyright (C) 2019-2020  The Software Heritage developers
+# Copyright (C) 2019-2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from textwrap import dedent
+import types
 import unittest
 
+from elasticsearch.helpers.errors import BulkIndexError
 import pytest
 
 from swh.search.metrics import OPERATIONS_METRIC
 
 from .test_search import CommonSearchTest
 
 
 class BaseElasticsearchTest(unittest.TestCase):
     @pytest.fixture(autouse=True)
     def _instantiate_search(self, swh_search, elasticsearch_host, mocker):
         self._elasticsearch_host = elasticsearch_host
         self.search = swh_search
         self.mocker = mocker
 
+        # override self.search.origin_update to catch painless script errors
+        # and pretty print them
+        origin_update = self.search.origin_update
+
+        def _origin_update(self, *args, **kwargs):
+            script_error = False
+            error_detail = ""
+            try:
+                origin_update(*args, **kwargs)
+            except BulkIndexError as e:
+                error = e.errors[0].get("update", {}).get("error", {}).get("caused_by")
+                if error and "script_stack" in error:
+                    script_error = True
+                    error_detail = dedent(
+                        f"""
+                        Painless update script failed ({error.get('reason')}).
+                        error type: {error.get('caused_by', {}).get('type')}
+                        error reason: {error.get('caused_by', {}).get('reason')}
+                        script stack:
+
+                        """
+                    )
+                    error_detail += "\n".join(error["script_stack"])
+                else:
+                    raise e
+            assert script_error is False, error_detail[1:]
+
+        self.search.origin_update = types.MethodType(_origin_update, self.search)
+
     def reset(self):
         self.search.deinitialize()
         self.search.initialize()
 
 
 class TestElasticsearchSearch(CommonSearchTest, BaseElasticsearchTest):
     def test_metrics_update_duration(self):
```

### Comparing `swh.search-0.8.1/swh/search/tests/test_in_memory.py` & `swh.search-0.9.0/swh/search/tests/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/tests/test_init.py` & `swh.search-0.9.0/swh/search/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh/search/tests/test_search.py` & `swh.search-0.9.0/swh/search/tests/test_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Copyright (C) 2019-2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from datetime import datetime, timedelta, timezone
+
 from hypothesis import given, settings, strategies
+import pytest
 
 from swh.core.api.classes import stream_results
 
 
 class CommonSearchTest:
     def test_origin_url_unique_word_prefix(self):
         origin_foobar_baz = {"url": "http://foobar.baz"}
@@ -180,14 +183,85 @@
                 ["svn", "git"],
                 ["hg", "git"],
                 ["hg", "svn"],
                 ["git", "hg", "svn"],
             ]
         )
 
+    def test_origin_nb_visits_update_search(self):
+        origin_url = "http://foobar.baz"
+        self.search.origin_update([{"url": origin_url}])
+        self.search.flush()
+
+        def _update_nb_visits(nb_visits):
+            self.search.origin_update([{"url": origin_url, "nb_visits": nb_visits}])
+            self.search.flush()
+
+        def _check_min_nb_visits(min_nb_visits):
+            actual_page = self.search.origin_search(
+                url_pattern=origin_url, min_nb_visits=min_nb_visits,
+            )
+            assert actual_page.next_page_token is None
+            results = [r["url"] for r in actual_page.results]
+            expected_results = [origin_url]
+            assert sorted(results) == sorted(expected_results)
+
+        _update_nb_visits(2)
+        _check_min_nb_visits(2)  # Works for = 2
+        _check_min_nb_visits(1)  # Works for < 2
+
+        with pytest.raises(AssertionError):
+            _check_min_nb_visits(
+                5
+            )  # No results for nb_visits >= 5 (should throw error)
+
+        _update_nb_visits(5)
+        _check_min_nb_visits(5)  # Works for = 5
+        _check_min_nb_visits(3)  # Works for < 5
+
+    def test_origin_last_visit_date_update_search(self):
+        origin_url = "http://foobar.baz"
+        self.search.origin_update([{"url": origin_url}])
+        self.search.flush()
+
+        def _update_last_visit_date(last_visit_date):
+            self.search.origin_update(
+                [{"url": origin_url, "last_visit_date": last_visit_date}]
+            )
+            self.search.flush()
+
+        def _check_min_last_visit_date(min_last_visit_date):
+            actual_page = self.search.origin_search(
+                url_pattern=origin_url, min_last_visit_date=min_last_visit_date,
+            )
+            assert actual_page.next_page_token is None
+            results = [r["url"] for r in actual_page.results]
+            expected_results = [origin_url]
+            assert sorted(results) == sorted(expected_results)
+
+        now = datetime.now(tz=timezone.utc).isoformat()
+        now_minus_5_hours = (
+            datetime.now(tz=timezone.utc) - timedelta(hours=5)
+        ).isoformat()
+        now_plus_5_hours = (
+            datetime.now(tz=timezone.utc) + timedelta(hours=5)
+        ).isoformat()
+
+        _update_last_visit_date(now)
+
+        _check_min_last_visit_date(now)  # Works for =
+        _check_min_last_visit_date(now_minus_5_hours)  # Works for <
+        with pytest.raises(AssertionError):
+            _check_min_last_visit_date(now_plus_5_hours)  # Fails for >
+
+        _update_last_visit_date(now_plus_5_hours)
+
+        _check_min_last_visit_date(now_plus_5_hours)  # Works for =
+        _check_min_last_visit_date(now)  # Works for <
+
     def test_origin_update_with_no_visit_types(self):
         """
         Update an origin with visit types first then with no visit types,
         check origin can still be searched with visit types afterwards.
         """
         origin_url = "http://foobar.baz"
         self.search.origin_update([{"url": origin_url, "visit_types": ["git"]}])
@@ -265,23 +339,28 @@
         self.search.flush()
 
         actual_page = self.search.origin_search(metadata_pattern="foo bar baz")
         assert actual_page.next_page_token is None
         assert actual_page.results == [origin3_foobarbaz]
 
     def test_origin_intrinsic_metadata_long_description(self):
+        """Checks ElasticSearch does not try to store large values untokenize,
+        which would be inefficient and crash it with:
+
+        Document contains at least one immense term in field="intrinsic_metadata.http://schema.org/description.@value" (whose UTF8 encoding is longer than the max length 32766), all of which were skipped.
+        """  # noqa
         origin1 = {"url": "http://origin1"}
 
         self.search.origin_update(
             [
                 {
                     **origin1,
                     "intrinsic_metadata": {
                         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
-                        "description": " ".join(f"foo{i}" for i in range(1000000)),
+                        "description": " ".join(f"foo{i}" for i in range(100000)),
                     },
                 },
             ]
         )
         self.search.flush()
 
         actual_page = self.search.origin_search(metadata_pattern="foo42")
@@ -414,59 +493,68 @@
         assert actual_page.next_page_token is None
         assert actual_page.results == [origin3_bazqux]
 
         actual_page = self.search.origin_search(metadata_pattern="foo bar")
         assert actual_page.next_page_token is None
         assert actual_page.results == [origin1_foobar]
 
-    def test_origin_intrinsic_metadata_date(self):
+    def test_origin_intrinsic_metadata_string_mapping(self):
         """Checks inserting a date-like in a field does not update the mapping to
         require every document uses a date in that field; or that search queries
         use a date either.
-        Likewise for numeric fields."""
+        Likewise for numeric and boolean fields."""
         origin1 = {"url": "http://origin1"}
         origin2 = {"url": "http://origin2"}
 
         self.search.origin_update(
             [
                 {
                     **origin1,
                     "intrinsic_metadata": {
                         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
                         "dateCreated": "2021-02-18T10:16:52",
                         "version": "1.0",
+                        "isAccessibleForFree": True,
                     },
                 }
             ]
         )
         self.search.flush()
-
         self.search.origin_update(
             [
                 {
                     **origin2,
                     "intrinsic_metadata": {
                         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
                         "dateCreated": "a long time ago",
                         "address": "in a galaxy far, far away",
                         "version": "a new hope",
+                        "isAccessibleForFree": "it depends",
                     },
                 },
             ]
         )
         self.search.flush()
 
         actual_page = self.search.origin_search(metadata_pattern="2021")
         assert actual_page.next_page_token is None
         assert actual_page.results == [origin1]
 
         actual_page = self.search.origin_search(metadata_pattern="long time ago")
         assert actual_page.next_page_token is None
         assert actual_page.results == [origin2]
 
+        actual_page = self.search.origin_search(metadata_pattern="true")
+        assert actual_page.next_page_token is None
+        assert actual_page.results == [origin1]
+
+        actual_page = self.search.origin_search(metadata_pattern="it depends")
+        assert actual_page.next_page_token is None
+        assert actual_page.results == [origin2]
+
     def test_origin_intrinsic_metadata_update(self):
         origin = {"url": "http://origin1"}
         origin_data = {
             **origin,
             "intrinsic_metadata": {
                 "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
                 "author": "John Doe",
```

### Comparing `swh.search-0.8.1/swh/search/tests/test_server.py` & `swh.search-0.9.0/swh/search/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/swh.search.egg-info/PKG-INFO` & `swh.search-0.9.0/swh.search.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: swh.search
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software Heritage search service
 Home-page: https://forge.softwareheritage.org/diffusion/DSEA
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-search
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-search/
-Description: swh-search
-        ==========
-        
-        Search service for the Software Heritage archive.
-        
-        It is similar to swh-storage in what it contains,
-        but provides different ways to query it: while swh-storage is mostly
-        a key-value store that returns an object from a primary key,
-        swh-search is focused on reverse indices, to allow finding objects that
-        match some criteria; for example full-text search.
-        
-        Currently uses ElasticSearch, and provides only origin search (by URL and metadata)
-        
-        # Dependencies
-        
-        Python tests for this module include tests that cannot be run without a local
-        ElasticSearch instance, so you need the ElasticSearch server executable on your
-        machine (no need to have a running ElasticSearch server).
-        
-        ## Debian-like host
-        
-        The elasticsearch package is required. As it's not part of debian-stable,
-        [another debian repository is required to be
-        configured](https://www.elastic.co/guide/en/elasticsearch/reference/current/deb.html#deb-repo)
-        
-        ## Non Debian-like host
-        
-        The tests expect:
-        - `/usr/share/elasticsearch/jdk/bin/java` to exist.
-        - `org.elasticsearch.bootstrap.Elasticsearch` to be in java's classpath.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+License-File: AUTHORS
+
+swh-search
+==========
+
+Search service for the Software Heritage archive.
+
+It is similar to swh-storage in what it contains,
+but provides different ways to query it: while swh-storage is mostly
+a key-value store that returns an object from a primary key,
+swh-search is focused on reverse indices, to allow finding objects that
+match some criteria; for example full-text search.
+
+Currently uses ElasticSearch, and provides only origin search (by URL and metadata)
+
+# Dependencies
+
+Python tests for this module include tests that cannot be run without a local
+ElasticSearch instance, so you need the ElasticSearch server executable on your
+machine (no need to have a running ElasticSearch server).
+
+## Debian-like host
+
+The elasticsearch package is required. As it's not part of debian-stable,
+[another debian repository is required to be
+configured](https://www.elastic.co/guide/en/elasticsearch/reference/current/deb.html#deb-repo)
+
+## Non Debian-like host
+
+The tests expect:
+- `/usr/share/elasticsearch/jdk/bin/java` to exist.
+- `org.elasticsearch.bootstrap.Elasticsearch` to be in java's classpath.
+
+
```

### Comparing `swh.search-0.8.1/swh.search.egg-info/SOURCES.txt` & `swh.search-0.9.0/swh.search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.search-0.8.1/tox.ini` & `swh.search-0.9.0/tox.ini`

 * *Files identical despite different names*

