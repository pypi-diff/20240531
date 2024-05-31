# Comparing `tmp/datamaestro-1.1.0.tar.gz` & `tmp/datamaestro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaestro-1.1.0.tar", last modified: Wed Mar  6 14:09:40 2024, max compression
+gzip compressed data, was "datamaestro-1.2.0.tar", last modified: Fri May 31 10:31:53 2024, max compression
```

## Comparing `datamaestro-1.1.0.tar` & `datamaestro-1.2.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.103267 datamaestro-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.111267 datamaestro-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-06 14:09:27.000000 datamaestro-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-06 14:09:27.000000 datamaestro-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-06 14:09:27.000000 datamaestro-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-06 14:09:27.000000 datamaestro-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-03-06 14:09:40.119267 datamaestro-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-03-06 14:09:27.000000 datamaestro-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-06 14:09:27.000000 datamaestro-1.1.0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.111267 datamaestro-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.111267 datamaestro-1.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.111267 datamaestro-1.1.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/api/data.md
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/api/download.rst
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/api/records.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/developping.md
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-06 14:09:27.000000 datamaestro-1.1.0/docs/source/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-06 14:09:27.000000 datamaestro-1.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-06 14:09:27.000000 datamaestro-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-06 14:09:27.000000 datamaestro-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-06 14:09:27.000000 datamaestro-1.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-06 14:09:27.000000 datamaestro-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-06 14:09:27.000000 datamaestro-1.1.0/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-06 14:09:40.123267 datamaestro-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-06 14:09:27.000000 datamaestro-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.107267 datamaestro-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.115267 datamaestro-1.1.0/src/datamaestro/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9024 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.115267 datamaestro-1.1.0/src/datamaestro/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/annotations/agreement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.115267 datamaestro-1.1.0/src/datamaestro/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/commands/mainstyle.css
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/commands/site.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.115267 datamaestro-1.1.0/src/datamaestro/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/data/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/data/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/data/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/src/datamaestro/download/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/single.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/download/todo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/src/datamaestro/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/stream/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/stream/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/src/datamaestro/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/templates/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/src/datamaestro/test/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/test_download_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/test/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-06 14:09:27.000000 datamaestro-1.1.0/src/datamaestro/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-06 14:09:39.000000 datamaestro-1.1.0/src/datamaestro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:09:40.119267 datamaestro-1.1.0/src/datamaestro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 14:09:40.000000 datamaestro-1.1.0/src/datamaestro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-06 14:09:27.000000 datamaestro-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.281442 datamaestro-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.coverage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.265442 datamaestro-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.269442 datamaestro-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-31 10:31:42.000000 datamaestro-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 10:31:42.000000 datamaestro-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-31 10:31:42.000000 datamaestro-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-31 10:31:42.000000 datamaestro-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-31 10:31:53.281442 datamaestro-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-31 10:31:42.000000 datamaestro-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 10:31:42.000000 datamaestro-1.2.0/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.269442 datamaestro-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.269442 datamaestro-1.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.269442 datamaestro-1.2.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/api/data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/api/download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/api/records.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/developping.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 10:31:42.000000 datamaestro-1.2.0/docs/source/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-31 10:31:42.000000 datamaestro-1.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-31 10:31:42.000000 datamaestro-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 10:31:42.000000 datamaestro-1.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 10:31:42.000000 datamaestro-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-31 10:31:42.000000 datamaestro-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 10:31:42.000000 datamaestro-1.2.0/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-31 10:31:53.281442 datamaestro-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 10:31:42.000000 datamaestro-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.265442 datamaestro-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.273442 datamaestro-1.2.0/src/datamaestro/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9024 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.273442 datamaestro-1.2.0/src/datamaestro/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/annotations/agreement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.273442 datamaestro-1.2.0/src/datamaestro/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/commands/mainstyle.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/commands/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/data/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/data/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/data/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/download/todo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/stream/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/stream/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/templates/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/test_download_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/test/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-31 10:31:42.000000 datamaestro-1.2.0/src/datamaestro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:31:53.277442 datamaestro-1.2.0/src/datamaestro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 10:31:53.000000 datamaestro-1.2.0/src/datamaestro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-31 10:31:42.000000 datamaestro-1.2.0/tox.ini
```

### Comparing `datamaestro-1.1.0/.github/workflows/pytest.yml` & `datamaestro-1.2.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/.github/workflows/python-publish.yml` & `datamaestro-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/LICENSE` & `datamaestro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/PKG-INFO` & `datamaestro-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaestro
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Dataset management command line and API"
 Home-page: https://github.com/experimaestro/datamaestro
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: dataset manager
 Platform: any
```

### Comparing `datamaestro-1.1.0/README.md` & `datamaestro-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/Makefile` & `datamaestro-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/make.bat` & `datamaestro-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/api/data.md` & `datamaestro-1.2.0/docs/source/api/data.md`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/api/download.rst` & `datamaestro-1.2.0/docs/source/api/download.rst`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/api/records.rst` & `datamaestro-1.2.0/docs/source/api/records.rst`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/conf.py` & `datamaestro-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/datasets.rst` & `datamaestro-1.2.0/docs/source/datasets.rst`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/docs/source/index.md` & `datamaestro-1.2.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/mkdocs.yml` & `datamaestro-1.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/setup.cfg` & `datamaestro-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/__main__.py` & `datamaestro-1.2.0/src/datamaestro/__main__.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/annotations/agreement.py` & `datamaestro-1.2.0/src/datamaestro/annotations/agreement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-import logging
-from datamaestro.definitions import DatasetAnnotation, AbstractDataset, hook
+from typing import Optional
+from datamaestro.definitions import AbstractDataset, hook
 
 
 @hook("pre-use")
-def useragreement(definition: AbstractDataset, message, id=None):
+def useragreement(definition: AbstractDataset, message: str, id: Optional[str] = None):
+    """Asks for a user-agreement
+
+    :param definition: The dataset for which the agreement is asked
+    :param message: The agreement text
+    :param id: The ID of the agreement (default to the dataset ID)
+    """
     # Skip agreement when testing
     if definition.context.running_test:
         return
 
     settings = definition.context.user_settings
     id = id or definition.id
     answer = settings.agreements.get(id, "no")
```

### Comparing `datamaestro-1.1.0/src/datamaestro/commands/site.py` & `datamaestro-1.2.0/src/datamaestro/commands/site.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/context.py` & `datamaestro-1.2.0/src/datamaestro/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,27 +106,28 @@
         for entry_point in pkg_resources.iter_entry_points("datamaestro.repositories"):
             yield entry_point.load().instance()
 
     def repository(self, repositoryid):
         if repositoryid is None:
             return None
 
-        l = [
+        entry_points = [
             x
             for x in pkg_resources.iter_entry_points(
                 "datamaestro.repositories", repositoryid
             )
         ]
-        if not l:
+        if not entry_points:
             raise Exception("No datasets repository named %s", repositoryid)
-        if len(l) > 1:
+        if len(entry_points) > 1:
             raise Exception(
-                "Too many datasets repository named %s (%d)" % (repositoryid, len(l))
+                "Too many datasets repository named %s (%d)"
+                % (repositoryid, len(entry_points))
             )
-        return l[0].load()(self)
+        return entry_points[0].load()(self)
 
     @property
     def running_test(self):
         return "PYTEST_CURRENT_TEST" in os.environ
 
     def datasets(self):
         """Returns an iterator over all files"""
@@ -171,28 +172,27 @@
 
         urlpath, dlpath = getPaths(hasher)
         urlpath.write_text(url)
 
         if dlpath.is_file():
             logging.debug("Using cached file %s for %s", dlpath, url)
         else:
-
             logging.info("Downloading %s", url)
             tmppath = dlpath.with_suffix(".tmp")
 
             downloadURL(url, tmppath, tmppath.is_file(), size=size)
 
             # Now, rename to original
             tmppath.rename(dlpath)
 
         return CachedFile(dlpath, keep=self.keep_downloads, others=[urlpath])
 
     def ask(self, question: str, options: Dict[str, str]):
         """Ask a question to the user"""
-        print(question)
+        print(question)  # noqa: T201
         answer = None
         while answer not in options:
             answer = input().strip().lower()
         return options[answer]
 
 
 class ResolvablePath:
@@ -264,26 +264,35 @@
                 (title if intitle else description).append(line)
 
         self._title = " ".join(title)
         self._description = "\n".join(description)
 
     def __iter__(self) -> Iterable["AbstractDataset"]:
         from .definitions import DatasetWrapper
+        from datamaestro.data import Base
 
         # Iterates over defined symbols
         for key, value in self.module.__dict__.items():
             # Ensures it is annotated
             if isinstance(value, DatasetWrapper):
                 # Ensure it comes from the module
                 if self.module.__name__ == value.t.__module__:
                     yield value
+            elif (
+                inspect.isclass(value)
+                and issubclass(value, Base)
+                and hasattr(value, "__dataset__")
+            ):
+                if self.module.__name__ == value.__module__:
+                    yield value.__dataset__
 
 
 class Repository:
-    """A repository regroup a set of datasets and their corresponding specific handlers (downloading, filtering, etc.)"""
+    """A repository regroup a set of datasets and their corresponding specific
+    handlers (downloading, filtering, etc.)"""
 
     def __init__(self, context: Context):
         """Initialize a new repository
 
         :param context: The dataset main context
         :param basedir: The base directory of the repository
             (by default, the same as the repository class)
@@ -311,15 +320,15 @@
     @classmethod
     def version(cls):
         from pkg_resources import get_distribution, DistributionNotFound
 
         try:
             return get_distribution(cls.__module__).version
         except DistributionNotFound:
-            __version__ = None
+            return None
 
     def __repr__(self):
         return "Repository(%s)" % self.basedir
 
     def __hash__(self):
         return self.basedir.__hash__()
```

### Comparing `datamaestro-1.1.0/src/datamaestro/data/__init__.py` & `datamaestro-1.2.0/src/datamaestro/data/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/data/csv.py` & `datamaestro-1.2.0/src/datamaestro/data/csv.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/data/huggingface.py` & `datamaestro-1.2.0/src/datamaestro/data/huggingface.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/data/tensor.py` & `datamaestro-1.2.0/src/datamaestro/data/tensor.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/definitions.py` & `datamaestro-1.2.0/src/datamaestro/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,23 +123,31 @@
     - can be searched for
     - has a data storage space
     - has specific attributes:
         - timestamp: whether the dataset version depends on the time of the download
     """
 
     name: Optional[str] = None
+    """The name of the dataset"""
+
+    url: Optional[str] = None
+    """The URL of the dataset"""
+
+    doi: Optional[str] = None
+    """The DOI of this dataset"""
 
     def __init__(self, repository: Optional["Repository"]):
         super().__init__()
         self.repository = repository
         self.timestamp = False
         self.aliases = set()
 
         # Associated resources
         self.resources: Dict[str, "Download"] = {}
+        self.ordered_resources = []
 
         # Hooks
         # pre-use: before returning the dataset object
         # pre-download: before downloading the dataset
         self.hooks = {"pre-use": [], "pre-download": []}
 
         self.url = None
@@ -190,21 +198,23 @@
         for key, value in data.__xpm__.values.items():
             if isinstance(value, Config):
                 self.setDataIDs(value, f"{id}.{key}")
 
     def download(self, force=False):
         """Download all the necessary resources"""
         success = True
-        for key, resource in self.resources.items():
+        logging.info("Materializing %d resources", len(self.ordered_resources))
+        for resource in self.ordered_resources:
             try:
                 resource.download(force)
             except Exception:
-                logging.error("Could not download resource %s", key)
+                logging.error("Could not download resource %s", resource)
                 traceback.print_exc()
                 success = False
+                break
         return success
 
     @staticmethod
     def find(name: str) -> "DataDefinition":
         """Find a dataset given its name"""
         logging.debug("Searching dataset %s", name)
         for repository in Context.instance().repositories():
@@ -245,21 +255,23 @@
     This is the standard way to define a dataset in datamaestro through
     annotations (otherwise, derive from `AbstractDataset`).
     """
 
     def __init__(self, annotation, t: type):
         self.t = t
         self.base = annotation.base
+        self.config = None
         assert self.base is not None, f"Could not set the Config type for {t}"
 
         repository, components = DataDefinition.repository_relpath(t)
         super().__init__(repository)
 
         # Set some variables
         self.url = annotation.url
+        self.doi = annotation.doi
 
         # Builds the ID:
         # Removes module_name.config prefix
         assert (
             components[0] == "config"
         ), f"A @dataset object should be in the .config module (not {t.__module__})"
 
@@ -318,41 +330,52 @@
     def __call__(self, *args, **kwargs):
         self.t(*args, **kwargs)
 
     def __getattr__(self, key):
         """Returns a pointer to a potential attribute"""
         return FutureAttr(self, [key])
 
+    def download(self, force=False):
+        if self.base is self.t:
+            self._prepare()
+        return super().download(force=force)
+
     def _prepare(self, download=False) -> "Base":
+        if self.config is not None:
+            return self.config
+
+        if self.base is self.t:
+            self.config = self.base.__create_dataset__(self)
+
         if download:
             for hook in self.hooks["pre-download"]:
                 hook(self)
             if not self.download(False):
                 raise Exception("Could not load necessary resources")
         logging.debug("Building with data type %s and dataset %s", self.base, self.t)
         for hook in self.hooks["pre-use"]:
             hook(self)
 
-        resources = {key: value.prepare() for key, value in self.resources.items()}
-        dict = self.t(**resources)
-        if dict is None:
-            name = self.t.__name__
-            filename = inspect.getfile(self.t)
-            raise Exception(
-                f"The dataset method {name} defined in "
-                f"{filename} returned a null object"
-            )
-
         # Construct the object
-        data = self.base(**dict)
+        if self.config is None:
+            resources = {key: value.prepare() for key, value in self.resources.items()}
+            dict = self.t(**resources)
+            if dict is None:
+                name = self.t.__name__
+                filename = inspect.getfile(self.t)
+                raise Exception(
+                    f"The dataset method {name} defined in "
+                    f"{filename} returned a null object"
+                )
+            self.config = self.base(**dict)
 
         # Set the ids
-        self.setDataIDs(data, self.id)
+        self.setDataIDs(self.config, self.id)
 
-        return data
+        return self.config
 
     @property
     def _path(self) -> Path:
         """Returns a unique relative path for this dataset"""
         path = Path(*self.id.split("."))
         if self.version:
             path = path.with_suffix(".v%s" % self.version)
@@ -451,15 +474,17 @@
 
 
 datatags = DataTagging(lambda d: d.tags)
 datatasks = DataTagging(lambda d: d.tasks)
 
 
 class dataset:
-    def __init__(self, base=None, *, timestamp=None, id=None, url=None, size=None):
+    def __init__(
+        self, base=None, *, timestamp=None, id=None, url=None, size=None, doi=None
+    ):
         """Creates a new (meta)dataset
 
         Meta-datasets are not associated with any base type
 
         Arguments:
             base {[type]} -- The base type (or None if infered from type
             annotation)
@@ -469,39 +494,54 @@
             (default: None)
 
             id {[type]} -- [description] (default: {None})
 
             url {[type]} -- [description] (default: {None})
 
             size {str} -- The size (should be a parsable format)
+
+            doi {str} -- The DOI of the corresponding paper
         """
         if hasattr(base, "__datamaestro__") and isinstance(
             base.__datamaestro__, metadataset
         ):
             self.base = base.__datamaestro__.base
         else:
             self.base = base
 
         self.id = id
         self.url = url
         self.meta = False
         self.timestamp = timestamp
         self.size = size
+        self.doi = doi
 
     def __call__(self, t):
         try:
             if self.base is None:
-                # Get type from return annotation
-                self.base = t.__annotations__["return"]
+                from datamaestro.data import Base
+
+                if inspect.isclass(t) and issubclass(t, Base):
+                    self.base = t
+                else:
+                    # Get type from return annotation
+                    try:
+                        self.base = t.__annotations__["return"]
+                    except KeyError:
+                        logging.warning("No return annotation in %s", t)
+                        raise
             object.__getattribute__(t, "__datamaestro__")
             raise AssertionError("@data should only be called once")
         except AttributeError:
             pass
 
         dw = DatasetWrapper(self, t)
+        t.__dataset__ = dw
+        if inspect.isclass(t) and issubclass(t, Base):
+            return t
         return dw
 
 
 class metadataset(AbstractDataset):
     """Annotation for object/functions which are abstract dataset definitions
 
     i.e. shared by more than one real dataset. This is useful to share tags,
```

### Comparing `datamaestro-1.1.0/src/datamaestro/download/__init__.py` & `datamaestro-1.2.0/src/datamaestro/download/huggingface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,45 @@
-from abc import ABC, abstractmethod
-from datamaestro.definitions import AbstractDataset, DatasetAnnotation
-from datamaestro.utils import deprecated
+import logging
+from typing import Optional
 
+from datamaestro.download import Download
 
-def initialized(method):
-    """Ensure the object is initialized"""
 
-    def wrapper(self, *args, **kwargs):
-        if not self._post:
-            self._post = True
-            self.postinit()
-        return method(self, *args, **kwargs)
+class hf_download(Download):
+    """Use Hugging Face to donwload a file"""
 
-    return wrapper
-
-
-class Download(DatasetAnnotation, ABC):
-    """
-    Base class for all download handlers
-    """
-
-    def __init__(self, varname: str):
-        self.varname = varname
-        # Ensures that the object is initialized
-        self._post = False
-
-    def annotate(self, dataset: AbstractDataset):
-        # Register has a resource download
-        if self.varname in dataset.resources:
-            raise AssertionError("Name %s already declared as a resource", self.varname)
-
-        dataset.resources[self.varname] = self
-        self.definition = dataset
-
-    @property
-    def context(self):
-        return self.definition.context
-
-    def postinit(self):
-        pass
-
-    def hasfiles(self):
-        return True
-
-    @abstractmethod
-    def download(self, force=False):
-        """Downloads the content"""
-        ...
-
-    @abstractmethod
-    def prepare(self):
-        """Prepares the dataset"""
-        ...
-
-
-class reference(Download):
-    def __init__(self, varname, reference):
+    def __init__(
+        self,
+        varname: str,
+        repo_id: str,
+        *,
+        data_files: Optional[str] = None,
+        split: Optional[str] = None
+    ):
+        """Use
+
+        Args:
+            varname: Variable name
+            repo_id: The HuggingFace repository ID
+        """
         super().__init__(varname)
-        self.reference = reference
-
-    def prepare(self):
-        v = self.reference.prepare()
-        if isinstance(v, AbstractDataset):
-            return v().prepare()
-        return v
+        self.repo_id = repo_id
+        self.data_files = data_files
+        self.split = split
 
     def download(self, force=False):
-        self.reference.__datamaestro__.download(force)
-
-    def hasfiles(self):
-        # We don't really have files
-        return False
+        try:
+            from datasets import load_dataset
+        except ModuleNotFoundError:
+            logging.error("the datasets library is not installed:")
+            logging.error("pip install datasets")
+            raise
 
+        self.dataset = load_dataset(self.repo_id, data_files=self.data_files)
+        return True
 
-Reference = deprecated("Use @reference instead of @Reference", reference)
+    def prepare(self):
+        return {
+            "repo_id": self.repo_id,
+            "data_files": self.data_files,
+            "split": self.split,
+        }
```

### Comparing `datamaestro-1.1.0/src/datamaestro/download/archive.py` & `datamaestro-1.2.0/src/datamaestro/download/archive.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/download/links.py` & `datamaestro-1.2.0/src/datamaestro/download/links.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/download/multiple.py` & `datamaestro-1.2.0/src/datamaestro/download/multiple.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/download/single.py` & `datamaestro-1.2.0/src/datamaestro/download/single.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/download/sync.py` & `datamaestro-1.2.0/src/datamaestro/download/sync.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/record.py` & `datamaestro-1.2.0/src/datamaestro/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,28 @@
                         " is already in the record"
                     )
                 self.items[base] = entry
 
     def __str__(self):
         return (
             "{"
-            + ", ".join(f"{key}: {value}" for key, value in self.items.items())
+            + ", ".join(
+                f"{key.__module__}.{key.__qualname__}: {value}"
+                for key, value in self.items.items()
+            )
+            + "}"
+        )
+
+    def __repr__(self):
+        return (
+            "{"
+            + ", ".join(
+                f"{key.__module__}.{key.__qualname__}: {repr(value)}"
+                for key, value in self.items.items()
+            )
             + "}"
         )
 
     def get(self, key: Type[T]) -> Optional[T]:
         """Get a given item or None if it does not exist"""
         try:
             return self[key]
```

### Comparing `datamaestro-1.1.0/src/datamaestro/registry.py` & `datamaestro-1.2.0/src/datamaestro/registry.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/search.py` & `datamaestro-1.2.0/src/datamaestro/search.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/settings.py` & `datamaestro-1.2.0/src/datamaestro/settings.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/sphinx.py` & `datamaestro-1.2.0/src/datamaestro/sphinx.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/stream/__init__.py` & `datamaestro-1.2.0/src/datamaestro/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/stream/lines.py` & `datamaestro-1.2.0/src/datamaestro/stream/lines.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/test/checks.py` & `datamaestro-1.2.0/src/datamaestro/test/checks.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/test/conftest.py` & `datamaestro-1.2.0/src/datamaestro/test/conftest.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/test/test_download_handlers.py` & `datamaestro-1.2.0/src/datamaestro/test/test_download_handlers.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/test/test_record.py` & `datamaestro-1.2.0/src/datamaestro/test/test_record.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro/utils.py` & `datamaestro-1.2.0/src/datamaestro/utils.py`

 * *Files identical despite different names*

### Comparing `datamaestro-1.1.0/src/datamaestro.egg-info/PKG-INFO` & `datamaestro-1.2.0/src/datamaestro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaestro
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Dataset management command line and API"
 Home-page: https://github.com/experimaestro/datamaestro
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: dataset manager
 Platform: any
```

### Comparing `datamaestro-1.1.0/src/datamaestro.egg-info/SOURCES.txt` & `datamaestro-1.2.0/src/datamaestro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

