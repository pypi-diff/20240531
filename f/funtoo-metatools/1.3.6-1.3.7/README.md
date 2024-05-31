# Comparing `tmp/funtoo-metatools-1.3.6.tar.gz` & `tmp/funtoo_metatools-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-metatools-1.3.6.tar", last modified: Sun Feb 25 07:58:31 2024, max compression
+gzip compressed data, was "funtoo_metatools-1.3.7.tar", last modified: Fri May 31 20:46:45 2024, max compression
```

## Comparing `funtoo-metatools-1.3.6.tar` & `funtoo_metatools-1.3.7.tar`

### file list

```diff
@@ -1,114 +1,122 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      118 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16379 2024-02-25 07:58:11.000000 funtoo-metatools-1.3.6/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1579 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1492 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/ROADMAP.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-02-25 07:57:56.000000 funtoo-metatools-1.3.6/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/blos-check
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4020 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      105 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     7143 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3917 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4996 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7601 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25486 2024-01-26 02:40:32.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25491 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9989 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19461 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9207 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14188 2024-02-16 00:09:35.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11198 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1579 2024-02-25 07:58:30.000000 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2098 2024-02-25 07:58:31.000000 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-02-25 07:58:30.000000 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2024-02-25 07:58:30.000000 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2024-02-25 07:58:30.000000 funtoo-metatools-1.3.6/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.102867 funtoo-metatools-1.3.6/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1149 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/blos.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1287 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/cmd.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5486 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2765 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3504 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8962 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    30966 2024-01-01 00:24:52.000000 funtoo-metatools-1.3.6/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      701 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    35017 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    22319 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/release.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21790 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18121 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-02-25 07:58:27.000000 funtoo-metatools-1.3.6/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/yaml_util.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/metatools/zmq/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/zmq/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/zmq/app_core.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/zmq/key_monkey.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/zmq/zmq_msg_breezyops.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/metatools/zmq/zmq_msg_core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-02-25 07:58:31.113700 funtoo-metatools-1.3.6/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2024-02-25 07:58:27.000000 funtoo-metatools-1.3.6/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2023-11-26 02:39:37.000000 funtoo-metatools-1.3.6/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      118 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17626 2024-05-31 20:41:28.000000 funtoo_metatools-1.3.7/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1579 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1492 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/ROADMAP.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-05-31 20:41:35.000000 funtoo_metatools-1.3.7/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/blos-check
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4020 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      105 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     7143 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3917 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4996 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7601 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.829121 funtoo_metatools-1.3.7/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25486 2024-01-26 02:40:32.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25527 2024-05-28 01:28:44.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9989 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15463 2024-05-28 02:40:09.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9207 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14188 2024-02-16 00:09:35.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11198 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1579 2024-05-31 20:46:45.000000 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2278 2024-05-31 20:46:45.000000 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-05-31 20:46:45.000000 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2024-05-31 20:46:45.000000 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2024-05-31 20:46:45.000000 funtoo_metatools-1.3.7/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1149 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/blos.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1287 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/cmd.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5486 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2765 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3504 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8962 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    30966 2024-01-01 00:24:52.000000 funtoo_metatools-1.3.7/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/fetch_cache.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/generator/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/generator/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1094 2024-04-13 17:57:10.000000 funtoo_metatools-1.3.7/metatools/generator/common.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7627 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/generator/transform.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      701 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    35059 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15272 2024-02-25 08:22:54.000000 funtoo_metatools-1.3.7/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    22319 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/release.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21790 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18121 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/tree.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/version/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/version/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2451 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/version/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      969 2024-04-11 20:45:03.000000 funtoo_metatools-1.3.7/metatools/version/generic.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-05-31 20:41:39.000000 funtoo_metatools-1.3.7/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/metatools/zmq/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/zmq/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-05-31 20:46:45.839121 funtoo_metatools-1.3.7/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2024-05-31 20:41:39.000000 funtoo_metatools-1.3.7/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2023-11-26 02:39:37.000000 funtoo_metatools-1.3.7/subpop.yaml
```

### Comparing `funtoo-metatools-1.3.6/.pre-commit-config.yaml` & `funtoo_metatools-1.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/ChangeLog.rst` & `funtoo_metatools-1.3.7/ChangeLog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+metatools 1.3.7
+===============
+
+Released on May 31, 2024.
+
+This is a feature and bug fix release.
+
+* An API change for ``BreezyBuild``'s ``artifacts=`` keyword
+  argument. Now, if a dictionary is specified, then this means
+  that each dictionary key is a conditional USE setting for
+  when the artifact or list of artifacts should be downloaded.
+  The special ``"global"`` key can be used to also specify
+  non-conditional downloads. Correspondingly, the ``assets=``
+  ``github.py`` ``release_gen()`` keyword argument has been
+  updated to work similarly, allowing for conditional USE to
+  be specified easily in ``github-1`` autogens via the ``assets:``
+  YAML. This also allows us to use ``SRC_URI="{{src_uri}}"``
+  almost globally in all templates.
+
+* For autogens, Implement ``versions.generic`` code to replace
+  the need to use Python's ``packaging.version`` code directly.
+  This prevents possible future breakage due to upstream Python
+  version logic changes and should be used by all autogens and
+  generators going forward.
+
+* Gentoo-compatible version code which is a work in progress.
+
+* Improved logging and error messages.
+
+* Disable moonbeam (intra-metatools messaging framework) if not
+  absolutely needed (thanks ``@borisp``)
+
+
 metatools 1.3.6
 ===============
 
 Released on February 25, 2024.
 
 This is a general bug fix release.
```

### Comparing `funtoo-metatools-1.3.6/PKG-INFO` & `funtoo_metatools-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.6
+Version: 1.3.7
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.6/README.rst` & `funtoo_metatools-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/ROADMAP.rst` & `funtoo_metatools-1.3.7/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/blos` & `funtoo_metatools-1.3.7/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/blos-check` & `funtoo_metatools-1.3.7/bin/blos-check`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/deepdive` & `funtoo_metatools-1.3.7/bin/deepdive`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/deepquery` & `funtoo_metatools-1.3.7/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/distfile-kit-fetch` & `funtoo_metatools-1.3.7/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/distfile-stats` & `funtoo_metatools-1.3.7/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/doit` & `funtoo_metatools-1.3.7/bin/doit`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/fastpull-daemon` & `funtoo_metatools-1.3.7/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/fastpull-daemon-ng` & `funtoo_metatools-1.3.7/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/fastpull-fixer` & `funtoo_metatools-1.3.7/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/fetch` & `funtoo_metatools-1.3.7/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/interkit-links` & `funtoo_metatools-1.3.7/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/list-kits` & `funtoo_metatools-1.3.7/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/mcafee-tool` & `funtoo_metatools-1.3.7/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/merge-gentoo-staging` & `funtoo_metatools-1.3.7/bin/merge-gentoo-staging`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/merge-kits` & `funtoo_metatools-1.3.7/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/missing-links` & `funtoo_metatools-1.3.7/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/release-yaml-test` & `funtoo_metatools-1.3.7/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/reposcan` & `funtoo_metatools-1.3.7/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/storage-test` & `funtoo_metatools-1.3.7/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/bin/test-metadata-extract` & `funtoo_metatools-1.3.7/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/deprecated/mongo_backends.py` & `funtoo_metatools-1.3.7/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/Makefile` & `funtoo_metatools-1.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/_ext/_static/consoleoutput.css` & `funtoo_metatools-1.3.7/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/_ext/consoleoutput.py` & `funtoo_metatools-1.3.7/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/autogen-dev.rst` & `funtoo_metatools-1.3.7/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/autogen.rst` & `funtoo_metatools-1.3.7/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/conf.py` & `funtoo_metatools-1.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/drafts/fastpull_object_store.rst` & `funtoo_metatools-1.3.7/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/drafts/repo_defs.rst` & `funtoo_metatools-1.3.7/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/features/dynamic-archives.rst` & `funtoo_metatools-1.3.7/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/index.rst` & `funtoo_metatools-1.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/install.rst` & `funtoo_metatools-1.3.7/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/intro.rst` & `funtoo_metatools-1.3.7/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/docs/meta-repo.rst` & `funtoo_metatools-1.3.7/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/autogen.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/ebuild.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/ebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import asyncio
 import logging
 import os
 import shutil
 import threading
 from asyncio import Task
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
 from collections.abc import Mapping
 from datetime import datetime
 from subprocess import getstatusoutput
 from typing import Optional, Tuple
 
 import jinja2
 
@@ -484,15 +484,15 @@
 				raise TypeError(f"Unrecognized type for revision= argument for {self.catpkg}: {repr(type(self._revision))}")
 			pkgtools.model.log.debug(f"Fixup-revision: {self.catpkg}: {type(self._revision)} {self._revision}")
 
 	def iter_artifacts(self):
 		if type(self.artifacts) == list:
 			for artifact in self.artifacts:
 				yield artifact
-		elif type(self.artifacts) in (dict, OrderedDict):
+		elif type(self.artifacts) in (dict, OrderedDict, defaultdict):
 			for key, artifact in self.artifacts.items():
 				if isinstance(artifact, list):
 					for lil_art in artifact:
 						yield lil_art
 				else:
 					yield artifact
 		else:
@@ -519,21 +519,20 @@
 					out += f"{artifact_list.src_uri}\n"
 				else:
 					ValueError(f"Found {artifact_list} of type {type(artifact_list)} inside artifacts.")
 			else:
 				if isinstance(artifact_list, list):
 					out += f"{key}? (\n"
 					for artifact in artifact_list:
-						out += f"{artifact.src_uri}\n"
+						out += f"  {artifact.src_uri}\n"
 					out += ")\n"
 				elif isinstance(artifact_list, Archive) or isinstance(artifact_list, Artifact):
 					out += f"{key}? ( {artifact_list.src_uri} )\n"
 				else:
 					ValueError(f"Found {artifact_list} of type {type(artifact_list)} inside artifacts.")
-
 		return out
 
 	async def setup(self):
 		"""
 		This method performs some special setup steps. We tend to treat Artifacts as stand-alone objects -- and they
 		can be -- such as if you instantiate an Artifact in `generate()` and fetch it because you need to extract it
 		and look inside it.
@@ -698,15 +697,15 @@
 						raise BreezyError(f"Unknown error processing {template_file}: {repr(te)}")
 			except FileNotFoundError as e:
 				log.error(f"Could not find template: {template_file}")
 				raise BreezyError(f"Template file not found: {template_file}")
 		else:
 			template = jinja2.Template(self.template_text)
 		# allow "src_uri" to be used inside all templates to print out official src_uri of all artifacts.
-		template.globals.update({"src_uri": self.src_uri})
+		template.globals.update({"src_uri": self.src_uri_with_use})
 		template.globals.update({"src_uri_with_use": self.src_uri_with_use})
 		with open(self.output_ebuild_path, "wb") as myf:
 			try:
 				myf.write(template.render(**self.template_args).encode("utf-8"))
 			except Exception as te:
 				raise BreezyError(f"Error rendering template: {repr(te)}")
 		log.info("Created: " + os.path.relpath(self.output_ebuild_path))
```

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/fetch.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/fetch.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/golang.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/golang.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/http.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/http.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/meson.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/pages.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/pyhelper.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo/pkgtools/rust.py` & `funtoo_metatools-1.3.7/funtoo/pkgtools/rust.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/funtoo_metatools.egg-info/PKG-INFO` & `funtoo_metatools-1.3.7/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.6
+Version: 1.3.7
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.6/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo_metatools-1.3.7/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -85,12 +85,18 @@
 metatools/config/autogen.py
 metatools/config/base.py
 metatools/config/merge.py
 metatools/config/mongodb.py
 metatools/fastpull/__init__.py
 metatools/fastpull/core.py
 metatools/fastpull/spider.py
+metatools/generator/__init__.py
+metatools/generator/common.py
+metatools/generator/transform.py
+metatools/version/__init__.py
+metatools/version/base.py
+metatools/version/generic.py
 metatools/zmq/__init__.py
 metatools/zmq/app_core.py
 metatools/zmq/key_monkey.py
 metatools/zmq/zmq_msg_breezyops.py
 metatools/zmq/zmq_msg_core.py
```

### Comparing `funtoo-metatools-1.3.6/make.sh` & `funtoo_metatools-1.3.7/make.sh`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/blos.py` & `funtoo_metatools-1.3.7/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/cmd.py` & `funtoo_metatools-1.3.7/metatools/cmd.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/config/autogen.py` & `funtoo_metatools-1.3.7/metatools/config/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/config/base.py` & `funtoo_metatools-1.3.7/metatools/config/base.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/config/merge.py` & `funtoo_metatools-1.3.7/metatools/config/merge.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/context.py` & `funtoo_metatools-1.3.7/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/fastpull/core.py` & `funtoo_metatools-1.3.7/metatools/fastpull/core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/fastpull/spider.py` & `funtoo_metatools-1.3.7/metatools/fastpull/spider.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/fetch_cache.py` & `funtoo_metatools-1.3.7/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/hashutils.py` & `funtoo_metatools-1.3.7/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/kit.py` & `funtoo_metatools-1.3.7/metatools/kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,16 @@
 	# Does this job controller update meta-repo? If so, this get set to True, otherwise False.
 	write = False
 	moonbeam = None
 	moonbeam_task = None
 
 	def __init__(self, model, write=None):
 		self.model = model
-		self.moonbeam = MoonBeam("merge-kits", bind_addr=f"ipc://{self.model.moonbeam_socket}")
+		if self.moonbeam:
+			self.moonbeam = MoonBeam("merge-kits", bind_addr=f"ipc://{self.model.moonbeam_socket}")
 		if write:
 			self.write = write
 		assert isinstance(self.write, bool)
 
 	def cleanup_error_logs(self):
 		# This should be explicitly called at the beginning of every command that generates metadata for kits:
 
@@ -821,15 +822,16 @@
 		success = await other_pool.run()
 		return success
 
 	async def distfile_sync(self):
 		await self.process_all_kits_in_release(method="distfile_scan")
 
 	async def generate(self):
-		self.moonbeam_task = asyncio.create_task(self.moonbeam.start())
+		if self.moonbeam:
+			self.moonbeam_task = asyncio.create_task(self.moonbeam.start())
 		model.log.debug(f"moonbeam: {self.moonbeam} {self.moonbeam_task}")
 		meta_repo_config = model.release_yaml.get_repo_config("meta-repo")
 		self.meta_repo = model.git_class(
 			name="meta-repo",
 			branch=model.release,
 			url=meta_repo_config['url'] if model.prod else None,
 			root=model.dest_trees + "/meta-repo",
```

### Comparing `funtoo-metatools-1.3.6/metatools/kit_cache.py` & `funtoo_metatools-1.3.7/metatools/kit_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/metadata.py` & `funtoo_metatools-1.3.7/metatools/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,20 +139,21 @@
 				ls = line.split()
 				if len(ls) <= 3 or ls[0] != "DIST":
 					continue
 				pos = 3
 				digests = {}
 				while pos < len(ls):
 					hash_type = ls[pos].lower()
+					if pos + 2 > len(ls):
+						raise ValueError(f'Invalid Manifest file format: {man_file}')
 					hash_digest = ls[pos + 1]
 					digests[hash_type] = hash_digest
 					pos += 2
 				man_info[ls[1]] = {"size": ls[2], "hashes": digests}
 	return man_info
-	return man_info
 
 
 def extract_uris(src_uri):
 	"""
 	This function will take a SRC_URI value from an ebuild, and it will return a dictionary in the following format:
 
 	{ "filename1.tar.gz" : { "src_uri" : [ "https://url1", "https//url2" ] } }
```

### Comparing `funtoo-metatools-1.3.6/metatools/model.py` & `funtoo_metatools-1.3.7/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/pretty_logging.py` & `funtoo_metatools-1.3.7/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/release.py` & `funtoo_metatools-1.3.7/metatools/release.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/steps.py` & `funtoo_metatools-1.3.7/metatools/steps.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/store.py` & `funtoo_metatools-1.3.7/metatools/store.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/tree.py` & `funtoo_metatools-1.3.7/metatools/tree.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/yaml_util.py` & `funtoo_metatools-1.3.7/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/zmq/app_core.py` & `funtoo_metatools-1.3.7/metatools/zmq/app_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/zmq/key_monkey.py` & `funtoo_metatools-1.3.7/metatools/zmq/key_monkey.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/zmq/zmq_msg_breezyops.py` & `funtoo_metatools-1.3.7/metatools/zmq/zmq_msg_breezyops.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/metatools/zmq/zmq_msg_core.py` & `funtoo_metatools-1.3.7/metatools/zmq/zmq_msg_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.6/setup.py` & `funtoo_metatools-1.3.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.3.6",
+	version="1.3.7",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
```

### Comparing `funtoo-metatools-1.3.6/setup.py.in` & `funtoo_metatools-1.3.7/setup.py.in`

 * *Files identical despite different names*

