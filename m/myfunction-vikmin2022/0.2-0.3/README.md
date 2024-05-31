# Comparing `tmp/myfunction_vikmin2022-0.2.tar.gz` & `tmp/myfunction_vikmin2022-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Vikmin2022/Python_class/Class5/dist/tmphoypg274/myfunction_vikmin2022-0.2.tar", last modified: Fri May 31 01:22:09 2024, max compression
+gzip compressed data, was "/mnt/Vikmin2022/Python_class/Class5/dist/tmp_4hxzaxj/myfunction_vikmin2022-0.3.tar", last modified: Fri May 31 01:31:23 2024, max compression
```

## Comparing `myfunction_vikmin2022-0.2.tar` & `myfunction_vikmin2022-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      648 2024-05-31 01:21:53.000000 myfunction_vikmin2022-0.2/setup.py
-drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/top_level.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      198 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/SOURCES.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/dependency_links.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      662 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/PKG-INFO
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      206 2024-05-31 01:17:47.000000 myfunction_vikmin2022-0.2/README.md
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      662 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/PKG-INFO
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)       38 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/setup.cfg
+drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      648 2024-05-31 01:31:05.000000 myfunction_vikmin2022-0.3/setup.py
+drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/top_level.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      198 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/SOURCES.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/dependency_links.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      831 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/PKG-INFO
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      375 2024-05-31 01:30:32.000000 myfunction_vikmin2022-0.3/README.md
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      831 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/PKG-INFO
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)       38 2024-05-31 01:31:23.000000 myfunction_vikmin2022-0.3/setup.cfg
```

### Comparing `myfunction_vikmin2022-0.2/setup.py` & `myfunction_vikmin2022-0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_vikmin2022',
-    version='0.02',
+    version='0.03',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/vikmin2022',
     license='MIT',
     author='Viktoriia Minosian',
     author_email='viktoriia.minosian@gmail.com',
     description='A description of your package',
```

### Comparing `myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/PKG-INFO` & `myfunction_vikmin2022-0.3/myfunction_vikmin2022.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: myfunction-vikmin2022
-Version: 0.2
+Version: 0.3
 Summary: A description of your package
 Home-page: https://github.com/vikmin2022
 Author: Viktoriia Minosian
 Author-email: viktoriia.minosian@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Usage
 .........
-# 1. Use function multiplication to do arifmetical tasks with multiplication. Colling the  function multiplication specify numbers you  want to multiply. Exeple: multiplication(1,2)  
+# 1. Use function multiplication to do arithmetic tasks with multiplication. Calling the function multiplication specify numbers you want to multiply. Exemple: multiplication(1,2)  
 
-# 2
+# 2. Use function multiplication to do arithmetic tasks with substruction. Calling the function substruction specify numbers you want to substruct. Exemple: substruction(6,3)
```

### Comparing `myfunction_vikmin2022-0.2/PKG-INFO` & `myfunction_vikmin2022-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: myfunction_vikmin2022
-Version: 0.2
+Version: 0.3
 Summary: A description of your package
 Home-page: https://github.com/vikmin2022
 Author: Viktoriia Minosian
 Author-email: viktoriia.minosian@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Usage
 .........
-# 1. Use function multiplication to do arifmetical tasks with multiplication. Colling the  function multiplication specify numbers you  want to multiply. Exeple: multiplication(1,2)  
+# 1. Use function multiplication to do arithmetic tasks with multiplication. Calling the function multiplication specify numbers you want to multiply. Exemple: multiplication(1,2)  
 
-# 2
+# 2. Use function multiplication to do arithmetic tasks with substruction. Calling the function substruction specify numbers you want to substruct. Exemple: substruction(6,3)
```

