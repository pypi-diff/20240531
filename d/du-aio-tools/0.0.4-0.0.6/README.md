# Comparing `tmp/du_aio_tools-0.0.4.tar.gz` & `tmp/du_aio_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "du_aio_tools-0.0.4.tar", last modified: Tue May 21 06:38:02 2024, max compression
+gzip compressed data, was "du_aio_tools-0.0.6.tar", last modified: Fri May 31 03:02:15 2024, max compression
```

## Comparing `du_aio_tools-0.0.4.tar` & `du_aio_tools-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.994034 du_aio_tools-0.0.4/
--rw-rw-rw-   0        0        0      515 2024-05-21 06:38:02.993537 du_aio_tools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       95 2024-03-06 06:35:10.000000 du_aio_tools-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.982610 du_aio_tools-0.0.4/du_aio_tools/
--rw-rw-rw-   0        0        0      856 2024-03-07 07:26:59.000000 du_aio_tools-0.0.4/du_aio_tools/Iterator_xml.py
--rw-rw-rw-   0        0        0        0 2022-12-16 08:31:49.000000 du_aio_tools-0.0.4/du_aio_tools/__init__.py
--rw-rw-rw-   0        0        0     2789 2024-05-21 06:37:14.000000 du_aio_tools-0.0.4/du_aio_tools/base_conn.py
--rw-rw-rw-   0        0        0     8691 2024-05-21 06:37:14.000000 du_aio_tools-0.0.4/du_aio_tools/base_spider.py
--rw-rw-rw-   0        0        0      201 2024-02-26 07:42:04.000000 du_aio_tools-0.0.4/du_aio_tools/exceptions.py
--rw-rw-rw-   0        0        0     2235 2024-02-19 09:14:48.000000 du_aio_tools-0.0.4/du_aio_tools/rsa.py
--rw-rw-rw-   0        0        0      528 2024-02-26 07:30:47.000000 du_aio_tools-0.0.4/du_aio_tools/schemas.py
--rw-rw-rw-   0        0        0     1501 2024-03-06 04:13:04.000000 du_aio_tools-0.0.4/du_aio_tools/time.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.988570 du_aio_tools-0.0.4/du_aio_tools.egg-info/
--rw-rw-rw-   0        0        0      515 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 06:38:02.994531 du_aio_tools-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1697 2024-05-21 06:34:41.000000 du_aio_tools-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.992544 du_aio_tools-0.0.4/tests/
--rw-rw-rw-   0        0        0      114 2024-02-18 02:18:14.000000 du_aio_tools-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2108 2024-02-26 07:08:32.000000 du_aio_tools-0.0.4/tests/conn.py
--rw-rw-rw-   0        0        0      937 2024-02-20 00:57:30.000000 du_aio_tools-0.0.4/tests/t1.py
--rw-rw-rw-   0        0        0      543 2024-02-26 07:13:24.000000 du_aio_tools-0.0.4/tests/t_html.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:02:15.945782 du_aio_tools-0.0.6/
+-rw-rw-rw-   0        0        0      515 2024-05-31 03:02:15.944789 du_aio_tools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-03-06 06:35:10.000000 du_aio_tools-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:02:15.932868 du_aio_tools-0.0.6/du_aio_tools/
+-rw-rw-rw-   0        0        0      856 2024-03-07 07:26:59.000000 du_aio_tools-0.0.6/du_aio_tools/Iterator_xml.py
+-rw-rw-rw-   0        0        0        0 2022-12-16 08:31:49.000000 du_aio_tools-0.0.6/du_aio_tools/__init__.py
+-rw-rw-rw-   0        0        0     2945 2024-05-31 02:45:06.000000 du_aio_tools-0.0.6/du_aio_tools/base_conn.py
+-rw-rw-rw-   0        0        0     8691 2024-05-21 06:37:14.000000 du_aio_tools-0.0.6/du_aio_tools/base_spider.py
+-rw-rw-rw-   0        0        0      201 2024-02-26 07:42:04.000000 du_aio_tools-0.0.6/du_aio_tools/exceptions.py
+-rw-rw-rw-   0        0        0     2235 2024-02-19 09:14:48.000000 du_aio_tools-0.0.6/du_aio_tools/rsa.py
+-rw-rw-rw-   0        0        0      528 2024-02-26 07:30:47.000000 du_aio_tools-0.0.6/du_aio_tools/schemas.py
+-rw-rw-rw-   0        0        0     1501 2024-03-06 04:13:04.000000 du_aio_tools-0.0.6/du_aio_tools/time.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:02:15.938332 du_aio_tools-0.0.6/du_aio_tools.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-05-31 03:02:15.000000 du_aio_tools-0.0.6/du_aio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-05-31 03:02:15.000000 du_aio_tools-0.0.6/du_aio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:02:15.000000 du_aio_tools-0.0.6/du_aio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-31 03:02:15.000000 du_aio_tools-0.0.6/du_aio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-31 03:02:15.000000 du_aio_tools-0.0.6/du_aio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:02:15.945782 du_aio_tools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2024-05-31 03:02:08.000000 du_aio_tools-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:02:15.943795 du_aio_tools-0.0.6/tests/
+-rw-rw-rw-   0        0        0      114 2024-02-18 02:18:14.000000 du_aio_tools-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     2108 2024-02-26 07:08:32.000000 du_aio_tools-0.0.6/tests/conn.py
+-rw-rw-rw-   0        0        0      937 2024-02-20 00:57:30.000000 du_aio_tools-0.0.6/tests/t1.py
+-rw-rw-rw-   0        0        0      543 2024-02-26 07:13:24.000000 du_aio_tools-0.0.6/tests/t_html.py
```

### Comparing `du_aio_tools-0.0.4/PKG-INFO` & `du_aio_tools-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: du_aio_tools
-Version: 0.0.4
+Version: 0.0.6
 Summary: async tools
 Author: DYZ
 Author-email: duyuchau@gmail.com
 Maintainer: DYZ
 Maintainer-email: duyuchau@gmail.com
 License: MIT
 Platform: all
```

### Comparing `du_aio_tools-0.0.4/du_aio_tools/Iterator_xml.py` & `du_aio_tools-0.0.6/du_aio_tools/Iterator_xml.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/du_aio_tools/base_conn.py` & `du_aio_tools-0.0.6/du_aio_tools/base_conn.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # @author: Dyz
 # @file: base_conn.py
 # @software: PyCharm
 import functools
 import warnings
 from typing import Optional
 
-from tortoise.models import ModelMeta
-from tortoise import BaseDBAsyncClient, Model, fields, Tortoise
+from loguru import logger
+from tortoise import BaseDBAsyncClient, models, fields, Tortoise
 
 
 async def init_db(tortoise_orm, create: bool = False):
     """
     >>> {
         "connections": {
             "conn": {
@@ -42,15 +42,15 @@
 
 
 async def close_db():
     """关闭数据库连接"""
     await Tortoise.close_connections()
 
 
-def load_db(tortoise_orm, create=False):
+def load_db(tortoise_orm, create: bool = False):
     """
     tortoise_orm: 数据库链接配置
     create: 创建表
     """
 
     def _load_db(func):
         """加载数据库"""
@@ -65,31 +65,36 @@
             return result
 
         return wrap
 
     return _load_db
 
 
-class MyModel(Model):
+class BaseModel(models.Model):
+    """基础模型类，包含创建时间和更新时间"""
+    id = fields.IntField(pk=True)
+    created_at = fields.DatetimeField(auto_now_add=True)
+    updated_at = fields.DatetimeField(auto_now=True)
+
+    class Meta:
+        abstract = True  # 标记为抽象类，不直接创建表
 
     @classmethod
     async def truncate_model(cls, using_db: Optional[BaseDBAsyncClient] = None):
         """截断表"""
         db = using_db or cls._choose_db(True)
         data = await cls.all().limit(1)
         if data:
-            return await db.execute_query('TRUNCATE TABLE {}'.format(cls._meta.db_table))
-        warnings.warn('TABLE {} 存在数据!'.format(cls._meta.db_table))
+            logger.info(f'截断表[{cls._meta.db_table}]')
+            return await db.execute_query(f'TRUNCATE TABLE {cls._meta.db_table}')
+        logger.warning(f'TABLE {cls._meta.db_table} 不存在数据!')
 
     @classmethod
     async def copy_old(cls, using_db: Optional[BaseDBAsyncClient] = None, name='_old'):
         """复制表"""
         db = using_db or cls._choose_db(True)
         _table = cls._meta.db_table
         old_table = _table + name
         data = await cls.all().limit(1)
         if data:
             await db.execute_query(f'DROP TABLE IF EXISTS {old_table}')
             return await db.execute_query(f'CREATE TABLE {old_table} SELECT * FROM {_table}')
-
-    create_time = fields.DatetimeField(null=False, auto_now_add=True, description='创建时间')
-    update_time = fields.DatetimeField(null=False, auto_now=True, description='更新时间')
```

### Comparing `du_aio_tools-0.0.4/du_aio_tools/base_spider.py` & `du_aio_tools-0.0.6/du_aio_tools/base_spider.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/du_aio_tools/rsa.py` & `du_aio_tools-0.0.6/du_aio_tools/rsa.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/du_aio_tools/schemas.py` & `du_aio_tools-0.0.6/du_aio_tools/schemas.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/du_aio_tools/time.py` & `du_aio_tools-0.0.6/du_aio_tools/time.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/du_aio_tools.egg-info/PKG-INFO` & `du_aio_tools-0.0.6/du_aio_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: du-aio-tools
-Version: 0.0.4
+Version: 0.0.6
 Summary: async tools
 Author: DYZ
 Author-email: duyuchau@gmail.com
 Maintainer: DYZ
 Maintainer-email: duyuchau@gmail.com
 License: MIT
 Platform: all
```

### Comparing `du_aio_tools-0.0.4/setup.py` & `du_aio_tools-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Software: PyCharm
 
 import os
 from setuptools import find_packages, setup
 
 # 提供一些有用的信息
 NAME = 'du_aio_tools'  # Python 包的名称，即在 pip install 时后面跟的包名
-VERSION = '0.0.4'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
+VERSION = '0.0.6'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
 DESCRIPTION = "async tools"  # 关于该包的剪短描述
 if os.path.exists('README.md'):  # 如果需要，可以加入一段较长的描述，比如读取 README.md，该段长描述会直接显示在 PyPI 的页面上
     with open('README.md', encoding='utf-8') as f:
         LONG_DESCRIPTION = f.read()
 else:
     LONG_DESCRIPTION = DESCRIPTION
 AUTHOR = 'DYZ'  # 留下大名
```

### Comparing `du_aio_tools-0.0.4/tests/conn.py` & `du_aio_tools-0.0.6/tests/conn.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/tests/t1.py` & `du_aio_tools-0.0.6/tests/t1.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.4/tests/t_html.py` & `du_aio_tools-0.0.6/tests/t_html.py`

 * *Files identical despite different names*

