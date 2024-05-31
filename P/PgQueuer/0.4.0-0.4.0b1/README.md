# Comparing `tmp/pgqueuer-0.4.0.tar.gz` & `tmp/pgqueuer-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.4.0.tar", last modified: Fri May 31 20:27:09 2024, max compression
+gzip compressed data, was "pgqueuer-0.4.0b1.tar", last modified: Fri May 31 20:18:33 2024, max compression
```

## Comparing `pgqueuer-0.4.0.tar` & `pgqueuer-0.4.0b1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.725117 pgqueuer-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.713117 pgqueuer-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.713117 pgqueuer-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-31 20:27:09.721117 pgqueuer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.717117 pgqueuer-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/benchmark.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/dashboard.md
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/database_initialization.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/docs/queuemanager.md
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:27:09.725117 pgqueuer-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.717117 pgqueuer-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.717117 pgqueuer-0.4.0/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.721117 pgqueuer-0.4.0/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 20:27:09.000000 pgqueuer-0.4.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.721117 pgqueuer-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.721117 pgqueuer-0.4.0/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:27:09.721117 pgqueuer-0.4.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 20:27:01.000000 pgqueuer-0.4.0/tools/ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.114762 pgqueuer-0.4.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/benchmark.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/database_initialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/queuemanager.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/tools/ex.py
```

### Comparing `pgqueuer-0.4.0/.github/workflows/ci.yml` & `pgqueuer-0.4.0b1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/.github/workflows/linting.yml` & `pgqueuer-0.4.0b1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/.github/workflows/release.yml` & `pgqueuer-0.4.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/.gitignore` & `pgqueuer-0.4.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/CONTRIBUTING.md` & `pgqueuer-0.4.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/LICENSE` & `pgqueuer-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/PKG-INFO` & `pgqueuer-0.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.4.0
+Version: 0.4.0b1
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.4.0/README.md` & `pgqueuer-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/Makefile` & `pgqueuer-0.4.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/benchmark.md` & `pgqueuer-0.4.0b1/docs/benchmark.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/dashboard.md` & `pgqueuer-0.4.0b1/docs/dashboard.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/database_initialization.md` & `pgqueuer-0.4.0b1/docs/database_initialization.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/index.rst` & `pgqueuer-0.4.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/introduction.md` & `pgqueuer-0.4.0b1/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/make.bat` & `pgqueuer-0.4.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/docs/queuemanager.md` & `pgqueuer-0.4.0b1/docs/queuemanager.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/pyproject.toml` & `pgqueuer-0.4.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/cli.py` & `pgqueuer-0.4.0b1/src/PgQueuer/cli.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/listeners.py` & `pgqueuer-0.4.0b1/src/PgQueuer/listeners.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/models.py` & `pgqueuer-0.4.0b1/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/qm.py` & `pgqueuer-0.4.0b1/src/PgQueuer/qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/queries.py` & `pgqueuer-0.4.0b1/src/PgQueuer/queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer/tm.py` & `pgqueuer-0.4.0b1/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.4.0b1/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.4.0
+Version: 0.4.0b1
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.4.0/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.4.0b1/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/test/conftest.py` & `pgqueuer-0.4.0b1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/test/db/Dockerfile` & `pgqueuer-0.4.0b1/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/test/test_qm.py` & `pgqueuer-0.4.0b1/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/test/test_queries.py` & `pgqueuer-0.4.0b1/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/test/test_tm.py` & `pgqueuer-0.4.0b1/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/tools/benchmark.py` & `pgqueuer-0.4.0b1/tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.4.0/tools/ex.py` & `pgqueuer-0.4.0b1/tools/ex.py`

 * *Files identical despite different names*

