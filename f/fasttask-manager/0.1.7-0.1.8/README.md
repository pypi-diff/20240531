# Comparing `tmp/fasttask_manager-0.1.7.tar.gz` & `tmp/fasttask_manager-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttask_manager-0.1.7.tar", last modified: Thu Mar 14 13:15:35 2024, max compression
+gzip compressed data, was "fasttask_manager-0.1.8.tar", last modified: Fri May 31 03:13:53 2024, max compression
```

## Comparing `fasttask_manager-0.1.7.tar` & `fasttask_manager-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/
--rw-r--r--   0 irid      (1000) irid      (1000)     1088 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/LICENSE
--rw-r--r--   0 irid      (1000) irid      (1000)      967 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/PKG-INFO
--rw-r--r--   0 irid      (1000) irid      (1000)      606 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/README.md
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.917850 fasttask_manager-0.1.7/fasttask_manager/
--rw-r--r--   0 irid      (1000) irid      (1000)       29 2024-01-25 17:36:32.000000 fasttask_manager-0.1.7/fasttask_manager/__init__.py
--rw-r--r--   0 irid      (1000) irid      (1000)     1102 2024-01-25 17:36:48.000000 fasttask_manager-0.1.7/fasttask_manager/create_project.py
--rw-r--r--   0 irid      (1000) irid      (1000)     3448 2024-03-14 13:14:21.000000 fasttask_manager-0.1.7/fasttask_manager/manager.py
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/fasttask_manager/project/
--rw-r--r--   0 irid      (1000) irid      (1000)      213 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/fasttask_manager/project/Dockerfile
--rw-r--r--   0 irid      (1000) irid      (1000)      248 2024-01-25 17:33:08.000000 fasttask_manager-0.1.7/fasttask_manager/project/docker-compose.yml
--rw-r--r--   0 irid      (1000) irid      (1000)        0 2024-01-25 17:35:52.000000 fasttask_manager-0.1.7/fasttask_manager/project/req.txt
--rw-r--r--   0 irid      (1000) irid      (1000)      520 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/fasttask_manager/project/setting.py
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/fasttask_manager/project/tasks/
--rw-r--r--   0 irid      (1000) irid      (1000)      618 2024-01-25 19:03:47.000000 fasttask_manager-0.1.7/fasttask_manager/project/tasks/get_hypotenuse.py
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/fasttask_manager/project/tasks/packages/
--rw-r--r--   0 irid      (1000) irid      (1000)        0 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/fasttask_manager/project/tasks/packages/__init__.py
--rw-r--r--   0 irid      (1000) irid      (1000)      129 2024-01-20 18:02:40.000000 fasttask_manager-0.1.7/fasttask_manager/project/tasks/packages/tools.py
-drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2024-03-14 13:15:35.917850 fasttask_manager-0.1.7/fasttask_manager.egg-info/
--rw-r--r--   0 irid      (1000) irid      (1000)      967 2024-03-14 13:15:35.000000 fasttask_manager-0.1.7/fasttask_manager.egg-info/PKG-INFO
--rw-r--r--   0 irid      (1000) irid      (1000)      616 2024-03-14 13:15:35.000000 fasttask_manager-0.1.7/fasttask_manager.egg-info/SOURCES.txt
--rw-r--r--   0 irid      (1000) irid      (1000)        1 2024-03-14 13:15:35.000000 fasttask_manager-0.1.7/fasttask_manager.egg-info/dependency_links.txt
--rw-r--r--   0 irid      (1000) irid      (1000)       15 2024-03-14 13:15:35.000000 fasttask_manager-0.1.7/fasttask_manager.egg-info/requires.txt
--rw-r--r--   0 irid      (1000) irid      (1000)       17 2024-03-14 13:15:35.000000 fasttask_manager-0.1.7/fasttask_manager.egg-info/top_level.txt
--rw-r--r--   0 irid      (1000) irid      (1000)       38 2024-03-14 13:15:35.921184 fasttask_manager-0.1.7/setup.cfg
--rw-r--r--   0 irid      (1000) irid      (1000)      838 2024-03-14 13:15:34.000000 fasttask_manager-0.1.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:53.035256 fasttask_manager-0.1.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1088 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1012 2024-05-31 03:13:53.034985 fasttask_manager-0.1.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      606 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:52.947814 fasttask_manager-0.1.8/fasttask_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-03-15 03:30:55.000000 fasttask_manager-0.1.8/fasttask_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1102 2024-03-15 03:30:55.000000 fasttask_manager-0.1.8/fasttask_manager/create_project.py
+-rwxrwxrwx   0 root         (0) root         (0)     3445 2024-05-29 11:12:03.000000 fasttask_manager-0.1.8/fasttask_manager/manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:53.033778 fasttask_manager-0.1.8/fasttask_manager/project/
+-rwxrwxrwx   0 root         (0) root         (0)      213 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/fasttask_manager/project/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      992 2024-05-29 11:23:13.000000 fasttask_manager-0.1.8/fasttask_manager/project/docker-compose.yml
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-15 03:30:55.000000 fasttask_manager-0.1.8/fasttask_manager/project/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)      520 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/fasttask_manager/project/setting.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:53.034018 fasttask_manager-0.1.8/fasttask_manager/project/tasks/
+-rwxrwxrwx   0 root         (0) root         (0)      618 2024-03-15 03:30:55.000000 fasttask_manager-0.1.8/fasttask_manager/project/tasks/get_hypotenuse.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:53.034425 fasttask_manager-0.1.8/fasttask_manager/project/tasks/packages/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/fasttask_manager/project/tasks/packages/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      129 2024-03-14 10:08:47.000000 fasttask_manager-0.1.8/fasttask_manager/project/tasks/packages/tools.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 03:13:53.034683 fasttask_manager-0.1.8/fasttask_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1012 2024-05-31 03:13:52.000000 fasttask_manager-0.1.8/fasttask_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      616 2024-05-31 03:13:52.000000 fasttask_manager-0.1.8/fasttask_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-31 03:13:52.000000 fasttask_manager-0.1.8/fasttask_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2024-05-31 03:13:52.000000 fasttask_manager-0.1.8/fasttask_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       17 2024-05-31 03:13:52.000000 fasttask_manager-0.1.8/fasttask_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-31 03:13:53.035325 fasttask_manager-0.1.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      838 2024-05-30 06:54:42.000000 fasttask_manager-0.1.8/setup.py
```

### Comparing `fasttask_manager-0.1.7/LICENSE` & `fasttask_manager-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/PKG-INFO` & `fasttask_manager-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: fasttask_manager
-Version: 0.1.7
+Version: 0.1.8
 Summary: fasttask's manager 
 Home-page: https://github.com/iridesc/fasttask_manager
 Author: Irid
 Author-email: irid.zzy@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: retry
+Requires-Dist: requests
 
 manager for [fasttask](https://github.com/iridesc/fasttask) 
 
 ### create project 
 
 ```bash
 python -m fasttask_manager.create_project
```

### Comparing `fasttask_manager-0.1.7/README.md` & `fasttask_manager-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/fasttask_manager/create_project.py` & `fasttask_manager-0.1.8/fasttask_manager/create_project.py`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/fasttask_manager/manager.py` & `fasttask_manager-0.1.8/fasttask_manager/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,22 +43,22 @@
                 r = requests.get(params=data, **params)
 
             r.raise_for_status()
             return r if raw_resp else r.json()
         return req()
 
     def run(self, params: dict) -> dict:
-        return self._req(path=f"/run/{self.task_name}/", data=params)
+        return self._req(path=f"/run/{self.task_name}", data=params)
 
     def create_task(self, params: dict) -> dict:
         self.logger.info(f"{self.log_prefix}: task creating...")
-        return self._req(path=f"/create/{self.task_name}/", data=params)
+        return self._req(path=f"/create/{self.task_name}", data=params)
 
     def check(self, result_id: str) -> dict:
-        resp = self._req(path=f"/check/{self.task_name}/", data={"result_id": result_id}, method="g")
+        resp = self._req(path=f"/check/{self.task_name}", data={"result_id": result_id}, method="g")
         self.logger.info(f"{self.log_prefix}: check task: {resp['state']}")
         return resp
 
     def upload(self, file_path) -> str:
         return self._req("/upload", method="p", file=file_path)["file_name"]
 
     def download(self, file_name, local_path):
```

### Comparing `fasttask_manager-0.1.7/fasttask_manager/project/setting.py` & `fasttask_manager-0.1.8/fasttask_manager/project/setting.py`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/fasttask_manager/project/tasks/get_hypotenuse.py` & `fasttask_manager-0.1.8/fasttask_manager/project/tasks/get_hypotenuse.py`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/fasttask_manager.egg-info/PKG-INFO` & `fasttask_manager-0.1.8/fasttask_manager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: fasttask-manager
-Version: 0.1.7
+Name: fasttask_manager
+Version: 0.1.8
 Summary: fasttask's manager 
 Home-page: https://github.com/iridesc/fasttask_manager
 Author: Irid
 Author-email: irid.zzy@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: retry
+Requires-Dist: requests
 
 manager for [fasttask](https://github.com/iridesc/fasttask) 
 
 ### create project 
 
 ```bash
 python -m fasttask_manager.create_project
```

### Comparing `fasttask_manager-0.1.7/fasttask_manager.egg-info/SOURCES.txt` & `fasttask_manager-0.1.8/fasttask_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasttask_manager-0.1.7/setup.py` & `fasttask_manager-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fasttask_manager",
-    version="0.1.7",
+    version="0.1.8",
     author="Irid",
     author_email="irid.zzy@gmail.com",
     description="fasttask's manager ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iridesc/fasttask_manager",
     packages=setuptools.find_packages(),
```

