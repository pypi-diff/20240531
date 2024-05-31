# Comparing `tmp/lcprogramtools-0.0.1.tar.gz` & `tmp/lcprogramtools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lcprogramtools-0.0.1.tar", last modified: Fri May 31 11:35:21 2024, max compression
+gzip compressed data, was "dist\lcprogramtools-0.0.2.tar", last modified: Fri May 31 11:42:17 2024, max compression
```

## Comparing `lcprogramtools-0.0.1.tar` & `lcprogramtools-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:35:21.194635 lcprogramtools-0.0.1/
--rw-rw-rw-   0        0        0      291 2024-05-31 11:35:21.193634 lcprogramtools-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 11:35:21.162634 lcprogramtools-0.0.1/lcprogramtools/
--rw-rw-rw-   0        0        0       48 2024-05-31 11:34:19.000000 lcprogramtools-0.0.1/lcprogramtools/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-31 11:34:16.000000 lcprogramtools-0.0.1/lcprogramtools/module.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:35:21.191643 lcprogramtools-0.0.1/lcprogramtools.egg-info/
--rw-rw-rw-   0        0        0      291 2024-05-31 11:35:20.000000 lcprogramtools-0.0.1/lcprogramtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-31 11:35:21.000000 lcprogramtools-0.0.1/lcprogramtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:35:20.000000 lcprogramtools-0.0.1/lcprogramtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-31 11:35:20.000000 lcprogramtools-0.0.1/lcprogramtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:35:21.195632 lcprogramtools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      344 2024-05-31 11:34:33.000000 lcprogramtools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:42:17.761954 lcprogramtools-0.0.2/
+-rw-rw-rw-   0        0        0      291 2024-05-31 11:42:17.748942 lcprogramtools-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 11:42:17.730941 lcprogramtools-0.0.2/lcprogramtools/
+-rw-rw-rw-   0        0        0      293 2024-05-31 11:41:59.000000 lcprogramtools-0.0.2/lcprogramtools/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-31 11:34:16.000000 lcprogramtools-0.0.2/lcprogramtools/module.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:42:17.746944 lcprogramtools-0.0.2/lcprogramtools.egg-info/
+-rw-rw-rw-   0        0        0      291 2024-05-31 11:42:17.000000 lcprogramtools-0.0.2/lcprogramtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-31 11:42:17.000000 lcprogramtools-0.0.2/lcprogramtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:42:17.000000 lcprogramtools-0.0.2/lcprogramtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-31 11:42:17.000000 lcprogramtools-0.0.2/lcprogramtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:42:17.763940 lcprogramtools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      344 2024-05-31 11:42:11.000000 lcprogramtools-0.0.2/setup.py
```

