# Comparing `tmp/test_1_varify_ic-0.1.tar.gz` & `tmp/test_1_varify_ic-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_1_varify_ic-0.1.tar", last modified: Sun May  5 22:09:54 2024, max compression
+gzip compressed data, was "test_1_varify_ic-0.2.tar", last modified: Fri May 31 15:27:43 2024, max compression
```

## Comparing `test_1_varify_ic-0.1.tar` & `test_1_varify_ic-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 22:09:54.823086 test_1_varify_ic-0.1/
--rw-rw-rw-   0        0        0      261 2024-05-05 22:09:54.820891 test_1_varify_ic-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-05-05 22:09:44.000000 test_1_varify_ic-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 22:09:54.823086 test_1_varify_ic-0.1/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-05-05 22:08:26.000000 test_1_varify_ic-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:09:54.819888 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-05 22:09:54.000000 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-05 22:09:54.000000 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:09:54.000000 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 22:09:54.000000 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:09:54.000000 test_1_varify_ic-0.1/test_1_varify_ic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 15:27:43.464908 test_1_varify_ic-0.2/
+-rw-rw-rw-   0        0        0     2526 2024-05-31 15:27:43.462910 test_1_varify_ic-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2245 2024-05-31 15:15:43.000000 test_1_varify_ic-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 15:27:43.464908 test_1_varify_ic-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-31 15:27:38.000000 test_1_varify_ic-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:27:43.460901 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/
+-rw-rw-rw-   0        0        0     2526 2024-05-31 15:27:43.000000 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-31 15:27:43.000000 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:27:43.000000 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 15:27:43.000000 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:27:43.000000 test_1_varify_ic-0.2/test_1_varify_ic.egg-info/top_level.txt
```

