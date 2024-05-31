# Comparing `tmp/cdepy-0.1.8.tar.gz` & `tmp/cdepy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdepy-0.1.8.tar", last modified: Thu May 23 02:46:50 2024, max compression
+gzip compressed data, was "cdepy-0.1.9.tar", last modified: Fri May 24 01:24:44 2024, max compression
```

## Comparing `cdepy-0.1.8.tar` & `cdepy-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.908887 cdepy-0.1.8/
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1070 2024-02-13 18:32:02.000000 cdepy-0.1.8/LICENSE
--rw-r--r--   0 pauldefusco   (502) staff       (20)       34 2023-10-11 18:06:12.000000 cdepy-0.1.8/MANIFEST.in
--rw-r--r--   0 pauldefusco   (502) staff       (20)     6565 2024-05-23 02:46:50.908706 cdepy-0.1.8/PKG-INFO
--rw-r--r--   0 pauldefusco   (502) staff       (20)     6005 2024-05-23 02:46:06.000000 cdepy-0.1.8/README.md
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.907290 cdepy-0.1.8/cdepy/
--rw-r--r--   0 pauldefusco   (502) staff       (20)        0 2023-10-11 17:22:42.000000 cdepy-0.1.8/cdepy/__init__.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     6014 2024-05-23 02:35:46.000000 cdepy-0.1.8/cdepy/cdeairflowpython.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1173 2024-02-13 17:13:33.000000 cdepy-0.1.8/cdepy/cdeconnection.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     5232 2024-02-13 17:13:32.000000 cdepy-0.1.8/cdepy/cdejob.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)    15142 2024-02-13 17:13:31.000000 cdepy-0.1.8/cdepy/cdemanager.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1663 2024-02-13 17:13:29.000000 cdepy-0.1.8/cdepy/cderesource.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     2116 2024-02-13 18:48:17.000000 cdepy-0.1.8/cdepy/utils.py
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.908441 cdepy-0.1.8/cdepy.egg-info/
--rw-r--r--   0 pauldefusco   (502) staff       (20)     6565 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/PKG-INFO
--rw-r--r--   0 pauldefusco   (502) staff       (20)      321 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/SOURCES.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)        1 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/dependency_links.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)       60 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/requires.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)        6 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/top_level.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)       38 2024-05-23 02:46:50.908947 cdepy-0.1.8/setup.cfg
--rw-r--r--   0 pauldefusco   (502) staff       (20)      951 2024-05-23 02:36:09.000000 cdepy-0.1.8/setup.py
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-24 01:24:44.530079 cdepy-0.1.9/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1070 2024-02-13 18:32:02.000000 cdepy-0.1.9/LICENSE
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       34 2023-10-11 18:06:12.000000 cdepy-0.1.9/MANIFEST.in
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     7848 2024-05-24 01:24:44.529910 cdepy-0.1.9/PKG-INFO
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     7288 2024-05-24 01:22:57.000000 cdepy-0.1.9/README.md
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-24 01:24:44.528870 cdepy-0.1.9/cdepy/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        0 2023-10-11 17:22:42.000000 cdepy-0.1.9/cdepy/__init__.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     6014 2024-05-23 02:35:46.000000 cdepy-0.1.9/cdepy/cdeairflowpython.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1173 2024-02-13 17:13:33.000000 cdepy-0.1.9/cdepy/cdeconnection.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     5232 2024-02-13 17:13:32.000000 cdepy-0.1.9/cdepy/cdejob.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)    15142 2024-02-13 17:13:31.000000 cdepy-0.1.9/cdepy/cdemanager.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     4119 2024-05-24 01:17:54.000000 cdepy-0.1.9/cdepy/cderepositories.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1663 2024-02-13 17:13:29.000000 cdepy-0.1.9/cdepy/cderesource.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     2116 2024-02-13 18:48:17.000000 cdepy-0.1.9/cdepy/utils.py
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-24 01:24:44.529653 cdepy-0.1.9/cdepy.egg-info/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     7848 2024-05-24 01:24:44.000000 cdepy-0.1.9/cdepy.egg-info/PKG-INFO
+-rw-r--r--   0 pauldefusco   (502) staff       (20)      346 2024-05-24 01:24:44.000000 cdepy-0.1.9/cdepy.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        1 2024-05-24 01:24:44.000000 cdepy-0.1.9/cdepy.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       60 2024-05-24 01:24:44.000000 cdepy-0.1.9/cdepy.egg-info/requires.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        6 2024-05-24 01:24:44.000000 cdepy-0.1.9/cdepy.egg-info/top_level.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       38 2024-05-24 01:24:44.530147 cdepy-0.1.9/setup.cfg
+-rw-r--r--   0 pauldefusco   (502) staff       (20)      951 2024-05-24 01:24:05.000000 cdepy-0.1.9/setup.py
```

### Comparing `cdepy-0.1.8/LICENSE` & `cdepy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/PKG-INFO` & `cdepy-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdepy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python Package for interacting with Cloudera Data Engineering Clusters
 Home-page: https://github.com/pdefusco/cdepy
 Author: Paul de Fusco
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -174,14 +174,15 @@
 
 ```
 CDE_RESOURCE_NAME = "myFilesCdeResource"
 
 myCdeClusterManager.deleteResource(CDE_RESOURCE_NAME)
 ```
 
+
 ### CDE AIRFLOW PYTHON ENVIRONMENTS
 
 NB: There is only one Airflow Python Environment per CDE Virtual Cluster.
 
 ```
 from cdepy import cdeconnection
 from cdepy import cdeairflowpython
@@ -273,7 +274,78 @@
 #### Optional: End the Maintenance Session once you have deleted the Python environment
 
 ```
 myAirflowPythonEnvManager.deleteMaintenanceSession()
 ```
 
 
+### CDE REPOSITORIES
+
+```
+from cdepy import cdeconnection
+from cdepy import cderepositories
+import os
+import json
+
+JOBS_API_URL = "<myJobsAPIurl>"
+WORKLOAD_USER = "<myusername>"
+WORKLOAD_PASSWORD = "<mypwd>"
+```
+
+#### Connect via CdeConnection Object
+
+```
+myCdeConnection = cdeconnection.CdeConnection(JOBS_API_URL, WORKLOAD_USER, WORKLOAD_PASSWORD)
+myCdeConnection.setToken()
+```
+
+#### Instantiate Repository Manager
+
+```
+myRepoManager = cderepositories.CdeRepositoryManager(myCdeConnection)
+```
+
+#### Provide example git repository information. This repository is available for tests.
+
+```
+repoName = "exampleGitRepository"
+repoPath = "https://github.com/pdefusco/cde_git_repo.git"
+```
+
+#### Create CDE Repository from Git Repository
+
+```
+myRepoManager.createRepository(repoName, repoPath, repoBranch="main")
+```
+
+#### Show available CDE repositories
+
+```
+myRepoManager.listRepositories()
+```
+
+#### Show CDE Repository Metadata
+
+```
+myRepoManager.describeRepository(repoName)
+```
+
+#### Download file from CDE Repository
+
+```
+filePath = "simple-pyspark-sql.py"
+myRepoManager.downloadFileFromRepo(repoName, filePath)
+```
+
+#### Delete CDE Repository
+
+```
+myRepoManager.deleteRepository(repoName)
+```
+
+#### Validate CDE Repository Deletion
+
+```
+myRepoManager.listRepositories()
+```
+
+
```

### Comparing `cdepy-0.1.8/README.md` & `cdepy-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 
 ```
 CDE_RESOURCE_NAME = "myFilesCdeResource"
 
 myCdeClusterManager.deleteResource(CDE_RESOURCE_NAME)
 ```
 
+
 ### CDE AIRFLOW PYTHON ENVIRONMENTS
 
 NB: There is only one Airflow Python Environment per CDE Virtual Cluster.
 
 ```
 from cdepy import cdeconnection
 from cdepy import cdeairflowpython
@@ -254,7 +255,78 @@
 ```
 
 #### Optional: End the Maintenance Session once you have deleted the Python environment
 
 ```
 myAirflowPythonEnvManager.deleteMaintenanceSession()
 ```
+
+
+### CDE REPOSITORIES
+
+```
+from cdepy import cdeconnection
+from cdepy import cderepositories
+import os
+import json
+
+JOBS_API_URL = "<myJobsAPIurl>"
+WORKLOAD_USER = "<myusername>"
+WORKLOAD_PASSWORD = "<mypwd>"
+```
+
+#### Connect via CdeConnection Object
+
+```
+myCdeConnection = cdeconnection.CdeConnection(JOBS_API_URL, WORKLOAD_USER, WORKLOAD_PASSWORD)
+myCdeConnection.setToken()
+```
+
+#### Instantiate Repository Manager
+
+```
+myRepoManager = cderepositories.CdeRepositoryManager(myCdeConnection)
+```
+
+#### Provide example git repository information. This repository is available for tests.
+
+```
+repoName = "exampleGitRepository"
+repoPath = "https://github.com/pdefusco/cde_git_repo.git"
+```
+
+#### Create CDE Repository from Git Repository
+
+```
+myRepoManager.createRepository(repoName, repoPath, repoBranch="main")
+```
+
+#### Show available CDE repositories
+
+```
+myRepoManager.listRepositories()
+```
+
+#### Show CDE Repository Metadata
+
+```
+myRepoManager.describeRepository(repoName)
+```
+
+#### Download file from CDE Repository
+
+```
+filePath = "simple-pyspark-sql.py"
+myRepoManager.downloadFileFromRepo(repoName, filePath)
+```
+
+#### Delete CDE Repository
+
+```
+myRepoManager.deleteRepository(repoName)
+```
+
+#### Validate CDE Repository Deletion
+
+```
+myRepoManager.listRepositories()
+```
```

### Comparing `cdepy-0.1.8/cdepy/cdeairflowpython.py` & `cdepy-0.1.9/cdepy/cdeairflowpython.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy/cdeconnection.py` & `cdepy-0.1.9/cdepy/cdeconnection.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy/cdejob.py` & `cdepy-0.1.9/cdepy/cdejob.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy/cdemanager.py` & `cdepy-0.1.9/cdepy/cdemanager.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy/cderesource.py` & `cdepy-0.1.9/cdepy/cderesource.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy/utils.py` & `cdepy-0.1.9/cdepy/utils.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.8/cdepy.egg-info/PKG-INFO` & `cdepy-0.1.9/cdepy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdepy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python Package for interacting with Cloudera Data Engineering Clusters
 Home-page: https://github.com/pdefusco/cdepy
 Author: Paul de Fusco
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -174,14 +174,15 @@
 
 ```
 CDE_RESOURCE_NAME = "myFilesCdeResource"
 
 myCdeClusterManager.deleteResource(CDE_RESOURCE_NAME)
 ```
 
+
 ### CDE AIRFLOW PYTHON ENVIRONMENTS
 
 NB: There is only one Airflow Python Environment per CDE Virtual Cluster.
 
 ```
 from cdepy import cdeconnection
 from cdepy import cdeairflowpython
@@ -273,7 +274,78 @@
 #### Optional: End the Maintenance Session once you have deleted the Python environment
 
 ```
 myAirflowPythonEnvManager.deleteMaintenanceSession()
 ```
 
 
+### CDE REPOSITORIES
+
+```
+from cdepy import cdeconnection
+from cdepy import cderepositories
+import os
+import json
+
+JOBS_API_URL = "<myJobsAPIurl>"
+WORKLOAD_USER = "<myusername>"
+WORKLOAD_PASSWORD = "<mypwd>"
+```
+
+#### Connect via CdeConnection Object
+
+```
+myCdeConnection = cdeconnection.CdeConnection(JOBS_API_URL, WORKLOAD_USER, WORKLOAD_PASSWORD)
+myCdeConnection.setToken()
+```
+
+#### Instantiate Repository Manager
+
+```
+myRepoManager = cderepositories.CdeRepositoryManager(myCdeConnection)
+```
+
+#### Provide example git repository information. This repository is available for tests.
+
+```
+repoName = "exampleGitRepository"
+repoPath = "https://github.com/pdefusco/cde_git_repo.git"
+```
+
+#### Create CDE Repository from Git Repository
+
+```
+myRepoManager.createRepository(repoName, repoPath, repoBranch="main")
+```
+
+#### Show available CDE repositories
+
+```
+myRepoManager.listRepositories()
+```
+
+#### Show CDE Repository Metadata
+
+```
+myRepoManager.describeRepository(repoName)
+```
+
+#### Download file from CDE Repository
+
+```
+filePath = "simple-pyspark-sql.py"
+myRepoManager.downloadFileFromRepo(repoName, filePath)
+```
+
+#### Delete CDE Repository
+
+```
+myRepoManager.deleteRepository(repoName)
+```
+
+#### Validate CDE Repository Deletion
+
+```
+myRepoManager.listRepositories()
+```
+
+
```

### Comparing `cdepy-0.1.8/setup.py` & `cdepy-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     author="Paul de Fusco",
     description="A Python Package for interacting with Cloudera Data Engineering Clusters",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     name="cdepy",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(include=["cdepy", "cdepy.*"]),
     install_requires=["pyparsing==3.0.9", "requests-toolbelt==1.0.0", "xmltodict==0.13.0"],
     python_requires=">=2.7",
     license="MIT",
     url = "https://github.com/pdefusco/cdepy",
     classifiers=[
         'Development Status :: 4 - Beta',
```

