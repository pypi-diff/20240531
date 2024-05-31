# Comparing `tmp/flaskz-1.8.0.tar.gz` & `tmp/flaskz-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.8.0.tar", last modified: Fri May 31 16:00:18 2024, max compression
+gzip compressed data, was "flaskz-1.8.0rc1.tar", last modified: Tue May 21 03:02:48 2024, max compression
```

## Comparing `flaskz-1.8.0.tar` & `flaskz-1.8.0rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:18.029032 flaskz-1.8.0/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.8.0/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)    10462 2024-05-31 16:00:18.028230 flaskz-1.8.0/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     9865 2024-05-31 03:19:49.000000 flaskz-1.8.0/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.8.0/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      775 2024-05-31 16:00:18.030333 flaskz-1.8.0/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.954853 flaskz-1.8.0/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.962045 flaskz-1.8.0/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       22 2024-05-28 08:14:04.000000 flaskz-1.8.0/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.972311 flaskz-1.8.0/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.8.0/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.8.0/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.979077 flaskz-1.8.0/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.8.0/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.8.0/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    22535 2024-05-27 03:11:11.000000 flaskz-1.8.0/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.981582 flaskz-1.8.0/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.8.0/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:17.992669 flaskz-1.8.0/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.8.0/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    31603 2024-05-13 10:53:54.000000 flaskz-1.8.0/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.8.0/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.8.0/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    13695 2024-05-27 11:59:47.000000 flaskz-1.8.0/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.8.0/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:18.000190 flaskz-1.8.0/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    29975 2024-05-07 04:04:59.000000 flaskz-1.8.0/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.8.0/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.8.0/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:18.024261 flaskz-1.8.0/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.8.0/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.8.0/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.8.0/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.8.0/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    15445 2024-05-28 11:25:47.000000 flaskz-1.8.0/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.8.0/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.8.0/src/flaskz/utils/_magic.py
--rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.8.0/src/flaskz/utils/_private.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     9439 2024-05-14 07:19:13.000000 flaskz-1.8.0/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.8.0/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.8.0/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.8.0/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-31 16:00:18.026021 flaskz-1.8.0/src/flaskz.egg-info/
--rw-r--r--   0 taozh      (501) staff       (20)    10462 2024-05-31 16:00:17.000000 flaskz-1.8.0/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-05-31 16:00:17.000000 flaskz-1.8.0/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-05-31 16:00:17.000000 flaskz-1.8.0/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-05-31 16:00:17.000000 flaskz-1.8.0/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-05-31 16:00:17.000000 flaskz-1.8.0/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.624008 flaskz-1.8.0rc1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.8.0rc1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)    10311 2024-05-21 03:02:48.623748 flaskz-1.8.0rc1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9710 2024-05-21 03:01:29.000000 flaskz-1.8.0rc1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.8.0rc1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-05-21 03:02:48.624797 flaskz-1.8.0rc1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.579816 flaskz-1.8.0rc1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.586160 flaskz-1.8.0rc1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-05-21 03:01:38.000000 flaskz-1.8.0rc1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.592264 flaskz-1.8.0rc1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.8.0rc1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.8.0rc1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.596192 flaskz-1.8.0rc1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.8.0rc1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.8.0rc1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    22535 2024-05-14 10:17:54.000000 flaskz-1.8.0rc1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.598135 flaskz-1.8.0rc1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.8.0rc1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.605485 flaskz-1.8.0rc1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.8.0rc1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    31603 2024-05-13 10:53:54.000000 flaskz-1.8.0rc1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.8.0rc1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.8.0rc1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13701 2024-05-15 09:49:31.000000 flaskz-1.8.0rc1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.8.0rc1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.609709 flaskz-1.8.0rc1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29975 2024-05-07 04:04:59.000000 flaskz-1.8.0rc1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.8.0rc1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.8.0rc1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.621692 flaskz-1.8.0rc1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.8.0rc1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.8.0rc1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.8.0rc1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.8.0rc1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.8.0rc1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.8.0rc1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.8.0rc1/src/flaskz/utils/_magic.py
+-rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.8.0rc1/src/flaskz/utils/_private.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9439 2024-05-14 07:19:13.000000 flaskz-1.8.0rc1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.8.0rc1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.8.0rc1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.8.0rc1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.622648 flaskz-1.8.0rc1/src/flaskz.egg-info/
+-rw-r--r--   0 taozh      (501) staff       (20)    10311 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.8.0/LICENSE` & `flaskz-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/PKG-INFO` & `flaskz-1.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.8.0
+Version: 1.8.0rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,23 +30,22 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.8.0** `2024/06/01`
+- **1.8.0rc1** `2024/05/21`
     - [A] 扩展`flaskz.rest`路由生成模块
         - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
         - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
         - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
         - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
-    - [A] 添加`flaskz.utils.request`函数(替代`flaskz.utils.api_request`函数)
-    - [A] 添加`flaskz.utils.json_dumps`函数以序列化对象为JSON字符串
-    - [F] 修复`flaskz.ext.ssh.SSH`中`_pre_commands_run`的未赋值问题
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
 - **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
     - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 - **1.7.2** `2024/02/01`
```

### Comparing `flaskz-1.8.0/README.md` & `flaskz-1.8.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.8.0** `2024/06/01`
+- **1.8.0rc1** `2024/05/21`
     - [A] 扩展`flaskz.rest`路由生成模块
         - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
         - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
         - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
         - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
-    - [A] 添加`flaskz.utils.request`函数(替代`flaskz.utils.api_request`函数)
-    - [A] 添加`flaskz.utils.json_dumps`函数以序列化对象为JSON字符串
-    - [F] 修复`flaskz.ext.ssh.SSH`中`_pre_commands_run`的未赋值问题
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
 - **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
     - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 - **1.7.2** `2024/02/01`
```

### Comparing `flaskz-1.8.0/setup.cfg` & `flaskz-1.8.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.8.0
+version = 1.8.0rc1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.8.0/src/flaskz/auth/_jws.py` & `flaskz-1.8.0rc1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/ext/cypher.py` & `flaskz-1.8.0rc1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/ext/ssh.py` & `flaskz-1.8.0rc1/src/flaskz/ext/ssh.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/log/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/models/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/models/_base.py` & `flaskz-1.8.0rc1/src/flaskz/models/_base.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/models/_model.py` & `flaskz-1.8.0rc1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/models/_query_util.py` & `flaskz-1.8.0rc1/src/flaskz/models/_query_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/models/_util.py` & `flaskz-1.8.0rc1/src/flaskz/models/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         query_from_g_cache(User, 1, to_dict=False)  # id=1(ins) # cache 'instance'
         query_from_g_cache(User, False)  # return 'all' users
 
     :param model_class: the model class to query and cache, ex)User
     :param by_value: the value to query, if False return all items ex) 1/'admin'
     :param attr: the attribute of the data to return, ex)'username'/'email'
     :param to_dict: cache data as dict or not, ex) True/False
-    :param mapping_key: the key used to create data mapping, if None, use the primary filed of the model_class, ex)'id'
+    :param mapping_key: the key used to create data mapping, if None, use the primary filed of the model_class, ex)'username'
     :param cache_key: the key used to cache data, if None use 'flaskz_' + class_name + '_model_cached_items'
     :return:
     """
     if by_value is None:
         return None
     class_name = model_class.get_class_name()
     if cache_key is None:
```

### Comparing `flaskz-1.8.0/src/flaskz/res_status_codes.py` & `flaskz-1.8.0rc1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/rest/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/rest/_mgmt.py` & `flaskz-1.8.0rc1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/rest/_util.py` & `flaskz-1.8.0rc1/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_app.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_cache.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_cls.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_common.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import json
 from collections.abc import Mapping
-from datetime import datetime, date, time
-from decimal import Decimal
 
 __all__ = [
     'filter_list', 'find_list', 'merge_list', 'each_list', 'get_list',
     'pop_dict_keys', 'del_dict_keys', 'get_deep', 'set_deep', 'merge_dict', 'get_ins_mapping', 'get_dict_mapping', 'get_dict_value_by_type',
-    'get_wrap_str', 'is_str', 'str_replace', 'str_contains_any',
     'is_list', 'is_dict', 'slice_str',
-    'json_dumps',
+    'get_wrap_str', 'is_str', 'str_replace', 'str_contains_any',
     'bulk_append_child',
     'parse_version'
 ]
 
 
 # -------------------------------------------list-------------------------------------------
 def filter_list(items, func=None, with_index=False, not_none=False):
@@ -505,59 +501,10 @@
         if v.isdigit():
             versions.append(int(v))
         else:
             versions.append(v)
     return versions
 
 
-# -------------------------------------------json-------------------------------------------
-def json_dumps(obj, **kwargs):
-    """
-    Serialize obj to a JSON formatted string, with support for additional data types.
-    The function extends the default JSON serialization capabilities of Python's json module by
-    providing custom serialization for types that are not natively supported,
-    such as datetime, date, time, Decimal, bytes, bytearray, set, and custom objects.
-
-    .. versionadded:: 1.8.0
-
-    Example:
-        json_dumps({
-            'str': 'example',
-            'integer': 1,
-            'float': 3.14,
-            'boolean': True,
-            'none': None,
-            'list': [1, 2, 3],
-            'dict': {'key': 'value'},
-            'tuple': (1, 2, 3),
-
-            'set': {1, 2, 3},
-            'datetime': datetime.now(),
-            'date': date.today(),
-            'time': datetime.now().time(),
-            'decimal': Decimal('10.5'),
-            'bytes': b'byte data',
-            'bytearray': bytearray(b'bytearray data')
-        }, indent=4)
-    :param obj:
-    :return:
-    """
-    if 'default' not in kwargs:
-        kwargs['default'] = _json_serializer
-    return json.dumps(obj, **kwargs)
-
-
-def _json_serializer(obj):
-    if isinstance(obj, (datetime, date, time)):
-        return obj.isoformat()
-    if isinstance(obj, (Decimal, bytes, bytearray)):
-        return str(obj)
-    if isinstance(obj, set):
-        return list(obj)
-    if hasattr(obj, '__dict__'):
-        return obj.__dict__
-    raise TypeError(f"Object of type '{obj.__class__.__name__}' is not JSON serializable")
-
-
 # -------------------------------------------private-------------------------------------------
 def _is_not_none(item, *args, **kwargs):
     return item is not None
```

### Comparing `flaskz-1.8.0/src/flaskz/utils/_func.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_magic.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_private.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_private.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_request_api.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_request_api.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_request_args.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_response.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz/utils/_timer.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.8.0/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.8.0rc1/src/flaskz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.8.0
+Version: 1.8.0rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,23 +30,22 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.8.0** `2024/06/01`
+- **1.8.0rc1** `2024/05/21`
     - [A] 扩展`flaskz.rest`路由生成模块
         - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
         - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
         - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
         - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
-    - [A] 添加`flaskz.utils.request`函数(替代`flaskz.utils.api_request`函数)
-    - [A] 添加`flaskz.utils.json_dumps`函数以序列化对象为JSON字符串
-    - [F] 修复`flaskz.ext.ssh.SSH`中`_pre_commands_run`的未赋值问题
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
 - **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
     - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 - **1.7.2** `2024/02/01`
```

### Comparing `flaskz-1.8.0/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.8.0rc1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

