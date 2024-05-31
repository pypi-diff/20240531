# Comparing `tmp/blockchain_data_subnet_shared_libs-0.0.2.tar.gz` & `tmp/blockchain_data_subnet_shared_libs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain_data_subnet_shared_libs-0.0.2.tar", last modified: Fri May 31 11:30:50 2024, max compression
+gzip compressed data, was "blockchain_data_subnet_shared_libs-1.0.0.tar", last modified: Thu May 30 19:41:18 2024, max compression
```

## Comparing `blockchain_data_subnet_shared_libs-0.0.2.tar` & `blockchain_data_subnet_shared_libs-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-31 11:30:50.523525 blockchain_data_subnet_shared_libs-0.0.2/
--rw-r--r--   0 saroot    (1000) saroot    (1000)     1069 2024-05-30 19:18:28.000000 blockchain_data_subnet_shared_libs-0.0.2/LICENSE
--rw-r--r--   0 saroot    (1000) saroot    (1000)      587 2024-05-31 11:30:50.523525 blockchain_data_subnet_shared_libs-0.0.2/PKG-INFO
--rw-r--r--   0 saroot    (1000) saroot    (1000)      151 2024-05-31 11:25:17.000000 blockchain_data_subnet_shared_libs-0.0.2/README.md
-drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-31 11:30:50.523525 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/
--rw-r--r--   0 saroot    (1000) saroot    (1000)      587 2024-05-31 11:30:50.000000 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/PKG-INFO
--rw-r--r--   0 saroot    (1000) saroot    (1000)      315 2024-05-31 11:30:50.000000 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/SOURCES.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-31 11:30:50.000000 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/dependency_links.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)       19 2024-05-31 11:30:50.000000 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/requires.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-31 11:30:50.000000 blockchain_data_subnet_shared_libs-0.0.2/blockchain_data_subnet_shared_libs.egg-info/top_level.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)       38 2024-05-31 11:30:50.523525 blockchain_data_subnet_shared_libs-0.0.2/setup.cfg
--rw-r--r--   0 saroot    (1000) saroot    (1000)      779 2024-05-31 11:30:23.000000 blockchain_data_subnet_shared_libs-0.0.2/setup.py
+drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/
+-rw-r--r--   0 saroot    (1000) saroot    (1000)     1069 2024-05-30 19:18:28.000000 blockchain_data_subnet_shared_libs-1.0.0/LICENSE
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      543 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/PKG-INFO
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      131 2024-05-30 15:27:10.000000 blockchain_data_subnet_shared_libs-1.0.0/README.md
+drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      543 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/PKG-INFO
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      315 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)       19 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/requires.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/top_level.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)       38 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/setup.cfg
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      735 2024-05-30 19:39:11.000000 blockchain_data_subnet_shared_libs-1.0.0/setup.py
```

### Comparing `blockchain_data_subnet_shared_libs-0.0.2/LICENSE` & `blockchain_data_subnet_shared_libs-1.0.0/LICENSE`

 * *Files identical despite different names*

