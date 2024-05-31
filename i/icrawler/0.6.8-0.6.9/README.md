# Comparing `tmp/icrawler-0.6.8.tar.gz` & `tmp/icrawler-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icrawler-0.6.8.tar", last modified: Wed May 15 04:20:23 2024, max compression
+gzip compressed data, was "icrawler-0.6.9.tar", last modified: Fri May 31 08:57:07 2024, max compression
```

## Comparing `icrawler-0.6.8.tar` & `icrawler-0.6.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 04:20:19.000000 icrawler-0.6.8/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-15 04:20:19.000000 icrawler-0.6.8/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 04:20:19.000000 icrawler-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 04:20:19.000000 icrawler-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 04:20:19.000000 icrawler-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 04:20:19.000000 icrawler-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-15 04:20:23.001942 icrawler-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-15 04:20:19.000000 icrawler-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/builtin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/extend.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/release_notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-15 04:20:19.000000 icrawler-0.6.8/examples/crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 04:20:19.000000 icrawler-0.6.8/examples/filelist_demo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.997942 icrawler-0.6.8/icrawler/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.997942 icrawler-0.6.8/icrawler/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/flickr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/urllist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/google_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/cached_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19650 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/proxy_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-15 04:20:19.000000 icrawler-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 04:20:19.000000 icrawler-0.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:20:23.001942 icrawler-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:20:19.000000 icrawler-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-15 04:20:19.000000 icrawler-0.6.8/tests/test_todo.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 04:20:19.000000 icrawler-0.6.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.832188 icrawler-0.6.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 08:57:03.000000 icrawler-0.6.9/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.832188 icrawler-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-31 08:57:03.000000 icrawler-0.6.9/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-31 08:57:03.000000 icrawler-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-31 08:57:03.000000 icrawler-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-31 08:57:03.000000 icrawler-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 08:57:03.000000 icrawler-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-31 08:57:07.840188 icrawler-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-31 08:57:03.000000 icrawler-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.836188 icrawler-0.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/extend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-31 08:57:03.000000 icrawler-0.6.9/docs/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.836188 icrawler-0.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-31 08:57:03.000000 icrawler-0.6.9/examples/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 08:57:03.000000 icrawler-0.6.9/examples/filelist_demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.836188 icrawler-0.6.9/icrawler/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/icrawler/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/builtin/urllist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/icrawler/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/storage/google_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/icrawler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/cached_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19650 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/proxy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-31 08:57:03.000000 icrawler-0.6.9/icrawler/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/icrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 08:57:07.000000 icrawler-0.6.9/icrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-31 08:57:03.000000 icrawler-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 08:57:03.000000 icrawler-0.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:57:07.840188 icrawler-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:57:03.000000 icrawler-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:07.840188 icrawler-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-31 08:57:03.000000 icrawler-0.6.9/tests/test_todo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-31 08:57:03.000000 icrawler-0.6.9/tox.ini
```

### Comparing `icrawler-0.6.8/.github/workflows/push.yaml` & `icrawler-0.6.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/.pre-commit-config.yaml` & `icrawler-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/LICENSE` & `icrawler-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/PKG-INFO` & `icrawler-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icrawler
-Version: 0.6.8
+Version: 0.6.9
 Summary: A multi-thread crawler framework with many builtin image crawlers provided.
 Author-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kai Chen
```

### Comparing `icrawler-0.6.8/README.rst` & `icrawler-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/Makefile` & `icrawler-0.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/api.rst` & `icrawler-0.6.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/builtin.rst` & `icrawler-0.6.9/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/conf.py` & `icrawler-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/extend.rst` & `icrawler-0.6.9/docs/extend.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/make.bat` & `icrawler-0.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/proxy.rst` & `icrawler-0.6.9/docs/proxy.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/docs/release_notes.rst` & `icrawler-0.6.9/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/examples/crawl.py` & `icrawler-0.6.9/examples/crawl.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/baidu.py` & `icrawler-0.6.9/icrawler/builtin/baidu.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/bing.py` & `icrawler-0.6.9/icrawler/builtin/bing.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/filter.py` & `icrawler-0.6.9/icrawler/builtin/filter.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/flickr.py` & `icrawler-0.6.9/icrawler/builtin/flickr.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/google.py` & `icrawler-0.6.9/icrawler/builtin/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,21 +157,20 @@
             # txt = re.sub(r"^AF_initDataCallback\({.*key: 'ds:(\d)'.+data:function\(\){return (.+)}}\);?$",
             #             "\\2", txt, 0, re.DOTALL)
             # meta = json.loads(txt)
             # data = meta[31][0][12][2]
             # uris = [img[1][3][0] for img in data if img[0] == 1]
 
             uris = re.findall(r"http[^\[]*?.(?:jpg|png|bmp)", txt)
+            if not uris:
+                uris = re.findall(r"http[^\[]*?\.(?:jpg|png|bmp)", txt)
             uris = [bytes(uri, "utf-8").decode("unicode-escape") for uri in uris]
             if uris:
                 return [{"file_url": uri} for uri in uris]
 
-            uris = re.findall(r"http[^\[]*?\.(?:jpg|png|bmp)", txt)
-            return [{"file_url": uri} for uri in uris]
-
 
 class GoogleImageCrawler(Crawler):
     def __init__(
         self, feeder_cls=GoogleFeeder, parser_cls=GoogleParser, downloader_cls=ImageDownloader, *args, **kwargs
     ):
         super().__init__(feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
```

### Comparing `icrawler-0.6.8/icrawler/builtin/greedy.py` & `icrawler-0.6.9/icrawler/builtin/greedy.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/builtin/urllist.py` & `icrawler-0.6.9/icrawler/builtin/urllist.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/crawler.py` & `icrawler-0.6.9/icrawler/crawler.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/downloader.py` & `icrawler-0.6.9/icrawler/downloader.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/feeder.py` & `icrawler-0.6.9/icrawler/feeder.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/parser.py` & `icrawler-0.6.9/icrawler/parser.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/storage/base.py` & `icrawler-0.6.9/icrawler/storage/base.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/storage/filesystem.py` & `icrawler-0.6.9/icrawler/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/storage/google_storage.py` & `icrawler-0.6.9/icrawler/storage/google_storage.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/utils/cached_queue.py` & `icrawler-0.6.9/icrawler/utils/cached_queue.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/utils/proxy_pool.py` & `icrawler-0.6.9/icrawler/utils/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/utils/session.py` & `icrawler-0.6.9/icrawler/utils/session.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/utils/signal.py` & `icrawler-0.6.9/icrawler/utils/signal.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler/utils/thread_pool.py` & `icrawler-0.6.9/icrawler/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/icrawler.egg-info/PKG-INFO` & `icrawler-0.6.9/icrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icrawler
-Version: 0.6.8
+Version: 0.6.9
 Summary: A multi-thread crawler framework with many builtin image crawlers provided.
 Author-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kai Chen
```

### Comparing `icrawler-0.6.8/icrawler.egg-info/SOURCES.txt` & `icrawler-0.6.9/icrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/pyproject.toml` & `icrawler-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.8/tests/test_todo.py` & `icrawler-0.6.9/tests/test_todo.py`

 * *Files identical despite different names*

