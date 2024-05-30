# Comparing `tmp/archiwith-1.1.2.tar.gz` & `tmp/archiwith-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archiwith-1.1.2.tar", last modified: Sun May 26 07:23:03 2024, max compression
+gzip compressed data, was "archiwith-1.2.tar", last modified: Thu May 30 23:50:25 2024, max compression
```

## Comparing `archiwith-1.1.2.tar` & `archiwith-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-26 07:23:03.368749 archiwith-1.1.2/
--rw-r--r--   0 nicospok   (501) staff       (20)     8196 2024-05-26 07:19:32.000000 archiwith-1.1.2/.DS_Store
--rw-r--r--   0 nicospok   (501) staff       (20)       44 2024-05-15 05:39:58.000000 archiwith-1.1.2/.gitignore
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:58.000000 archiwith-1.1.2/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     2214 2024-05-26 07:23:03.367398 archiwith-1.1.2/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     1753 2024-05-15 05:39:58.000000 archiwith-1.1.2/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-26 07:23:03.365904 archiwith-1.1.2/archiwith.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     2214 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      179 2024-05-26 07:23:03.000000 archiwith-1.1.2/archiwith.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-26 07:23:03.369070 archiwith-1.1.2/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      650 2024-05-26 07:21:32.000000 archiwith-1.1.2/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-30 23:50:25.611873 archiwith-1.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-30 22:05:15.000000 archiwith-1.2/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     3186 2024-05-30 23:50:25.611005 archiwith-1.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     2727 2024-05-30 23:49:00.000000 archiwith-1.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-30 23:50:25.605567 archiwith-1.2/archiwith/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1770 2024-05-30 23:21:06.000000 archiwith-1.2/archiwith/archiwith.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-30 23:50:25.610107 archiwith-1.2/archiwith.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     3186 2024-05-30 23:50:24.000000 archiwith-1.2/archiwith.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      181 2024-05-30 23:50:25.000000 archiwith-1.2/archiwith.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-30 23:50:24.000000 archiwith-1.2/archiwith.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-30 23:50:24.000000 archiwith-1.2/archiwith.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-30 23:50:25.612192 archiwith-1.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      649 2024-05-30 23:36:32.000000 archiwith-1.2/setup.py
```

### Comparing `archiwith-1.1.2/LICENSE` & `archiwith-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archiwith-1.1.2/PKG-INFO` & `archiwith-1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: archiwith
-Version: 1.1.2
-Summary: File opener and closener when managed via `with`.
-Home-page: https://github.com/niCodeLine/archiwith
-Author: Nico Spok
-Author-email: nicospok@hotmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Archiwith
 Class that gives you the mini help to avoid to write `open(file_path,'r')` or `open(file_path,'w')` every time ypu want to work with some text file.
 
 
 ## Installation
 
 You can easily install `archiwith` using pip:
@@ -83,14 +68,47 @@
 writer = Archiwith('path/to/your/file').escribir()
 
 # Using the with method
 with writer as file:
     # Write the file
 ```
 
+## ObjetiFiles 
+
+This implementation speeds up file handling by allowing access to file names as attributes, eliminating the need to manually write them out one by one. For example, lets say your folder has a structure like this:
+
+```css
+your_folder/
+│
+├── firstcode.py
+├── another_folder/
+├── outputs.txt
+├── tests.txt
+└── my programs.py
+
+```
+You can access to the names via:
+
+```python
+from archiwith import ObjectiFiles
+
+path = 'path/to/your_folder'
+files = ObjectiFiles(path)
+
+```
+This will create the `files` object with the valid files as attributes and nameing them with a `f_file_name__ext` form. So:
+
+```python
+>>> files.f_tests__txt
+'tests.txt'
+>>> files.f_my_programs__py
+'my programs.py'
+```
+If you have suggestions enabled in your code editor (command I in VS Code), you will get the names when typing `files.f`. The `f` prefix comes from File and is to get a clearer view of what are the files in the autocomplete suggestions.
+
 ## Features
 That would be it.
 ## Contributions
 
 Contributions are welcome! If you have improvements or fixes, please send a pull request or open an issue in the GitHub repository.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `archiwith-1.1.2/setup.py` & `archiwith-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='archiwith',
-    version='1.1.2',
+    version='1.2',
     packages=find_packages(),
     description='File opener and closener when managed via `with`.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/archiwith',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
@@ -14,8 +14,8 @@
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-)
+)
```

