# Comparing `tmp/reverse_life-1.2.2.tar.gz` & `tmp/reverse_life-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_life-1.2.2.tar", last modified: Wed May 22 02:20:57 2024, max compression
+gzip compressed data, was "reverse_life-1.2.5.tar", last modified: Fri May 31 05:48:12 2024, max compression
```

## Comparing `reverse_life-1.2.2.tar` & `reverse_life-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 02:20:57.287545 reverse_life-1.2.2/
--rw-rw-rw-   0        0        0     1085 2024-05-22 02:02:06.000000 reverse_life-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3620 2024-05-22 02:20:57.287545 reverse_life-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1891 2024-05-22 02:09:21.000000 reverse_life-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 02:20:57.281960 reverse_life-1.2.2/reverse-life/
--rw-rw-rw-   0        0        0      128 2024-02-22 12:39:42.000000 reverse_life-1.2.2/reverse-life/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:20:57.283159 reverse_life-1.2.2/reverse-life/pjstealth/
--rw-rw-rw-   0        0        0      108 2024-02-04 06:11:10.000000 reverse_life-1.2.2/reverse-life/pjstealth/__init__.py
--rw-rw-rw-   0        0        0     7777 2024-02-04 06:11:10.000000 reverse_life-1.2.2/reverse-life/pjstealth/env_data.py
--rw-rw-rw-   0        0        0     1347 2024-02-04 06:11:10.000000 reverse_life-1.2.2/reverse-life/pjstealth/pjstealth.py
--rw-rw-rw-   0        0        0    16138 2024-02-04 06:11:10.000000 reverse_life-1.2.2/reverse-life/pjstealth/stealth.py
--rw-rw-rw-   0        0        0     1679 2024-04-16 22:11:54.000000 reverse_life-1.2.2/reverse-life/reverse_oklink.py
--rw-rw-rw-   0        0        0     3648 2024-04-16 22:12:36.000000 reverse_life-1.2.2/reverse-life/reverse_sxfae.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:20:57.287042 reverse_life-1.2.2/reverse_life.egg-info/
--rw-rw-rw-   0        0        0     3620 2024-05-22 02:20:57.000000 reverse_life-1.2.2/reverse_life.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-05-22 02:20:57.000000 reverse_life-1.2.2/reverse_life.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 02:20:57.000000 reverse_life-1.2.2/reverse_life.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      325 2024-05-22 02:20:57.000000 reverse_life-1.2.2/reverse_life.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-22 02:20:57.000000 reverse_life-1.2.2/reverse_life.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 02:20:57.287545 reverse_life-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2222 2024-05-22 02:19:02.000000 reverse_life-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:48:12.329844 reverse_life-1.2.5/
+-rw-rw-rw-   0        0        0     1085 2024-05-20 01:10:24.000000 reverse_life-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     3617 2024-05-31 05:48:12.329339 reverse_life-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2024-05-20 01:37:16.000000 reverse_life-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:48:12.309254 reverse_life-1.2.5/reverse-life/
+-rw-rw-rw-   0        0        0      128 2024-02-22 12:39:42.000000 reverse_life-1.2.5/reverse-life/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:48:12.326327 reverse_life-1.2.5/reverse-life/pjstealth/
+-rw-rw-rw-   0        0        0      108 2024-02-04 06:11:10.000000 reverse_life-1.2.5/reverse-life/pjstealth/__init__.py
+-rw-rw-rw-   0        0        0     7777 2024-02-04 06:11:10.000000 reverse_life-1.2.5/reverse-life/pjstealth/env_data.py
+-rw-rw-rw-   0        0        0     1347 2024-02-04 06:11:10.000000 reverse_life-1.2.5/reverse-life/pjstealth/pjstealth.py
+-rw-rw-rw-   0        0        0    16138 2024-02-04 06:11:10.000000 reverse_life-1.2.5/reverse-life/pjstealth/stealth.py
+-rw-rw-rw-   0        0        0     1679 2024-04-16 22:11:54.000000 reverse_life-1.2.5/reverse-life/reverse_oklink.py
+-rw-rw-rw-   0        0        0     3648 2024-04-16 22:12:36.000000 reverse_life-1.2.5/reverse-life/reverse_sxfae.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:48:12.328894 reverse_life-1.2.5/reverse_life.egg-info/
+-rw-rw-rw-   0        0        0     3617 2024-05-31 05:48:12.000000 reverse_life-1.2.5/reverse_life.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-31 05:48:12.000000 reverse_life-1.2.5/reverse_life.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:48:12.000000 reverse_life-1.2.5/reverse_life.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      322 2024-05-31 05:48:12.000000 reverse_life-1.2.5/reverse_life.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 05:48:12.000000 reverse_life-1.2.5/reverse_life.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:48:12.329844 reverse_life-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2219 2024-05-31 05:47:49.000000 reverse_life-1.2.5/setup.py
```

### Comparing `reverse_life-1.2.2/LICENSE` & `reverse_life-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/PKG-INFO` & `reverse_life-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse-life
-Version: 1.2.2
+Version: 1.2.5
 Summary: This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
 Home-page: https://github.com/yanjlee/reverse-life
 Author: yanjlee
 Author-email: yanjlee@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 Requires-Dist: Flask-Cors
 Requires-Dist: frida
 Requires-Dist: gevent
 Requires-Dist: httpx
 Requires-Dist: Jinja2
 Requires-Dist: langchain
 Requires-Dist: langchain-community
-Requires-Dist: langchain-core
+Requires-Dist: suiutils-py
 
 
 # Web Reverse Engineering Project
 
 ## Introduction
 
 This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
@@ -60,15 +60,15 @@
 
 ## Installation
 
 To use the resources of this project, you need to set up your development environment first. Below are the basic installation instructions:
 
 ```bash
 # Clone the repository
-git clone https://github.com/yanjlee/reverse-life.git
+git clone https://github.com/yanjlee/reverse_life.git
 
 # Enter the project directory
 cd your-repository-name
 
 # Install dependencies (if any)
 pip install -r requirements.txt
 ```
```

### Comparing `reverse_life-1.2.2/README.md` & `reverse_life-1.2.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-
-# Web Reverse Engineering Project
-
-## Introduction
-
-This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
-
-## Features
-
-- **Educational Material**: Provides tutorials on web reverse engineering techniques from beginner to advanced levels.
-- **Tools and Resources**: Shares effective reverse engineering tools and resource links.
-- **Case Studies**: Delve into actual web reverse cases, analyzing techniques and strategies.
-
-## Installation
-
-To use the resources of this project, you need to set up your development environment first. Below are the basic installation instructions:
-
-```bash
-# Clone the repository
-git clone https://github.com/yanjlee/reverse-life.git
-
-# Enter the project directory
-cd your-repository-name
-
-# Install dependencies (if any)
-pip install -r requirements.txt
-```
-
-## Usage
-
-This project provides examples and tools for various web reverse engineering techniques. Here is how to use them:
-
-```python
-# Example: Using a tool to reverse a website
-python reverse_example.py
-```
-
-## Contribution
-
-Contributions of any kind are welcome, be it new cases, documentation improvements, or code updates. Please read `CONTRIBUTING.md` for information on how to start contributing.
-
-## License
-
-This project is licensed under the MIT License. For more details, please check the `LICENSE` file.
-
-## Contact
-
-If you have any questions or suggestions, please contact me through Issues or directly via email.
+
+# Web Reverse Engineering Project
+
+## Introduction
+
+This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
+
+## Features
+
+- **Educational Material**: Provides tutorials on web reverse engineering techniques from beginner to advanced levels.
+- **Tools and Resources**: Shares effective reverse engineering tools and resource links.
+- **Case Studies**: Delve into actual web reverse cases, analyzing techniques and strategies.
+
+## Installation
+
+To use the resources of this project, you need to set up your development environment first. Below are the basic installation instructions:
+
+```bash
+# Clone the repository
+git clone https://github.com/yanjlee/reverse_life.git
+
+# Enter the project directory
+cd your-repository-name
+
+# Install dependencies (if any)
+pip install -r requirements.txt
+```
+
+## Usage
+
+This project provides examples and tools for various web reverse engineering techniques. Here is how to use them:
+
+```python
+# Example: Using a tool to reverse a website
+python reverse_example.py
+```
+
+## Contribution
+
+Contributions of any kind are welcome, be it new cases, documentation improvements, or code updates. Please read `CONTRIBUTING.md` for information on how to start contributing.
+
+## License
+
+This project is licensed under the MIT License. For more details, please check the `LICENSE` file.
+
+## Contact
+
+If you have any questions or suggestions, please contact me through Issues or directly via email.
```

### Comparing `reverse_life-1.2.2/reverse-life/pjstealth/env_data.py` & `reverse_life-1.2.5/reverse-life/pjstealth/env_data.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/reverse-life/pjstealth/pjstealth.py` & `reverse_life-1.2.5/reverse-life/pjstealth/pjstealth.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/reverse-life/pjstealth/stealth.py` & `reverse_life-1.2.5/reverse-life/pjstealth/stealth.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/reverse-life/reverse_oklink.py` & `reverse_life-1.2.5/reverse-life/reverse_oklink.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/reverse-life/reverse_sxfae.py` & `reverse_life-1.2.5/reverse-life/reverse_sxfae.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.2.2/reverse_life.egg-info/PKG-INFO` & `reverse_life-1.2.5/reverse_life.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse-life
-Version: 1.2.2
+Version: 1.2.5
 Summary: This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
 Home-page: https://github.com/yanjlee/reverse-life
 Author: yanjlee
 Author-email: yanjlee@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 Requires-Dist: Flask-Cors
 Requires-Dist: frida
 Requires-Dist: gevent
 Requires-Dist: httpx
 Requires-Dist: Jinja2
 Requires-Dist: langchain
 Requires-Dist: langchain-community
-Requires-Dist: langchain-core
+Requires-Dist: suiutils-py
 
 
 # Web Reverse Engineering Project
 
 ## Introduction
 
 This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
@@ -60,15 +60,15 @@
 
 ## Installation
 
 To use the resources of this project, you need to set up your development environment first. Below are the basic installation instructions:
 
 ```bash
 # Clone the repository
-git clone https://github.com/yanjlee/reverse-life.git
+git clone https://github.com/yanjlee/reverse_life.git
 
 # Enter the project directory
 cd your-repository-name
 
 # Install dependencies (if any)
 pip install -r requirements.txt
 ```
```

### Comparing `reverse_life-1.2.2/setup.py` & `reverse_life-1.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import shutil
 
 # 删除dist/目录
 shutil.rmtree('dist', ignore_errors=True)
 
 setuptools.setup(
     name="reverse-life",
-    version="1.2.2",
+    version="1.2.5",
     author="yanjlee",
-    author_email="yanjlee@163.com", 
+    author_email="yanjlee@163.com",
     description="This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.",  # 模块简介
     install_requires=[
         'requests',
         'faker',
         'execjs',
         'loguru',
         'base64',
@@ -45,15 +45,15 @@
         'Flask-Cors',
         'frida',
         'gevent',
         'httpx',
         'Jinja2',
         'langchain',
         'langchain-community',
-        'langchain-core'
+        'suiutils-py',
     ],
     long_description=open(r'readme.md', encoding='utf-8').read(),  # 读取readme自述文件
     long_description_content_type="text/markdown",
     url="https://github.com/yanjlee/reverse-life",  # 模块github地址
     packages=setuptools.find_packages(),     # 自动列出项目下的包
     classifiers=[
         "Programming Language :: Python :: 3",
```

