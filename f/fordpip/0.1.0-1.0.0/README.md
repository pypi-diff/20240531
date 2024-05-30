# Comparing `tmp/fordpip-0.1.0.tar.gz` & `tmp/fordpip-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fordpip-0.1.0.tar", last modified: Mon Apr 15 17:49:44 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fordpip-0.1.0.tar` & `fordpip-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:49:44.303443 fordpip-0.1.0/
--rw-rw-rw-   0        0        0      304 2024-04-15 17:49:44.301445 fordpip-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:49:44.298455 fordpip-0.1.0/fordpip.egg-info/
--rw-rw-rw-   0        0        0      304 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:49:44.304542 fordpip-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-04-15 17:38:18.000000 fordpip-0.1.0/setup.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fordpip-1.0.0/.pypirc
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fordpip-1.0.0/requirements.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip/start.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip/test.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip.egg-info/requires.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fordpip-1.0.0/fordpip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fordpip-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fordpip-1.0.0/LICENSE
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fordpip-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fordpip-1.0.0/readme.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fordpip-1.0.0/PKG-INFO
```

