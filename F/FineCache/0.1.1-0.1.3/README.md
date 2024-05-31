# Comparing `tmp/finecache-0.1.1.tar.gz` & `tmp/finecache-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finecache-0.1.1.tar", last modified: Wed May 29 18:45:48 2024, max compression
+gzip compressed data, was "finecache-0.1.3.tar", last modified: Fri May 31 03:39:13 2024, max compression
```

## Comparing `finecache-0.1.1.tar` & `finecache-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/FineCache/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/CachedCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/FineCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/FineCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 18:45:44.000000 finecache-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-29 18:45:48.585533 finecache-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-29 18:45:44.000000 finecache-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:45:48.585533 finecache-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 18:45:44.000000 finecache-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-29 18:45:44.000000 finecache-0.1.1/tests/test_cachelib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:13.689788 finecache-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:13.689788 finecache-0.1.3/FineCache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-31 03:39:08.000000 finecache-0.1.3/FineCache/CachedCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-05-31 03:39:08.000000 finecache-0.1.3/FineCache/FineCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 03:39:08.000000 finecache-0.1.3/FineCache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-31 03:39:08.000000 finecache-0.1.3/FineCache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:13.689788 finecache-0.1.3/FineCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-31 03:39:13.000000 finecache-0.1.3/FineCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 03:39:13.000000 finecache-0.1.3/FineCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:39:13.000000 finecache-0.1.3/FineCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 03:39:13.000000 finecache-0.1.3/FineCache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 03:39:08.000000 finecache-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-31 03:39:13.689788 finecache-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-31 03:39:08.000000 finecache-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-31 03:39:08.000000 finecache-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:39:13.689788 finecache-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-31 03:39:08.000000 finecache-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:13.689788 finecache-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-31 03:39:08.000000 finecache-0.1.3/tests/test_cachelib.py
```

### Comparing `finecache-0.1.1/FineCache/CachedCall.py` & `finecache-0.1.3/FineCache/CachedCall.py`

 * *Files identical despite different names*

### Comparing `finecache-0.1.1/FineCache/FineCache.py` & `finecache-0.1.3/FineCache/FineCache.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,29 +65,31 @@
             @wraps(func)
             def _get_result(*args, **kwargs):
                 call = CachedCall(func, args, kwargs)
                 filename = config.get_filename(call, args_hash=args_hash, kwargs_hash=kwargs_hash)
                 cache_filename = os.path.join(self.base_path, filename)
                 if os.path.exists(cache_filename) and os.path.isfile(cache_filename):
                     # 从缓存文件获取结果
+                    logger.warning(f'Acquire cached {func.__qualname__} result from: {cache_filename}')
                     return agent.get(call, cache_filename)
                 else:
                     # 将运行结果缓存到缓存文件中
                     result = call.result
                     agent.set(call, result, cache_filename)
                     return result
 
             return _get_result
 
         return _cache
 
     @contextmanager
-    def record_context(self, inc_dir: IncrementDir, comment: str, tracking_files: List[str] = None,
+    def record_context(self, inc_dir: IncrementDir, comment: str = "", tracking_files: List[str] = None,
                        save_output: bool = True):
         """
+        :param inc_dir:
         :param comment: 注释
         :param tracking_files: 保存的追踪文件
         :param save_output: 是否保存输出到单独文件
         """
 
         class Tee:
             def __init__(self, stdout, file):
@@ -109,29 +111,36 @@
             log_filename = os.path.join(record_dir, 'console.log')
             log_fp = open(log_filename, 'a', encoding='utf-8')
             old_stdout = sys.stdout
             sys.stdout = Tee(old_stdout, log_fp)
 
         # 将追踪的文件复制到相应位置
         tracking_files = [] if tracking_files is None else tracking_files
-        patterns = [re.compile(p) for p in tracking_files]
+        patterns = {re.compile(p): p for p in tracking_files}
         tracking_records = defaultdict(list)
         for root, dirs, files in os.walk(self.project_root):
+            if os.path.samefile(root, increment_dir.base_path):
+                dirs[:] = []  # 清空dirs列表以跳过此目录及子目录
+                continue
             for file in files:
-                # 构建完整的文件路径
-                full_path = os.path.join(root, file)
-                relative_path = os.path.relpath(full_path, self.project_root)
+
                 for pattern in patterns:
                     # 检查是否匹配正则表达式
                     if pattern.search(file):
-                        # 记录匹配文件的位置
-                        tracking_records[pattern].append(relative_path)
+                        # 构建完整的文件路径
+                        full_path = os.path.join(root, file)
+                        relative_path = os.path.relpath(full_path, self.project_root)
+                        # 构造目标文件路径
+                        dest_file_path = os.path.join(record_dir, relative_path)
+                        os.makedirs(os.path.dirname(dest_file_path), exist_ok=True)
                         # 复制文件
-                        shutil.copy(full_path, record_dir)
-                        logger.debug(f'Recording {full_path} to {record_dir}')
+                        shutil.copy(full_path, dest_file_path)
+                        logger.debug(f'Recording {full_path} to {dest_file_path}')
+                        # 记录匹配文件的位置
+                        tracking_records[patterns[pattern]].append(full_path)
 
         # 记录改动及信息
         patch_location = os.path.join(record_dir, 'current_changes.patch')
         with open(patch_location, 'w', encoding='utf-8') as patch_file:
             patch_file.write(self.patch_content)
         information = {
             'commit': self.commit_hash,
```

### Comparing `finecache-0.1.1/FineCache/utils.py` & `finecache-0.1.3/FineCache/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         :param base_path: 基础目录路径。
         :param dir_prefix: 目录名的前缀。
         """
         self.base_path = Path(base_path)
         self.dir_prefix = dir_prefix
 
     @property
-    def latest_number(self) -> (Optional[int], Optional[str]):
+    def latest_dir(self) -> (Optional[int], Optional[str]):
         """
         返回基础路径下按数字递增命名的最新目录的数字部分。
 
         :return: 最新目录的数字部分及最新目录名，如果找不到则返回None, None。
         """
         dirs = [d for d in os.listdir(self.base_path) if
                 os.path.isdir(os.path.join(self.base_path, d)) and d.startswith(self.dir_prefix)]
@@ -104,15 +104,15 @@
     def create_new_dir(self, dir_suffix: str = "") -> str:
         """
         创建一个新的目录，目录名基于当前最大数字加一，包含自定义的前缀和后缀。
 
         :param dir_suffix: 目录名的后缀，默认为空。
         :return: 新创建的目录的完整路径。
         """
-        latest_num, _ = self.latest_number
+        latest_num, _ = self.latest_dir
         new_num = latest_num + 1 if latest_num is not None else 1
         if len(dir_suffix) != 0:
             new_dir_name = f"{self.dir_prefix}{new_num}-{dir_suffix}"
         else:
             new_dir_name = f"{self.dir_prefix}{new_num}"
         new_dir_path = self.base_path / new_dir_name
         new_dir_path.mkdir(exist_ok=True)
```

### Comparing `finecache-0.1.1/FineCache.egg-info/PKG-INFO` & `finecache-0.1.3/FineCache.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: FineCache
-Version: 0.1.1
-Summary: 科研项目缓存中间结果和实验变动记录工具
+Version: 0.1.3
+Summary: 科研项目中缓存和实验变动记录工具
 Home-page: https://github.com/ciaranchen/FineCache
 Author: Ciaran Chen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author-email: ciaranchen <ciaranchen@qq.com>
+License: MIT
+Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FineCache
 
-科研项目缓存中间结果和实验变动记录工具。主要提供两个装饰器：
+科研项目中缓存和实验变动记录工具。主要提供两个装饰器：
 
 - `FineCache.cache` : 缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 - `FineCache.record`: 记录实验进行时的代码改动、配置文件及运行信息。
 
 ## 安装
 
 ```shell
```

### Comparing `finecache-0.1.1/LICENSE` & `finecache-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finecache-0.1.1/PKG-INFO` & `finecache-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: FineCache
-Version: 0.1.1
-Summary: 科研项目缓存中间结果和实验变动记录工具
+Version: 0.1.3
+Summary: 科研项目中缓存和实验变动记录工具
 Home-page: https://github.com/ciaranchen/FineCache
 Author: Ciaran Chen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author-email: ciaranchen <ciaranchen@qq.com>
+License: MIT
+Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FineCache
 
-科研项目缓存中间结果和实验变动记录工具。主要提供两个装饰器：
+科研项目中缓存和实验变动记录工具。主要提供两个装饰器：
 
 - `FineCache.cache` : 缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 - `FineCache.record`: 记录实验进行时的代码改动、配置文件及运行信息。
 
 ## 安装
 
 ```shell
```

### Comparing `finecache-0.1.1/README.md` & `finecache-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # FineCache
 
-科研项目缓存中间结果和实验变动记录工具。主要提供两个装饰器：
+科研项目中缓存和实验变动记录工具。主要提供两个装饰器：
 
 - `FineCache.cache` : 缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 - `FineCache.record`: 记录实验进行时的代码改动、配置文件及运行信息。
 
 ## 安装
 
 ```shell
```

### Comparing `finecache-0.1.1/setup.py` & `finecache-0.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="FineCache",
-  version="0.1.1",
+  version="0.1.3",
   author="Ciaran Chen",
   author_email="ciaranchen@qq.com",
-  description="科研项目缓存中间结果和实验变动记录工具",
+  description="科研项目中缓存和实验变动记录工具 ",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ciaranchen/FineCache",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `finecache-0.1.1/tests/test_cachelib.py` & `finecache-0.1.3/tests/test_cachelib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
 import os
 import pickle
 import unittest
+from pathlib import Path
 from shutil import rmtree
 
 from FineCache import FineCache, IncrementDir
 
 
 def func(a1: int, a2: int, k1="v1", k2="v2"):
     """normal run function"""
@@ -14,49 +16,57 @@
     # print(a1, a2, k1, k2)
     # print(a1, "+ 1 =", a1 + 1)
     return a3, a4, kr1, kr2
 
 
 class TestFineCache(unittest.TestCase):
     def setUp(self) -> None:
-        self.pc = FineCache('.p_cache')
+        self.inc = IncrementDir('.cache', dir_prefix='test')
+        self.fc = FineCache('.cache')
 
     def tearDown(self):
         super().tearDown()
         # Clear folders...
-        if os.path.exists('.p_cache'):
-            rmtree('.p_cache')
+        if os.path.exists('.cache'):
+            rmtree('.cache')
+        if os.path.exists('temp.yml'):
+            os.remove('temp.yml')
 
     def test_wrapped(self):
-        wrapped = self.pc.cache()(func)
+        wrapped = self.fc.cache()(func)
         self.assertEqual(wrapped.__qualname__, func.__qualname__)
         self.assertEqual(wrapped.__doc__, func.__doc__)
 
+        wrapped = self.fc.record()(func)
+        self.assertEqual(wrapped.__qualname__, func.__qualname__)
+        self.assertEqual(wrapped.__doc__, func.__doc__)
+
+    # Test for Cache
     def test_pickle_cache(self):
         args = (3,)
         kwargs = {'a2': 4, 'k1': "v3"}
-        wrapped = self.pc.cache()(func)
+        wrapped = self.fc.cache()(func)
         self.assertEqual(func(*args, **kwargs), wrapped(*args, **kwargs))
         self.assertEqual(func(*args, **kwargs), wrapped(*args, **kwargs))
 
     def test_unpicklable_args(self):
         def _test_unpicklable(a1, a2, k1, k2):
             # print(a1, a2, k1, k2)
             return a1, k1
 
         args = (3, lambda x: x + 2)
         kwargs = {'k1': 4, 'k2': lambda x: x + 3}
         _test_unpicklable(*args, **kwargs)
 
-        wrapped = self.pc.cache()(_test_unpicklable)
+        wrapped = self.fc.cache()(_test_unpicklable)
         wrapped(*args, **kwargs)
 
-        filepaths = [file for file in os.listdir('.p_cache') if file.startswith(_test_unpicklable.__name__)]
+        filepaths = [file for file in os.listdir('.cache') if file.startswith(_test_unpicklable.__name__)]
         self.assertEqual(len(filepaths), 1)
-        with open(os.path.join('.p_cache', filepaths[0]), 'rb') as fp:
+        with open(os.path.join('.cache', filepaths[0]), 'rb') as fp:
             data = pickle.load(fp)
         self.assertEqual(data['func'], _test_unpicklable.__qualname__)
 
         self.assertEqual(len(data['args']), 2)
         self.assertEqual(data['args'][0], 3)
         self.assertIsNone(data['args'][1])
 
@@ -66,66 +76,87 @@
     def test_unpicklable_different_action(self):
         def _test_lambda(a1, func1):
             return func1(a1)
 
         args = (3, lambda x: x)
         res0 = _test_lambda(*args)
         self.assertEqual(res0, 3)
-        wrapped = self.pc.cache()(_test_lambda)
+        wrapped = self.fc.cache()(_test_lambda)
         res1 = wrapped(*args)
         self.assertEqual(res1, 3)
 
         args2 = (3, lambda x: x + 1)
         # 此处不会产生相同结果
         res2 = wrapped(*args2)
         self.assertEqual(res2, 4)
 
     def test_not_picklable_result(self):
         def _test_unpicklable_result():
             return lambda x: 0
 
-        wrapped = self.pc.cache()(_test_unpicklable_result)
+        wrapped = self.fc.cache()(_test_unpicklable_result)
         try:
             wrapped()
         except pickle.PickleError as e:
             pass
 
     def test_self_defined_hash(self):
         def test_func(a1, a2):
             return a1, a2
 
-        wrapped = self.pc.cache(args_hash=[lambda a1: 'x', lambda a2: 'y'])(test_func)
+        wrapped = self.fc.cache(args_hash=[lambda a1: 'x', lambda a2: 'y'])(test_func)
         wrapped('a1', 'a2')
-        self.assertTrue(os.path.exists(os.path.join('.p_cache', "test_func('x','y';).pk")))
+        self.assertTrue(os.path.exists(os.path.join('.cache', "test_func('x','y';).pk")))
 
+    # Test for Record
 
-class TestHistoryCache(unittest.TestCase):
-    def tearDown(self):
-        super().tearDown()
-        # Clear folders...
-        if os.path.exists('.h_cache'):
-            rmtree('.h_cache')
-
-    def setUp(self) -> None:
-        self.inc = IncrementDir('.h_cache', dir_prefix='test')
-        self.hc = FineCache('.h_cache', increment_dir=self.inc)
-
-    def test_wrapped(self):
-        wrapped = self.hc.record()(func)
-        self.assertEqual(wrapped.__qualname__, func.__qualname__)
-        self.assertEqual(wrapped.__doc__, func.__doc__)
+    def test_record_context(self):
+        Path('./temp.yml').touch()
 
-    def test_output_duplicate(self):
-        @self.hc.record()
         def output():
             print('123456789')
 
-        output()
-        _, latest_dir = self.inc.latest_number
-        filename = os.path.join('.h_cache', latest_dir, 'console.log')
+        with self.fc.record_context(self.inc, comment="test_record_context", tracking_files=[r'.*\.yml']) as info:
+            output()
+            info['output'] = 'abcdefg'
+
+        _, latest_dir = self.inc.latest_dir
+        self.assertTrue('test_record_context' in latest_dir)
+        filename = os.path.join('.cache', latest_dir, 'console.log')
+        self.assertTrue(os.path.exists(filename))
         with open(filename) as fp:
             content = fp.read()
         self.assertTrue('123456789' in content)
+        filename = os.path.join('.cache', latest_dir, 'information.json')
+        self.assertTrue(os.path.exists(filename))
+        with open(filename) as fp:
+            content = fp.read()
+        self.assertTrue('abcdefg' in content)
+        self.assertTrue(os.path.exists(os.path.join('.cache', latest_dir, 'tests', 'temp.yml')))
+
+    def test_record(self):
+        Path('./temp.yml').touch()
+
+        @self.fc.record(self.inc, comment="test_record", tracking_files=[r'.*\.yml'])
+        def output():
+            pass
+
+        for _ in range(3):
+            output()
+        num, latest_dir = self.inc.latest_dir
+        self.assertEqual(num, 3)
+        self.assertEqual(len(os.listdir('.cache')), 3)
+        self.assertTrue('test_record' in latest_dir)
+
+        filename = os.path.join('.cache', latest_dir, 'information.json')
+        self.assertTrue(os.path.exists(filename))
+        with open(filename) as fp:
+            data = json.load(fp)
+        self.assertEqual(data['record_function'], output.__qualname__)
+
+        # 测试是否循环复制了tracking_files
+        self.assertFalse(os.path.exists(os.path.join('.cache', latest_dir, 'tests', '.cache')))
+        self.assertTrue(os.path.exists(os.path.join('.cache', latest_dir, 'tests', 'temp.yml')))
 
 
 if __name__ == '__main__':
     unittest.main()
```

