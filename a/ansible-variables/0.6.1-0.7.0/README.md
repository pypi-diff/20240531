# Comparing `tmp/ansible-variables-0.6.1.tar.gz` & `tmp/ansible_variables-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.6.1.tar", last modified: Sun Mar 10 11:46:20 2024, max compression
+gzip compressed data, was "ansible_variables-0.7.0.tar", last modified: Fri May 31 06:32:03 2024, max compression
```

## Comparing `ansible-variables-0.6.1.tar` & `ansible_variables-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.931363 ansible-variables-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-03-10 11:46:20.931363 ansible-variables-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.923363 ansible-variables-0.6.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.927363 ansible-variables-0.6.1/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.927363 ansible-variables-0.6.1/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.927363 ansible-variables-0.6.1/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.927363 ansible-variables-0.6.1/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-10 11:46:20.000000 ansible-variables-0.6.1/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-10 11:46:20.931363 ansible-variables-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 11:46:20.927363 ansible-variables-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-03-10 11:46:15.000000 ansible-variables-0.6.1/tests/test_variablesource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.480381 ansible_variables-0.7.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.480381 ansible_variables-0.7.0/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 06:32:03.000000 ansible_variables-0.7.0/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:32:03.484381 ansible_variables-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-31 06:31:59.000000 ansible_variables-0.7.0/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.6.1/LICENSE` & `ansible_variables-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/PKG-INFO` & `ansible_variables-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.6.1
+Version: 0.7.0
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
 Project-URL: Repository, https://github.com/hille721/ansible-variables
@@ -51,15 +51,15 @@
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
-Tested with `ansible-core` 2.11 - 2.16.
+Tested with `ansible-core` 2.11 - 2.17.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
```

### Comparing `ansible-variables-0.6.1/README.md` & `ansible_variables-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
-Tested with `ansible-core` 2.11 - 2.16.
+Tested with `ansible-core` 2.11 - 2.17.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
```

### Comparing `ansible-variables-0.6.1/lib/ansible_variables/cli/__init__.py` & `ansible_variables-0.7.0/lib/ansible_variables/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/lib/ansible_variables/cli/variables.py` & `ansible_variables-0.7.0/lib/ansible_variables/cli/variables.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/lib/ansible_variables/utils/vars.py` & `ansible_variables-0.7.0/lib/ansible_variables/utils/vars.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/lib/ansible_variables.egg-info/PKG-INFO` & `ansible_variables-0.7.0/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.6.1
+Version: 0.7.0
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
 Project-URL: Repository, https://github.com/hille721/ansible-variables
@@ -51,15 +51,15 @@
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
-Tested with `ansible-core` 2.11 - 2.16.
+Tested with `ansible-core` 2.11 - 2.17.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
```

### Comparing `ansible-variables-0.6.1/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible_variables-0.7.0/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/setup.cfg` & `ansible_variables-0.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-variables
-version = 0.6.1
+version = 0.7.0
 description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls =
```

### Comparing `ansible-variables-0.6.1/tests/test_cli.py` & `ansible_variables-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/tests/test_utils.py` & `ansible_variables-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.6.1/tests/test_variablesource.py` & `ansible_variables-0.7.0/tests/test_variablesource.py`

 * *Files identical despite different names*

