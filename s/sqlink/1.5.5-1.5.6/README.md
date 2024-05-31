# Comparing `tmp/sqlink-1.5.5.tar.gz` & `tmp/sqlink-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlink-1.5.5.tar", last modified: Thu May 30 07:48:34 2024, max compression
+gzip compressed data, was "sqlink-1.5.6.tar", last modified: Fri May 31 11:28:31 2024, max compression
```

## Comparing `sqlink-1.5.5.tar` & `sqlink-1.5.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.095013 sqlink-1.5.5/
--rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1049 2024-05-30 07:48:34.095013 sqlink-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 07:48:34.095013 sqlink-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      647 2024-05-30 07:47:17.000000 sqlink-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.069451 sqlink-1.5.5/sqlink/
--rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.5/sqlink/__init__.py
--rw-rw-rw-   0        0        0    24029 2024-05-30 07:46:14.000000 sqlink-1.5.5/sqlink/dao.py
--rw-rw-rw-   0        0        0     4912 2024-05-30 07:46:14.000000 sqlink-1.5.5/sqlink/database.py
--rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.5/sqlink/entity.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.074490 sqlink-1.5.5/sqlink.egg-info/
--rw-rw-rw-   0        0        0     1049 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.093012 sqlink-1.5.5/test/
--rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_basic_dao.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_comment.py
--rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_create_table.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_database.py
--rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_entity.py
--rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.5/test/test_entity_check_ignore_type.py
--rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_entity_parse.py
--rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_env.py
--rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_execte_sql_with_daofunc.py
--rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_execute_sql_without_dao_func.py
--rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_fetch_one.py
--rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_fetch_type.py
--rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_foreign_key.py
--rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_handle_bool.py
--rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_ignore.py
--rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_insert_conflict.py
--rw-rw-rw-   0        0        0      526 2024-04-23 08:39:29.000000 sqlink-1.5.5/test/test_main.py
--rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_select_one_field.py
--rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_table_substitute.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:28:31.622045 sqlink-1.5.6/
+-rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1049 2024-05-31 11:28:31.622045 sqlink-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:28:31.622045 sqlink-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      647 2024-05-31 11:22:37.000000 sqlink-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:28:31.551210 sqlink-1.5.6/sqlink/
+-rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.6/sqlink/__init__.py
+-rw-rw-rw-   0        0        0    23950 2024-05-31 11:22:37.000000 sqlink-1.5.6/sqlink/dao.py
+-rw-rw-rw-   0        0        0     4912 2024-05-30 07:46:14.000000 sqlink-1.5.6/sqlink/database.py
+-rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.6/sqlink/entity.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:28:31.582283 sqlink-1.5.6/sqlink.egg-info/
+-rw-rw-rw-   0        0        0     1049 2024-05-31 11:28:31.000000 sqlink-1.5.6/sqlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-31 11:28:31.000000 sqlink-1.5.6/sqlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:28:31.000000 sqlink-1.5.6/sqlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-31 11:28:31.000000 sqlink-1.5.6/sqlink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 11:28:31.619051 sqlink-1.5.6/test/
+-rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_basic_dao.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_comment.py
+-rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_create_table.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_database.py
+-rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_entity.py
+-rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.6/test/test_entity_check_ignore_type.py
+-rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_entity_parse.py
+-rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_env.py
+-rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_execte_sql_with_daofunc.py
+-rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_execute_sql_without_dao_func.py
+-rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_fetch_one.py
+-rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_fetch_type.py
+-rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_foreign_key.py
+-rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_handle_bool.py
+-rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_ignore.py
+-rw-rw-rw-   0        0        0     4828 2024-05-31 11:24:52.000000 sqlink-1.5.6/test/test_insert_conflict.py
+-rw-rw-rw-   0        0        0      536 2024-05-30 07:48:55.000000 sqlink-1.5.6/test/test_main.py
+-rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_select_one_field.py
+-rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.6/test/test_table_substitute.py
```

### Comparing `sqlink-1.5.5/LICENSE.txt` & `sqlink-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/PKG-INFO` & `sqlink-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.5
+Version: 1.5.6
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.5/README.md` & `sqlink-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/setup.py` & `sqlink-1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_pypi.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlink",
-    version="1.5.5",
+    version="1.5.6",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a efficient and concise sql framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/sqlink",
     packages=['sqlink'],
```

### Comparing `sqlink-1.5.5/sqlink/dao.py` & `sqlink-1.5.6/sqlink/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,18 +168,17 @@
 
     def decorator(func, conflict=conflict):  # noqa
         def wrapper(self, entity):
             """entity参数是传入的数据类实例（对象），而self.entity是定义的数据类（类）"""
             # 获取entity类的属性名和类型
             fields = [field_name for field_name, _ in self.entity.__annotations__.items()]
             # 过滤属性
-            ignore_fields = {CONSTRAINT_TYPE_AUTO_PRIMARY_KEY, CONSTRAINT_TYPE_IGNORE}
             ignore_fields = [
                 field_name for field_name in fields
-                if any(constraint.type in ignore_fields
+                if any(constraint.type == CONSTRAINT_TYPE_IGNORE
                        for constraint in _parse_constraints(getattr(self.entity, field_name, None)))
             ]
             filtered_fields = [field_name for field_name in fields
                                if field_name not in ignore_fields]
 
             sql_prefix = __process_conflict(value=conflict, db_type=self.db_type)
             sql = f"{self.entity.__name__} " \
```

### Comparing `sqlink-1.5.5/sqlink/database.py` & `sqlink-1.5.6/sqlink/database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/sqlink/entity.py` & `sqlink-1.5.6/sqlink/entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/sqlink.egg-info/PKG-INFO` & `sqlink-1.5.6/sqlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.5
+Version: 1.5.6
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.5/sqlink.egg-info/SOURCES.txt` & `sqlink-1.5.6/sqlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_basic_dao.py` & `sqlink-1.5.6/test/test_basic_dao.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_comment.py` & `sqlink-1.5.6/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_create_table.py` & `sqlink-1.5.6/test/test_create_table.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_database.py` & `sqlink-1.5.6/test/test_database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_entity.py` & `sqlink-1.5.6/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_entity_check_ignore_type.py` & `sqlink-1.5.6/test/test_entity_check_ignore_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_entity_parse.py` & `sqlink-1.5.6/test/test_entity_parse.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_env.py` & `sqlink-1.5.6/test/test_env.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_execte_sql_with_daofunc.py` & `sqlink-1.5.6/test/test_execte_sql_with_daofunc.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_execute_sql_without_dao_func.py` & `sqlink-1.5.6/test/test_execute_sql_without_dao_func.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_fetch_one.py` & `sqlink-1.5.6/test/test_fetch_one.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_fetch_type.py` & `sqlink-1.5.6/test/test_fetch_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_foreign_key.py` & `sqlink-1.5.6/test/test_foreign_key.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_handle_bool.py` & `sqlink-1.5.6/test/test_handle_bool.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_ignore.py` & `sqlink-1.5.6/test/test_ignore.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_insert_conflict.py` & `sqlink-1.5.6/test/test_insert_conflict.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,9 +129,22 @@
     db.commit()
 
     select_student = students[0]
     student_conflict = db.dao_student.get_student_by_name(name=select_student.name)
     assert student_conflict.age == students[1].age
 
 
+def test_insert_replace_on_primary_key(init_db: Database):
+    db = init_db
+    students = [Student(name='张三', age=10, id=1),
+                Student(name='张三', age=11, id=1)]
+    for student in students:
+        db.dao_student.insert_replace(student)
+    db.commit()
+
+    select_student = students[0]
+    student_conflict = db.dao_student.get_student_by_name(name=select_student.name)
+    assert student_conflict.age == students[1].age
+
+
 if __name__ == '__main__':
     pytest.main(["-vv", "--capture=no", __file__])
```

### Comparing `sqlink-1.5.5/test/test_main.py` & `sqlink-1.5.6/test/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 if __name__ == "__main__":
     os.environ['DB_IMPL'] = 'sqlite'
     print("Running tests with SqliteDatabase...")
     pytest.main([".", "-vv", "--ignore=test_env.py"])
     # 清除环境变量，以防对其他进程产生影响
     del os.environ['DB_IMPL']
 
-    os.environ['DB_IMPL'] = 'mysql'
-    print("\nRunning tests with MysqlMetaDatabase...")
-    pytest.main([".", "-vv", "--ignore=test_env.py"])
-    # 清除环境变量
-    del os.environ['DB_IMPL']
+    # os.environ['DB_IMPL'] = 'mysql'
+    # print("\nRunning tests with MysqlMetaDatabase...")
+    # pytest.main([".", "-vv", "--ignore=test_env.py"])
+    # # 清除环境变量
+    # del os.environ['DB_IMPL']
```

### Comparing `sqlink-1.5.5/test/test_select_one_field.py` & `sqlink-1.5.6/test/test_select_one_field.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.5/test/test_table_substitute.py` & `sqlink-1.5.6/test/test_table_substitute.py`

 * *Files identical despite different names*

