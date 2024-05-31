# Comparing `tmp/dbfaker-1.2.2.post1.tar.gz` & `tmp/dbfaker-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbfaker-1.2.2.post1.tar", last modified: Mon May 30 14:53:00 2022, max compression
+gzip compressed data, was "dbfaker-1.2.3.tar", last modified: Fri May 31 03:43:18 2024, max compression
```

## Comparing `dbfaker-1.2.2.post1.tar` & `dbfaker-1.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/
--rw-r--r--   0 guolong    (501) staff       (20)     9228 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/LICENSE
--rw-r--r--   0 guolong    (501) staff       (20)    13538 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/PKG-INFO
--rw-r--r--   0 guolong    (501) staff       (20)    12830 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/README.md
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker/
--rw-r--r--   0 guolong    (501) staff       (20)      136 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/__init__.py
--rw-r--r--   0 guolong    (501) staff       (20)       86 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/__main__.py
--rw-r--r--   0 guolong    (501) staff       (20)     3458 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/cli.py
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker/common/
--rw-r--r--   0 guolong    (501) staff       (20)        0 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/__init__.py
--rw-r--r--   0 guolong    (501) staff       (20)     4748 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/database.py
--rw-r--r--   0 guolong    (501) staff       (20)     1632 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/db_helper.py
--rw-r--r--   0 guolong    (501) staff       (20)      466 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/drivers.py
--rw-r--r--   0 guolong    (501) staff       (20)     2605 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/logger.py
--rw-r--r--   0 guolong    (501) staff       (20)      869 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/setting.py
--rw-r--r--   0 guolong    (501) staff       (20)      557 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/common/tools.py
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker/nsqlparse/
--rw-r--r--   0 guolong    (501) staff       (20)        0 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/nsqlparse/__init__.py
--rwxr-xr-x   0 guolong    (501) staff       (20)     1777 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/nsqlparse/mysql_create_table_lex.py
--rwxr-xr-x   0 guolong    (501) staff       (20)     8938 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/nsqlparse/mysql_create_table_yacc.py
--rw-r--r--   0 guolong    (501) staff       (20)     7939 2022-05-30 12:55:14.000000 dbfaker-1.2.2.post1/dbfaker/table2yml.py
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker/utils/
--rw-r--r--   0 guolong    (501) staff       (20)        0 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/utils/__init__.py
--rw-r--r--   0 guolong    (501) staff       (20)      211 2022-05-30 14:52:50.000000 dbfaker-1.2.2.post1/dbfaker/utils/constant.py
--rw-r--r--   0 guolong    (501) staff       (20)     3225 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/utils/faker_date_time.py
--rw-r--r--   0 guolong    (501) staff       (20)     7674 2022-05-30 14:23:46.000000 dbfaker-1.2.2.post1/dbfaker/utils/faker_tool.py
--rw-r--r--   0 guolong    (501) staff       (20)     8093 2022-05-30 14:48:25.000000 dbfaker-1.2.2.post1/dbfaker/utils/gendata.py
--rw-r--r--   0 guolong    (501) staff       (20)      707 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/utils/generator.py
--rw-r--r--   0 guolong    (501) staff       (20)     3177 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/dbfaker/utils/init_project.py
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/
--rw-r--r--   0 guolong    (501) staff       (20)    13538 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/PKG-INFO
--rw-r--r--   0 guolong    (501) staff       (20)      877 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/SOURCES.txt
--rw-r--r--   0 guolong    (501) staff       (20)        1 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/dependency_links.txt
--rw-r--r--   0 guolong    (501) staff       (20)       80 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/entry_points.txt
--rw-r--r--   0 guolong    (501) staff       (20)       65 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/requires.txt
--rw-r--r--   0 guolong    (501) staff       (20)        8 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/top_level.txt
--rw-r--r--   0 guolong    (501) staff       (20)        1 2021-10-22 11:44:10.000000 dbfaker-1.2.2.post1/dbfaker.egg-info/zip-safe
--rw-r--r--   0 guolong    (501) staff       (20)       38 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/setup.cfg
--rw-r--r--   0 guolong    (501) staff       (20)     2229 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/setup.py
-drwxr-xr-x   0 guolong    (501) staff       (20)        0 2022-05-30 14:53:00.000000 dbfaker-1.2.2.post1/test/
--rw-r--r--   0 guolong    (501) staff       (20)      831 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/test/test_gendata.py
--rw-r--r--   0 guolong    (501) staff       (20)     2018 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/test/test_mfaker.py
--rw-r--r--   0 guolong    (501) staff       (20)      664 2021-10-22 10:53:31.000000 dbfaker-1.2.2.post1/test/test_table2yml.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.606697 dbfaker-1.2.3/
+-rw-r--r--   0 mac        (501) staff       (20)     9228 2023-02-27 08:29:32.000000 dbfaker-1.2.3/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)    13532 2024-05-31 03:43:18.606047 dbfaker-1.2.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)    12830 2023-02-27 08:29:32.000000 dbfaker-1.2.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.574926 dbfaker-1.2.3/dbfaker/
+-rw-r--r--   0 mac        (501) staff       (20)      136 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       86 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/__main__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3458 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/cli.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.582597 dbfaker-1.2.3/dbfaker/common/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4748 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/database.py
+-rw-r--r--   0 mac        (501) staff       (20)     1632 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/db_helper.py
+-rw-r--r--   0 mac        (501) staff       (20)      466 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/drivers.py
+-rw-r--r--   0 mac        (501) staff       (20)     2605 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/logger.py
+-rw-r--r--   0 mac        (501) staff       (20)      869 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/setting.py
+-rw-r--r--   0 mac        (501) staff       (20)      557 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/common/tools.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.584770 dbfaker-1.2.3/dbfaker/nsqlparse/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/nsqlparse/__init__.py
+-rwxr-xr-x   0 mac        (501) staff       (20)     1777 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/nsqlparse/mysql_create_table_lex.py
+-rwxr-xr-x   0 mac        (501) staff       (20)     8938 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/nsqlparse/mysql_create_table_yacc.py
+-rw-r--r--   0 mac        (501) staff       (20)     7939 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/table2yml.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.599578 dbfaker-1.2.3/dbfaker/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      209 2024-05-31 03:36:38.000000 dbfaker-1.2.3/dbfaker/utils/constant.py
+-rw-r--r--   0 mac        (501) staff       (20)     3225 2023-02-27 11:17:45.000000 dbfaker-1.2.3/dbfaker/utils/faker_date_time.py
+-rw-r--r--   0 mac        (501) staff       (20)     7674 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/utils/faker_tool.py
+-rw-r--r--   0 mac        (501) staff       (20)     8093 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/utils/gendata.py
+-rw-r--r--   0 mac        (501) staff       (20)      707 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/utils/generator.py
+-rw-r--r--   0 mac        (501) staff       (20)     3177 2023-02-27 08:29:32.000000 dbfaker-1.2.3/dbfaker/utils/init_project.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.578060 dbfaker-1.2.3/dbfaker.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    13532 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      877 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       80 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)      130 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-31 03:43:18.000000 dbfaker-1.2.3/dbfaker.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-02-27 08:30:51.000000 dbfaker-1.2.3/dbfaker.egg-info/zip-safe
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-31 03:43:18.607172 dbfaker-1.2.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     2294 2023-02-27 08:39:44.000000 dbfaker-1.2.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-31 03:43:18.603709 dbfaker-1.2.3/test/
+-rw-r--r--   0 mac        (501) staff       (20)      831 2023-02-27 08:29:32.000000 dbfaker-1.2.3/test/test_gendata.py
+-rw-r--r--   0 mac        (501) staff       (20)     2018 2023-02-27 08:29:32.000000 dbfaker-1.2.3/test/test_mfaker.py
+-rw-r--r--   0 mac        (501) staff       (20)      664 2023-02-27 08:29:32.000000 dbfaker-1.2.3/test/test_table2yml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dbfaker-1.2.2.post1/LICENSE` & `dbfaker-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/PKG-INFO` & `dbfaker-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbfaker
-Version: 1.2.2.post1
+Version: 1.2.3
 Summary: 基于数据库层面批量生成有逻辑关联的数据
 Home-page: https://gitee.com/guojongg/dbfaker
 Author: Long Guo
 Author-email: 565169745@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbfaker-1.2.2.post1/README.md` & `dbfaker-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/cli.py` & `dbfaker-1.2.3/dbfaker/cli.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/common/database.py` & `dbfaker-1.2.3/dbfaker/common/database.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/common/db_helper.py` & `dbfaker-1.2.3/dbfaker/common/db_helper.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/common/logger.py` & `dbfaker-1.2.3/dbfaker/common/logger.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/common/setting.py` & `dbfaker-1.2.3/dbfaker/common/setting.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/common/tools.py` & `dbfaker-1.2.3/dbfaker/common/tools.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/nsqlparse/mysql_create_table_lex.py` & `dbfaker-1.2.3/dbfaker/nsqlparse/mysql_create_table_lex.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/nsqlparse/mysql_create_table_yacc.py` & `dbfaker-1.2.3/dbfaker/nsqlparse/mysql_create_table_yacc.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/table2yml.py` & `dbfaker-1.2.3/dbfaker/table2yml.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/utils/faker_date_time.py` & `dbfaker-1.2.3/dbfaker/utils/faker_date_time.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/utils/faker_tool.py` & `dbfaker-1.2.3/dbfaker/utils/faker_tool.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/utils/gendata.py` & `dbfaker-1.2.3/dbfaker/utils/gendata.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/utils/generator.py` & `dbfaker-1.2.3/dbfaker/utils/generator.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker/utils/init_project.py` & `dbfaker-1.2.3/dbfaker/utils/init_project.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/dbfaker.egg-info/PKG-INFO` & `dbfaker-1.2.3/dbfaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbfaker
-Version: 1.2.2.post1
+Version: 1.2.3
 Summary: 基于数据库层面批量生成有逻辑关联的数据
 Home-page: https://gitee.com/guojongg/dbfaker
 Author: Long Guo
 Author-email: 565169745@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbfaker-1.2.2.post1/dbfaker.egg-info/SOURCES.txt` & `dbfaker-1.2.3/dbfaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/setup.py` & `dbfaker-1.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,23 +51,23 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': [
         'dbfaker = dbfaker.cli:run',
         'table2yml = dbfaker.table2yml:main'
     ]},
     install_requires=[
-        'PyMySQL',
-        'PyYAML',
-        'pypinyin',
-        'Faker',
-        'Jinja2',
-        'SQLAlchemy',
-        'ply',
-        'tqdm',
-        'dbutils'
+        'PyMySQL==0.10.0',
+        'PyYAML==5.3.1',
+        'pypinyin==0.39.0',
+        'Faker==2.0.2',
+        'Jinja2==2.11.2',
+        'SQLAlchemy==1.3.19',
+        'ply==3.11',
+        'tqdm==4.49.0',
+        'DBUtils==2.0'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
```

### Comparing `dbfaker-1.2.2.post1/test/test_gendata.py` & `dbfaker-1.2.3/test/test_gendata.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/test/test_mfaker.py` & `dbfaker-1.2.3/test/test_mfaker.py`

 * *Files identical despite different names*

### Comparing `dbfaker-1.2.2.post1/test/test_table2yml.py` & `dbfaker-1.2.3/test/test_table2yml.py`

 * *Files identical despite different names*

