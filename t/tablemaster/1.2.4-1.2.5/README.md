# Comparing `tmp/tablemaster-1.2.4.tar.gz` & `tmp/tablemaster-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.2.4.tar", last modified: Thu May 30 05:26:33 2024, max compression
+gzip compressed data, was "tablemaster-1.2.5.tar", last modified: Fri May 31 06:42:38 2024, max compression
```

## Comparing `tablemaster-1.2.4.tar` & `tablemaster-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.837568 tablemaster-1.2.4/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.4/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-30 05:26:33.832441 tablemaster-1.2.4/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.4/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2024-05-30 05:26:33.837646 tablemaster-1.2.4/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      517 2024-05-30 05:23:55.000000 tablemaster-1.2.4/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.831525 tablemaster-1.2.4/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      685 2024-05-30 05:22:49.000000 tablemaster-1.2.4/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/feishu.py
--rw-r--r--   0 livid      (501) staff       (20)     1266 2024-05-30 05:21:07.000000 tablemaster-1.2.4/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/local.py
--rw-r--r--   0 livid      (501) staff       (20)     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.4/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.832194 tablemaster-1.2.4/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      332 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)       77 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-31 06:42:38.765567 tablemaster-1.2.5/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.5/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-31 06:42:38.765350 tablemaster-1.2.5/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.5/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2024-05-31 06:42:38.765608 tablemaster-1.2.5/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      517 2024-05-31 06:41:55.000000 tablemaster-1.2.5/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-31 06:42:38.764274 tablemaster-1.2.5/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      685 2024-05-30 05:22:49.000000 tablemaster-1.2.5/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.5/tablemaster/feishu.py
+-rw-r--r--   0 livid      (501) staff       (20)     1266 2024-05-30 05:21:07.000000 tablemaster-1.2.5/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.5/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     5910 2024-05-31 06:41:41.000000 tablemaster-1.2.5/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2024-05-20 11:04:14.000000 tablemaster-1.2.5/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-31 06:42:38.765078 tablemaster-1.2.5/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-31 06:42:38.000000 tablemaster-1.2.5/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      332 2024-05-31 06:42:38.000000 tablemaster-1.2.5/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2024-05-31 06:42:38.000000 tablemaster-1.2.5/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)       77 2024-05-31 06:42:38.000000 tablemaster-1.2.5/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2024-05-31 06:42:38.000000 tablemaster-1.2.5/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.2.4/LICENSE` & `tablemaster-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/README.md` & `tablemaster-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/setup.py` & `tablemaster-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.2.4',
+    version='1.2.5',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.2.4/tablemaster/__init__.py` & `tablemaster-1.2.5/tablemaster/__init__.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/tablemaster/feishu.py` & `tablemaster-1.2.5/tablemaster/feishu.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/tablemaster/gspread.py` & `tablemaster-1.2.5/tablemaster/gspread.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/tablemaster/local.py` & `tablemaster-1.2.5/tablemaster/local.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.4/tablemaster/mysql.py` & `tablemaster-1.2.5/tablemaster/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,19 @@
         try:
             query(sql = f"SELECT * FROM {self.table} LIMIT 1", configs=configs)
             print("table exist!")
         except:
             print("table not found!")
 
     def delete_table(self):
-        opt(f'DROP TABLE {self.table}', self)
-        print(f'{self.table} deleted!')
+        try:
+            opt(f'DROP TABLE {self.table}', self)
+            print(f'{self.table} deleted!')
+        except:
+            print('Table was not deleted!')
 
     def par_del(self, clause):
         del_clause = f"DELETE FROM {self.table} WHERE {clause}"
         opt(del_clause, self)
         print(f'records of table that {clause} are deleted!')
 
     def change_data_type(self, cols_name, data_type):
```

### Comparing `tablemaster-1.2.4/tablemaster/utils.py` & `tablemaster-1.2.5/tablemaster/utils.py`

 * *Files identical despite different names*

