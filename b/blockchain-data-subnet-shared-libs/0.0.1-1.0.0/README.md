# Comparing `tmp/blockchain_data_subnet_shared_libs-0.0.1.tar.gz` & `tmp/blockchain_data_subnet_shared_libs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain_data_subnet_shared_libs-0.0.1.tar", last modified: Fri May 31 11:29:10 2024, max compression
+gzip compressed data, was "blockchain_data_subnet_shared_libs-1.0.0.tar", last modified: Thu May 30 19:41:18 2024, max compression
```

## Comparing `blockchain_data_subnet_shared_libs-0.0.1.tar` & `blockchain_data_subnet_shared_libs-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-31 11:29:10.736940 blockchain_data_subnet_shared_libs-0.0.1/
--rw-r--r--   0 saroot    (1000) saroot    (1000)     1069 2024-05-30 19:18:28.000000 blockchain_data_subnet_shared_libs-0.0.1/LICENSE
--rw-r--r--   0 saroot    (1000) saroot    (1000)      587 2024-05-31 11:29:10.736940 blockchain_data_subnet_shared_libs-0.0.1/PKG-INFO
--rw-r--r--   0 saroot    (1000) saroot    (1000)      151 2024-05-31 11:25:17.000000 blockchain_data_subnet_shared_libs-0.0.1/README.md
-drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-31 11:29:10.736940 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/
--rw-r--r--   0 saroot    (1000) saroot    (1000)      587 2024-05-31 11:29:10.000000 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/PKG-INFO
--rw-r--r--   0 saroot    (1000) saroot    (1000)      315 2024-05-31 11:29:10.000000 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/SOURCES.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-31 11:29:10.000000 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/dependency_links.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)       19 2024-05-31 11:29:10.000000 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/requires.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-31 11:29:10.000000 blockchain_data_subnet_shared_libs-0.0.1/blockchain_data_subnet_shared_libs.egg-info/top_level.txt
--rw-r--r--   0 saroot    (1000) saroot    (1000)       38 2024-05-31 11:29:10.736940 blockchain_data_subnet_shared_libs-0.0.1/setup.cfg
--rw-r--r--   0 saroot    (1000) saroot    (1000)      779 2024-05-31 11:25:17.000000 blockchain_data_subnet_shared_libs-0.0.1/setup.py
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

### Comparing `blockchain_data_subnet_shared_libs-0.0.1/LICENSE` & `blockchain_data_subnet_shared_libs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain_data_subnet_shared_libs-0.0.1/setup.py` & `blockchain_data_subnet_shared_libs-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='blockchain-data-subnet-shared-libs',
-    version='0.0.1',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'pydantic',
         'bittensor',
     ],
     author='Dmytro Savenkov',
     author_email='dmytro.savenkov@chain-insights.ai',
-    description='All shared libs that all components, executables, and services of blockchain data subnet are based on',
-    url='https://github.com/blockchain-insights/blockchain-data-subnet-shared-libs',
+    description='All shared libs that all components, executables, and services of Sn15 are based on',
+    url='https://github.com/YOUR_USERNAME/YOUR_REPOSITORY',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.6',
 )
```

