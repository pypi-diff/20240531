# Comparing `tmp/openi-2.0.0b2.tar.gz` & `tmp/openi-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-2.0.0b2.tar", last modified: Thu May 23 06:51:20 2024, max compression
+gzip compressed data, was "openi-2.0.0b5.tar", last modified: Tue May 28 08:21:33 2024, max compression
```

## Comparing `openi-2.0.0b2.tar` & `openi-2.0.0b5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.753149 openi-2.0.0b2/
--rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.751138 openi-2.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b2/README.md
--rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 06:51:20.753149 openi-2.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-05-23 06:47:17.000000 openi-2.0.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.695720 openi-2.0.0b2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.725884 openi-2.0.0b2/src/openi/
--rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/__init__.py
--rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b2/src/openi/_dataclass.py
--rw-rw-rw-   0        0        0     7895 2024-05-23 04:00:55.000000 openi-2.0.0b2/src/openi/_exceptions.py
--rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b2/src/openi/_file.py
--rw-rw-rw-   0        0        0     4576 2024-05-23 03:19:45.000000 openi-2.0.0b2/src/openi/_login.py
--rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b2/src/openi/_session.py
--rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/_tqdm.py
--rw-rw-rw-   0        0        0    36678 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.743909 openi-2.0.0b2/src/openi/commands/
--rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/__init__.py
--rw-rw-rw-   0        0        0     6802 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/dataset.py
--rw-rw-rw-   0        0        0     8628 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/model.py
--rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/openi_cli.py
--rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b2/src/openi/commands/user.py
--rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/constants.py
--rw-rw-rw-   0        0        0    10840 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/downloader.py
--rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/log.py
--rw-rw-rw-   0        0        0     9731 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi/uploader.py
--rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.749653 openi-2.0.0b2/src/openi.egg-info/
--rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.746944 openi-2.0.0b2/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b2/test/test.py
--rw-rw-rw-   0        0        0      179 2024-05-23 03:08:38.000000 openi-2.0.0b2/test/test_openi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.348173 openi-2.0.0b5/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1970 2024-05-28 08:21:33.348043 openi-2.0.0b5/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1449 2024-05-27 02:29:47.000000 openi-2.0.0b5/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       76 2024-05-11 03:27:02.000000 openi-2.0.0b5/pyproject.toml
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2024-05-28 08:21:33.348212 openi-2.0.0b5/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      972 2024-05-28 08:21:04.000000 openi-2.0.0b5/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.340989 openi-2.0.0b5/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.344761 openi-2.0.0b5/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      210 2024-05-28 03:43:35.000000 openi-2.0.0b5/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10627 2024-05-27 02:29:47.000000 openi-2.0.0b5/src/openi/_dataclass.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     7634 2024-05-28 03:43:35.000000 openi-2.0.0b5/src/openi/_exceptions.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     6950 2024-05-27 07:47:40.000000 openi-2.0.0b5/src/openi/_file.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     4416 2024-05-27 02:29:47.000000 openi-2.0.0b5/src/openi/_login.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     9346 2024-05-28 03:43:35.000000 openi-2.0.0b5/src/openi/_session.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     3979 2024-05-15 13:58:49.000000 openi-2.0.0b5/src/openi/_tqdm.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    23837 2024-05-28 08:21:28.000000 openi-2.0.0b5/src/openi/api.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.346778 openi-2.0.0b5/src/openi/commands/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      315 2024-05-16 02:26:01.000000 openi-2.0.0b5/src/openi/commands/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     6691 2024-05-28 08:15:13.000000 openi-2.0.0b5/src/openi/commands/dataset.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     8377 2024-05-28 08:16:44.000000 openi-2.0.0b5/src/openi/commands/model.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      862 2024-05-16 02:34:46.000000 openi-2.0.0b5/src/openi/commands/openi_cli.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2481 2024-05-27 02:29:47.000000 openi-2.0.0b5/src/openi/commands/user.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2059 2024-05-28 03:43:35.000000 openi-2.0.0b5/src/openi/constants.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10474 2024-05-28 08:15:33.000000 openi-2.0.0b5/src/openi/downloader.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     3708 2024-04-16 08:41:16.000000 openi-2.0.0b5/src/openi/log.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     9468 2024-05-28 08:16:28.000000 openi-2.0.0b5/src/openi/uploader.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2667 2024-05-16 01:40:03.000000 openi-2.0.0b5/src/openi/utils.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.345580 openi-2.0.0b5/src/openi.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1970 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      705 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       56 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/entry_points.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       33 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2024-05-28 08:21:33.000000 openi-2.0.0b5/src/openi.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-05-28 08:21:33.347637 openi-2.0.0b5/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     7375 2024-02-28 01:14:22.000000 openi-2.0.0b5/test/test.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      911 2024-02-28 01:14:24.000000 openi-2.0.0b5/test/test_client.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      428 2024-03-17 16:28:42.000000 openi-2.0.0b5/test/test_tqdm.py
```

### Comparing `openi-2.0.0b2/PKG-INFO` & `openi-2.0.0b5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-Metadata-Version: 2.1
-Name: openi
-Version: 2.0.0b2
-Summary: A package for openi pypi
-Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
-Author: chenzh05
-Author-email: chenzh.ds@outlook.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: deprecated
-Requires-Dist: pwinput
-
-# OpenI
-
-> PYPI package for 启智 AI 协作平台。
-
-## 安装
-
-_适配 python3.8 及以上版本_
-
-```bash
-pip install openi
-```
-
-## 功能介绍
-
-- 支持进行本地上传与下载文件到启智社区
-- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
-- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
-
-## 使用示例
-- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
-
-```python
-# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
-from openi import download_file
-path = download_file(
-    file="MnistDataset_mindspore.zip",
-    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
-)
-```
-
-- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
-
-```bash
-openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
-```
-
-- 执行结果，显示下载进度条与本地保存路径
-```bash
-✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
-文件已下载到: D:\MnistDataset_mindspore.zip
-```
-
-- 更多使用指南请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+Metadata-Version: 2.1
+Name: openi
+Version: 2.0.0b5
+Summary: A package for openi pypi
+Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
+Author: chenzh05
+Author-email: chenzh.ds@outlook.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# OpenI
+
+> PYPI package for 启智 AI 协作平台。
+
+## 安装
+
+_适配 python3.8 及以上版本_
+
+```bash
+pip install openi
+```
+
+## 功能介绍
+
+- 支持进行本地上传与下载文件到启智社区
+- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
+- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+
+## 使用示例
+- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
+
+```python
+# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
+from openi import download_file
+path = download_file(
+    file="MnistDataset_mindspore.zip",
+    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
+)
+```
+
+- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
+
+```bash
+openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
+```
+
+- 执行结果，显示下载进度条与本地保存路径
+```bash
+✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
+文件已下载到: D:\MnistDataset_mindspore.zip
+```
+
+- 更多使用指南请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
```

### Comparing `openi-2.0.0b2/README.md` & `openi-2.0.0b5/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# OpenI
-
-> PYPI package for 启智 AI 协作平台。
-
-## 安装
-
-_适配 python3.8 及以上版本_
-
-```bash
-pip install openi
-```
-
-## 功能介绍
-
-- 支持进行本地上传与下载文件到启智社区
-- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
-- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
-
-## 使用示例
-- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
-
-```python
-# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
-from openi import download_file
-path = download_file(
-    file="MnistDataset_mindspore.zip",
-    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
-)
-```
-
-- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
-
-```bash
-openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
-```
-
-- 执行结果，显示下载进度条与本地保存路径
-```bash
-✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
-文件已下载到: D:\MnistDataset_mindspore.zip
-```
-
+# OpenI
+
+> PYPI package for 启智 AI 协作平台。
+
+## 安装
+
+_适配 python3.8 及以上版本_
+
+```bash
+pip install openi
+```
+
+## 功能介绍
+
+- 支持进行本地上传与下载文件到启智社区
+- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
+- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+
+## 使用示例
+- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
+
+```python
+# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
+from openi import download_file
+path = download_file(
+    file="MnistDataset_mindspore.zip",
+    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
+)
+```
+
+- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
+
+```bash
+openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
+```
+
+- 执行结果，显示下载进度条与本地保存路径
+```bash
+✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
+文件已下载到: D:\MnistDataset_mindspore.zip
+```
+
 - 更多使用指南请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
```

### Comparing `openi-2.0.0b2/src/openi/_dataclass.py` & `openi-2.0.0b5/src/openi/_dataclass.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,379 +1,379 @@
-from dataclasses import dataclass
-from datetime import datetime
-from typing import List, Optional
-
-from .utils import parse_time
-
-
-@dataclass
-class UserInfo:
-    """
-    User Info Dataclass
-
-    Attributes:
-        username (str):
-            username for OpenI links and repo_id
-        id (int):
-            unique number id of user
-        login (str):
-            username used for login purpose
-        full_name (str):
-            self-defined name for display
-        email (str):
-            registered email address
-        avatar_url (str):
-            user avatar url
-        language (str):
-            user default language
-        is_admin (bool):
-            whether the user is admin or not
-        is_active (bool):
-            whether the user is active or not
-        last_login (str):
-            last login time
-        created (str):
-            created time
-    """
-
-    username: str
-    id: Optional[int]
-    login: Optional[str]
-    full_name: Optional[str]
-    email: Optional[str]
-    avatar_url: Optional[str]
-    language: Optional[str]
-    is_admin: Optional[bool]
-    is_active: Optional[bool]
-    last_login: Optional[str]
-    created: Optional[str]
-
-
-@dataclass
-class RepoPermission:
-    """
-    Permission Info Dataclass
-
-    Attributes:
-        admin (bool):
-            whether the user is admin or not
-        push (bool):
-            whether the user can push to the repository or not
-        pull (bool):
-            whether the user can pull from the repository or not
-    """
-
-    admin: bool
-    push: bool
-    pull: bool
-
-
-@dataclass
-class RepoInfo:
-    """
-    Repo Info Dataclass
-
-    Attributes:
-        id (int):
-            repo id
-        owner (UserInfo):
-            owner info
-        name (str):
-            repo name
-        repo_id (str):
-            repo id in `Username/Reponame` format
-        size (int):
-            repo size
-        html_url (str):
-            repo url
-        permissions (RepoPermission):
-            repo permissions
-        created_at (str):
-            created time
-        updated_at (str):
-            updated time
-    """
-
-    id: int
-    owner: UserInfo
-    name: str
-    repo_id: str
-    size: Optional[int]
-    html_url: Optional[str]
-    permissions: Optional[RepoPermission]
-    created_at: Optional[datetime]
-    updated_at: Optional[datetime]
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop("id")
-        self.owner = UserInfo(**kwargs.pop("owner"))
-        self.name = kwargs.pop("name")
-        self.repo_id = kwargs.pop("full_name")
-
-        self.size = kwargs.pop("size", None)
-        self.html_url = kwargs.pop("html_url", None)
-        permissions = kwargs.pop("permissions", None)
-        self.permissions = (
-            RepoPermission(**permissions) if permissions else None
-        )
-
-        created_at = kwargs.pop("created_at", None)
-        self.created_at = parse_time(created_at) if created_at else None
-        updated_at = kwargs.pop("updated_at", None)
-        self.updated_at = parse_time(updated_at) if updated_at else None
-
-
-@dataclass
-class DatasetFile:
-    """TODO"""
-
-    uuid: str
-    name: str
-    size: int
-    type: int
-    id: int
-    datasetId: int
-    repo_id: str
-    uploaderId: Optional[int]
-    isPrivate: Optional[bool]
-    decompressState: Optional[int]
-
-    def __init__(self, **kwargs):
-        self.uuid = kwargs.pop("uuid")
-        self.name = kwargs.pop("name")
-        self.size = kwargs.pop("size")
-        self.type = kwargs.pop("type")
-        self.id = kwargs.pop("id")
-        self.datasetId = kwargs.pop("datasetId")
-        self.repo_id = kwargs.pop("repo_id")
-
-        self.uploaderId = kwargs.pop("uploaderId", None)
-        self.isPrivate = kwargs.pop("isPrivate", None)
-        self.decompressState = kwargs.pop("decompressState", None)
-
-
-@dataclass
-class DatasetInfo:
-    """TODO"""
-
-    id: str
-    userId: int
-    repoId: int
-    title: str
-    repo_id: str
-    attachments: Optional[List[DatasetFile]]
-    status: Optional[int]
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop("id")
-        self.userId = kwargs.pop("userId")
-        self.repoId = kwargs.pop("repoId")
-        self.title = kwargs.pop("title")
-        self.repo_id = kwargs.pop("repo_id")
-
-        attachments = kwargs.pop("attachments", [])
-        if attachments:
-            for data in attachments:
-                data.update({"repo_id": self.repo_id})
-            self.attachments = [DatasetFile(**data) for data in attachments]
-        else:
-            self.attachments = None
-
-        self.status = kwargs.pop("status", None)
-        self.recommend = kwargs.pop("recommend", None)
-
-
-@dataclass
-class FileChunkInfo:
-    """
-    File Chunk Info Dataclass
-
-    API Response (dict):
-        - dataset "/attachments/get_chunks"
-            "uuid":        fileChunk.UUID,
-            "uploaded":    strconv.Itoa(fileChunk.IsUploaded),
-            "uploadID":    fileChunk.UploadID,
-            "chunks":      string(chunks),
-            "attachID":    "0",
-            "datasetID":   "0",
-            "fileName":    "",
-            "datasetName": "",
-
-        - model "/attachments/model/get_chunks"
-            "uuid":      fileChunk.UUID,
-            "uploaded":  strconv.Itoa(fileChunk.IsUploaded),
-            "uploadID":  fileChunk.UploadID,
-            "chunks":    string(chunks),
-            "attachID":  "0",
-            "modeluuid": modeluuid,
-            "datasetID": "0",
-            "fileName":  "",
-            "modelName": "",
-
-        - error response
-            "result_code": "-1",
-            "msg":         errStr,
-
-    Attributes:
-        result_code (int):
-            return 0 when success, otherwise return -1 with error message
-        msg (str):
-            return plain string error message, return "success" when None
-        uploaded (Optional[bool]):
-            whether the file is uploaded or not
-        attachID (Optional[int]):
-            attachment id
-        uploaded_chunks (Optional[list]):
-            list of uploaded chunks
-        uploadID (Optional[str]):
-            upload id
-        uuid (Optional[str]):
-            file uuid
-        repo_id (Optional[str]):
-            repo id in `Username/Reponame` format
-        dataset_or_model_name (Optional[str]):
-            dataset or model name
-    """
-
-    result_code: int
-    msg: str
-    uploaded: Optional[bool]
-    md5: Optional[str]
-    fileName: Optional[str]
-    attachID: Optional[int]
-    uploaded_chunks: Optional[list]
-    uploadID: Optional[str]
-    uuid: Optional[str]
-    repo_id: Optional[str]
-    dataset_or_model_name: Optional[str]
-
-    def __init__(self, **kwargs):
-        result_code = kwargs.pop("result_code", 0)
-        self.result_code = int(result_code)
-        self.msg = kwargs.pop("msg", "success")
-
-        uploaded = kwargs.pop("uploaded", None)
-        self.uploaded = True if uploaded == "1" else False
-        self.attachID = kwargs.pop("attachID", None)
-
-        raw_chunks = kwargs.pop("chunks", "")
-        uploaded_chunks = [i for i in raw_chunks.split(",") if i != ""]
-        # uploaded_chunks = []
-        # if raw_chunks and raw_chunks != "":
-        #     uploaded_chunks = [i for i in raw_chunks.split(",") if i != ""]
-        #     # uploaded_chunks = [int(i.split("-")[0]) for i in raw_chunks]
-        #     uploaded_chunks.sort()
-        #     # uploaded_chunks.pop(-1)
-        self.uploaded_chunks = uploaded_chunks
-
-        uploadID = kwargs.pop("uploadID", None)
-        self.uploadID = uploadID if uploadID and uploadID != "" else None
-        uuid = kwargs.pop("uuid", None)
-        self.uuid = uuid if uuid and uuid != "" else None
-
-        repo = kwargs.pop("repoName", None)
-        owner = kwargs.pop("repoOwner", None)
-        self.repo_id = owner + "/" + repo if owner and repo else None
-
-        if kwargs.pop("upload_mode") == "dataset":
-            self.dataset_or_model_name = kwargs.pop("datasetName", None)
-        else:
-            self.dataset_or_model_name = kwargs.pop("modelName", None)
-
-        self.fileName = kwargs.pop("fileName", None)
-        self.md5 = kwargs.pop("md5", None)
-
-
-@dataclass
-class NewMultipart:
-    """TODO"""
-
-    result_code: int
-    msg: str
-    uuid: Optional[str]
-    uploadID: Optional[str]
-
-    def __init__(self, **kwargs):
-        result_code = kwargs.pop("result_code", 0)
-        self.result_code = int(result_code)
-        self.msg = kwargs.pop("msg", "success")
-        self.uuid = kwargs.pop("uuid", None)
-        self.uploadID = kwargs.pop("uploadID", None)
-
-
-@dataclass
-class MultipartUrl:
-    """TODO"""
-
-    url: Optional[str] = None
-    msg: Optional[str] = None
-
-
-@dataclass
-class ModelFile:
-    FileName: Optional[str]
-    ModTime: Optional[str]
-    IsDir: Optional[bool]
-    Size: Optional[int]
-    ParenDir: Optional[str]
-    UUID: Optional[str]
-    RelativePath: Optional[str]
-    repo_id: Optional[str]
-    model_id: Optional[str]
-
-
-@dataclass
-class ModelInfo:
-    id: Optional[str]
-    name: Optional[str]
-    size: Optional[int]
-    path: Optional[str]
-    repo_id: Optional[str]
-    repoId: Optional[int]
-    userId: Optional[int]
-    userName: Optional[str]
-    isCanOper: Optional[bool]
-    isCanDelete: Optional[bool]
-    isCanDownload: Optional[bool]
-    repoName: Optional[str]
-    repoOwnerName: Optional[str]
-    modelFileList: Optional[List[ModelFile]]
-    modelType: Optional[int]
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop("id", None)
-        self.name = kwargs.pop("name", None)
-        self.size = kwargs.pop("size", None)
-        self.path = kwargs.pop("path", None)
-        self.repo_id = kwargs.pop("repo_id", None)
-        self.repoId = kwargs.pop("repoId", None)
-        self.userId = kwargs.pop("userId", None)
-        self.userName = kwargs.pop("userName", None)
-        self.isCanOper = kwargs.pop("isCanOper", None)
-        self.isCanDelete = kwargs.pop("isCanDelete", None)
-        self.isCanDownload = kwargs.pop("isCanDownload", None)
-        self.repoName = kwargs.pop("repoName", None)
-        self.repoOwnerName = kwargs.pop("repoOwnerName", None)
-
-        modelFileList = kwargs.pop("modelFileList", [])
-        if modelFileList:
-            for data in modelFileList:
-                data.update({"repo_id": self.repo_id, "model_id": self.id})
-            self.modelFileList = [ModelFile(**data) for data in modelFileList]
-        else:
-            self.modelFileList = None
-
-        self.modelType = kwargs.pop("modelType", None)
-
-
-@dataclass
-class ModelCreate:
-    code: str
-    msg: Optional[str] = None
-    id: Optional[int] = None
-
-
-@dataclass
-class BasicResp:
-    code: int
-    msg: str
-    data: any
+from dataclasses import dataclass
+from datetime import datetime
+from typing import List, Optional
+
+from .utils import parse_time
+
+
+@dataclass
+class UserInfo:
+    """
+    User Info Dataclass
+
+    Attributes:
+        username (str):
+            username for OpenI links and repo_id
+        id (int):
+            unique number id of user
+        login (str):
+            username used for login purpose
+        full_name (str):
+            self-defined name for display
+        email (str):
+            registered email address
+        avatar_url (str):
+            user avatar url
+        language (str):
+            user default language
+        is_admin (bool):
+            whether the user is admin or not
+        is_active (bool):
+            whether the user is active or not
+        last_login (str):
+            last login time
+        created (str):
+            created time
+    """
+
+    username: str
+    id: Optional[int]
+    login: Optional[str]
+    full_name: Optional[str]
+    email: Optional[str]
+    avatar_url: Optional[str]
+    language: Optional[str]
+    is_admin: Optional[bool]
+    is_active: Optional[bool]
+    last_login: Optional[str]
+    created: Optional[str]
+
+
+@dataclass
+class RepoPermission:
+    """
+    Permission Info Dataclass
+
+    Attributes:
+        admin (bool):
+            whether the user is admin or not
+        push (bool):
+            whether the user can push to the repository or not
+        pull (bool):
+            whether the user can pull from the repository or not
+    """
+
+    admin: bool
+    push: bool
+    pull: bool
+
+
+@dataclass
+class RepoInfo:
+    """
+    Repo Info Dataclass
+
+    Attributes:
+        id (int):
+            repo id
+        owner (UserInfo):
+            owner info
+        name (str):
+            repo name
+        repo_id (str):
+            repo id in `Username/Reponame` format
+        size (int):
+            repo size
+        html_url (str):
+            repo url
+        permissions (RepoPermission):
+            repo permissions
+        created_at (str):
+            created time
+        updated_at (str):
+            updated time
+    """
+
+    id: int
+    owner: UserInfo
+    name: str
+    repo_id: str
+    size: Optional[int]
+    html_url: Optional[str]
+    permissions: Optional[RepoPermission]
+    created_at: Optional[datetime]
+    updated_at: Optional[datetime]
+
+    def __init__(self, **kwargs):
+        self.id = kwargs.pop("id")
+        self.owner = UserInfo(**kwargs.pop("owner"))
+        self.name = kwargs.pop("name")
+        self.repo_id = kwargs.pop("full_name")
+
+        self.size = kwargs.pop("size", None)
+        self.html_url = kwargs.pop("html_url", None)
+        permissions = kwargs.pop("permissions", None)
+        self.permissions = (
+            RepoPermission(**permissions) if permissions else None
+        )
+
+        created_at = kwargs.pop("created_at", None)
+        self.created_at = parse_time(created_at) if created_at else None
+        updated_at = kwargs.pop("updated_at", None)
+        self.updated_at = parse_time(updated_at) if updated_at else None
+
+
+@dataclass
+class DatasetFile:
+    """TODO"""
+
+    uuid: str
+    name: str
+    size: int
+    type: int
+    id: int
+    datasetId: int
+    repo_id: str
+    uploaderId: Optional[int]
+    isPrivate: Optional[bool]
+    decompressState: Optional[int]
+
+    def __init__(self, **kwargs):
+        self.uuid = kwargs.pop("uuid")
+        self.name = kwargs.pop("name")
+        self.size = kwargs.pop("size")
+        self.type = kwargs.pop("type")
+        self.id = kwargs.pop("id")
+        self.datasetId = kwargs.pop("datasetId")
+        self.repo_id = kwargs.pop("repo_id")
+
+        self.uploaderId = kwargs.pop("uploaderId", None)
+        self.isPrivate = kwargs.pop("isPrivate", None)
+        self.decompressState = kwargs.pop("decompressState", None)
+
+
+@dataclass
+class DatasetInfo:
+    """TODO"""
+
+    id: str
+    userId: int
+    repoId: int
+    title: str
+    repo_id: str
+    attachments: Optional[List[DatasetFile]]
+    status: Optional[int]
+
+    def __init__(self, **kwargs):
+        self.id = kwargs.pop("id")
+        self.userId = kwargs.pop("userId")
+        self.repoId = kwargs.pop("repoId")
+        self.title = kwargs.pop("title")
+        self.repo_id = kwargs.pop("repo_id")
+
+        attachments = kwargs.pop("attachments", [])
+        if attachments:
+            for data in attachments:
+                data.update({"repo_id": self.repo_id})
+            self.attachments = [DatasetFile(**data) for data in attachments]
+        else:
+            self.attachments = None
+
+        self.status = kwargs.pop("status", None)
+        self.recommend = kwargs.pop("recommend", None)
+
+
+@dataclass
+class FileChunkInfo:
+    """
+    File Chunk Info Dataclass
+
+    API Response (dict):
+        - dataset "/attachments/get_chunks"
+            "uuid":        fileChunk.UUID,
+            "uploaded":    strconv.Itoa(fileChunk.IsUploaded),
+            "uploadID":    fileChunk.UploadID,
+            "chunks":      string(chunks),
+            "attachID":    "0",
+            "datasetID":   "0",
+            "fileName":    "",
+            "datasetName": "",
+
+        - model "/attachments/model/get_chunks"
+            "uuid":      fileChunk.UUID,
+            "uploaded":  strconv.Itoa(fileChunk.IsUploaded),
+            "uploadID":  fileChunk.UploadID,
+            "chunks":    string(chunks),
+            "attachID":  "0",
+            "modeluuid": modeluuid,
+            "datasetID": "0",
+            "fileName":  "",
+            "modelName": "",
+
+        - error response
+            "result_code": "-1",
+            "msg":         errStr,
+
+    Attributes:
+        result_code (int):
+            return 0 when success, otherwise return -1 with error message
+        msg (str):
+            return plain string error message, return "success" when None
+        uploaded (Optional[bool]):
+            whether the file is uploaded or not
+        attachID (Optional[int]):
+            attachment id
+        uploaded_chunks (Optional[list]):
+            list of uploaded chunks
+        uploadID (Optional[str]):
+            upload id
+        uuid (Optional[str]):
+            file uuid
+        repo_id (Optional[str]):
+            repo id in `Username/Reponame` format
+        dataset_or_model_name (Optional[str]):
+            dataset or model name
+    """
+
+    result_code: int
+    msg: str
+    uploaded: Optional[bool]
+    md5: Optional[str]
+    fileName: Optional[str]
+    attachID: Optional[int]
+    uploaded_chunks: Optional[list]
+    uploadID: Optional[str]
+    uuid: Optional[str]
+    repo_id: Optional[str]
+    dataset_or_model_name: Optional[str]
+
+    def __init__(self, **kwargs):
+        result_code = kwargs.pop("result_code", 0)
+        self.result_code = int(result_code)
+        self.msg = kwargs.pop("msg", "success")
+
+        uploaded = kwargs.pop("uploaded", None)
+        self.uploaded = True if uploaded == "1" else False
+        self.attachID = kwargs.pop("attachID", None)
+
+        raw_chunks = kwargs.pop("chunks", "")
+        uploaded_chunks = [i for i in raw_chunks.split(",") if i != ""]
+        # uploaded_chunks = []
+        # if raw_chunks and raw_chunks != "":
+        #     uploaded_chunks = [i for i in raw_chunks.split(",") if i != ""]
+        #     # uploaded_chunks = [int(i.split("-")[0]) for i in raw_chunks]
+        #     uploaded_chunks.sort()
+        #     # uploaded_chunks.pop(-1)
+        self.uploaded_chunks = uploaded_chunks
+
+        uploadID = kwargs.pop("uploadID", None)
+        self.uploadID = uploadID if uploadID and uploadID != "" else None
+        uuid = kwargs.pop("uuid", None)
+        self.uuid = uuid if uuid and uuid != "" else None
+
+        repo = kwargs.pop("repoName", None)
+        owner = kwargs.pop("repoOwner", None)
+        self.repo_id = owner + "/" + repo if owner and repo else None
+
+        if kwargs.pop("upload_mode") == "dataset":
+            self.dataset_or_model_name = kwargs.pop("datasetName", None)
+        else:
+            self.dataset_or_model_name = kwargs.pop("modelName", None)
+
+        self.fileName = kwargs.pop("fileName", None)
+        self.md5 = kwargs.pop("md5", None)
+
+
+@dataclass
+class NewMultipart:
+    """TODO"""
+
+    result_code: int
+    msg: str
+    uuid: Optional[str]
+    uploadID: Optional[str]
+
+    def __init__(self, **kwargs):
+        result_code = kwargs.pop("result_code", 0)
+        self.result_code = int(result_code)
+        self.msg = kwargs.pop("msg", "success")
+        self.uuid = kwargs.pop("uuid", None)
+        self.uploadID = kwargs.pop("uploadID", None)
+
+
+@dataclass
+class MultipartUrl:
+    """TODO"""
+
+    url: Optional[str] = None
+    msg: Optional[str] = None
+
+
+@dataclass
+class ModelFile:
+    FileName: Optional[str]
+    ModTime: Optional[str]
+    IsDir: Optional[bool]
+    Size: Optional[int]
+    ParenDir: Optional[str]
+    UUID: Optional[str]
+    RelativePath: Optional[str]
+    repo_id: Optional[str]
+    model_id: Optional[str]
+
+
+@dataclass
+class ModelInfo:
+    id: Optional[str]
+    name: Optional[str]
+    size: Optional[int]
+    path: Optional[str]
+    repo_id: Optional[str]
+    repoId: Optional[int]
+    userId: Optional[int]
+    userName: Optional[str]
+    isCanOper: Optional[bool]
+    isCanDelete: Optional[bool]
+    isCanDownload: Optional[bool]
+    repoName: Optional[str]
+    repoOwnerName: Optional[str]
+    modelFileList: Optional[List[ModelFile]]
+    modelType: Optional[int]
+
+    def __init__(self, **kwargs):
+        self.id = kwargs.pop("id", None)
+        self.name = kwargs.pop("name", None)
+        self.size = kwargs.pop("size", None)
+        self.path = kwargs.pop("path", None)
+        self.repo_id = kwargs.pop("repo_id", None)
+        self.repoId = kwargs.pop("repoId", None)
+        self.userId = kwargs.pop("userId", None)
+        self.userName = kwargs.pop("userName", None)
+        self.isCanOper = kwargs.pop("isCanOper", None)
+        self.isCanDelete = kwargs.pop("isCanDelete", None)
+        self.isCanDownload = kwargs.pop("isCanDownload", None)
+        self.repoName = kwargs.pop("repoName", None)
+        self.repoOwnerName = kwargs.pop("repoOwnerName", None)
+
+        modelFileList = kwargs.pop("modelFileList", [])
+        if modelFileList:
+            for data in modelFileList:
+                data.update({"repo_id": self.repo_id, "model_id": self.id})
+            self.modelFileList = [ModelFile(**data) for data in modelFileList]
+        else:
+            self.modelFileList = None
+
+        self.modelType = kwargs.pop("modelType", None)
+
+
+@dataclass
+class ModelCreate:
+    code: str
+    msg: Optional[str] = None
+    id: Optional[int] = None
+
+
+@dataclass
+class BasicResp:
+    code: int
+    msg: str
+    data: any
```

### Comparing `openi-2.0.0b2/src/openi/_exceptions.py` & `openi-2.0.0b5/src/openi/_exceptions.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-import re
-from functools import wraps
-from inspect import signature
-from pathlib import Path
-from typing import Callable, Type, TypeVar
-
-from .constants import REPO_ID_REGEX
-from .log import setup_logger
-
-logger = setup_logger("info")
-
-
-class TokenNotFoundWarn(Warning):
-    def __init__(self, message):
-        self.message = (
-            "未找到本地 token；若遇到提示 PageNotFound 或 UnauthorizedError，"
-            "则需要使用 `login` 保存启智账户 token 到本地以获取授权。"
-        )
-
-    def __str__(self):
-        return repr(self.message)
-
-
-class OpenIError(BaseException):
-    def __init__(self, msg):
-        self.msg = msg
-
-    def __str__(self):
-        return "❌ " + self.msg
-
-    def __repr__(self):
-        return "❌ " + self.msg
-
-
-class ServerError(OpenIError):
-    def __init__(self):
-        self.msg = "OpenI服务器暂时不可用，请联系社区管理员或稍后再试"
-
-
-class OpenIProxyError(OpenIError):
-    def __init__(self):
-        self.msg = "无法连接到服务器，请检查网络代理"
-
-
-class OpenIConnectionError(OpenIError):
-    def __init__(self):
-        self.msg = "无法连接网络，请检查网络设置"
-
-
-class InvalidTokenError(OpenIError):
-    def __init__(self):
-        self.msg = f"Invalid or broken OpenI token."
-
-
-class TokenNotFoundError(OpenIError):
-    def __init__(self):
-        self.msg = "未找到本地 token；请先使用 `openi.login` 保存启智账户 token 到本地以获取授权。"
-
-
-class UnauthorizedError(OpenIError):
-    def __init__(self):
-        self.msg = "您无权建立此连接。请确保您拥有对应的权限。"
-
-
-class PageNotFound(OpenIError):
-    def __init__(self):
-        self.msg = "无效请求，请确保仓库路径填写正确并且您拥有对应的权限"
-
-
-class ParamsTypeError(OpenIError):
-    def __init__(
-        self,
-        arg_name: str,
-        arg_value: any,
-        accepted_type: Type[any],
-    ):
-        self.msg = (
-            f"`{arg_name}` 参数类型错误 {type(arg_value)}: `{arg_value}`. "
-            f"正确的参数类型为 {accepted_type}"
-        )
-
-
-class RepoIdError(OpenIError):
-    def __init__(self, repo_id):
-        self.msg = f"`{repo_id}` 参数格式错误. 正确的 `repo_id` 参数格式应为: `用户名/仓库名`"
-
-
-class RepoNotFoundError(OpenIError):
-    def __init__(self, repo_id):
-        self.msg = f"仓库不存在: `{repo_id}`"
-
-
-class KeyboardInterruptError(OpenIError):
-    def __init__(self, msg):
-        self.msg = f"用户中断操作; {msg}"
-
-
-class DatasetNotFound(OpenIError):
-    def __init__(self, repo_id, dataset_url):
-        self.msg = f"`{repo_id}` 仓库尚未创建数据集: {dataset_url}"
-
-
-class EmptyDataset(OpenIError):
-    def __init__(self, repo_id, dataset_url):
-        self.msg = f"`{repo_id}` 仓库数据集内未找到任何文件: {dataset_url}"
-
-
-class ModelNotFoundError(OpenIError):
-    def __init__(self, model_name, model_list_url):
-        self.msg = f"模型不存在 `{model_name}`; 请在网页端查看正确模型名称: {model_list_url}"
-
-
-class ServerFileExistsError(OpenIError):
-    def __init__(self, filename: str, existing_filename: str = None):
-        if existing_filename:
-            self.msg = f"`{filename}` 文件已被上传为 `{existing_filename}`, 无法重复上传"
-        else:
-            self.msg = f"`{filename}` 文件已上传, 无法重复上传"
-
-
-class ServerFileNotFoundError(OpenIError):
-    def __init__(self, msg):
-        self.msg = msg
-
-
-class EmptyFolderError(OpenIError):
-    def __init__(self, local_dir: Path):
-        self.msg = f"空目录，未能找到任何本地文件: {local_dir.absolute()}"
-
-
-class LocalPathNotFound(OpenIError):
-    def __init__(self, filepath: Path):
-        self.msg = f"本地文件或目录不存在: {filepath.absolute()}"
-
-
-class LocalDirNotFound(OpenIError):
-    def __init__(self, local_dir: Path):
-        self.msg = f"本地目录不存在: {local_dir.absolute()}"
-
-
-class FileTypeError(OpenIError):
-    def __init__(self, filepath: Path):
-        self.msg = f"非压缩文件(`.zip` 或 `.tar.gz`): {filepath.absolute()}"
-
-
-class FileSizeError(OpenIError):
-    def __init__(self, msg):
-        self.msg = msg
-
-
-class PutUploadError(OpenIError):
-    def __init__(self, msg):
-        self.msg = msg
-
-
-class UploadError(OpenIError):
-    def __init__(self, msg):
-        self.msg = msg
-
-
-CallableT = TypeVar("CallableT", bound=Callable)
-
-
-def validate_openi_args(fn: CallableT) -> CallableT:
-    """Decorator that retrieves and prints all input arguments of a function.
-
-    Args:
-        fn: The function to be decorated.
-
-    Returns:
-        A wrapper function that prints arguments and calls the original function.
-    """
-
-    @wraps(fn)
-    def _inner_fn(*args, **kwargs):
-        params = signature(fn).parameters
-        arg_names = [param.name for param in params.values()]
-
-        _kwargs = dict()
-
-        for i, arg_name in enumerate(arg_names):
-            if i < len(args):
-                value = args[i]
-            else:
-                value = kwargs.get(arg_name, None)
-            _kwargs.update({arg_name: value})
-
-        repo_id = _kwargs.get("repo_id", None)
-        if not repo_id or not isinstance(repo_id, str):
-            raise ParamsTypeError(
-                arg_name="repo_id",
-                arg_value=repo_id,
-                accepted_type=str,
-            )
-        if not re.match(REPO_ID_REGEX, repo_id):
-            raise RepoIdError(
-                repo_id=repo_id,
-            )
-
-        filename = _kwargs.get("file", None)
-        if filename and not isinstance(filename, (Path, str)):
-            raise ParamsTypeError(
-                arg_name="file",
-                arg_value=filename,
-                accepted_type="either a pathlib.Path() object or str",
-            )
-
-        cluster = _kwargs.get("cluster", None)
-        if cluster and (
-            not isinstance(cluster, str)
-            or cluster.lower() not in ["gpu", "npu"]
-        ):
-            raise ParamsTypeError(
-                arg_name="cluster",
-                arg_value=cluster,
-                accepted_type="['gpu', 'npu'] case insensitive",
-            )
-
-        save_path = _kwargs.get("save_path", None)
-        if save_path and not isinstance(save_path, (Path, str)):
-            raise ParamsTypeError(
-                arg_name="save_path",
-                arg_value=save_path,
-                accepted_type="either a pathlib.Path() object or str",
-            )
-
-        force = _kwargs.get("force", None)
-        if force and not isinstance(force, bool):
-            raise ParamsTypeError(
-                arg_name="force",
-                arg_value=force,
-                accepted_type=bool,
-            )
-
-        model_name = _kwargs.get("model_name", None)
-        if model_name and not isinstance(model_name, str):
-            raise ParamsTypeError(
-                arg_name="model_name",
-                arg_value=model_name,
-                accepted_type=str,
-            )
-
-        upload_name = _kwargs.get("upload_name", None)
-        if upload_name and not isinstance(upload_name, str):
-            raise ParamsTypeError(
-                arg_name="upload_name",
-                arg_value=upload_name,
-                accepted_type=str,
-            )
-
-        folder = _kwargs.get("folder", None)
-        if folder and not isinstance(folder, (Path, str)):
-            raise ParamsTypeError(
-                arg_name="folder",
-                arg_value=folder,
-                accepted_type=str,
-            )
-
-        return fn(*args, **kwargs)
-
-    return _inner_fn
+import re
+from functools import wraps
+from inspect import signature
+from pathlib import Path
+from typing import Callable, Type, TypeVar
+
+from .constants import REPO_ID_REGEX
+from .log import setup_logger
+
+logger = setup_logger("info")
+
+
+class TokenNotFoundWarn(Warning):
+    def __init__(self, message):
+        self.message = (
+            "未找到本地 token；若遇到提示 PageNotFound 或 UnauthorizedError，"
+            "则需要使用 `login` 保存启智账户 token 到本地以获取授权。"
+        )
+
+    def __str__(self):
+        return repr(self.message)
+
+
+class OpenIError(BaseException):
+    def __init__(self, msg):
+        self.msg = msg
+
+    def __str__(self):
+        return "❌ " + self.msg
+
+    def __repr__(self):
+        return "❌ " + self.msg
+
+
+class ServerError(OpenIError):
+    def __init__(self):
+        self.msg = "OpenI服务器暂时不可用，请联系社区管理员或稍后再试"
+
+
+class OpenIProxyError(OpenIError):
+    def __init__(self):
+        self.msg = "无法连接到服务器，请检查网络代理"
+
+
+class OpenIConnectionError(OpenIError):
+    def __init__(self):
+        self.msg = "无法连接网络，请检查网络设置"
+
+
+class InvalidTokenError(OpenIError):
+    def __init__(self):
+        self.msg = f"Invalid or broken OpenI token."
+
+
+class TokenNotFoundError(OpenIError):
+    def __init__(self):
+        self.msg = "未找到本地 token；请先使用 `openi.login` 保存启智账户 token 到本地以获取授权。"
+
+
+class UnauthorizedError(OpenIError):
+    def __init__(self):
+        self.msg = "您无权建立此连接。请确保您拥有对应的权限。"
+
+
+class PageNotFound(OpenIError):
+    def __init__(self):
+        self.msg = "无效请求，请确保仓库路径填写正确并且您拥有对应的权限"
+
+
+class ParamsTypeError(OpenIError):
+    def __init__(
+        self,
+        arg_name: str,
+        arg_value: any,
+        accepted_type: Type[any],
+    ):
+        self.msg = (
+            f"`{arg_name}` 参数类型错误 {type(arg_value)}: `{arg_value}`. "
+            f"正确的参数类型为 {accepted_type}"
+        )
+
+
+class RepoIdError(OpenIError):
+    def __init__(self, repo_id):
+        self.msg = f"`{repo_id}` 参数格式错误. 正确的 `repo_id` 参数格式应为: `用户名/仓库名`"
+
+
+class RepoNotFoundError(OpenIError):
+    def __init__(self, repo_id):
+        self.msg = f"仓库不存在: `{repo_id}`"
+
+
+class KeyboardInterruptError(OpenIError):
+    def __init__(self, msg):
+        self.msg = f"用户中断操作; {msg}"
+
+
+class DatasetNotFound(OpenIError):
+    def __init__(self, repo_id, dataset_url):
+        self.msg = f"`{repo_id}` 仓库尚未创建数据集: {dataset_url}"
+
+
+class EmptyDataset(OpenIError):
+    def __init__(self, repo_id, dataset_url):
+        self.msg = f"`{repo_id}` 仓库数据集内未找到任何文件: {dataset_url}"
+
+
+class ModelNotFoundError(OpenIError):
+    def __init__(self, model_name, model_list_url):
+        self.msg = f"模型不存在 `{model_name}`; 请在网页端查看正确模型名称: {model_list_url}"
+
+
+class ServerFileExistsError(OpenIError):
+    def __init__(self, filename: str, existing_filename: str = None):
+        if existing_filename:
+            self.msg = f"`{filename}` 文件已被上传为 `{existing_filename}`, 无法重复上传"
+        else:
+            self.msg = f"`{filename}` 文件已上传, 无法重复上传"
+
+
+class ServerFileNotFoundError(OpenIError):
+    def __init__(self, msg):
+        self.msg = msg
+
+
+class EmptyFolderError(OpenIError):
+    def __init__(self, local_dir: Path):
+        self.msg = f"空目录，未能找到任何本地文件: {local_dir.absolute()}"
+
+
+class LocalPathNotFound(OpenIError):
+    def __init__(self, filepath: Path):
+        self.msg = f"本地文件或目录不存在: {filepath.absolute()}"
+
+
+class LocalDirNotFound(OpenIError):
+    def __init__(self, local_dir: Path):
+        self.msg = f"本地目录不存在: {local_dir.absolute()}"
+
+
+class FileTypeError(OpenIError):
+    def __init__(self, filepath: Path):
+        self.msg = f"非压缩文件(`.zip` 或 `.tar.gz`): {filepath.absolute()}"
+
+
+class FileSizeError(OpenIError):
+    def __init__(self, msg):
+        self.msg = msg
+
+
+class PutUploadError(OpenIError):
+    def __init__(self, msg):
+        self.msg = msg
+
+
+class UploadError(OpenIError):
+    def __init__(self, msg):
+        self.msg = msg
+
+
+CallableT = TypeVar("CallableT", bound=Callable)
+
+
+def validate_openi_args(fn: CallableT) -> CallableT:
+    """Decorator that retrieves and prints all input arguments of a function.
+
+    Args:
+        fn: The function to be decorated.
+
+    Returns:
+        A wrapper function that prints arguments and calls the original function.
+    """
+
+    @wraps(fn)
+    def _inner_fn(*args, **kwargs):
+        params = signature(fn).parameters
+        arg_names = [param.name for param in params.values()]
+
+        _kwargs = dict()
+
+        for i, arg_name in enumerate(arg_names):
+            if i < len(args):
+                value = args[i]
+            else:
+                value = kwargs.get(arg_name, None)
+            _kwargs.update({arg_name: value})
+
+        repo_id = _kwargs.get("repo_id", None)
+        if not repo_id or not isinstance(repo_id, str):
+            raise ParamsTypeError(
+                arg_name="repo_id",
+                arg_value=repo_id,
+                accepted_type=str,
+            )
+        if not re.match(REPO_ID_REGEX, repo_id):
+            raise RepoIdError(
+                repo_id=repo_id,
+            )
+
+        filename = _kwargs.get("file", None)
+        if filename and not isinstance(filename, (Path, str)):
+            raise ParamsTypeError(
+                arg_name="file",
+                arg_value=filename,
+                accepted_type="either a pathlib.Path() object or str",
+            )
+
+        cluster = _kwargs.get("cluster", None)
+        if cluster and (
+            not isinstance(cluster, str)
+            or cluster.lower() not in ["gpu", "npu"]
+        ):
+            raise ParamsTypeError(
+                arg_name="cluster",
+                arg_value=cluster,
+                accepted_type="['gpu', 'npu'] case insensitive",
+            )
+
+        save_path = _kwargs.get("save_path", None)
+        if save_path and not isinstance(save_path, (Path, str)):
+            raise ParamsTypeError(
+                arg_name="save_path",
+                arg_value=save_path,
+                accepted_type="either a pathlib.Path() object or str",
+            )
+
+        force = _kwargs.get("force", None)
+        if force and not isinstance(force, bool):
+            raise ParamsTypeError(
+                arg_name="force",
+                arg_value=force,
+                accepted_type=bool,
+            )
+
+        model_name = _kwargs.get("model_name", None)
+        if model_name and not isinstance(model_name, str):
+            raise ParamsTypeError(
+                arg_name="model_name",
+                arg_value=model_name,
+                accepted_type=str,
+            )
+
+        upload_name = _kwargs.get("upload_name", None)
+        if upload_name and not isinstance(upload_name, str):
+            raise ParamsTypeError(
+                arg_name="upload_name",
+                arg_value=upload_name,
+                accepted_type=str,
+            )
+
+        folder = _kwargs.get("folder", None)
+        if folder and not isinstance(folder, (Path, str)):
+            raise ParamsTypeError(
+                arg_name="folder",
+                arg_value=folder,
+                accepted_type=str,
+            )
+
+        return fn(*args, **kwargs)
+
+    return _inner_fn
```

### Comparing `openi-2.0.0b2/src/openi/_file.py` & `openi-2.0.0b5/src/openi/_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,261 @@
-import hashlib
-import math
-from pathlib import Path
-from typing import Iterator, List, Optional, Tuple, Union
-
-from .constants import CHUNK_SIZE, FILE_CACHE_PREFIX
-
-
-class UploadFile:
-    """
-    file object for upload
-    """
-
-    def __init__(self, path: Union[str, Path], name: Optional[str] = None):
-        if isinstance(path, str):
-            path = Path(path).absolute()
-
-        self.path = path
-        self.name: str = name if name else path.name
-        self.chunk_size = CHUNK_SIZE
-
-    def __repr__(self):
-        return (
-            f"UploadFile(path={self.path}, name={self.name}, "
-            f"size={self.size}, md5={self.md5}, "
-            f"total_chunks_count={self.total_chunks_count})"
-        )
-
-    def exists(self) -> bool:
-        if self.path.exists() and self.path.is_file():
-            return True
-        else:
-            return False
-
-    def is_zip(self) -> bool:
-        suffixes = "".join(self.path.suffixes)
-        return ".zip" in suffixes or ".tar.gz" in suffixes
-
-    @property
-    def size(self) -> int:
-        return self.path.stat().st_size
-
-    @property
-    def md5(self) -> str:
-        return get_file_md5(self.path, chunk_size=self.chunk_size)
-
-    @property
-    def total_chunks_count(self) -> int:
-        return get_file_total_chunks_count(
-            self.path, chunk_size=self.chunk_size
-        )
-
-
-class CacheFile:
-    """
-    file object for download
-    """
-
-    def __init__(
-        self,
-        name: str,
-        size: int,
-        save_path: Union[Path, str],
-        force: bool = False,
-    ):
-        self.name: str = name
-        self.size: int = size
-
-        if isinstance(save_path, str):
-            save_path = Path(save_path).absolute()
-        self.save_path: Path = save_path
-
-        self.file_path = self.save_path / self.name
-        self.cache_path = self.save_path / f"{FILE_CACHE_PREFIX}{self.name}"
-
-        if force:
-            self.force_download()
-
-        if not self.cache_path.exists():
-            self.cache_path.parent.mkdir(parents=True, exist_ok=True)
-            self.cache_path.touch(exist_ok=True)
-
-    def __repr__(self):
-        return (
-            f"CacheFile(name={self.name}, size={self.size}, "
-            f"save_path={self.save_path},"
-            f"file_path={self.file_path}, cache_path={self.cache_path})"
-        )
-
-    @property
-    def cache_size(self) -> int:
-        return self.cache_path.stat().st_size
-
-    def as_completed(self, rename_existing: bool = True) -> bool:
-        if self.cache_size != self.size:
-            return False
-
-        if rename_existing and self.file_path.exists():
-            self.file_path = rename_existing_file(self.file_path)
-
-        self.cache_path.rename(self.file_path)
-        return True
-
-    def force_download(self) -> None:
-        self.file_path.unlink(missing_ok=True)
-        self.cache_path.unlink(missing_ok=True)
-
-
-def rename_existing_file(filepath: Union[str, Path]) -> Path:
-    """Renames a file by adding a digital suffix in case of conflicts.
-
-    Args:
-        filepath (Path): The path to the file to rename.
-
-    Returns:
-        Path: The new path of the renamed file.
-    """
-    if isinstance(filepath, str):
-        filepath = Path(filepath).absolute()
-
-    filename = filepath.name.split(".")
-    stem, suffix = filename[0], ".".join(filename[1:])
-    new_filepath = filepath
-
-    i = 1
-    while new_filepath.exists():
-        new_filepath = filepath.with_name(f"{stem}({i}).{suffix}")
-        i += 1
-
-    return new_filepath
-
-
-def is_file(filepath: Path) -> bool:
-    return filepath.is_file()
-
-
-def is_dir(filepath: Path) -> bool:
-    return filepath.is_dir()
-
-
-def is_zip(filepath: Path) -> bool:
-    suffixes = "".join(filepath.suffixes)
-    return ".zip" in suffixes or ".tar.gz" in suffixes
-
-
-def get_file_size(filepath: Path) -> int:
-    return filepath.stat().st_size
-
-
-def get_file_md5(filepath: Path, chunk_size: int = CHUNK_SIZE) -> str:
-    # upload_mode: Literal["model", "dataset"],
-    m = hashlib.md5()
-    with open(filepath, "rb") as f:
-        while True:
-            data = f.read(chunk_size)
-            if not data:
-                break
-            md5_data = data[
-                : 1024 * 1024
-            ]  # if upload_mode == "dataset" else data
-            m.update(md5_data)
-    return m.hexdigest()
-
-
-def get_file_total_chunks_count(
-    filepath: Path, chunk_size: int = CHUNK_SIZE
-) -> int:
-    file_size = get_file_size(filepath)
-    return math.ceil(file_size / chunk_size)
-
-
-def file_chunk_iterator(
-    filepath: Path,
-    chunk_size: int = CHUNK_SIZE,
-    start_from_chunk: int = 1,
-) -> Iterator[Tuple[int, bytes]]:
-    """
-    Iterate over file chunks data.
-
-    Args:
-        filepath (Union[str, Path]): local file path
-        chunk_size (int, optional): chunk size.
-        start_from_chunk (int, optional): start from chunk. Defaults to 1.
-
-    Yields:
-        Tuple[int, bytes]: chunk number and chunk data
-    """
-    chunk_number = start_from_chunk
-
-    with open(filepath, "rb") as f_reader:
-        f_reader.seek((start_from_chunk - 1) * chunk_size)
-        while True:
-            chunk_data = f_reader.read(chunk_size)
-            if not chunk_data:
-                break
-
-            yield chunk_number, chunk_data
-
-            chunk_number += 1
-
-
-def split_subdir_name(filename: str) -> Tuple[str, str]:
-    """
-    Split the filename into subdirectory and name.
-
-    Args:
-        filename (str): The name of the file.
-
-    Returns:
-        Tuple[str, str]: The subdirectory and the name of the file.
-    """
-    as_path = Path(filename.lstrip("/"))
-    return as_path.parent.as_posix(), as_path.name
-
-
-def get_local_dir_files(local_dir: Path) -> List[Path]:
-    """
-    Returns a list of filepath in given directory.
-    """
-    return [file for file in local_dir.rglob("*") if file.is_file()]
-
-
-# def get_local_dir_zipfiles(local_dir: Union[Path, str]) -> List[UploadFile]:
-#     """
-#     Returns a list of dictionaries containing file information.
-#
-#     Args:
-#         folder_path (Path): Path to the folder to process.
-#
-#     Returns:
-#         list: A list of dictionaries with the following structure:
-#             {
-#                 "path": Path object representing the file path,
-#                 "name": Relative path of the file from the given folder
-#             }
-#     """
-#     if isinstance(local_dir, str):
-#         local_dir = Path(local_dir).absolute()
-#
-#     if not local_dir.is_dir():
-#         raise LocalDirNotFound(f"{local_dir} is not a directory")
-#
-#     file_list = list()
-#     for file in local_dir.rglob("*"):
-#         if file.is_file() and is_zip(file):
-#             path = file
-#             name = file.name
-#             size = get_file_size(file)
-#
-#             file_obj = UploadFile(path=path, name=name, size=size)
-#
-#             file_list.append(file_obj)
-#
-#     return file_list
+import hashlib
+import math
+from pathlib import Path
+from typing import (
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Union
+)
+
+from .constants import (
+    CHUNK_SIZE,
+    FILE_CACHE_PREFIX
+)
+
+
+class UploadFile:
+    """
+    file object for upload
+    """
+
+    def __init__(self, path: Union[str, Path], name: Optional[str] = None):
+        if isinstance(path, str):
+            path = Path(path).absolute()
+
+        self.path = path
+        self.name: str = name if name else path.name
+        self.chunk_size = CHUNK_SIZE
+
+    def __repr__(self):
+        return (
+            f"UploadFile(path={self.path}, name={self.name}, "
+            f"size={self.size}, md5={self.md5}, "
+            f"total_chunks_count={self.total_chunks_count})"
+        )
+
+    def exists(self) -> bool:
+        if self.path.exists() and self.path.is_file():
+            return True
+        else:
+            return False
+
+    def is_zip(self) -> bool:
+        suffixes = "".join(self.path.suffixes)
+        return ".zip" in suffixes or ".tar.gz" in suffixes
+
+    @property
+    def size(self) -> int:
+        return self.path.stat().st_size
+
+    @property
+    def md5(self) -> str:
+        return get_file_md5(self.path, chunk_size=self.chunk_size)
+
+    @property
+    def total_chunks_count(self) -> int:
+        return get_file_total_chunks_count(self.path, chunk_size=self.chunk_size)
+
+
+class CacheFile:
+    """
+    file object for download
+    """
+
+    def __init__(
+        self,
+        name: str,
+        size: int,
+        save_path: Union[Path, str],
+        force: bool = False,
+    ):
+        self.name: str = name
+        self.size: int = size
+
+        if isinstance(save_path, str):
+            save_path = Path(save_path).absolute()
+        self.save_path: Path = save_path
+
+        self.file_path = self.save_path / self.name
+        self.cache_path = self.save_path / f"{FILE_CACHE_PREFIX}{self.name}"
+
+        if force:
+            self.force_download()
+
+        if not self.cache_path.exists():
+            self.cache_path.parent.mkdir(parents=True, exist_ok=True)
+            self.cache_path.touch(exist_ok=True)
+
+    def __repr__(self):
+        return (
+            f"CacheFile(name={self.name}, size={self.size}, "
+            f"save_path={self.save_path},"
+            f"file_path={self.file_path}, cache_path={self.cache_path})"
+        )
+
+    @property
+    def cache_size(self) -> int:
+        return self.cache_path.stat().st_size
+
+    def as_completed(self, rename_existing: bool = True) -> bool:
+        if self.cache_size != self.size:
+            return False
+
+        if rename_existing and self.file_path.exists():
+            self.file_path = rename_existing_file(self.file_path)
+
+        self.cache_path.rename(self.file_path)
+        return True
+
+    def force_download(self) -> None:
+        self.file_path.unlink(missing_ok=True)
+        self.cache_path.unlink(missing_ok=True)
+
+
+def rename_existing_file(filepath: Union[str, Path]) -> Path:
+    """Renames a file by adding a digital suffix in case of conflicts.
+
+    Args:
+        filepath (Path): The path to the file to rename.
+
+    Returns:
+        Path: The new path of the renamed file.
+    """
+    if isinstance(filepath, str):
+        filepath = Path(filepath).absolute()
+
+    stem, suffix = filepath.stem, filepath.suffix
+
+    # special handling for '.tar.gz' files
+    if suffix == ".gz" and ".tar" in stem:
+        stem = Path(stem).stem
+        suffix = ".tar.gz"
+
+    i = 1
+    new_filepath = filepath
+    while new_filepath.exists():
+        new_filepath = filepath.with_name(f"{stem}({i}){suffix}")
+        i += 1
+
+    return new_filepath
+
+
+def is_file(filepath: Path) -> bool:
+    return filepath.is_file()
+
+
+def is_dir(filepath: Path) -> bool:
+    return filepath.is_dir()
+
+
+def is_zip(filepath: Path) -> bool:
+    suffixes = "".join(filepath.suffixes)
+    return ".zip" in suffixes or ".tar.gz" in suffixes
+
+
+def get_file_size(filepath: Path) -> int:
+    return filepath.stat().st_size
+
+
+def get_file_md5(filepath: Path, chunk_size: int = CHUNK_SIZE) -> str:
+    # upload_mode: Literal["model", "dataset"],
+    m = hashlib.md5()
+    with open(filepath, "rb") as f:
+        while True:
+            data = f.read(chunk_size)
+            if not data:
+                break
+            md5_data = data[: 1024 * 1024]  # if upload_mode == "dataset" else data
+            m.update(md5_data)
+    return m.hexdigest()
+
+
+def get_file_total_chunks_count(filepath: Path, chunk_size: int = CHUNK_SIZE) -> int:
+    file_size = get_file_size(filepath)
+    return math.ceil(file_size / chunk_size)
+
+
+def file_chunk_iterator(
+    filepath: Path,
+    chunk_size: int = CHUNK_SIZE,
+    start_from_chunk: int = 1,
+) -> Iterator[Tuple[int, bytes]]:
+    """
+    Iterate over file chunks data.
+
+    Args:
+        filepath (Union[str, Path]): local file path
+        chunk_size (int, optional): chunk size.
+        start_from_chunk (int, optional): start from chunk. Defaults to 1.
+
+    Yields:
+        Tuple[int, bytes]: chunk number and chunk data
+    """
+    chunk_number = start_from_chunk
+
+    with open(filepath, "rb") as f_reader:
+        f_reader.seek((start_from_chunk - 1) * chunk_size)
+        while True:
+            chunk_data = f_reader.read(chunk_size)
+            if not chunk_data:
+                break
+
+            yield chunk_number, chunk_data
+
+            chunk_number += 1
+
+
+def split_subdir_name(filename: str) -> Tuple[str, str]:
+    """
+    Split the filename into subdirectory and name.
+
+    Args:
+        filename (str): The name of the file.
+
+    Returns:
+        Tuple[str, str]: The subdirectory and the name of the file.
+    """
+    as_path = Path(filename.lstrip("/"))
+    return as_path.parent.as_posix(), as_path.name
+
+
+def get_local_dir_files(local_dir: Path) -> List[Path]:
+    """
+    Returns a list of filepath in given directory.
+    """
+    return [file for file in local_dir.rglob("*") if file.is_file()]
+
+
+# def get_local_dir_zipfiles(local_dir: Union[Path, str]) -> List[UploadFile]:
+#     """
+#     Returns a list of dictionaries containing file information.
+#
+#     Args:
+#         folder_path (Path): Path to the folder to process.
+#
+#     Returns:
+#         list: A list of dictionaries with the following structure:
+#             {
+#                 "path": Path object representing the file path,
+#                 "name": Relative path of the file from the given folder
+#             }
+#     """
+#     if isinstance(local_dir, str):
+#         local_dir = Path(local_dir).absolute()
+#
+#     if not local_dir.is_dir():
+#         raise LocalDirNotFound(f"{local_dir} is not a directory")
+#
+#     file_list = list()
+#     for file in local_dir.rglob("*"):
+#         if file.is_file() and is_zip(file):
+#             path = file
+#             name = file.name
+#             size = get_file_size(file)
+#
+#             file_obj = UploadFile(path=path, name=name, size=size)
+#
+#             file_list.append(file_obj)
+#
+#     return file_list
```

### Comparing `openi-2.0.0b2/src/openi/_session.py` & `openi-2.0.0b5/src/openi/_session.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-#!/usr/bin/env python
-import json
-import os
-from time import sleep
-from typing import Any, Callable, Optional
-
-import requests
-
-from ._exceptions import (
-    OpenIConnectionError,
-    OpenIProxyError,
-    PageNotFound,
-    ServerError,
-    TokenNotFoundError,
-    UnauthorizedError,
-)
-from .constants import (
-    DEFAULT_BASE_URL,
-    HTTP_MAX_RETRIES,
-    HTTP_RETRY_DELAY,
-    TOKEN_FILE_PATH,
-)
-from .log import setup_logger
-
-logger = setup_logger()
-
-
-def retry(func: Callable) -> Callable:
-    """
-    Decorator that retries a function a certain number of times with a delay between each retry.
-
-    Args:
-        func (Callable): The function to be retried.
-
-    Returns:
-        Callable: The decorated function.
-
-    """
-    retries: int = HTTP_MAX_RETRIES
-    delay: float = HTTP_RETRY_DELAY
-
-    def _retry(*args, **kwargs) -> Any:
-        for i in range(1, retries + 1):
-            if func.__name__ == "put_upload":
-                url = args[1] if len(args) > 1 else kwargs.get("url", None)
-
-            if func.__name__ == "http_request":
-                url = args[2] if len(args) > 2 else kwargs.get("route", None)
-
-            try:
-                return func(*args, **kwargs)
-
-            except Exception as e:
-                if i == retries:
-                    logger.error(f"{i} failed; Error: {repr(e)}")
-                    logger.error(f"`{url}` failed after {retries} retries; ")
-
-                    if isinstance(e, requests.exceptions.ProxyError):
-                        raise OpenIProxyError()
-
-                    if isinstance(e, requests.exceptions.ConnectionError):
-                        raise OpenIConnectionError()
-
-                    else:
-                        raise e
-
-                else:
-                    logger.error(
-                        f"{i} failed -> Retrying...; Error: {repr(e)}"
-                    )
-                    sleep(delay)
-
-    return _retry
-
-
-@retry
-def put_upload(
-    url,
-    filedata: bytes,
-    filename: str,
-    upload_type: int = 0,
-    **kwargs,
-) -> Optional[str]:
-    """Override the put method
-
-    Args:
-        url (str): URL of CloudStorage to upload file data
-        filedata (bytes): Binary file data to upload
-        upload_type (int, optional): 0 for minio, 1 for obs
-
-    Returns:
-        Response: Response object from requests
-    """
-    headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
-
-    resp = requests.put(url, data=filedata, headers=headers, **kwargs)
-    etag = resp.headers.get("ETag", None)
-
-    logger.info(f"PUT {resp.status_code} `{filename}`; etag: {etag}")
-    return etag
-
-
-class OpenISession(requests.Session):
-    def __init__(self, *args: list, **kwargs: dict):
-        """
-        Initialize OpenISession object
-        """
-        super(OpenISession, self).__init__(*args, **kwargs)
-        self.endpoint: str = DEFAULT_BASE_URL
-        self.token: Optional[str] = None
-        self.dev_mode: bool = False
-
-    def __repr__(self):
-        return f"OpenISession(endpoint={self.endpoint}, token={self.token})"
-
-    @staticmethod
-    def get_local_auth() -> Optional[dict]:
-        """
-        Load saved `token.json` on local machine for set_basic_auth()
-
-        Returns:
-            tuple: (endpoint, token), loaded from `token.json`
-        """
-        try:
-            return json.loads(TOKEN_FILE_PATH.read_text())
-
-        except FileNotFoundError:
-            logger.error(f"No token file found at `{TOKEN_FILE_PATH}`.")
-            return None
-
-        except json.decoder.JSONDecodeError:
-            logger.error(f"Invalid JSON format at `{TOKEN_FILE_PATH}`.")
-            return None
-
-        except Exception as e:
-            logger.error(f"Unknown Error: {repr(e)}")
-            raise None
-
-    def set_basic_auth(
-        self,
-        token: Optional[str],
-        endpoint: Optional[str],
-    ) -> None:
-        """Set the credentials for Basic Auth on the session object
-        Priority:
-            1. provided arguments
-            2. local saved token.json
-            3. environment variables
-        """
-        # get from saved token file
-        token_saved, endpoint_saved = None, None
-        saved_auth = self.get_local_auth()
-        if saved_auth:
-            token_saved = saved_auth.get("token", None)
-            endpoint_saved = saved_auth.get("endpoint", None)
-
-        # get from environment variables
-        token_env = os.getenv("OPENI_TOKEN", None)
-        endpoint_env = os.getenv("OPENI_ENDPOINT", None)
-
-        self.token = token or token_saved or token_env or self.token
-        self.endpoint = (
-            endpoint or endpoint_saved or endpoint_env or self.endpoint
-        )
-        self.endpoint = self.endpoint.rstrip("/")
-
-    def _build_url(self, route: str) -> str:
-        """Generate the full URL based on the self.endpoint plus the provided
-        resource (API endpoint)
-
-        Args:
-            url (str): API Endpoint suffix as found in the API documentation
-
-        Returns:
-            str: Full URL for API call
-        """
-        return self.endpoint + "/api/v1" + route
-
-    def _build_token_headers(self, headers: Optional[dict]) -> Optional[dict]:
-        """Adding token to the request's parameters
-
-        Returns:
-            dict: Arbitrary Request's keyword arguments with `token` key,value added in
-                query parameter `params`.
-        """
-        headers = dict() if headers is None else headers
-
-        if self.token is not None:
-            headers.update({"Authorization": f"token {self.token}"})
-
-        return headers
-
-    @staticmethod
-    def request_info(resp: requests.Response) -> None:
-        print(f"{'=' * 20}")
-        print(f"{resp.request.method} {resp.status_code} {resp.url}")
-        print(f"{resp.request.headers}")
-        print(f"{'=' * 20}")
-
-    # @retry
-    def send_request(
-        self, method: str, route: str, **kwargs
-    ) -> requests.Response:
-        """Customized request method
-
-        adding customized HTTP request mechanism here, e.g. retry mechanism
-
-
-        Args:
-            method (str): HTTP Method
-            route (str): API Endpoint suffix as found in `AiForge/api`
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            Response: Response object from requests
-        """
-        full_url = self._build_url(route)
-
-        headers = kwargs.pop("headers", None)
-        headers_with_token = self._build_token_headers(headers)
-
-        auth = headers_with_token.get("Authorization", None)
-
-        resp = super(OpenISession, self).request(
-            method=method,
-            url=full_url,
-            headers=headers_with_token,
-            **kwargs,
-        )
-
-        logger.info(f"{method} {resp.status_code} {resp.url};")
-        if self.dev_mode:
-            self.request_info(resp)
-
-        if resp.status_code in [401, 403, 404]:
-            if not auth:
-                # warnings.warn(
-                #     "\033[0;31mNo local access token found."
-                #     "If you cannot access the following, "
-                #     "please `login` with your token.\033[0m",
-                #     TokenNotFoundWarn,
-                # )
-                raise TokenNotFoundError()
-            if resp.status_code == 404:
-                raise PageNotFound()
-            else:
-                raise UnauthorizedError()
-
-        if resp.status_code in [500, 502]:
-            raise ServerError()
-
-        return resp
-
-    def get(self, route, **kwargs):
-        """Override the get method
-
-        Args:
-            route (str): API Endpoint suffix as found in `AiForge/api`
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            Response: Response object from requests
-        """
-        return self.send_request("GET", route, **kwargs)
-
-    def post(self, route, json: Optional[dict] = None, **kwargs):
-        """Override the post method
-
-        Args:
-            route (str): API Endpoint suffix as found in `AiForge/api`
-            json (dict, optional): Request's body data
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            Response: Response object from requests
-        """
-        return self.send_request("POST", route, json=json, **kwargs)
-
-    # @retry
-    def put_upload(
-        self,
-        url,
-        filedata: bytes,
-        upload_type: int = 1,
-        **kwargs,
-    ) -> Optional[str]:
-        """Override the put method
-
-        Args:
-            url (str): URL of CloudStorage to upload file data
-            filedata (bytes): Binary file data to upload
-            filename (str): Name of the file to upload
-            upload_type (int, optional): 0 for minio, 1 for obs
-
-        Returns:
-            Response: Response object from requests
-        """
-        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
-
-        resp = super(OpenISession, self).request(
-            method="PUT",
-            url=url,
-            data=filedata,
-            headers=headers,
-            **kwargs,
-        )
-        if not resp or resp.status_code != 200:
-            logger.error(f"PUT upload failed to make requests")
-            return None
-
-        etag = resp.headers.get("ETag", None)
-        if etag:
-            logger.info(f"ETag: {etag}")
-        else:
-            logger.error(f"Failed to fetch ETag")
-
-        return etag
+#!/usr/bin/env python
+import json
+import os
+from time import sleep
+from typing import Any, Callable, Optional
+
+import requests
+
+from ._exceptions import (
+    OpenIConnectionError,
+    OpenIProxyError,
+    PageNotFound,
+    ServerError,
+    TokenNotFoundError,
+    UnauthorizedError,
+)
+from .constants import (
+    DEFAULT_BASE_URL,
+    HTTP_MAX_RETRIES,
+    HTTP_RETRY_DELAY,
+    TOKEN_FILE_PATH,
+)
+from .log import setup_logger
+
+logger = setup_logger()
+
+
+def retry(func: Callable) -> Callable:
+    """
+    Decorator that retries a function a certain number of times with a delay between each retry.
+
+    Args:
+        func (Callable): The function to be retried.
+
+    Returns:
+        Callable: The decorated function.
+
+    """
+    retries: int = HTTP_MAX_RETRIES
+    delay: float = HTTP_RETRY_DELAY
+
+    def _retry(*args, **kwargs) -> Any:
+        for i in range(1, retries + 1):
+            if func.__name__ == "put_upload":
+                url = args[1] if len(args) > 1 else kwargs.get("url", None)
+
+            if func.__name__ == "http_request":
+                url = args[2] if len(args) > 2 else kwargs.get("route", None)
+
+            try:
+                return func(*args, **kwargs)
+
+            except Exception as e:
+                if i == retries:
+                    logger.error(f"{i} failed; Error: {repr(e)}")
+                    logger.error(f"`{url}` failed after {retries} retries; ")
+
+                    if isinstance(e, requests.exceptions.ProxyError):
+                        raise OpenIProxyError()
+
+                    if isinstance(e, requests.exceptions.ConnectionError):
+                        raise OpenIConnectionError()
+
+                    else:
+                        raise e
+
+                else:
+                    logger.error(
+                        f"{i} failed -> Retrying...; Error: {repr(e)}"
+                    )
+                    sleep(delay)
+
+    return _retry
+
+
+@retry
+def put_upload(
+    url,
+    filedata: bytes,
+    filename: str,
+    upload_type: int = 0,
+    **kwargs,
+) -> Optional[str]:
+    """Override the put method
+
+    Args:
+        url (str): URL of CloudStorage to upload file data
+        filedata (bytes): Binary file data to upload
+        upload_type (int, optional): 0 for minio, 1 for obs
+
+    Returns:
+        Response: Response object from requests
+    """
+    headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
+
+    resp = requests.put(url, data=filedata, headers=headers, **kwargs)
+    etag = resp.headers.get("ETag", None)
+
+    logger.info(f"PUT {resp.status_code} `{filename}`; etag: {etag}")
+    return etag
+
+
+class OpenISession(requests.Session):
+    def __init__(self, *args: list, **kwargs: dict):
+        """
+        Initialize OpenISession object
+        """
+        super(OpenISession, self).__init__(*args, **kwargs)
+        self.endpoint: str = DEFAULT_BASE_URL
+        self.token: Optional[str] = None
+        self.dev_mode: bool = False
+
+    def __repr__(self):
+        return f"OpenISession(endpoint={self.endpoint}, token={self.token})"
+
+    @staticmethod
+    def get_local_auth() -> Optional[dict]:
+        """
+        Load saved `token.json` on local machine for set_basic_auth()
+
+        Returns:
+            tuple: (endpoint, token), loaded from `token.json`
+        """
+        try:
+            return json.loads(TOKEN_FILE_PATH.read_text())
+
+        except FileNotFoundError:
+            logger.error(f"No token file found at `{TOKEN_FILE_PATH}`.")
+            return None
+
+        except json.decoder.JSONDecodeError:
+            logger.error(f"Invalid JSON format at `{TOKEN_FILE_PATH}`.")
+            return None
+
+        except Exception as e:
+            logger.error(f"Unknown Error: {repr(e)}")
+            raise None
+
+    def set_basic_auth(
+        self,
+        token: Optional[str],
+        endpoint: Optional[str],
+    ) -> None:
+        """Set the credentials for Basic Auth on the session object
+        Priority:
+            1. provided arguments
+            2. local saved token.json
+            3. environment variables
+        """
+        # get from saved token file
+        token_saved, endpoint_saved = None, None
+        saved_auth = self.get_local_auth()
+        if saved_auth:
+            token_saved = saved_auth.get("token", None)
+            endpoint_saved = saved_auth.get("endpoint", None)
+
+        # get from environment variables
+        token_env = os.getenv("OPENI_TOKEN", None)
+        endpoint_env = os.getenv("OPENI_ENDPOINT", None)
+
+        self.token = token or token_saved or token_env or self.token
+        self.endpoint = (
+            endpoint or endpoint_saved or endpoint_env or self.endpoint
+        )
+        self.endpoint = self.endpoint.rstrip("/")
+
+    def _build_url(self, route: str) -> str:
+        """Generate the full URL based on the self.endpoint plus the provided
+        resource (API endpoint)
+
+        Args:
+            url (str): API Endpoint suffix as found in the API documentation
+
+        Returns:
+            str: Full URL for API call
+        """
+        return self.endpoint + "/api/v1" + route
+
+    def _build_token_headers(self, headers: Optional[dict]) -> Optional[dict]:
+        """Adding token to the request's parameters
+
+        Returns:
+            dict: Arbitrary Request's keyword arguments with `token` key,value added in
+                query parameter `params`.
+        """
+        headers = dict() if headers is None else headers
+
+        if self.token is not None:
+            headers.update({"Authorization": f"token {self.token}"})
+
+        return headers
+
+    @staticmethod
+    def request_info(resp: requests.Response) -> None:
+        print(f"{'=' * 20}")
+        print(f"{resp.request.method} {resp.status_code} {resp.url}")
+        print(f"{resp.request.headers}")
+        print(f"{'=' * 20}")
+
+    # @retry
+    def send_request(
+        self, method: str, route: str, **kwargs
+    ) -> requests.Response:
+        """Customized request method
+
+        adding customized HTTP request mechanism here, e.g. retry mechanism
+
+
+        Args:
+            method (str): HTTP Method
+            route (str): API Endpoint suffix as found in `AiForge/api`
+            **kwargs: Arbitrary keyword arguments
+
+        Returns:
+            Response: Response object from requests
+        """
+        full_url = self._build_url(route)
+
+        headers = kwargs.pop("headers", None)
+        headers_with_token = self._build_token_headers(headers)
+
+        auth = headers_with_token.get("Authorization", None)
+
+        resp = super(OpenISession, self).request(
+            method=method,
+            url=full_url,
+            headers=headers_with_token,
+            **kwargs,
+        )
+
+        logger.info(f"{method} {resp.status_code} {resp.url};")
+        if self.dev_mode:
+            self.request_info(resp)
+
+        if resp.status_code in [401, 403, 404]:
+            if not auth:
+                # warnings.warn(
+                #     "\033[0;31mNo local access token found."
+                #     "If you cannot access the following, "
+                #     "please `login` with your token.\033[0m",
+                #     TokenNotFoundWarn,
+                # )
+                raise TokenNotFoundError()
+            if resp.status_code == 404:
+                raise PageNotFound()
+            else:
+                raise UnauthorizedError()
+
+        if resp.status_code in [500, 502]:
+            raise ServerError()
+
+        return resp
+
+    def get(self, route, **kwargs):
+        """Override the get method
+
+        Args:
+            route (str): API Endpoint suffix as found in `AiForge/api`
+            **kwargs: Arbitrary keyword arguments
+
+        Returns:
+            Response: Response object from requests
+        """
+        return self.send_request("GET", route, **kwargs)
+
+    def post(self, route, json: Optional[dict] = None, **kwargs):
+        """Override the post method
+
+        Args:
+            route (str): API Endpoint suffix as found in `AiForge/api`
+            json (dict, optional): Request's body data
+            **kwargs: Arbitrary keyword arguments
+
+        Returns:
+            Response: Response object from requests
+        """
+        return self.send_request("POST", route, json=json, **kwargs)
+
+    # @retry
+    def put_upload(
+        self,
+        url,
+        filedata: bytes,
+        upload_type: int = 1,
+        **kwargs,
+    ) -> Optional[str]:
+        """Override the put method
+
+        Args:
+            url (str): URL of CloudStorage to upload file data
+            filedata (bytes): Binary file data to upload
+            filename (str): Name of the file to upload
+            upload_type (int, optional): 0 for minio, 1 for obs
+
+        Returns:
+            Response: Response object from requests
+        """
+        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
+
+        resp = super(OpenISession, self).request(
+            method="PUT",
+            url=url,
+            data=filedata,
+            headers=headers,
+            **kwargs,
+        )
+        if not resp or resp.status_code != 200:
+            logger.error(f"PUT upload failed to make requests")
+            return None
+
+        etag = resp.headers.get("ETag", None)
+        if etag:
+            logger.info(f"ETag: {etag}")
+        else:
+            logger.error(f"Failed to fetch ETag")
+
+        return etag
```

### Comparing `openi-2.0.0b2/src/openi/_tqdm.py` & `openi-2.0.0b5/src/openi/_tqdm.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-from __future__ import annotations
-
-from typing import Optional
-
-from tqdm.auto import tqdm
-
-
-class FileProgressBar(tqdm):
-    """
-    Customized `Tqdm` class for OpenI uploads and downloads.
-    It displays a file progress bar of the operation.
-
-
-    Args:
-        display_name (`str`):
-            The name of the file being uploaded or downloaded.
-        size (`int`):
-            The total size of the file in bytes.
-        position (`int`, `optional`, defaults to `0`):
-            The display position of the progress bar if multiple bars are created.
-        initial (`int`, `optional`, defaults to `0`):
-            The initial progress of the progress bar.
-        colour (`str`, `optional`, defaults to `None`):
-            The colour of the progress bar.
-        max_width (`int`, `optional`, defaults to `None`):
-            The maximum width of the `display_name` parameter.
-            If provided, the `display_name` will be truncated to this length.
-
-    Example:
-    ```python
-    >>> pbar = FileProgressBar("sample.zip", 1024*1024*64)
-    ⏳ sample.zip:   0%|          | 0.00/64.0M [00:00<?, ?B/s]
-
-    >>> pbar.update(1024*1024*32)
-    ⏳ sample.zip:   50%|█████     | 32.0M/64.0M [00:00<?, ?B/s]
-    ```
-    """
-
-    def __init__(
-        self,
-        display_name: str,
-        size: int,
-        position: int = 0,
-        initial: int = 0,
-        colour: Optional[str] = None,
-        max_width: Optional[int] = None,
-    ):
-        if max_width:
-            if len(display_name) > max_width:
-                display_name = f"…{display_name[-1 * max_width :]}"
-            else:
-                display_name = f"{display_name.rjust(max_width + 1)}"
-
-        self.display_name = display_name
-        desc = f"⏳ {display_name}"
-
-        super().__init__(
-            total=size,
-            initial=initial,
-            desc=desc,
-            position=position,
-            colour=colour,
-            dynamic_ncols=True,
-            unit_scale=True,
-            unit_divisor=1024,
-            unit="B",
-        )
-
-    def waiting(self) -> None:
-        self.set_description_str(f"⏳ {self.display_name}")
-
-    def uploading(self) -> None:
-        self.set_description_str(f"⬆️ {self.display_name}")
-        self.refresh()
-
-    def downloading(self) -> None:
-        self.set_description_str(f"⬇️ {self.display_name}")
-        self.refresh()
-
-    def completed(self) -> None:
-        self.set_description_str(f"✅ {self.display_name}")
-        self.colour = "green"
-        self.refresh()
-        self.close()
-
-    def failed(self) -> None:
-        self.set_description_str(f"❌ {self.display_name}")
-        self.colour = "red"
-        self.refresh()
-        self.close()
-
-    def skipped(self, msg) -> None:
-        self.set_description_str(f"➖ {msg}")
-        # self.n = self.total
-        # self.colour = "green"
-        self.refresh()
-        self.close()
-
-
-def create_pbar(
-    display_name: str,
-    size: int,
-    position: int = 0,
-    initial: int = 0,
-) -> FileProgressBar:
-    return FileProgressBar(
-        display_name=display_name,
-        size=size,
-        position=position,
-        initial=initial,
-    )
-
-
-def close_all_pbar(pbar_list: list[FileProgressBar]) -> None:
-    for pbar in pbar_list:
-        pbar.close()
-
-
-# def create_pbar_list(
-#     list_of_files: Union[LocalFile, ModelFile, DatasetFile]
-# ) -> List[FileProgressBar]:
-#     list_of_files_pbars: List[FileProgressBar] = list()
-#
-#     for pos, f in enumerate(list_of_files):
-#         if isinstance(f, ModelFile):
-#             filename = f.fileName
-#         if isinstance(f, DatasetFile):
-#             filename = f.name
-#         if isinstance(f, LocalFile):
-#             filename = f.name
-#
-#         filesize = f.size
-#
-#         pbar = create_pbar(
-#             display_name=filename,
-#             size=filesize,
-#             position=pos,
-#         )
-#         list_of_files_pbars.append(pbar)
-#
-#     return list_of_files_pbars
+from __future__ import annotations
+
+from typing import Optional
+
+from tqdm.auto import tqdm
+
+
+class FileProgressBar(tqdm):
+    """
+    Customized `Tqdm` class for OpenI uploads and downloads.
+    It displays a file progress bar of the operation.
+
+
+    Args:
+        display_name (`str`):
+            The name of the file being uploaded or downloaded.
+        size (`int`):
+            The total size of the file in bytes.
+        position (`int`, `optional`, defaults to `0`):
+            The display position of the progress bar if multiple bars are created.
+        initial (`int`, `optional`, defaults to `0`):
+            The initial progress of the progress bar.
+        colour (`str`, `optional`, defaults to `None`):
+            The colour of the progress bar.
+        max_width (`int`, `optional`, defaults to `None`):
+            The maximum width of the `display_name` parameter.
+            If provided, the `display_name` will be truncated to this length.
+
+    Example:
+    ```python
+    >>> pbar = FileProgressBar("sample.zip", 1024*1024*64)
+    ⏳ sample.zip:   0%|          | 0.00/64.0M [00:00<?, ?B/s]
+
+    >>> pbar.update(1024*1024*32)
+    ⏳ sample.zip:   50%|█████     | 32.0M/64.0M [00:00<?, ?B/s]
+    ```
+    """
+
+    def __init__(
+        self,
+        display_name: str,
+        size: int,
+        position: int = 0,
+        initial: int = 0,
+        colour: Optional[str] = None,
+        max_width: Optional[int] = None,
+    ):
+        if max_width:
+            if len(display_name) > max_width:
+                display_name = f"…{display_name[-1 * max_width :]}"
+            else:
+                display_name = f"{display_name.rjust(max_width + 1)}"
+
+        self.display_name = display_name
+        desc = f"⏳ {display_name}"
+
+        super().__init__(
+            total=size,
+            initial=initial,
+            desc=desc,
+            position=position,
+            colour=colour,
+            dynamic_ncols=True,
+            unit_scale=True,
+            unit_divisor=1024,
+            unit="B",
+        )
+
+    def waiting(self) -> None:
+        self.set_description_str(f"⏳ {self.display_name}")
+
+    def uploading(self) -> None:
+        self.set_description_str(f"⬆️ {self.display_name}")
+        self.refresh()
+
+    def downloading(self) -> None:
+        self.set_description_str(f"⬇️ {self.display_name}")
+        self.refresh()
+
+    def completed(self) -> None:
+        self.set_description_str(f"✅ {self.display_name}")
+        self.colour = "green"
+        self.refresh()
+        self.close()
+
+    def failed(self) -> None:
+        self.set_description_str(f"❌ {self.display_name}")
+        self.colour = "red"
+        self.refresh()
+        self.close()
+
+    def skipped(self, msg) -> None:
+        self.set_description_str(f"➖ {msg}")
+        # self.n = self.total
+        # self.colour = "green"
+        self.refresh()
+        self.close()
+
+
+def create_pbar(
+    display_name: str,
+    size: int,
+    position: int = 0,
+    initial: int = 0,
+) -> FileProgressBar:
+    return FileProgressBar(
+        display_name=display_name,
+        size=size,
+        position=position,
+        initial=initial,
+    )
+
+
+def close_all_pbar(pbar_list: list[FileProgressBar]) -> None:
+    for pbar in pbar_list:
+        pbar.close()
+
+
+# def create_pbar_list(
+#     list_of_files: Union[LocalFile, ModelFile, DatasetFile]
+# ) -> List[FileProgressBar]:
+#     list_of_files_pbars: List[FileProgressBar] = list()
+#
+#     for pos, f in enumerate(list_of_files):
+#         if isinstance(f, ModelFile):
+#             filename = f.fileName
+#         if isinstance(f, DatasetFile):
+#             filename = f.name
+#         if isinstance(f, LocalFile):
+#             filename = f.name
+#
+#         filesize = f.size
+#
+#         pbar = create_pbar(
+#             display_name=filename,
+#             size=filesize,
+#             position=pos,
+#         )
+#         list_of_files_pbars.append(pbar)
+#
+#     return list_of_files_pbars
```

### Comparing `openi-2.0.0b2/src/openi/commands/model.py` & `openi-2.0.0b5/src/openi/commands/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from argparse import (
-    _SubParsersAction,
-    Namespace,
-    SUPPRESS,
-)
-from pathlib import Path
-from typing import Optional
-
-from openi.commands import BaseOpeniCLICommand
-from .._exceptions import LocalPathNotFound
-from ..constants import DEFAULT_SAVE_PATH
-from ..downloader import (
-    download_model,
-    download_model_file,
-)
-from ..log import setup_logger
-from ..uploader import (
-    upload_model,
-    upload_model_file,
-)
-
-logger = setup_logger()
-
-
-class ModelCommands(BaseOpeniCLICommand):
-    @staticmethod
-    def register_subcommand(parser: _SubParsersAction):
-        """
-        model command
-        """
-        parser_model = parser.add_parser(
-            "model",
-            help="{upload,download} 上传/下载启智AI协作平台的模型",
-            description="上传/下载启智AI协作平台的模型",
-            aliases=["m"],
-        )
-        parser_model._action_groups.pop()
-        subparsers_model = parser_model.add_subparsers(
-            title="commands",
-            dest="commands",
-        )
-        subparsers_model.required = True
-
-        # Add subcommand
-        DownloadCommand.register_subcommand(subparsers_model)
-        UploadCommand.register_subcommand(subparsers_model)
-
-
-class BaseModelCommand:
-    def __init__(self, args):
-        self.args = args
-
-
-class DownloadCommand(BaseModelCommand):
-    @staticmethod
-    def register_subcommand(subparsers_model):
-        """
-        download subcommand
-        """
-        download_parser = subparsers_model.add_parser(
-            "download",
-            help="下载模型, openi model download -h 查看更多说明",
-            usage="openi model download REPO_ID MODEL_NAME  [--filename FILENAME] [--save_path PATH] [--force]",
-            description="下载模型或模型文件，需指定仓库路径及模型名称，下载公开模型无需登陆",
-        )
-        download_parser._action_groups.pop()
-
-        """
-        arguments
-        """
-        download_parser_args = download_parser.add_argument_group("arguments")
-        download_parser_args.add_argument(
-            "repo_id",
-            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
-        )
-        download_parser_args.add_argument(
-            "model_name",
-            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
-        )
-
-        """
-        optional arguments
-        """
-        download_parser_optional_args = download_parser.add_argument_group(
-            "optional arguments"
-        )
-        download_parser_optional_args.add_argument(
-            "-f",
-            "--filename",
-            dest="filename",
-            metavar="",
-            required=False,
-            help="选填: 指定下载模型中的某个文件，不填写此参数则会下载模型内所有文件",
-        )
-        download_parser_optional_args.add_argument(
-            "-p",
-            "--save_path",
-            dest="save_path",
-            metavar="",
-            default=DEFAULT_SAVE_PATH,
-            required=False,
-            help="选填: 指定本地的保存目录，默认为当前目录；若下载整个模型，则会在当前目录默认创建 `模型名称` 文件夹",
-        )
-        download_parser_optional_args.add_argument(
-            "--force",
-            dest="force",
-            action="store_true",
-            required=False,
-            help="选填: 添加此参数将删除本地的缓存与同名文件，强行重新下载文件",
-        )
-        download_parser_optional_args.add_argument(
-            "-t",
-            "--token",
-            dest="token",
-            required=False,
-            help=SUPPRESS,
-        )
-        download_parser_optional_args.add_argument(
-            "-e",
-            "--endpoint",
-            dest="endpoint",
-            required=False,
-            help=SUPPRESS,
-        )
-        download_parser.set_defaults(func=lambda args: DownloadCommand(args))
-
-    def __init__(self, args: Namespace) -> None:
-        self.repo_id: str = args.repo_id
-        self.model_name: str = args.model_name
-
-        self.filename: Optional[str] = args.filename
-        self.save_path: Optional[str] = args.save_path
-        self.force: bool = args.force
-
-        self.token: Optional[str] = args.token
-        self.endpoint: Optional[str] = args.endpoint
-
-    def run(self):
-        if self.filename is not None:
-            download_model_file(
-                file=self.filename,
-                repo_id=self.repo_id,
-                model_name=self.model_name,
-                save_path=self.save_path,
-                force=self.force,
-                token=self.token,
-                endpoint=self.endpoint,
-            )
-        else:
-            download_model(
-                repo_id=self.repo_id,
-                model_name=self.model_name,
-                save_path=self.save_path,
-                force=self.force,
-                token=self.token,
-                endpoint=self.endpoint,
-            )
-
-
-class UploadCommand(BaseModelCommand):
-    @staticmethod
-    def register_subcommand(subparsers_model):
-        """
-        upload subcommand
-        """
-        upload_parser = subparsers_model.add_parser(
-            "upload",
-            help="上传模型, openi model upload -h 查看更多说明",
-            usage="openi model upload FILE_PATH REPO_ID MODEL_NAME  [--upload_name FILENAME]",
-            description="上传本地模型或模型文件，需指定本地路径、仓库路径及模型名称",
-        )
-        upload_parser._action_groups.pop()
-
-        """
-        arguments
-        """
-        upload_parser_args = upload_parser.add_argument_group("arguments")
-        upload_parser_args.add_argument(
-            "file_path",
-            help="本地路径，可传入`本地文件`或`本地文件夹`路径；上传`文件夹`时将包含所有文件与子目录文件",
-        )
-        upload_parser_args.add_argument(
-            "repo_id",
-            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
-        )
-        upload_parser_args.add_argument(
-            "model_name",
-            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
-        )
-
-        """
-        optional arguments
-        """
-        upload_parser_optional_args = upload_parser.add_argument_group(
-            "optional arguments"
-        )
-        upload_parser_optional_args.add_argument(
-            "-n",
-            "--upload_name",
-            dest="upload_name",
-            metavar="",
-            required=False,
-            help="选填: 自定义上传文件名，当上传`文件夹`时，本参数失效",
-        )
-        upload_parser_optional_args.add_argument(
-            "-t",
-            "--token",
-            dest="token",
-            required=False,
-            help=SUPPRESS,
-        )
-        upload_parser_optional_args.add_argument(
-            "-e",
-            "--endpoint",
-            dest="endpoint",
-            required=False,
-            help=SUPPRESS,
-        )
-        upload_parser.set_defaults(func=lambda args: UploadCommand(args))
-
-    def __init__(self, args: Namespace) -> None:
-        self.repo_id: str = args.repo_id
-        self.model_name: str = args.model_name
-        self.file_path: Path = Path(args.file_path).absolute()
-
-        self.upload_name: Optional[str] = args.upload_name
-        self.token: Optional[str] = args.token
-        self.endpoint: Optional[str] = args.endpoint
-
-    def run(self):
-        if not self.file_path.exists():
-            raise LocalPathNotFound(self.file_path)
-
-        if self.file_path.is_dir():
-            upload_model(
-                folder=self.file_path,
-                repo_id=self.repo_id,
-                model_name=self.model_name,
-                token=self.token,
-                endpoint=self.endpoint,
-            )
-        else:
-            upload_model_file(
-                file=self.file_path,
-                repo_id=self.repo_id,
-                model_name=self.model_name,
-                upload_name=self.upload_name,
-                token=self.token,
-                endpoint=self.endpoint,
-            )
+from argparse import (
+    _SubParsersAction,
+    Namespace,
+    SUPPRESS,
+)
+from pathlib import Path
+from typing import Optional
+
+from openi.commands import BaseOpeniCLICommand
+from .._exceptions import LocalPathNotFound
+from ..constants import DEFAULT_SAVE_PATH
+from ..downloader import (
+    download_model,
+    download_model_file,
+)
+from ..log import setup_logger
+from ..uploader import (
+    upload_model,
+    upload_model_file,
+)
+
+logger = setup_logger()
+
+
+class ModelCommands(BaseOpeniCLICommand):
+    @staticmethod
+    def register_subcommand(parser: _SubParsersAction):
+        """
+        model command
+        """
+        parser_model = parser.add_parser(
+            "model",
+            help="{upload,download} 上传/下载启智AI协作平台的模型",
+            description="上传/下载启智AI协作平台的模型",
+            aliases=["m"],
+        )
+        parser_model._action_groups.pop()
+        subparsers_model = parser_model.add_subparsers(
+            title="commands",
+            dest="commands",
+        )
+        subparsers_model.required = True
+
+        # Add subcommand
+        DownloadCommand.register_subcommand(subparsers_model)
+        UploadCommand.register_subcommand(subparsers_model)
+
+
+class BaseModelCommand:
+    def __init__(self, args):
+        self.args = args
+
+
+class DownloadCommand(BaseModelCommand):
+    @staticmethod
+    def register_subcommand(subparsers_model):
+        """
+        download subcommand
+        """
+        download_parser = subparsers_model.add_parser(
+            "download",
+            help="下载模型, openi model download -h 查看更多说明",
+            usage="openi model download REPO_ID MODEL_NAME  [--filename FILENAME] [--save_path PATH] [--force]",
+            description="下载模型或模型文件，需指定仓库路径及模型名称，下载公开模型无需登陆",
+        )
+        download_parser._action_groups.pop()
+
+        """
+        arguments
+        """
+        download_parser_args = download_parser.add_argument_group("arguments")
+        download_parser_args.add_argument(
+            "repo_id",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
+        )
+        download_parser_args.add_argument(
+            "model_name",
+            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
+        )
+
+        """
+        optional arguments
+        """
+        download_parser_optional_args = download_parser.add_argument_group(
+            "optional arguments"
+        )
+        download_parser_optional_args.add_argument(
+            "-f",
+            "--filename",
+            dest="filename",
+            metavar="",
+            required=False,
+            help="选填: 指定下载模型中的某个文件，不填写此参数则会下载模型内所有文件",
+        )
+        download_parser_optional_args.add_argument(
+            "-p",
+            "--save_path",
+            dest="save_path",
+            metavar="",
+            default=DEFAULT_SAVE_PATH,
+            required=False,
+            help="选填: 指定本地的保存目录，默认为当前目录；若下载整个模型，则会在当前目录默认创建 `模型名称` 文件夹",
+        )
+        download_parser_optional_args.add_argument(
+            "--force",
+            dest="force",
+            action="store_true",
+            required=False,
+            help="选填: 添加此参数将删除本地的缓存与同名文件，强行重新下载文件",
+        )
+        download_parser_optional_args.add_argument(
+            "-t",
+            "--token",
+            dest="token",
+            required=False,
+            help=SUPPRESS,
+        )
+        download_parser_optional_args.add_argument(
+            "-e",
+            "--endpoint",
+            dest="endpoint",
+            required=False,
+            help=SUPPRESS,
+        )
+        download_parser.set_defaults(func=lambda args: DownloadCommand(args))
+
+    def __init__(self, args: Namespace) -> None:
+        self.repo_id: str = args.repo_id
+        self.model_name: str = args.model_name
+
+        self.filename: Optional[str] = args.filename
+        self.save_path: Optional[str] = args.save_path
+        self.force: bool = args.force
+
+        self.token: Optional[str] = args.token
+        self.endpoint: Optional[str] = args.endpoint
+
+    def run(self):
+        if self.filename is not None:
+            download_model_file(
+                file=self.filename,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                save_path=self.save_path,
+                force=self.force,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+        else:
+            download_model(
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                save_path=self.save_path,
+                force=self.force,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+
+
+class UploadCommand(BaseModelCommand):
+    @staticmethod
+    def register_subcommand(subparsers_model):
+        """
+        upload subcommand
+        """
+        upload_parser = subparsers_model.add_parser(
+            "upload",
+            help="上传模型, openi model upload -h 查看更多说明",
+            usage="openi model upload REPO_ID MODEL_NAME FILE_PATH [--upload_name FILENAME]",
+            description="上传本地模型或模型文件，需指定本地路径、仓库路径及模型名称",
+        )
+        upload_parser._action_groups.pop()
+
+        """
+        arguments
+        """
+        upload_parser_args = upload_parser.add_argument_group("arguments")
+        upload_parser_args.add_argument(
+            "repo_id",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
+        )
+        upload_parser_args.add_argument(
+            "model_name",
+            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
+        )
+        upload_parser_args.add_argument(
+            "file_path",
+            help="本地路径，可传入`本地文件`或`本地文件夹`路径；上传`文件夹`时将包含所有文件与子目录文件",
+        )
+
+        """
+        optional arguments
+        """
+        upload_parser_optional_args = upload_parser.add_argument_group(
+            "optional arguments"
+        )
+        upload_parser_optional_args.add_argument(
+            "-n",
+            "--upload_name",
+            dest="upload_name",
+            metavar="",
+            required=False,
+            help="选填: 自定义上传文件名，当上传`文件夹`时，本参数失效",
+        )
+        upload_parser_optional_args.add_argument(
+            "-t",
+            "--token",
+            dest="token",
+            required=False,
+            help=SUPPRESS,
+        )
+        upload_parser_optional_args.add_argument(
+            "-e",
+            "--endpoint",
+            dest="endpoint",
+            required=False,
+            help=SUPPRESS,
+        )
+        upload_parser.set_defaults(func=lambda args: UploadCommand(args))
+
+    def __init__(self, args: Namespace) -> None:
+        self.repo_id: str = args.repo_id
+        self.model_name: str = args.model_name
+        self.file_path: Path = Path(args.file_path).absolute()
+
+        self.upload_name: Optional[str] = args.upload_name
+        self.token: Optional[str] = args.token
+        self.endpoint: Optional[str] = args.endpoint
+
+    def run(self):
+        if not self.file_path.exists():
+            raise LocalPathNotFound(self.file_path)
+
+        if self.file_path.is_dir():
+            upload_model(
+                folder=self.file_path,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+        else:
+            upload_model_file(
+                file=self.file_path,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                upload_name=self.upload_name,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
```

### Comparing `openi-2.0.0b2/src/openi/commands/openi_cli.py` & `openi-2.0.0b5/src/openi/commands/openi_cli.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from argparse import ArgumentParser, RawDescriptionHelpFormatter
-
-from .dataset import DatasetCommands
-from .model import ModelCommands
-from .user import UserCommands
-from ..constants import CLI_DESCRIPTION, OPENI_LOGO_ASCII
-
-
-def main():
-    parser = ArgumentParser(
-        "openi",
-        formatter_class=RawDescriptionHelpFormatter,
-        description=OPENI_LOGO_ASCII + CLI_DESCRIPTION,
-    )
-    commands_parser = parser.add_subparsers()
-
-    # Register commands
-    UserCommands.register_subcommand(commands_parser)
-    ModelCommands.register_subcommand(commands_parser)
-    DatasetCommands.register_subcommand(commands_parser)
-
-    # Let's go
-    args = parser.parse_args()
-
-    if not hasattr(args, "func"):
-        parser.print_help()
-        exit(1)
-
-    # Run
-    service = args.func(args)
-    service.run()
-
-
-if __name__ == "__main__":
-    main()
+from argparse import ArgumentParser, RawDescriptionHelpFormatter
+
+from .dataset import DatasetCommands
+from .model import ModelCommands
+from .user import UserCommands
+from ..constants import CLI_DESCRIPTION, OPENI_LOGO_ASCII
+
+
+def main():
+    parser = ArgumentParser(
+        "openi",
+        formatter_class=RawDescriptionHelpFormatter,
+        description=OPENI_LOGO_ASCII + CLI_DESCRIPTION,
+    )
+    commands_parser = parser.add_subparsers()
+
+    # Register commands
+    UserCommands.register_subcommand(commands_parser)
+    ModelCommands.register_subcommand(commands_parser)
+    DatasetCommands.register_subcommand(commands_parser)
+
+    # Let's go
+    args = parser.parse_args()
+
+    if not hasattr(args, "func"):
+        parser.print_help()
+        exit(1)
+
+    # Run
+    service = args.func(args)
+    service.run()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `openi-2.0.0b2/src/openi/commands/user.py` & `openi-2.0.0b5/src/openi/commands/user.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from argparse import _SubParsersAction
-
-from openi.commands import BaseOpeniCLICommand
-from .._exceptions import UnauthorizedError
-from .._login import login, logout, whoami
-from ..constants import DEFAULT_BASE_URL
-from ..log import setup_logger
-
-logger = setup_logger()
-
-
-class UserCommands(BaseOpeniCLICommand):
-    @staticmethod
-    def register_subcommand(parser: _SubParsersAction):
-        login_parser = parser.add_parser(
-            "login",
-            usage="openi login [-t token] [-e endpoint] [-h]",
-            help="使用启智社区令牌登录并保存到本地",
-            description="使用启智社区网页端生成的令牌登录: https://openi.pcl.ac.cn/user/settings/applications",
-        )
-        login_parser.add_argument(
-            "-t",
-            "--token",
-            dest="token",
-            metavar="",
-            default=None,
-            type=str,
-            required=False,
-            help="选填: 启智社区令牌，填写此参数将会跳过命令行输入",
-        )
-        login_parser.add_argument(
-            "-e",
-            "--endpoint",
-            dest="endpoint",
-            metavar="",
-            default=DEFAULT_BASE_URL,
-            type=str,
-            required=False,
-            help="选填: 仅内部使用",  # "For internal distribution only",
-        )
-        login_parser.set_defaults(func=lambda args: LoginCommand(args))
-
-        whoami_parser = parser.add_parser(
-            "whoami",
-            usage="openi whoami [-h]",
-            help="查询当前登录用户",
-            description="查询当前登录用户",
-        )
-        whoami_parser.set_defaults(func=lambda args: WhoamiCommand(args))
-
-        logout_parser = parser.add_parser(
-            "logout",
-            usage="openi logout [-h]",
-            help="退出登录并删除本地保存的令牌",
-            description="退出登录并删除本地保存的令牌",
-        )
-        logout_parser.set_defaults(func=lambda args: LogoutCommand(args))
-
-
-class BaseUserCommand:
-    def __init__(self, args):
-        self.args = args
-
-
-class LoginCommand(BaseUserCommand):
-    def run(self):
-        login(token=self.args.token, endpoint=self.args.endpoint)
-
-
-class LogoutCommand(BaseUserCommand):
-    def run(self):
-        logout()
-
-
-class WhoamiCommand(BaseUserCommand):
-    def run(self):
-        try:
-            _ = whoami()
-        except UnauthorizedError:
-            print("Not logged in")
-            exit()
+from argparse import _SubParsersAction
+
+from openi.commands import BaseOpeniCLICommand
+from .._exceptions import UnauthorizedError
+from .._login import login, logout, whoami
+from ..constants import DEFAULT_BASE_URL
+from ..log import setup_logger
+
+logger = setup_logger()
+
+
+class UserCommands(BaseOpeniCLICommand):
+    @staticmethod
+    def register_subcommand(parser: _SubParsersAction):
+        login_parser = parser.add_parser(
+            "login",
+            usage="openi login [-t token] [-e endpoint] [-h]",
+            help="使用启智社区令牌登录并保存到本地",
+            description="使用启智社区网页端生成的令牌登录: https://openi.pcl.ac.cn/user/settings/applications",
+        )
+        login_parser.add_argument(
+            "-t",
+            "--token",
+            dest="token",
+            metavar="",
+            default=None,
+            type=str,
+            required=False,
+            help="选填: 启智社区令牌，填写此参数将会跳过命令行输入",
+        )
+        login_parser.add_argument(
+            "-e",
+            "--endpoint",
+            dest="endpoint",
+            metavar="",
+            default=DEFAULT_BASE_URL,
+            type=str,
+            required=False,
+            help="选填: 仅内部使用",  # "For internal distribution only",
+        )
+        login_parser.set_defaults(func=lambda args: LoginCommand(args))
+
+        whoami_parser = parser.add_parser(
+            "whoami",
+            usage="openi whoami [-h]",
+            help="查询当前登录用户",
+            description="查询当前登录用户",
+        )
+        whoami_parser.set_defaults(func=lambda args: WhoamiCommand(args))
+
+        logout_parser = parser.add_parser(
+            "logout",
+            usage="openi logout [-h]",
+            help="退出登录并删除本地保存的令牌",
+            description="退出登录并删除本地保存的令牌",
+        )
+        logout_parser.set_defaults(func=lambda args: LogoutCommand(args))
+
+
+class BaseUserCommand:
+    def __init__(self, args):
+        self.args = args
+
+
+class LoginCommand(BaseUserCommand):
+    def run(self):
+        login(token=self.args.token, endpoint=self.args.endpoint)
+
+
+class LogoutCommand(BaseUserCommand):
+    def run(self):
+        logout()
+
+
+class WhoamiCommand(BaseUserCommand):
+    def run(self):
+        try:
+            _ = whoami()
+        except UnauthorizedError:
+            print("Not logged in")
+            exit()
```

### Comparing `openi-2.0.0b2/src/openi/constants.py` & `openi-2.0.0b5/src/openi/constants.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from pathlib import Path
-from typing import Literal
-
-OPENI_LOGO_ASCII = """\n
-         ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
-        ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
-        ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
-        ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
-        ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
-         ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝\n
-"""
-CLI_DESCRIPTION = "         OpenI command line tool 启智AI协作平台命令行工具"
-
-REPO_ID_REGEX = r"^[.a-zA-Z0-9_-]+/[.a-zA-Z0-9_-]+$"
-REPO_INFO_REGEX = r"[\w\d]+/[\w\d]+"
-TOKEN_REGEX = r"^[0-9a-z]{40}$"
-
-DEFAULT_BASE_URL = "https://openi.pcl.ac.cn"
-AI_MODEL_VERSION_FILE = "openi_resource.version"
-FILE_CACHE_PREFIX = ".openi-cache-"
-
-HTTP_MAX_RETRIES: int = 3
-HTTP_RETRY_DELAY: float = 1
-
-# file storage
-UPLOAD_TYPE = {"gpu": 0, "npu": 1}
-CHUNK_SIZE = 1024 * 1024 * 64  # 64MB
-MAX_FILE_SIZE = 1024 * 1024 * 1024 * 200  # 200GB
-DOWNLOAD_RATES = 1024 * 1024 * 5
-
-# api
-OPENI_ROOT = Path.home() / ".openi"
-if not OPENI_ROOT.exists():
-    OPENI_ROOT.mkdir(parents=True)
-
-TOKEN_FILE_PATH = Path(OPENI_ROOT) / "token.json"
-
-LOG_FILE_ROOT = Path(OPENI_ROOT) / "logs"
-if not LOG_FILE_ROOT.exists():
-    LOG_FILE_ROOT.mkdir(parents=True)
-
-LOG_FILE = LOG_FILE_ROOT / "openi.log"
-if not LOG_FILE.exists():
-    LOG_FILE.touch()
-
-DEFAULT_SAVE_PATH = Path.cwd()
-if not DEFAULT_SAVE_PATH.exists():
-    DEFAULT_SAVE_PATH.mkdir(parents=True)
-
-UPLOAD_MODE = Literal["dataset", "model"]
-UPLOAD_ENDPOINT = dict(dataset="/attachments", model="/attachments/model")
-UPLOAD_ID_PARAM = dict(dataset="dataset_id", model="modeluuid")
+from pathlib import Path
+from typing import Literal
+
+OPENI_LOGO_ASCII = """\n
+         ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
+        ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
+        ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
+        ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
+        ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
+         ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝\n
+"""
+CLI_DESCRIPTION = "         OpenI command line tool 启智AI协作平台命令行工具"
+
+REPO_ID_REGEX = r"^[.a-zA-Z0-9_-]+/[.a-zA-Z0-9_-]+$"
+REPO_INFO_REGEX = r"[\w\d]+/[\w\d]+"
+TOKEN_REGEX = r"^[0-9a-z]{40}$"
+
+DEFAULT_BASE_URL = "https://openi.pcl.ac.cn"
+AI_MODEL_VERSION_FILE = "openi_resource.version"
+FILE_CACHE_PREFIX = ".openi-cache-"
+
+HTTP_MAX_RETRIES: int = 3
+HTTP_RETRY_DELAY: float = 1
+
+# file storage
+UPLOAD_TYPE = {"gpu": 0, "npu": 1}
+CHUNK_SIZE = 1024 * 1024 * 64  # 64MB
+MAX_FILE_SIZE = 1024 * 1024 * 1024 * 200  # 200GB
+DOWNLOAD_RATES = 1024 * 1024 * 5
+
+# api
+OPENI_ROOT = Path.home() / ".openi"
+if not OPENI_ROOT.exists():
+    OPENI_ROOT.mkdir(parents=True)
+
+TOKEN_FILE_PATH = Path(OPENI_ROOT) / "token.json"
+
+LOG_FILE_ROOT = Path(OPENI_ROOT) / "logs"
+if not LOG_FILE_ROOT.exists():
+    LOG_FILE_ROOT.mkdir(parents=True)
+
+LOG_FILE = LOG_FILE_ROOT / "openi.log"
+if not LOG_FILE.exists():
+    LOG_FILE.touch()
+
+DEFAULT_SAVE_PATH = Path.cwd()
+if not DEFAULT_SAVE_PATH.exists():
+    DEFAULT_SAVE_PATH.mkdir(parents=True)
+
+UPLOAD_MODE = Literal["dataset", "model"]
+UPLOAD_ENDPOINT = dict(dataset="/attachments", model="/attachments/model")
+UPLOAD_ID_PARAM = dict(dataset="dataset_id", model="modeluuid")
```

### Comparing `openi-2.0.0b2/src/openi/downloader.py` & `openi-2.0.0b5/src/openi/downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,361 +1,361 @@
-from pathlib import Path
-from typing import (
-    Literal,
-    Optional,
-    Union,
-)
-
-from ._dataclass import (
-    DatasetFile,
-    ModelFile,
-)
-from ._exceptions import (
-    KeyboardInterruptError,
-    OpenIError,
-    ServerFileNotFoundError,
-    validate_openi_args,
-)
-from ._file import (
-    CacheFile,
-    split_subdir_name,
-)
-from ._tqdm import (
-    create_pbar,
-    FileProgressBar,
-)
-from .api import OpenIApi
-from .constants import (
-    DEFAULT_SAVE_PATH,
-    UPLOAD_TYPE,
-)
-from .log import setup_logger
-
-logger = setup_logger()
-
-
-def single_file_downloader(
-    api: OpenIApi,
-    src_file: Union[DatasetFile, ModelFile],
-    filename: str,
-    filesize: int,
-    filepath: Path,
-    pbar: Optional[FileProgressBar] = None,
-) -> Optional[Union[BaseException, OpenIError]]:
-    """Download a file from the OpenI platform using tqdm.
-
-    Args:
-        api (OpenIApi):
-            The OpenI API instance.
-        src_file (Union[DatasetFile, ModelFile]):
-            The dataset or model file to download.
-        filename (str):
-            The name of the file to download.
-        filesize (int):
-            The size of the file to download.
-        filepath (Path):
-            The path to save the downloaded file.
-        pbar (Optional[FileProgressBar], optional):
-            The progress bar to display. Defaults to None.
-
-    Returns:
-        bool: Whether the download was successful.
-
-    Raises:
-        Exception: If an error occurs during the download.
-    """
-
-    err: Optional[Union[BaseException, OpenIError]] = None
-
-    if pbar is None:
-        pbar: FileProgressBar = create_pbar(
-            display_name=filename,
-            size=filesize,
-        )
-
-    try:
-        pbar.downloading()
-
-        for data in api.download_file_iterator(
-            src_file=src_file,
-            filepath=filepath,
-        ):
-            pbar.update(data)
-
-        if pbar.n == filesize:
-            pbar.completed()
-
-    except KeyboardInterrupt:
-        pbar.failed()
-        err = KeyboardInterruptError(
-            "文件下载未完成，缓存内容已保存; 再次下载到相同路径时，文件将会被断点续传",
-        )
-
-    except Exception as e:
-        pbar.failed()
-        err = e
-
-    finally:
-        pbar.refresh()
-        pbar.close()
-
-    return err
-
-
-@validate_openi_args
-def download_file(
-    file: str,
-    repo_id: str,
-    cluster: Literal["gpu", "npu"] = "npu",
-    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
-    force: bool = False,
-    token: Optional[str] = None,
-    endpoint: Optional[str] = None,
-) -> Optional[Path]:
-    """Download a dataset file
-
-    Args:
-        file (str): The name of the file to download.
-        repo_id (str): The ID of the repository to download from.
-        cluster (Literal["gpu", "npu"], optional): The cluster to download from. Defaults to "npu".
-        save_path (Union[Path, str], optional): The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
-        force (bool, optional): Whether to force download the file. Defaults to False.
-        token (Optional[str], optional): The OpenI API token. Defaults to None.
-        endpoint (Optional[str], optional): The OpenI API endpoint. Defaults to None.
-
-    Returns:
-        Optional[Path]: The path to the downloaded file if successfully downloaded.
-
-    Raises:
-        ServerFileNotFoundError: If the file is not found in the dataset.
-    """
-    api = OpenIApi(token=token, endpoint=endpoint)
-
-    upload_type = UPLOAD_TYPE.get(cluster.lower())
-
-    dataset_file = api.query_dataset_file(
-        repo_id=repo_id,
-        filename=file,
-        upload_type=upload_type,
-    )
-    if not dataset_file:
-        dataset_url = api.get_dataset_url(repo_id=repo_id)
-        raise ServerFileNotFoundError(
-            f"`{file}` 数据集文件不存在 ; 请在网页端查看: {dataset_url}",
-        )
-
-    cache_file: CacheFile = CacheFile(
-        name=dataset_file.name,
-        size=dataset_file.size,
-        save_path=save_path,
-        force=force,
-    )
-
-    err = single_file_downloader(
-        api=api,
-        src_file=dataset_file,
-        filename=cache_file.name,
-        filesize=cache_file.size,
-        filepath=cache_file.cache_path,
-    )
-    if err is not None:
-        raise err
-
-    completed = cache_file.as_completed()
-    if completed:
-        print(f"文件已下载到: {cache_file.file_path}")
-        return cache_file.file_path
-    else:
-        print(f"文件下载出错，请使用 `force=True` 参数重新下载")
-        return None
-
-
-@validate_openi_args
-def download_model_file(
-    file: str,
-    repo_id: str,
-    model_name: str,
-    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
-    force: bool = False,
-    token: Optional[str] = None,
-    endpoint: Optional[str] = None,
-) -> Optional[Path]:
-    """Download a model file.
-
-    Args:
-        file (str):
-            The name of the file to download.
-        repo_id (str):
-            The ID of the repository to download from.
-        model_name (str):
-            The name of the model to download from.
-        save_path (Union[Path, str], optional):
-            The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
-        force (bool, optional):
-            Whether to force download the file. Defaults to False.
-        token (Optional[str], optional):
-            The OpenI API token. Defaults to None.
-        endpoint (Optional[str], optional):
-            The OpenI API endpoint. Defaults to None.
-
-    Returns:
-        Optional[Path]: The path to the downloaded file if successfully downloaded.
-
-    Raises:
-        ServerFileNotFoundError: If the file is not found in the model.
-    """
-    api = OpenIApi(token=token, endpoint=endpoint)
-
-    filename = file.lstrip("/")
-    model_file = api.query_model_file(
-        filename=filename,
-        repo_id=repo_id,
-        model_name=model_name,
-    )
-    if not model_file:
-        model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
-        raise ServerFileNotFoundError(
-            f" `{model_name}` 模型内未找到 `{file}` 文件; 请在网页端查看: {model_url}",
-        )
-
-    if not isinstance(save_path, Path):
-        save_path = Path(save_path)
-
-    if save_path == DEFAULT_SAVE_PATH:
-        save_path = DEFAULT_SAVE_PATH / model_name
-
-    subdir, filename = split_subdir_name(model_file.FileName)
-    save_path = save_path / subdir
-
-    cache_file: CacheFile = CacheFile(
-        name=filename,
-        size=model_file.Size,
-        save_path=save_path,
-        force=force,
-    )
-
-    err = single_file_downloader(
-        api=api,
-        src_file=model_file,
-        filename=cache_file.name,
-        filesize=cache_file.size,
-        filepath=cache_file.cache_path,
-    )
-    if err is not None:
-        raise err
-
-    completed = cache_file.as_completed()
-    if completed:
-        print(f"文件已下载到: {cache_file.file_path}")
-        return cache_file.file_path
-    else:
-        print(f"文件下载出错，请使用 `force=True` 参数重新下载")
-        return None
-
-
-@validate_openi_args
-def download_model(
-    repo_id: str,
-    model_name: str,
-    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
-    force: bool = False,
-    token: Optional[str] = None,
-    endpoint: Optional[str] = None,
-) -> Optional[Path]:
-    """Download an entire model.
-
-    Args:
-        repo_id (str):
-            The ID of the repository to download from.
-        model_name (str):
-            The name of the model to download.
-        save_path (Union[Path, str], optional):
-            The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
-        force (bool, optional):
-            Whether to force download the file. Defaults to False.
-        token (Optional[str], optional):
-            The OpenI API token. Defaults to None.
-        endpoint (Optional[str], optional):
-            The OpenI API endpoint. Defaults to None.
-
-    Returns:
-        Optional[Path]: The path to the downloaded file if successfully downloaded.
-    """
-    api = OpenIApi(token=token, endpoint=endpoint)
-
-    model_file_list = api.list_model_files(
-        repo_id=repo_id,
-        model_name=model_name,
-    )
-    if not model_file_list:
-        model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
-        raise ServerFileNotFoundError(
-            f"模型 `{model_name}` 内无任何文件; 请在网页端查看: {model_url}",
-        )
-
-    if not isinstance(save_path, Path):
-        save_path = Path(save_path)
-
-    if save_path == DEFAULT_SAVE_PATH:
-        save_path = DEFAULT_SAVE_PATH / model_name
-
-    model_file_list.sort(key=lambda x: x.Size)
-    pbar_list = list()
-    cache_file_list = list()
-    for pos, f in enumerate(model_file_list):
-        subdir, filename = split_subdir_name(f.FileName)
-        file_save_path = save_path / subdir
-
-        cache_file: CacheFile = CacheFile(
-            name=filename,
-            size=f.Size,
-            save_path=file_save_path,
-            force=force,
-        )
-        cache_file_list.append(cache_file)
-
-        pbar: FileProgressBar = create_pbar(
-            display_name=cache_file.name,
-            size=cache_file.size,
-            position=pos,
-        )
-        pbar_list.append(pbar)
-
-    completed_count = 0
-    raise_err = None
-    for model_file, cache_file, pbar in zip(
-        model_file_list,
-        cache_file_list,
-        pbar_list,
-    ):
-        if cache_file.file_path.exists():
-            cache_file.cache_path.unlink(missing_ok=True)
-            pbar.update(cache_file.size)
-            pbar.completed()
-            pbar.close()
-            completed_count += 1
-            continue
-
-        err = single_file_downloader(
-            api=api,
-            src_file=model_file,
-            filename=cache_file.name,
-            filesize=cache_file.size,
-            filepath=cache_file.cache_path,
-            pbar=pbar,
-        )
-        if err is not None:
-            raise_err = err
-        if isinstance(err, KeyboardInterruptError):
-            raise err
-        else:
-            completed = cache_file.as_completed(rename_existing=False)
-            if completed:
-                completed_count += 1
-
-    # close_all_pbar(pbar_list)
-    if completed_count == len(model_file_list):
-        print(f"\n模型 `{model_name}` 已成功下载到: {save_path}")
-        return save_path
-    else:
-        print(f"\n{raise_err}; 模型下载出错，请重新下载")
-        return None
+from pathlib import Path
+from typing import (
+    Literal,
+    Optional,
+    Union,
+)
+
+from ._dataclass import (
+    DatasetFile,
+    ModelFile,
+)
+from ._exceptions import (
+    KeyboardInterruptError,
+    OpenIError,
+    ServerFileNotFoundError,
+    validate_openi_args,
+)
+from ._file import (
+    CacheFile,
+    split_subdir_name,
+)
+from ._tqdm import (
+    create_pbar,
+    FileProgressBar,
+)
+from .api import OpenIApi
+from .constants import (
+    DEFAULT_SAVE_PATH,
+    UPLOAD_TYPE,
+)
+from .log import setup_logger
+
+logger = setup_logger()
+
+
+def single_file_downloader(
+    api: OpenIApi,
+    src_file: Union[DatasetFile, ModelFile],
+    filename: str,
+    filesize: int,
+    filepath: Path,
+    pbar: Optional[FileProgressBar] = None,
+) -> Optional[Union[BaseException, OpenIError]]:
+    """Download a file from the OpenI platform using tqdm.
+
+    Args:
+        api (OpenIApi):
+            The OpenI API instance.
+        src_file (Union[DatasetFile, ModelFile]):
+            The dataset or model file to download.
+        filename (str):
+            The name of the file to download.
+        filesize (int):
+            The size of the file to download.
+        filepath (Path):
+            The path to save the downloaded file.
+        pbar (Optional[FileProgressBar], optional):
+            The progress bar to display. Defaults to None.
+
+    Returns:
+        bool: Whether the download was successful.
+
+    Raises:
+        Exception: If an error occurs during the download.
+    """
+
+    err: Optional[Union[BaseException, OpenIError]] = None
+
+    if pbar is None:
+        pbar: FileProgressBar = create_pbar(
+            display_name=filename,
+            size=filesize,
+        )
+
+    try:
+        pbar.downloading()
+
+        for data in api.download_file_iterator(
+            src_file=src_file,
+            filepath=filepath,
+        ):
+            pbar.update(data)
+
+        if pbar.n == filesize:
+            pbar.completed()
+
+    except KeyboardInterrupt:
+        pbar.failed()
+        err = KeyboardInterruptError(
+            "文件下载未完成，缓存内容已保存; 再次下载到相同路径时，文件将会被断点续传",
+        )
+
+    except Exception as e:
+        pbar.failed()
+        err = e
+
+    finally:
+        pbar.refresh()
+        pbar.close()
+
+    return err
+
+
+@validate_openi_args
+def download_file(
+    repo_id: str,
+    file: str,
+    cluster: Literal["gpu", "npu"] = "npu",
+    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
+    force: bool = False,
+    token: Optional[str] = None,
+    endpoint: Optional[str] = None,
+) -> Optional[Path]:
+    """Download a dataset file
+
+    Args:
+        file (str): The name of the file to download.
+        repo_id (str): The ID of the repository to download from.
+        cluster (Literal["gpu", "npu"], optional): The cluster to download from. Defaults to "npu".
+        save_path (Union[Path, str], optional): The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
+        force (bool, optional): Whether to force download the file. Defaults to False.
+        token (Optional[str], optional): The OpenI API token. Defaults to None.
+        endpoint (Optional[str], optional): The OpenI API endpoint. Defaults to None.
+
+    Returns:
+        Optional[Path]: The path to the downloaded file if successfully downloaded.
+
+    Raises:
+        ServerFileNotFoundError: If the file is not found in the dataset.
+    """
+    api = OpenIApi(token=token, endpoint=endpoint)
+
+    upload_type = UPLOAD_TYPE.get(cluster.lower())
+
+    dataset_file = api.query_dataset_file(
+        repo_id=repo_id,
+        filename=file,
+        upload_type=upload_type,
+    )
+    if not dataset_file:
+        dataset_url = api.get_dataset_url(repo_id=repo_id)
+        raise ServerFileNotFoundError(
+            f"`{file}` 数据集文件不存在 ; 请在网页端查看: {dataset_url}",
+        )
+
+    cache_file: CacheFile = CacheFile(
+        name=dataset_file.name,
+        size=dataset_file.size,
+        save_path=save_path,
+        force=force,
+    )
+
+    err = single_file_downloader(
+        api=api,
+        src_file=dataset_file,
+        filename=cache_file.name,
+        filesize=cache_file.size,
+        filepath=cache_file.cache_path,
+    )
+    if err is not None:
+        raise err
+
+    completed = cache_file.as_completed()
+    if completed:
+        print(f"文件已下载到: {cache_file.file_path}")
+        return cache_file.file_path
+    else:
+        print(f"文件下载出错，请使用 `force=True` 参数重新下载")
+        return None
+
+
+@validate_openi_args
+def download_model_file(
+    repo_id: str,
+    model_name: str,
+    file: str,
+    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
+    force: bool = False,
+    token: Optional[str] = None,
+    endpoint: Optional[str] = None,
+) -> Optional[Path]:
+    """Download a model file.
+
+    Args:
+        file (str):
+            The name of the file to download.
+        repo_id (str):
+            The ID of the repository to download from.
+        model_name (str):
+            The name of the model to download from.
+        save_path (Union[Path, str], optional):
+            The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
+        force (bool, optional):
+            Whether to force download the file. Defaults to False.
+        token (Optional[str], optional):
+            The OpenI API token. Defaults to None.
+        endpoint (Optional[str], optional):
+            The OpenI API endpoint. Defaults to None.
+
+    Returns:
+        Optional[Path]: The path to the downloaded file if successfully downloaded.
+
+    Raises:
+        ServerFileNotFoundError: If the file is not found in the model.
+    """
+    api = OpenIApi(token=token, endpoint=endpoint)
+
+    filename = file.lstrip("/")
+    model_file = api.query_model_file(
+        filename=filename,
+        repo_id=repo_id,
+        model_name=model_name,
+    )
+    if not model_file:
+        model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
+        raise ServerFileNotFoundError(
+            f" `{model_name}` 模型内未找到 `{file}` 文件; 请在网页端查看: {model_url}",
+        )
+
+    if not isinstance(save_path, Path):
+        save_path = Path(save_path)
+
+    if save_path == DEFAULT_SAVE_PATH:
+        save_path = DEFAULT_SAVE_PATH / model_name
+
+    subdir, filename = split_subdir_name(model_file.FileName)
+    save_path = save_path / subdir
+
+    cache_file: CacheFile = CacheFile(
+        name=filename,
+        size=model_file.Size,
+        save_path=save_path,
+        force=force,
+    )
+
+    err = single_file_downloader(
+        api=api,
+        src_file=model_file,
+        filename=cache_file.name,
+        filesize=cache_file.size,
+        filepath=cache_file.cache_path,
+    )
+    if err is not None:
+        raise err
+
+    completed = cache_file.as_completed()
+    if completed:
+        print(f"文件已下载到: {cache_file.file_path}")
+        return cache_file.file_path
+    else:
+        print(f"文件下载出错，请使用 `force=True` 参数重新下载")
+        return None
+
+
+@validate_openi_args
+def download_model(
+    repo_id: str,
+    model_name: str,
+    save_path: Union[Path, str] = DEFAULT_SAVE_PATH,
+    force: bool = False,
+    token: Optional[str] = None,
+    endpoint: Optional[str] = None,
+) -> Optional[Path]:
+    """Download an entire model.
+
+    Args:
+        repo_id (str):
+            The ID of the repository to download from.
+        model_name (str):
+            The name of the model to download.
+        save_path (Union[Path, str], optional):
+            The path to save the downloaded file. Defaults to DEFAULT_SAVE_PATH.
+        force (bool, optional):
+            Whether to force download the file. Defaults to False.
+        token (Optional[str], optional):
+            The OpenI API token. Defaults to None.
+        endpoint (Optional[str], optional):
+            The OpenI API endpoint. Defaults to None.
+
+    Returns:
+        Optional[Path]: The path to the downloaded file if successfully downloaded.
+    """
+    api = OpenIApi(token=token, endpoint=endpoint)
+
+    model_file_list = api.list_model_files(
+        repo_id=repo_id,
+        model_name=model_name,
+    )
+    if not model_file_list:
+        model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
+        raise ServerFileNotFoundError(
+            f"模型 `{model_name}` 内无任何文件; 请在网页端查看: {model_url}",
+        )
+
+    if not isinstance(save_path, Path):
+        save_path = Path(save_path)
+
+    if save_path == DEFAULT_SAVE_PATH:
+        save_path = DEFAULT_SAVE_PATH / model_name
+
+    model_file_list.sort(key=lambda x: x.Size)
+    pbar_list = list()
+    cache_file_list = list()
+    for pos, f in enumerate(model_file_list):
+        subdir, filename = split_subdir_name(f.FileName)
+        file_save_path = save_path / subdir
+
+        cache_file: CacheFile = CacheFile(
+            name=filename,
+            size=f.Size,
+            save_path=file_save_path,
+            force=force,
+        )
+        cache_file_list.append(cache_file)
+
+        pbar: FileProgressBar = create_pbar(
+            display_name=f.FileName,
+            size=cache_file.size,
+            position=pos,
+        )
+        pbar_list.append(pbar)
+
+    completed_count = 0
+    raise_err = None
+    for model_file, cache_file, pbar in zip(
+        model_file_list,
+        cache_file_list,
+        pbar_list,
+    ):
+        if cache_file.file_path.exists():
+            cache_file.cache_path.unlink(missing_ok=True)
+            pbar.update(cache_file.size)
+            pbar.completed()
+            pbar.close()
+            completed_count += 1
+            continue
+
+        err = single_file_downloader(
+            api=api,
+            src_file=model_file,
+            filename=cache_file.name,
+            filesize=cache_file.size,
+            filepath=cache_file.cache_path,
+            pbar=pbar,
+        )
+        if err is not None:
+            raise_err = err
+        if isinstance(err, KeyboardInterruptError):
+            raise err
+        else:
+            completed = cache_file.as_completed(rename_existing=False)
+            if completed:
+                completed_count += 1
+
+    # close_all_pbar(pbar_list)
+    if completed_count == len(model_file_list):
+        print(f"\n模型 `{model_name}` 已成功下载到: {save_path}")
+        return save_path
+    else:
+        print(f"\n{raise_err}; 模型下载出错，请重新下载")
+        return None
```

### Comparing `openi-2.0.0b2/src/openi/log.py` & `openi-2.0.0b5/src/openi/log.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import logging
-from logging.handlers import TimedRotatingFileHandler
-
-from .constants import LOG_FILE
-
-
-def setup_logger(log_level: str = "info"):
-    """
-    Output logs to a file with a rotating file handler
-
-    1. `filename='~/.openi/log/openi.log'`: This parameter specifies the filename of the log file. In this case, it's set to `'~/.openi/log/openi.log'`, which means the log file will be located at `~/.openi/log/openi.log`, where `~` represents the user's home directory.
-    2. `when="D"`: This parameter specifies the type of interval for rotating the log files. In this case, it's set to `"D"`, which stands for daily rotation. This means that a new log file will be created every day.
-    3. `interval=1`: This parameter specifies the interval at which log files should be rotated. In this case, it's set to `1`, which means the rotation will occur every `1` unit of the interval type specified in the `when` parameter. Since `when` is set to `"D"`, the rotation will occur every day.
-    4. `backupCount=3`: This parameter specifies the number of backup log files to retain. In this case, it's set to `3`, which means that up to `3` backup log files will be kept in addition to the current log file.
-    Now, let's visualize how the log directory will look like in the future. Assuming today's date is March 1, 2024, and the log files are rotated daily:
-
-    ```
-    ~/.openi/log/
-        ├── openi.log (current log file)
-        ├── openi.log.20240301 (log file for March 1, 2024)
-        ├── openi.log.20240302 (log file for March 2, 2024)
-        ├── openi.log.20240303 (log file for March 3, 2024)
-        ├── openi.log.20240304 (log file for March 4, 2024)
-        └── ...
-    ```
-
-    Each day, a new log file will be created with the date appended to its filename, and the previous day's log file will be renamed accordingly. Up to `3` backup log files will be retained (`openi.log.20240301`, `openi.log.20240302`, and `openi.log.20240303`), and older log files will be deleted once the limit is reached.
-
-    """
-    # Check if logger already exists
-    logger = logging.getLogger(__name__)
-    if logger.handlers:
-        return logger
-
-    LOG_FORMAT = "%(asctime)s [%(levelname)s] %(funcName)s(): %(message)s"
-    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-
-    # Define the TimedRotatingFileHandler with the specified parameters
-    handler = TimedRotatingFileHandler(filename=LOG_FILE, when="D", interval=1, backupCount=3)
-    handler.setFormatter(logging.Formatter(LOG_FORMAT, datefmt=DATE_FORMAT))
-
-    # Create a logger and set its level
-    logger = logging.getLogger(__name__)
-    logger.setLevel(logging.DEBUG)  # Set the logger's level to DEBUG to ensure all levels are captured
-
-    # Add the handler to the logger
-    logger.addHandler(handler)
-
-    # Define custom log levels
-    logging.addLevelName(25, "HTTP")
-    logging.addLevelName(26, "RESPONSE")
-
-    # Define custom logging methods for HTTP and RESPONSE levels
-    def http(self, message, *args, **kws):
-        if self.isEnabledFor(25):
-            self._log(25, message, args, **kws)
-
-    def response(self, message, *args, **kws):
-        if self.isEnabledFor(26):
-            self._log(26, message, args, **kws)
-
-    # Add custom logging methods to the logger
-    logging.Logger.http = http
-    logging.Logger.response = response
-
-    # Set the logger's level based on the input log_level
-    valid_log_levels = ["debug", "info", "warning", "error", "critical"]
-    if log_level.lower() not in valid_log_levels:
-        raise ValueError(f"Invalid log level: {log_level}. Choose from {valid_log_levels}")
-    logger.setLevel(getattr(logging, log_level.upper()))
-
-    return logger
+import logging
+from logging.handlers import TimedRotatingFileHandler
+
+from .constants import LOG_FILE
+
+
+def setup_logger(log_level: str = "info"):
+    """
+    Output logs to a file with a rotating file handler
+
+    1. `filename='~/.openi/log/openi.log'`: This parameter specifies the filename of the log file. In this case, it's set to `'~/.openi/log/openi.log'`, which means the log file will be located at `~/.openi/log/openi.log`, where `~` represents the user's home directory.
+    2. `when="D"`: This parameter specifies the type of interval for rotating the log files. In this case, it's set to `"D"`, which stands for daily rotation. This means that a new log file will be created every day.
+    3. `interval=1`: This parameter specifies the interval at which log files should be rotated. In this case, it's set to `1`, which means the rotation will occur every `1` unit of the interval type specified in the `when` parameter. Since `when` is set to `"D"`, the rotation will occur every day.
+    4. `backupCount=3`: This parameter specifies the number of backup log files to retain. In this case, it's set to `3`, which means that up to `3` backup log files will be kept in addition to the current log file.
+    Now, let's visualize how the log directory will look like in the future. Assuming today's date is March 1, 2024, and the log files are rotated daily:
+
+    ```
+    ~/.openi/log/
+        ├── openi.log (current log file)
+        ├── openi.log.20240301 (log file for March 1, 2024)
+        ├── openi.log.20240302 (log file for March 2, 2024)
+        ├── openi.log.20240303 (log file for March 3, 2024)
+        ├── openi.log.20240304 (log file for March 4, 2024)
+        └── ...
+    ```
+
+    Each day, a new log file will be created with the date appended to its filename, and the previous day's log file will be renamed accordingly. Up to `3` backup log files will be retained (`openi.log.20240301`, `openi.log.20240302`, and `openi.log.20240303`), and older log files will be deleted once the limit is reached.
+
+    """
+    # Check if logger already exists
+    logger = logging.getLogger(__name__)
+    if logger.handlers:
+        return logger
+
+    LOG_FORMAT = "%(asctime)s [%(levelname)s] %(funcName)s(): %(message)s"
+    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
+
+    # Define the TimedRotatingFileHandler with the specified parameters
+    handler = TimedRotatingFileHandler(filename=LOG_FILE, when="D", interval=1, backupCount=3)
+    handler.setFormatter(logging.Formatter(LOG_FORMAT, datefmt=DATE_FORMAT))
+
+    # Create a logger and set its level
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.DEBUG)  # Set the logger's level to DEBUG to ensure all levels are captured
+
+    # Add the handler to the logger
+    logger.addHandler(handler)
+
+    # Define custom log levels
+    logging.addLevelName(25, "HTTP")
+    logging.addLevelName(26, "RESPONSE")
+
+    # Define custom logging methods for HTTP and RESPONSE levels
+    def http(self, message, *args, **kws):
+        if self.isEnabledFor(25):
+            self._log(25, message, args, **kws)
+
+    def response(self, message, *args, **kws):
+        if self.isEnabledFor(26):
+            self._log(26, message, args, **kws)
+
+    # Add custom logging methods to the logger
+    logging.Logger.http = http
+    logging.Logger.response = response
+
+    # Set the logger's level based on the input log_level
+    valid_log_levels = ["debug", "info", "warning", "error", "critical"]
+    if log_level.lower() not in valid_log_levels:
+        raise ValueError(f"Invalid log level: {log_level}. Choose from {valid_log_levels}")
+    logger.setLevel(getattr(logging, log_level.upper()))
+
+    return logger
```

### Comparing `openi-2.0.0b2/src/openi/utils.py` & `openi-2.0.0b5/src/openi/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import json
-import time
-from datetime import datetime
-from typing import Callable, Union
-
-from .log import setup_logger
-
-logger = setup_logger()
-
-
-def caltime(func: Callable) -> Callable:
-    """
-    Decorator to calculate the time of a function.
-
-    Args:
-        func (function): function to be decorated
-
-    Returns:
-        function: wrapper function
-    """
-
-    def wrapper(*args, **kwargs):
-        start_time = time.time()
-        result = func(*args, **kwargs)
-        end_time = time.time()
-        elapsed_time = end_time - start_time
-        print(f"{func.__name__} took {elapsed_time:.4f} seconds to run.")
-        return result
-
-    return wrapper
-
-
-def parse_time(timestamp: Union[str, int]) -> datetime:
-    """
-    Parse timestamp to python datetime
-
-    Args:
-        timestamp (Union[str, int]):
-            unix timestamp data, either in plaintext or integer
-
-    Returns:
-        datetime: python datetime object without timezone information
-    """
-    if isinstance(timestamp, int):
-        return datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc).replace(
-            tzinfo=None
-        )
-    elif isinstance(timestamp, str):
-        return datetime.fromisoformat(timestamp).replace(tzinfo=None)
-    else:
-        raise ValueError("Invalid timestamp format")
-
-
-def jprint(input_dict: dict, indent: int = 4):
-    """Print a dict in json format
-
-    Args:
-        input_dict (dict): dict to print
-        indent (int, optional): indent level. Defaults to 4.
-
-    Example:
-        >>> jprint({"a": 1, "bb": 2, "ccc": 3})
-        {
-            "a": 1,
-            "bb": 2,
-            "ccc": 3
-        }
-    """
-    print(json.dumps(input_dict, indent=4, ensure_ascii=False))
-
-
-def aprint(input_dict: dict, colon=False):
-    """
-    print a dict in aligned format
-
-    :param input_dict: dict to be printed
-    :param colon: aligned colon or not
-    :return: None
-
-    e.g.
-    >>> aprint({"a": 1, "bb": 2, "ccc": 3})
-    a:   1
-    bb:  2
-    ccc: 3
-    """
-    max_key_length = max(len(key) for key in input_dict.keys())
-    for key, value in input_dict.items():
-        if not colon:
-            key += ":"
-            formatted_key = f"{key:{max_key_length + 1}}"
-            print(f"{formatted_key} {value}")
-        else:
-            formatted_key = f"{key:{max_key_length}}"
-            print(f"{formatted_key}: {value}")
-
-
-def convert_bytes(byte):
-    """
-    Convert bytes to human-readable units (bytes, KB, MB, GB, TB).
-    """
-    units = ["bytes", "KB", "MB", "GB", "TB"]
-    index = 0
-
-    while byte >= 1024 and index < len(units) - 1:
-        byte /= 1024.0
-        index += 1
-
-    return f"{byte:.2f} {units[index]}"
+import json
+import time
+from datetime import datetime
+from typing import Callable, Union
+
+from .log import setup_logger
+
+logger = setup_logger()
+
+
+def caltime(func: Callable) -> Callable:
+    """
+    Decorator to calculate the time of a function.
+
+    Args:
+        func (function): function to be decorated
+
+    Returns:
+        function: wrapper function
+    """
+
+    def wrapper(*args, **kwargs):
+        start_time = time.time()
+        result = func(*args, **kwargs)
+        end_time = time.time()
+        elapsed_time = end_time - start_time
+        print(f"{func.__name__} took {elapsed_time:.4f} seconds to run.")
+        return result
+
+    return wrapper
+
+
+def parse_time(timestamp: Union[str, int]) -> datetime:
+    """
+    Parse timestamp to python datetime
+
+    Args:
+        timestamp (Union[str, int]):
+            unix timestamp data, either in plaintext or integer
+
+    Returns:
+        datetime: python datetime object without timezone information
+    """
+    if isinstance(timestamp, int):
+        return datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc).replace(
+            tzinfo=None
+        )
+    elif isinstance(timestamp, str):
+        return datetime.fromisoformat(timestamp).replace(tzinfo=None)
+    else:
+        raise ValueError("Invalid timestamp format")
+
+
+def jprint(input_dict: dict, indent: int = 4):
+    """Print a dict in json format
+
+    Args:
+        input_dict (dict): dict to print
+        indent (int, optional): indent level. Defaults to 4.
+
+    Example:
+        >>> jprint({"a": 1, "bb": 2, "ccc": 3})
+        {
+            "a": 1,
+            "bb": 2,
+            "ccc": 3
+        }
+    """
+    print(json.dumps(input_dict, indent=4, ensure_ascii=False))
+
+
+def aprint(input_dict: dict, colon=False):
+    """
+    print a dict in aligned format
+
+    :param input_dict: dict to be printed
+    :param colon: aligned colon or not
+    :return: None
+
+    e.g.
+    >>> aprint({"a": 1, "bb": 2, "ccc": 3})
+    a:   1
+    bb:  2
+    ccc: 3
+    """
+    max_key_length = max(len(key) for key in input_dict.keys())
+    for key, value in input_dict.items():
+        if not colon:
+            key += ":"
+            formatted_key = f"{key:{max_key_length + 1}}"
+            print(f"{formatted_key} {value}")
+        else:
+            formatted_key = f"{key:{max_key_length}}"
+            print(f"{formatted_key}: {value}")
+
+
+def convert_bytes(byte):
+    """
+    Convert bytes to human-readable units (bytes, KB, MB, GB, TB).
+    """
+    units = ["bytes", "KB", "MB", "GB", "TB"]
+    index = 0
+
+    while byte >= 1024 and index < len(units) - 1:
+        byte /= 1024.0
+        index += 1
+
+    return f"{byte:.2f} {units[index]}"
```

### Comparing `openi-2.0.0b2/src/openi.egg-info/PKG-INFO` & `openi-2.0.0b5/src/openi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-Metadata-Version: 2.1
-Name: openi
-Version: 2.0.0b2
-Summary: A package for openi pypi
-Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
-Author: chenzh05
-Author-email: chenzh.ds@outlook.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: deprecated
-Requires-Dist: pwinput
-
-# OpenI
-
-> PYPI package for 启智 AI 协作平台。
-
-## 安装
-
-_适配 python3.8 及以上版本_
-
-```bash
-pip install openi
-```
-
-## 功能介绍
-
-- 支持进行本地上传与下载文件到启智社区
-- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
-- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
-
-## 使用示例
-- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
-
-```python
-# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
-from openi import download_file
-path = download_file(
-    file="MnistDataset_mindspore.zip",
-    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
-)
-```
-
-- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
-
-```bash
-openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
-```
-
-- 执行结果，显示下载进度条与本地保存路径
-```bash
-✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
-文件已下载到: D:\MnistDataset_mindspore.zip
-```
-
-- 更多使用指南请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+Metadata-Version: 2.1
+Name: openi
+Version: 2.0.0b5
+Summary: A package for openi pypi
+Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
+Author: chenzh05
+Author-email: chenzh.ds@outlook.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# OpenI
+
+> PYPI package for 启智 AI 协作平台。
+
+## 安装
+
+_适配 python3.8 及以上版本_
+
+```bash
+pip install openi
+```
+
+## 功能介绍
+
+- 支持进行本地上传与下载文件到启智社区
+- 支持代码调用函数，可在本地Python脚本或notebook使用；支持终端命令行，方便在服务器上使用。
+- 具体请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+
+## 使用示例
+- `python` 代码中下载 [MNIST示例数据集](https://openi.pcl.ac.cn/OpenIOSSG/OpenI_Cloudbrain_Example/datasets) 为例：
+
+```python
+# 可复制到 python 文件中直接运行，函数的返回值为下载文件的本地保存路径
+from openi import download_file
+path = download_file(
+    file="MnistDataset_mindspore.zip",
+    repo_id="OpenIOSSG/OpenI_Cloudbrain_Example",
+)
+```
+
+- 上述代码调用对应的终端命令（可直接复制到终端命令行中运行）
+
+```bash
+openi dataset download MnistDataset_mindspore.zip OpenIOSSG/OpenI_Cloudbrain_Example
+```
+
+- 执行结果，显示下载进度条与本地保存路径
+```bash
+✅ MnistDataset_mindspore.zip: 100%|██████████████████████████████████████████████| 10.3M/10.3M [00:00<00:00, 24.7MB/s]
+文件已下载到: D:\MnistDataset_mindspore.zip
+```
+
+- 更多使用指南请参考 [帮助文档](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
```

### Comparing `openi-2.0.0b2/src/openi.egg-info/SOURCES.txt` & `openi-2.0.0b5/src/openi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 src/openi.egg-info/top_level.txt
 src/openi/commands/__init__.py
 src/openi/commands/dataset.py
 src/openi/commands/model.py
 src/openi/commands/openi_cli.py
 src/openi/commands/user.py
 test/test.py
-test/test_openi.py
+test/test_client.py
+test/test_tqdm.py
```

