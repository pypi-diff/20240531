# Comparing `tmp/gpt-repository-loader-0.9.2.tar.gz` & `tmp/gpt-repository-loader-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-repository-loader-0.9.2.tar", last modified: Wed May 29 05:27:35 2024, max compression
+gzip compressed data, was "gpt-repository-loader-0.9.3.tar", last modified: Fri May 31 17:48:22 2024, max compression
```

## Comparing `gpt-repository-loader-0.9.2.tar` & `gpt-repository-loader-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 05:27:35.110740 gpt-repository-loader-0.9.2/
--rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.9.2/LICENSE
--rw-r--r--   0 harshwork   (502) staff       (20)     1948 2024-05-29 05:27:35.110485 gpt-repository-loader-0.9.2/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)     1151 2024-05-29 05:27:03.000000 gpt-repository-loader-0.9.2/README.md
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 05:27:35.109053 gpt-repository-loader-0.9.2/gpt_repository_loader/
--rw-r--r--   0 harshwork   (502) staff       (20)      100 2023-03-21 06:32:35.000000 gpt-repository-loader-0.9.2/gpt_repository_loader/__init__.py
--rwxr-xr-x   0 harshwork   (502) staff       (20)     4358 2024-05-21 05:52:23.000000 gpt-repository-loader-0.9.2/gpt_repository_loader/gpt_repository_loader.py
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 05:27:35.110229 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/
--rw-r--r--   0 harshwork   (502) staff       (20)     1948 2024-05-29 05:27:34.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)      379 2024-05-29 05:27:35.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/SOURCES.txt
--rw-r--r--   0 harshwork   (502) staff       (20)        1 2024-05-29 05:27:34.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/dependency_links.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       69 2024-05-29 05:27:34.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/entry_points.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       10 2024-05-29 05:27:34.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/requires.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       22 2024-05-29 05:27:34.000000 gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/top_level.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       38 2024-05-29 05:27:35.110787 gpt-repository-loader-0.9.2/setup.cfg
--rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2024-05-29 05:27:31.000000 gpt-repository-loader-0.9.2/setup.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-31 17:48:22.266683 gpt-repository-loader-0.9.3/
+-rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.9.3/LICENSE
+-rw-r--r--   0 harshwork   (502) staff       (20)     1939 2024-05-31 17:48:22.266369 gpt-repository-loader-0.9.3/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)     1142 2024-05-29 05:29:10.000000 gpt-repository-loader-0.9.3/README.md
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-31 17:48:22.262087 gpt-repository-loader-0.9.3/gpt_repository_loader/
+-rw-r--r--   0 harshwork   (502) staff       (20)      100 2023-03-21 06:32:35.000000 gpt-repository-loader-0.9.3/gpt_repository_loader/__init__.py
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     4956 2024-05-31 17:44:06.000000 gpt-repository-loader-0.9.3/gpt_repository_loader/gpt_repository_loader.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-31 17:48:22.263754 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/
+-rw-r--r--   0 harshwork   (502) staff       (20)     1939 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)      379 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)        1 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       69 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/entry_points.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       10 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/requires.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       22 2024-05-31 17:48:22.000000 gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/top_level.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       38 2024-05-31 17:48:22.266740 gpt-repository-loader-0.9.3/setup.cfg
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2024-05-31 17:47:31.000000 gpt-repository-loader-0.9.3/setup.py
```

### Comparing `gpt-repository-loader-0.9.2/LICENSE` & `gpt-repository-loader-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-repository-loader-0.9.2/PKG-INFO` & `gpt-repository-loader-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-repository-loader
-Version: 0.9.2
+Version: 0.9.3
 Summary: A utility to convert a Git repository into a text representation.
 Home-page: https://github.com/felvin-search/gpt-repository-loader
 Author: Felvin
 Author-email: team@felvin.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 
-```
 # gpt-repository-loader
 
 ## Installation
 
 `pip install gpt-repository-loader`
 
 ## Linux Requirements
@@ -47,9 +46,7 @@
 
 ## What to use it for?
 - Build a README for codebases
 - Work with Legacy code
 - Debug issues
 
 Gemini's 1M context window is REALLLY big, and it under utilized.
-
-```
```

### Comparing `gpt-repository-loader-0.9.2/README.md` & `gpt-repository-loader-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-```
 # gpt-repository-loader
 
 ## Installation
 
 `pip install gpt-repository-loader`
 
 ## Linux Requirements
@@ -25,10 +24,8 @@
 * `-c`, `--copy`: Copies the repository contents to the clipboard. If not provided, the output will be written to a file named `output.txt` in the current directory.
 
 ## What to use it for?
 - Build a README for codebases
 - Work with Legacy code
 - Debug issues
 
-Gemini's 1M context window is REALLLY big, and it under utilized.
-
-```
+Gemini's 1M context window is REALLLY big, and it under utilized.
```

### Comparing `gpt-repository-loader-0.9.2/gpt_repository_loader/gpt_repository_loader.py` & `gpt-repository-loader-0.9.3/gpt_repository_loader/gpt_repository_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,19 @@
         with open(ignore_file_path, 'r') as ignore_file:
             for line in ignore_file:
                 line = line.strip()
                 if not line or line.startswith("#"):
                     continue
                 ignore_list.append(line)
 
-    default_ignore_list = ['dist', 'dist/','dist/*','sdist', 'sdist/','sdist/*' '.git/', '/.git/', '.git', '.git/*', '.gptignore', '.gitignore', 'node_modules', 'node_modules/*', '__pycache__', '__pycache__/*', 'package-lock.json']
-    ignore_list += default_ignore_list
+    default_ignore_list = ['dist', 'dist/','dist/*','sdist', 'sdist/','sdist/*' '.git/', '/.git/', '.git', '.git/*', '.gptignore', '.gitignore', 'node_modules', 'node_modules/*', '__pycache__', '__pycache__/*', 'package-lock.json', 'yarn.lock', 'yarn-error.log']
+    image_ignore_list = ['*.png', '*.jpg', '*.jpeg', '*.gif', '*.bmp', '*.ico', '*.cur', '*.tiff', '*.webp', '*.avif']
+    video_ignore_list = ['*.mp4', '*.mov', '*.wmv', '*.avi', '*.mkv', '*.flv', '*.webm', '*.mp3', '*.wav', '*.aac', '*.m4a', '*.mpa', '*.mpeg', '*.mpe', '*.mpg', '*.mpi', '*.mpt', '*.mpx', '*.ogv', '*.webm', '*.wmv', '*.yuv']
+    audio_ignore_list = ['*.mp3', '*.wav', '*.aac', '*.m4a', '*.mpa', '*.mpeg', '*.mpe', '*.mpg', '*.mpi', '*.mpt', '*.mpx', '*.ogv', '*.webm', '*.wmv', '*.yuv']
+    ignore_list += default_ignore_list + image_ignore_list + video_ignore_list + audio_ignore_list
 
     return ignore_list
 
 def process_repository(repo_path, ignore_list, output_stream):
     git_files = subprocess.check_output(["git", "ls-files"], cwd=repo_path, universal_newlines=True).splitlines()
 
     for file_path in git_files:
```

### Comparing `gpt-repository-loader-0.9.2/gpt_repository_loader.egg-info/PKG-INFO` & `gpt-repository-loader-0.9.3/gpt_repository_loader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-repository-loader
-Version: 0.9.2
+Version: 0.9.3
 Summary: A utility to convert a Git repository into a text representation.
 Home-page: https://github.com/felvin-search/gpt-repository-loader
 Author: Felvin
 Author-email: team@felvin.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 
-```
 # gpt-repository-loader
 
 ## Installation
 
 `pip install gpt-repository-loader`
 
 ## Linux Requirements
@@ -47,9 +46,7 @@
 
 ## What to use it for?
 - Build a README for codebases
 - Work with Legacy code
 - Debug issues
 
 Gemini's 1M context window is REALLLY big, and it under utilized.
-
-```
```

### Comparing `gpt-repository-loader-0.9.2/setup.py` & `gpt-repository-loader-0.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-repository-loader",
-    version="0.9.2",
+    version="0.9.3",
     author="Felvin",
     author_email="team@felvin.com",
     description="A utility to convert a Git repository into a text representation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/felvin-search/gpt-repository-loader",
     packages=find_packages(),
```

