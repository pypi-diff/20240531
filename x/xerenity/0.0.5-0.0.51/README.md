# Comparing `tmp/xerenity-0.0.5.tar.gz` & `tmp/xerenity-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerenity-0.0.5.tar", last modified: Fri May 31 15:59:03 2024, max compression
+gzip compressed data, was "xerenity-0.0.51.tar", last modified: Fri May 31 18:48:51 2024, max compression
```

## Comparing `xerenity-0.0.5.tar` & `xerenity-0.0.51.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.834955 xerenity-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:58:54.000000 xerenity-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:59:03.834955 xerenity-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:59:03.834955 xerenity-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-31 15:58:54.000000 xerenity-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.830955 xerenity-0.0.5/xerenity/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-31 15:58:54.000000 xerenity-0.0.5/xerenity/Xerenity.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 15:58:54.000000 xerenity-0.0.5/xerenity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.834955 xerenity-0.0.5/xerenity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:51.719297 xerenity-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:42.000000 xerenity-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-31 18:48:51.719297 xerenity-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:48:51.719297 xerenity-0.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-31 18:48:42.000000 xerenity-0.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:51.715297 xerenity-0.0.51/xerenity/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:51.719297 xerenity-0.0.51/xerenity/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:42.000000 xerenity-0.0.51/xerenity/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-31 18:48:42.000000 xerenity-0.0.51/xerenity/connection/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:51.719297 xerenity-0.0.51/xerenity/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:42.000000 xerenity-0.0.51/xerenity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-31 18:48:42.000000 xerenity-0.0.51/xerenity/search/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:51.719297 xerenity-0.0.51/xerenity/xerenity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-31 18:48:51.000000 xerenity-0.0.51/xerenity/xerenity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 18:48:51.000000 xerenity-0.0.51/xerenity/xerenity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:48:51.000000 xerenity-0.0.51/xerenity/xerenity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:48:51.000000 xerenity-0.0.51/xerenity/xerenity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 18:48:51.000000 xerenity-0.0.51/xerenity/xerenity.egg-info/top_level.txt
```

