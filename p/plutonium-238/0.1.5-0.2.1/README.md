# Comparing `tmp/plutonium-238-0.1.5.tar.gz` & `tmp/plutonium-238-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutonium-238-0.1.5.tar", last modified: Mon May  8 16:08:38 2023, max compression
+gzip compressed data, was "plutonium-238-0.2.1.tar", last modified: Fri May 31 02:08:16 2024, max compression
```

## Comparing `plutonium-238-0.1.5.tar` & `plutonium-238-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.105626 plutonium-238-0.1.5/
--rw-r--r--   0 john       (501) staff       (20)      868 2023-05-08 16:08:38.105420 plutonium-238-0.1.5/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.1.5/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.101536 plutonium-238-0.1.5/plutonium/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.1.5/plutonium/__init__.py
--rw-r--r--   0 john       (501) staff       (20)    10433 2023-05-08 16:07:57.000000 plutonium-238-0.1.5/plutonium/cli.py
--rw-r--r--   0 john       (501) staff       (20)     4391 2023-05-08 15:48:01.000000 plutonium-238-0.1.5/plutonium/config.py
--rw-r--r--   0 john       (501) staff       (20)    12000 2023-05-08 15:59:36.000000 plutonium-238-0.1.5/plutonium/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.104886 plutonium-238-0.1.5/plutonium_238.egg-info/
--rw-r--r--   0 john       (501) staff       (20)      868 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      320 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       50 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)        9 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       10 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-05-08 16:08:38.105676 plutonium-238-0.1.5/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     1205 2023-05-08 16:08:29.000000 plutonium-238-0.1.5/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.147294 plutonium-238-0.2.1/
+-rw-r--r--   0 john       (501) staff       (20)      868 2024-05-31 02:08:16.146921 plutonium-238-0.2.1/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.2.1/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.142185 plutonium-238-0.2.1/plutonium/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.2.1/plutonium/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     6753 2024-05-31 02:00:51.000000 plutonium-238-0.2.1/plutonium/cli.py
+-rw-r--r--   0 john       (501) staff       (20)     3190 2024-05-31 01:52:11.000000 plutonium-238-0.2.1/plutonium/config.py
+-rw-r--r--   0 john       (501) staff       (20)     7802 2024-05-31 01:52:11.000000 plutonium-238-0.2.1/plutonium/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.145886 plutonium-238-0.2.1/plutonium_238.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)      868 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      320 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       50 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)        9 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       10 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2024-05-31 02:08:16.147378 plutonium-238-0.2.1/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1205 2024-05-31 02:01:45.000000 plutonium-238-0.2.1/setup.py
```

### Comparing `plutonium-238-0.1.5/PKG-INFO` & `plutonium-238-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.1.5
+Version: 0.2.1
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.1.5/plutonium/utils.py` & `plutonium-238-0.2.1/plutonium/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,89 @@
 import subprocess
 import logging
 import os
 import sys
+import zipfile
 import shutil
 import requests
 import plutonium.config as config
 from uuid import uuid4
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter(config.LOG_FORMAT)
 file_handler = logging.FileHandler(config.LOG_FILENAME)
 file_handler.setFormatter(formatter)
 console_handler = logging.StreamHandler()
 console_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 logger.addHandler(console_handler)
 logger.setLevel(config.LOG_LEVEL)
-# 忽略目录
-def filter_ignored_dirs(dirs):
-    [
-        dirs.remove(d)
-        for d in list(dirs)
-        if d.lower() in config.ignore_directories or d.startswith(".")
-    ]
-    return dirs
-# 查找python依赖文件
-def find_python_reqfiles(path):
-    result = []
-    req_files = [
-        "requirements.txt",
-        "Pipfile",
-        "poetry.lock",
-        "Pipfile.lock",
-        "conda.yml",
-    ]
-    for root, dirs, files in os.walk(path):
-        filter_ignored_dirs(dirs)
-        for name in req_files:
-            if name in files:
-                result.append(os.path.join(root, name))
-    return result
-# 判断是否是二进制字符
-def is_binary_string(content):
-    textchars = bytearray({7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7F})
-    return bool(content.translate(None, textchars))
-# 判断是否是二进制文件
-def is_exe(src):
-    if os.path.isfile(src):
-        try:
-            return is_binary_string(open(src, "rb").read(1024))
-        except Exception:
-            return False
-    return False
-# 查找指定后缀文件
-def find_files(src, src_ext_name, quick=False, filter=True):
-    result = []
-    for root, dirs, files in os.walk(src):
-        if filter:
-            filter_ignored_dirs(dirs)
-        for file in files:
-            if file == src_ext_name or file.endswith(src_ext_name):
-                result.append(os.path.join(root, file))
-                if quick:
-                    return result
-    return result
 # 获取路径
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.dirname(__file__)
     return os.path.join(base_path, relative_path)
 # 执行命令
-def exec_tool(args, cwd=None, stdout=subprocess.PIPE):
+def exec_tool(args, log_file, timeout=config.CMD_TIME_OUT, cwd=None, ):
+    result = {
+        'status': False,
+        'message': '',
+        'data': ''
+    }
     try:
         logger.debug('Executing "{}"'.format(" ".join(args)))
+
         if os.environ.get("FETCH_LICENSE"):
             logger.debug(
                 "License information would be fetched from the registry. This would take several minutes ..."
             )
-        cp = subprocess.run(
-            args,
-            stdout=stdout,
-            stderr=subprocess.STDOUT,
-            cwd=cwd,
-            env=os.environ.copy(),
-            check=False,
-            shell=False,
-            encoding="utf-8",
-        )
-        logger.debug(cp.stdout)
-        return cp.stdout
+        with open(log_file, 'a') as f:
+            cp = subprocess.run(
+                args,
+                stdout=f,
+                stderr=subprocess.STDOUT,
+                cwd=cwd,
+                env=os.environ.copy(),
+                check=False,
+                shell=False,
+                encoding="utf-8",
+                timeout=timeout
+            )
+            logger.debug(cp.stdout)
+            result['status'] = True
+    except subprocess.TimeoutExpired as timeout_error:
+        logger.error(timeout)
+        result['message'] = '执行超时-{}'.format(timeout_error)
     except Exception as e:
         logger.exception(e)
+        result['message'] = str(e)
         return str(e)
-# 检测项目开发语言
-# go/python/java/nodejs
-def detect_project_language(src_dir):
-    if find_python_reqfiles(src_dir):
-        return "python"
-    if find_files(src_dir, "pom.xml", quick=True) or find_files(
-            src_dir, ".gradle", quick=True
-    ):
-        return "java"
-    if (
-            find_files(src_dir, "package.json", quick=True)
-            or find_files(src_dir, "yarn.lock", quick=True)
-            or find_files(src_dir, "rush.json", quick=True)
-    ):
-        return "nodejs"
-    if find_files(src_dir, "go.sum", quick=True) or find_files(
-            src_dir, "Gopkg.lock", quick=True
-    ):
-        return "go"
+    print(result)
+    return result
 
-    return "other"
+def zip_folder(file_dir):
+    target_file = file_dir+'/../'+file_dir.strip('/').split('/')[-1]+'.zip'
+    print(target_file)
+    with zipfile.ZipFile(target_file, 'w', zipfile.ZIP_DEFLATED) as zipf:
+        for root, dirs, files in os.walk(file_dir):
+            for file in files:
+                file_path = os.path.join(root, file)
+                zipf.write(file_path, os.path.relpath(file_path, file_dir))
+    
 
 # 通过cdxgen来生成sbom
-def sca_by_cdxgen(language, bom_file, src_dir=".", deep=False):
+def sca_by_cdxgen(bom_file, src_dir=".", timeout=config.CMD_TIME_OUT):
     result = {
         'status': False,
-        'data': None,
-        'message': ''
+        'data': {
+            'cmd': '',
+            'result_file': bom_file
+        },
+        'message': '',
     }
     cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
     if not shutil.which(cdxgen_cmd):
         local_bin = resource_path(
             os.path.join(
                 "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
             )
@@ -135,121 +94,38 @@
         try:
             cdxgen_cmd = local_bin
             # Set the plugins directory as an environment variable
             os.environ["CDXGEN_PLUGINS_DIR"] = resource_path("local_bin")
         except Exception as e:
             result['message'] = e
             return result
-    if language:
-        sca_args = [cdxgen_cmd, "-r", "-t", language, "-o", bom_file]
-    else:
-        sca_args = [cdxgen_cmd, "-o", bom_file]
-    if deep:
-        sca_args.append("--deep")
+    sca_args = [cdxgen_cmd, "-o", bom_file]
     sca_args.append(src_dir)
-    print(sca_args)
-    exec_tool(sca_args, )
-    result['status'] = True
-    result['data'] = ' '.join(sca_args)
-    return result
-
-# 获取sca分析
-def get_sca_info(src_dir, language=None, sca_tool=True, package_cmd=True, package_file=True,docker_file=True, deep=False):
-    result = {
-        'language': '',
-        # 通过sca工具分析
-        'sca_tool': [],
-        # 通过命令读取的结果
-        'package_cmd': [],
-        # 通过包文件读取
-        'package_file': [],
-        'docker_file': [],
-    }
-    if not language:
-        language = detect_project_language(src_dir)
-    result['language'] = language
-
-    # 1.通过cdxgen来生成
-    cdxgen_sbom_file = config.SCA_TOOLS['cdxgen']['sbom_file'].format(uuid4().hex)
-    cdxgen_result = sca_by_cdxgen(language, cdxgen_sbom_file, src_dir)
-    cdxgen_item = {
-        'tool': 'cdxgen',
-        'cmd': cdxgen_result['data'],
-        'result': cdxgen_sbom_file if cdxgen_result['status'] else cdxgen_result['message']
-    }
-    result['sca_tool'].append(cdxgen_item)
-    
-    # 2.通过包列举命令获取包信息
-    if package_cmd:
-        for i in config.LANG_PACKAGE_CMD[language]:
-            # 若不同语言继续有细分，可在此进行各个语言的处理
-            if language == 'python':
-                try:
-                    item = {
-                        'cmd': i,
-                        'result': None
-                    }
-                    # 虚拟环境
-                    if os.path.exists(src_dir + '/venv'):
-                        res = exec_tool((src_dir + '/venv/bin/' + i).split(), cwd=src_dir)
-                        item['result'] = res
-                    else:
-                        res = exec_tool(i.split(), cwd=src_dir)
-                        item['result'] = res
-                    result['package_cmd'].append(item)
-                except Exception as e:
-                    logger.error(e)
-            else:
-                try:
-                    item = {
-                        'cmd': i,
-                        'result': None
-                    }
-                    res = exec_tool(i.split(), cwd=src_dir)
-                    item['result'] = res
-                    result['package_cmd'].append(item)
-                except Exception as e:
-                    logger.error(e)
-    # 3.读取依赖文件
-    if package_file:
-        for i in config.LANG_PACKAGE_FILE[language]:
-            if os.path.exists(src_dir + '/' + i):
-                logger.info('存在包文件-{}'.format(src_dir + '/' + i))
-                result['package_file'].append(src_dir + '/' + i)
-    # 4.读取dockerfile
-    if docker_file:
-        for i in config.DOCKER_FILE_LIST:
-            if os.path.exists(src_dir + '/' + i):
-                logger.info('存在dockerfile文件-{}'.format(src_dir + '/' + i))
-                result['docker_file'].append(src_dir + '/' + i)
+    logger.info(sca_args)
+    exec_status = exec_tool(sca_args, config.LOG_FILENAME, timeout )
+    result['status'] = exec_status['status']
+    result['message'] = exec_status['message']
+    result['data']['cmd'] = ' '.join(sca_args)
     return result
 
-# 基础工具检测
-def base_tool_check():
-    pass
-
-# 依赖工具安装
-def base_tool_install():
-    pass
-
 
 # 服务端检测
 class VoyagerDetect():
-    def __init__(self, token=None, url=None, username=None, password=None):
+    def __init__(self, token=None, url=None, username=None, password=None, api=None):
         self.api_url = url
         self.api_token = token
         self.api_username = username
         self.api_password = password
         self.req = requests.Session()
 
     # 1.token生成，token有效期较长，失效后再进行重新生成
     def get_new_token(self):
         try:
             self.req.headers = {}
-            res = self.req.post(self.api_url + 'api/member/get-auth-token/',
+            res = self.req.post(self.api_url + config.VOYAGER_GET_TOKEN_API,
                                 data={'username': self.api_username, 'password': self.api_password})
             token = res.json()['token']
             headers = {
                 # 注意Token后有空格
                 'Authorization': 'Token ' + token
             }
             self.req.headers = headers
@@ -261,15 +137,15 @@
     def check_token_valid(self):
         headers = {
             # 注意Token后有空格
             'Authorization': 'Token ' + self.api_token
         }
         self.req.headers = headers
         try:
-            res = self.req.get(self.api_url + 'api/member/check-token/', )
+            res = self.req.get(self.api_url + config.VOYAGER_CHECK_TOKEN_API, )
             if res.status_code == 200 and res.json()['success']:
                 return True
         except Exception as e:
             logger.error(e)
         return False
 
     # 登录认证
@@ -303,48 +179,49 @@
                 login_status['message'] = '无法生成访问token，账号密码可能错误'
         else:
             login_status['message'] = '请提供API账号以及密码信息'
         logger.info(login_status['message'])
         return login_status
 
     # sca分析
-    def sca_analysis(self, language, src_dir=".", sca_tool=True, package_cmd=True, package_file=True, docker_file=True, deep=False):
-        result = get_sca_info(language=language, src_dir=src_dir, sca_tool=sca_tool,
-                              package_cmd=package_cmd, package_file=package_file,docker_file=docker_file, deep=deep)
-        return result
+    def sca_analysis(self, src_dir=".", tool='cdxgen'):
+        if tool == 'cdxgen':
+            result_file = config.DATA_DIR+'/{}_{}.json'.format(tool, uuid4().hex)
+            return sca_by_cdxgen(result_file, src_dir)
 
-    # 0.4旧版本的流水线卡点的扫描
-    def scan(self, data, files):
+        return None
+
+    # upload
+    def upload(self, data, files):
         login_status = self.login()
         if login_status['status']:
             if files:
-                response = self.req.post(self.api_url + 'api/scan/detect/', data=data, files=files)
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_API, data=data, files=files)
             else:
-                response = self.req.post(self.api_url + 'api/scan/detect/', data=data, files=[ ('files', ('', None, )),])
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_API, data=data,
+                                         files=[('files', ('', None,)), ])
             return response.json()
         else:
-            return login_status
-
-
+            return login_status['message']
     # 获取扫描结果或报告
     def get_scan_result(self, task_id):
         login_status = self.login()
         if login_status['status']:
-            response = self.req.get(self.api_url + 'api/scan/scan-log/?task_id={}'.format(task_id),)
+            response = self.req.get(self.api_url + VOYAGER_BASE_API+'?task_id={}'.format(task_id),)
             return response.json()
         else:
             return login_status
     
     # 新版的与服务端交互
-    def base_scan(self, data, files):
+    def scan(self, data, files):
         login_status = self.login()
         if login_status['status']:
             if files:
-                response = self.req.post(self.api_url + config.VOYAGER_BASE_SCAN_API, data=data, files=files)
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_API, data=data, files=files)
             else:
-                response = self.req.post(self.api_url + config.VOYAGER_BASE_SCAN_API, data=data, files=[('files', ('', None,)), ])
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_API, data=data, files=[('files', ('', None,)), ])
             return response.json()
         else:
             return login_status['message']
```

### Comparing `plutonium-238-0.1.5/plutonium_238.egg-info/PKG-INFO` & `plutonium-238-0.2.1/plutonium_238.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.1.5
+Version: 0.2.1
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.1.5/setup.py` & `plutonium-238-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plutonium-238",
-    version="0.1.5",
+    version="0.2.1",
     author="tom",
     author_email="tom@google.com",
     description="SCA Agent, Copyright@Plutonium",
     entry_points={
         "console_scripts": ["plutonium=plutonium.cli:main",]
     },
     license="MIT",
```

