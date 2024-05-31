# Comparing `tmp/static_analysis_script-0.2.4.tar.gz` & `tmp/static_analysis_script-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.2.4.tar", last modified: Fri May 31 07:06:28 2024, max compression
+gzip compressed data, was "static_analysis_script-0.2.6.tar", last modified: Fri May 31 07:45:53 2024, max compression
```

## Comparing `static_analysis_script-0.2.4.tar` & `static_analysis_script-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:28.561754 static_analysis_script-0.2.4/
--rw-rw-rw-   0        0        0     2383 2024-05-31 07:06:28.560754 static_analysis_script-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2024-05-31 06:44:58.000000 static_analysis_script-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 07:06:28.561754 static_analysis_script-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1633 2024-05-31 06:44:58.000000 static_analysis_script-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:28.539753 static_analysis_script-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:28.541754 static_analysis_script-0.2.4/src/analysis/
--rw-rw-rw-   0        0        0        0 2024-05-31 06:44:58.000000 static_analysis_script-0.2.4/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    13417 2024-05-31 07:04:38.000000 static_analysis_script-0.2.4/src/analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:28.541754 static_analysis_script-0.2.4/src/bin/
--rwxrwxrwx   0        0        0   370056 2024-05-31 06:44:58.000000 static_analysis_script-0.2.4/src/bin/strings.exe
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:28.559753 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2383 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 07:06:28.000000 static_analysis_script-0.2.4/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 07:45:53.958033 static_analysis_script-0.2.6/
+-rw-rw-rw-   0        0        0       33 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/.gitignore
+-rw-rw-rw-   0        0        0     2414 2024-05-31 07:45:53.957033 static_analysis_script-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/README.md
+-rw-rw-rw-   0        0        0       32 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:45:53.958033 static_analysis_script-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1705 2024-05-31 07:34:23.000000 static_analysis_script-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:45:53.927033 static_analysis_script-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 07:45:53.937033 static_analysis_script-0.2.6/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13106 2024-05-31 07:39:30.000000 static_analysis_script-0.2.6/src/analysis/main.py
+-rwxrwxrwx   0        0        0   370056 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/src/analysis/strings.exe
+-rwxrwxrwx   0        0        0   108544 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/src/analysis/trid.exe
+drwxrwxrwx   0        0        0        0 2024-05-31 07:45:53.941033 static_analysis_script-0.2.6/src/bin/
+-rwxrwxrwx   0        0        0   370056 2024-05-31 07:37:59.000000 static_analysis_script-0.2.6/src/bin/strings.exe
+drwxrwxrwx   0        0        0        0 2024-05-31 07:45:53.957033 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2414 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 07:45:53.000000 static_analysis_script-0.2.6/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.2.4/PKG-INFO` & `static_analysis_script-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.2.4
+Version: 0.2.6
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyPDF2
 Requires-Dist: tqdm
 Requires-Dist: numpy
 Requires-Dist: pyfiglet
 Requires-Dist: colorama
+Requires-Dist: setuptools_scm
 
 
 ## Static-analysis-script 
 Welcome to the Static Analysis Script! This Python tool is crafted to extract emails, paths, files, URLs, and IPs from the specified file for analysis.
 ## Purpose
 This tool aids in the collection of data essential for static analysis, accelerating the detection of Indicators of Compromise (IOCs) and other potentially malicious activities executed by files.
 ## Installation
```

### Comparing `static_analysis_script-0.2.4/README.md` & `static_analysis_script-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.2.4/setup.py` & `static_analysis_script-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.2.4',
+    use_scm_version=True,
+    setup_requires=['setuptools_scm'],
     author='Perzibel',
     author_email='perzibel@outlook.com',
     description='A utility to perform static analysis on files.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',  # This is important for rendering Markdown from README
     url='https://github.com/perzibel/static-analysis-script',
     packages=find_packages(where="src"),
@@ -24,15 +25,16 @@
         ],
     },
     install_requires=[
         'PyPDF2',
         'tqdm',
         'numpy',
         'pyfiglet',
-        'colorama'
+        'colorama',
+        'setuptools_scm'
     ],
     include_package_data=True,
     package_data={
         "analysis": ["../bin/strings.exe"],  # Make sure the path matches your structure
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `static_analysis_script-0.2.4/src/analysis/main.py` & `static_analysis_script-0.2.6/src/analysis/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from PyPDF2 import PdfReader
 from tqdm import tqdm
 import os
 import sys
 import time
 import pyfiglet
 from colorama import Fore, Back, Style
+from setuptools_scm import get_version
 
 entropy_threshold = 7.0
 
 
 def winApiStrings(strings):
     winAPIList = ['Open', 'Write', 'Wget', 'Wset', 'Create', 'Exec', 'Wait', 'Virtual', 'Set', 'Get', 'Http', 'Load',
                   'Exit', 'Kill', 'Free', 'Sleep', 'Time', 'Callee']
@@ -288,37 +289,31 @@
           "-e, -E    Print out the entropy calculation only. \n"
           "-c, -C    Print certificate information, including supplementary details. \n"
           "--version Script current version. \n \n"
           "for more information or requests, please visit the project repository. ")
 
 
 def print_version():
-    dir_path = os.path.dirname(os.path.realpath(__file__))
-    parent_dir = os.path.dirname(dir_path)
-    src_dir = os.path.dirname(parent_dir)
-    process = subprocess.Popen(f'type "{src_dir}\\setup.py" | findstr "version"', shell=True,
-                               stdout=subprocess.PIPE,
-                               stderr=subprocess.PIPE)
-    output, error = process.communicate()
-    return output.decode('utf-8')
+    """Print the version of the code."""
+    version = get_version()
+    print(f"Code Version: {version}")
 
 
 def main():
     import sys
 
     num_args = len(sys.argv)
     if num_args == 2 or num_args == 3:
         UserInput = sys.argv[1]
         try:
             clean_path = UserInput.replace('"', "")
             if UserInput == ('-h' or '-H'):
                 print_help()
             elif UserInput in '--version':
-                ver = print_version()
-                print(ver)
+                print_version()
             elif os.path.isfile(clean_path):
                 print_heaeder()
                 try:
                     if sys.argv[2] in ('-C', '-c'):
                         certInfo = extract_cert_info(clean_path)
                         print(certInfo)
                     elif sys.argv[2] in ('-E', '-e'):
@@ -344,15 +339,15 @@
                     print("\n Emails:", findings[0])
                     print("\n IPs:", findings[1])
                     print("\n Paths:", findings[2])
                     print("\n Files and DLLs:", findings[3])
                     print("\n Urls:", findings[4])
                     print("\n Windows API:", findings[5])
             else:
-                print("file doesn't exists, please read main.py -h for further explanation")
+                print("file path doesn't exists, please read main.py -h for further explanation")
         except Exception as e:
             print("\n ----- error: ", e, " ---------")
     else:
         print_help()
 
 
 if __name__ == "__main__":
```

### Comparing `static_analysis_script-0.2.4/src/bin/strings.exe` & `static_analysis_script-0.2.6/src/analysis/strings.exe`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.2.4/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.2.6/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.2.4
+Version: 0.2.6
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyPDF2
 Requires-Dist: tqdm
 Requires-Dist: numpy
 Requires-Dist: pyfiglet
 Requires-Dist: colorama
+Requires-Dist: setuptools_scm
 
 
 ## Static-analysis-script 
 Welcome to the Static Analysis Script! This Python tool is crafted to extract emails, paths, files, URLs, and IPs from the specified file for analysis.
 ## Purpose
 This tool aids in the collection of data essential for static analysis, accelerating the detection of Indicators of Compromise (IOCs) and other potentially malicious activities executed by files.
 ## Installation
```

