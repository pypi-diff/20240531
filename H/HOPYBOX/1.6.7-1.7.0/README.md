# Comparing `tmp/HOPYBOX-1.6.7.tar.gz` & `tmp/hopybox-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HOPYBOX-1.6.7.tar", last modified: Fri Feb  3 04:26:24 2023, max compression
+gzip compressed data, was "hopybox-1.7.0.tar", last modified: Fri May 31 12:36:39 2024, max compression
```

## Comparing `HOPYBOX-1.6.7.tar` & `hopybox-1.7.0.tar`

### file list

```diff
@@ -1,40 +1,37 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-02-03 04:26:24.391501 HOPYBOX-1.6.7/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-02-03 04:26:24.019501 HOPYBOX-1.6.7/HOPYBOX.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1701 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      704 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       71 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)      102 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-02-03 04:26:23.000000 HOPYBOX-1.6.7/HOPYBOX.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)    35148 2022-05-02 12:39:15.000000 HOPYBOX-1.6.7/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1701 2023-02-03 04:26:24.375501 HOPYBOX-1.6.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      997 2022-05-28 13:03:20.000000 HOPYBOX-1.6.7/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-02-03 04:26:24.367501 HOPYBOX-1.6.7/hopybox/
--rw-rw----   0 root         (0) everybody  (9997)    35185 2022-05-24 13:10:42.000000 HOPYBOX-1.6.7/hopybox/LICENSE.py
--rw-rw----   0 root         (0) everybody  (9997)      374 2022-08-20 01:54:58.000000 HOPYBOX-1.6.7/hopybox/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5294 2023-02-03 01:40:45.000000 HOPYBOX-1.6.7/hopybox/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     2907 2022-06-02 22:28:33.000000 HOPYBOX-1.6.7/hopybox/caculate.py
--rw-rw----   0 root         (0) everybody  (9997)      866 2022-12-24 00:10:29.000000 HOPYBOX-1.6.7/hopybox/check.py
--rw-rw----   0 root         (0) everybody  (9997)     1189 2022-06-14 05:07:01.000000 HOPYBOX-1.6.7/hopybox/clear.py
--rw-rw----   0 root         (0) everybody  (9997)      103 2022-05-26 11:33:47.000000 HOPYBOX-1.6.7/hopybox/copyright.py
--rw-rw----   0 root         (0) everybody  (9997)     1786 2023-01-11 10:55:45.000000 HOPYBOX-1.6.7/hopybox/dirtree.py
--rw-rw----   0 root         (0) everybody  (9997)      443 2022-05-28 12:57:26.000000 HOPYBOX-1.6.7/hopybox/download.py
--rw-rw----   0 root         (0) everybody  (9997)     3406 2022-06-15 12:19:17.000000 HOPYBOX-1.6.7/hopybox/filetoolbox.py
--rw-rw----   0 root         (0) everybody  (9997)      312 2022-05-24 12:40:11.000000 HOPYBOX-1.6.7/hopybox/fps.py
--rw-rw----   0 root         (0) everybody  (9997)      664 2022-06-12 07:50:44.000000 HOPYBOX-1.6.7/hopybox/headers.py
--rw-rw----   0 root         (0) everybody  (9997)     3037 2022-12-23 06:38:32.000000 HOPYBOX-1.6.7/hopybox/helps.py
--rw-rw----   0 root         (0) everybody  (9997)      642 2022-08-15 05:41:20.000000 HOPYBOX-1.6.7/hopybox/hopter.py
--rw-rw----   0 root         (0) everybody  (9997)     1182 2022-05-28 05:09:05.000000 HOPYBOX-1.6.7/hopybox/ipway.py
--rw-rw----   0 root         (0) everybody  (9997)      954 2022-05-28 04:41:14.000000 HOPYBOX-1.6.7/hopybox/qqget.py
--rw-rw----   0 root         (0) everybody  (9997)     4310 2022-08-20 01:41:13.000000 HOPYBOX-1.6.7/hopybox/scan.py
--rw-rw----   0 root         (0) everybody  (9997)      895 2022-05-21 02:53:37.000000 HOPYBOX-1.6.7/hopybox/sdemail.py
--rw-rw----   0 root         (0) everybody  (9997)     1348 2023-02-03 01:59:47.000000 HOPYBOX-1.6.7/hopybox/system.py
--rw-rw----   0 root         (0) everybody  (9997)      413 2022-05-28 04:07:26.000000 HOPYBOX-1.6.7/hopybox/timetoolbox.py
--rw-rw----   0 root         (0) everybody  (9997)      907 2022-07-22 04:31:31.000000 HOPYBOX-1.6.7/hopybox/translate.py
--rw-rw----   0 root         (0) everybody  (9997)     1761 2022-08-20 01:39:23.000000 HOPYBOX-1.6.7/hopybox/tree_dir.py
--rw-rw----   0 root         (0) everybody  (9997)     2718 2023-02-03 04:23:06.000000 HOPYBOX-1.6.7/hopybox/update.py
--rw-rw----   0 root         (0) everybody  (9997)     2915 2022-05-28 12:14:16.000000 HOPYBOX-1.6.7/hopybox/urlget.py
--rw-rw----   0 root         (0) everybody  (9997)      583 2023-02-03 04:21:44.000000 HOPYBOX-1.6.7/hopybox/version.py
--rw-rw----   0 root         (0) everybody  (9997)      310 2022-07-22 04:31:54.000000 HOPYBOX-1.6.7/hopybox/weather.py
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-02-03 04:26:24.391501 HOPYBOX-1.6.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1397 2023-02-03 04:22:13.000000 HOPYBOX-1.6.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-31 12:36:39.765568 hopybox-1.7.0/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-31 12:36:39.745568 hopybox-1.7.0/HOPYBOX.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1754 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      643 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       84 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       57 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2024-05-31 12:36:39.000000 hopybox-1.7.0/HOPYBOX.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)    35148 2023-09-09 09:14:15.000000 hopybox-1.7.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1754 2024-05-31 12:36:39.753568 hopybox-1.7.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      906 2024-05-31 10:29:42.000000 hopybox-1.7.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-31 12:36:39.721568 hopybox-1.7.0/hopybox/
+-rw-rw----   0 root         (0) everybody  (9997)      447 2023-10-25 05:41:44.000000 hopybox-1.7.0/hopybox/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3602 2024-05-29 04:38:47.000000 hopybox-1.7.0/hopybox/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)      338 2023-10-25 01:13:00.000000 hopybox-1.7.0/hopybox/basedtool.py
+-rw-rw----   0 root         (0) everybody  (9997)     2901 2023-09-06 04:42:41.000000 hopybox-1.7.0/hopybox/caculate.py
+-rw-rw----   0 root         (0) everybody  (9997)     1189 2022-06-14 05:07:01.000000 hopybox-1.7.0/hopybox/clear.py
+-rw-rw----   0 root         (0) everybody  (9997)     5283 2024-05-31 05:08:07.000000 hopybox-1.7.0/hopybox/command.py
+-rw-rw----   0 root         (0) everybody  (9997)     2963 2024-05-31 05:08:49.000000 hopybox-1.7.0/hopybox/connect.py
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-10-26 10:52:44.000000 hopybox-1.7.0/hopybox/debug.py
+-rw-rw----   0 root         (0) everybody  (9997)     2334 2024-03-09 05:12:35.000000 hopybox-1.7.0/hopybox/device.py
+-rw-rw----   0 root         (0) everybody  (9997)      462 2023-08-20 10:00:38.000000 hopybox-1.7.0/hopybox/download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3234 2024-05-25 12:31:23.000000 hopybox-1.7.0/hopybox/filetool.py
+-rw-rw----   0 root         (0) everybody  (9997)      802 2023-09-28 08:49:20.000000 hopybox-1.7.0/hopybox/headers.py
+-rw-rw----   0 root         (0) everybody  (9997)     3001 2024-05-28 04:35:51.000000 hopybox-1.7.0/hopybox/helps.py
+-rw-rw----   0 root         (0) everybody  (9997)      755 2023-09-09 08:46:52.000000 hopybox-1.7.0/hopybox/hopter.py
+-rw-rw----   0 root         (0) everybody  (9997)      807 2023-09-28 12:55:43.000000 hopybox-1.7.0/hopybox/mail.py
+-rw-rw----   0 root         (0) everybody  (9997)      567 2023-10-25 03:12:33.000000 hopybox-1.7.0/hopybox/prompt.py
+-rw-rw----   0 root         (0) everybody  (9997)      954 2022-05-28 04:41:14.000000 hopybox-1.7.0/hopybox/qqget.py
+-rw-rw----   0 root         (0) everybody  (9997)     4310 2022-08-20 01:41:13.000000 hopybox-1.7.0/hopybox/scan.py
+-rw-rw----   0 root         (0) everybody  (9997)     1532 2023-09-29 00:21:34.000000 hopybox-1.7.0/hopybox/system.py
+-rw-rw----   0 root         (0) everybody  (9997)       22 2023-10-09 05:10:45.000000 hopybox-1.7.0/hopybox/timetool.py
+-rw-rw----   0 root         (0) everybody  (9997)     1355 2023-10-25 03:06:01.000000 hopybox-1.7.0/hopybox/translate.py
+-rw-rw----   0 root         (0) everybody  (9997)     1750 2023-10-22 04:51:41.000000 hopybox-1.7.0/hopybox/tree_dir.py
+-rw-rw----   0 root         (0) everybody  (9997)     3802 2024-05-25 13:13:58.000000 hopybox-1.7.0/hopybox/update.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2024-05-31 12:36:39.765568 hopybox-1.7.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1433 2024-02-16 12:16:36.000000 hopybox-1.7.0/setup.py
```

### Comparing `HOPYBOX-1.6.7/HOPYBOX.egg-info/PKG-INFO` & `hopybox-1.7.0/HOPYBOX.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: HOPYBOX
-Version: 1.6.7
-Summary: This is an open source, practical command Python box
+Version: 1.7.0
+Summary: This is an open source, practical command Python box.
 Home-page: https://github.com/HOStudio123/HOPYBOX
 Author: ChenJinlin
 Author-email: hostudio.hopybox@foxmail.com
 License: GPL-3.0-or-later
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: filetype
+Requires-Dist: yagmail
+Requires-Dist: rich
+Requires-Dist: bs4
+Requires-Dist: chardet
+Requires-Dist: psutil>=5.8.0
 
 # HOPYBOX
 This is an open source, practical command python box
 ## Introduce
 This is an open source, practical command python box, since it is made in python language, so I named it **HOPYBOX**.
 ## Installing
 Install with `pip` or your favorite PyPI package manager.
@@ -46,32 +52,25 @@
 ## Import method
 ```python
 >>>import hopybox
 ```
 ## Usage (How to use)
 See help built in the program
 ```sh
-HOPYBOX/Command:help
+HOPYBOX/Program:help
 ```
 ## Update version
 Enter in the `HOPYBOX` console:
 ```sh
-HOPYBOX/Command:check version
+HOPYBOX/Program:update
 ```
 or like these
 ```sh
 $ pip install -U HOPYBOX
 ```
 ```sh
 $ pip install -U hopybox
 ```
-```sh
-HOPYBOX/Command:install HOPYBOX
-```
-```sh
-HOPYBOX/Command:install hopybox
-```
 ## Github
 [HOStudio123](https://github.com/HOStudio123)
 ## Email
 hostudio.hopybox@foxmail.com
-
```

### Comparing `HOPYBOX-1.6.7/LICENSE` & `hopybox-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HOPYBOX-1.6.7/PKG-INFO` & `hopybox-1.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: HOPYBOX
-Version: 1.6.7
-Summary: This is an open source, practical command Python box
+Version: 1.7.0
+Summary: This is an open source, practical command Python box.
 Home-page: https://github.com/HOStudio123/HOPYBOX
 Author: ChenJinlin
 Author-email: hostudio.hopybox@foxmail.com
 License: GPL-3.0-or-later
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: filetype
+Requires-Dist: yagmail
+Requires-Dist: rich
+Requires-Dist: bs4
+Requires-Dist: chardet
+Requires-Dist: psutil>=5.8.0
 
 # HOPYBOX
 This is an open source, practical command python box
 ## Introduce
 This is an open source, practical command python box, since it is made in python language, so I named it **HOPYBOX**.
 ## Installing
 Install with `pip` or your favorite PyPI package manager.
@@ -46,32 +52,25 @@
 ## Import method
 ```python
 >>>import hopybox
 ```
 ## Usage (How to use)
 See help built in the program
 ```sh
-HOPYBOX/Command:help
+HOPYBOX/Program:help
 ```
 ## Update version
 Enter in the `HOPYBOX` console:
 ```sh
-HOPYBOX/Command:check version
+HOPYBOX/Program:update
 ```
 or like these
 ```sh
 $ pip install -U HOPYBOX
 ```
 ```sh
 $ pip install -U hopybox
 ```
-```sh
-HOPYBOX/Command:install HOPYBOX
-```
-```sh
-HOPYBOX/Command:install hopybox
-```
 ## Github
 [HOStudio123](https://github.com/HOStudio123)
 ## Email
 hostudio.hopybox@foxmail.com
-
```

### Comparing `HOPYBOX-1.6.7/README.md` & `hopybox-1.7.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -26,31 +26,25 @@
 ## Import method
 ```python
 >>>import hopybox
 ```
 ## Usage (How to use)
 See help built in the program
 ```sh
-HOPYBOX/Command:help
+HOPYBOX/Program:help
 ```
 ## Update version
 Enter in the `HOPYBOX` console:
 ```sh
-HOPYBOX/Command:check version
+HOPYBOX/Program:update
 ```
 or like these
 ```sh
 $ pip install -U HOPYBOX
 ```
 ```sh
 $ pip install -U hopybox
 ```
-```sh
-HOPYBOX/Command:install HOPYBOX
-```
-```sh
-HOPYBOX/Command:install hopybox
-```
 ## Github
 [HOStudio123](https://github.com/HOStudio123)
 ## Email
 hostudio.hopybox@foxmail.com
```

### Comparing `HOPYBOX-1.6.7/hopybox/caculate.py` & `hopybox-1.7.0/hopybox/caculate.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,9 +80,9 @@
   except ValueError as e:
     Error_pta('ValueError','Command',str(e),'triangle …')
   except UnicodeEncodeError as e:
     Error_pta('UnicodeEncodeError','Command',str(e),'triangle …')
 
 #Other calculations
 
-def pi_print():
+def pi():
   print('\033[92m'+str(math.pi))
```

### Comparing `HOPYBOX-1.6.7/hopybox/clear.py` & `hopybox-1.7.0/hopybox/clear.py`

 * *Files identical despite different names*

### Comparing `HOPYBOX-1.6.7/hopybox/dirtree.py` & `hopybox-1.7.0/hopybox/tree_dir.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-import os
-import rich
+import os,rich
 from rich.text import Text
 from rich.tree import Tree
+from rich.console import Console
+
+console = Console()
+max_level = None
+no_recursion_calc = None
 
 def get_file_size(file):
   try:
     return os.path.getsize(file)
   except:
     pass
 
 def format_file_size(size):
   if size is None:
-    return "Error:No permission"
+    return 'Failed'
   num = 0
   while size > 1024:
     size /= 1024
     num += 1
-    unit = ["IB", "KIB", "MIB", "GIB", "TIB" ,"PIB"]
-    return f"{size:.2f}".rstrip(".0").zfill(1) + unit[num]
-
-
-def walk_dir(path, tree, level=0) -> int:
-    global max_level, no_recursion_calc
-    try:
-        listdir = os.listdir(path)
-    except:
-        return 0
-    total_size = 0
-    for file in listdir:
-        if no_recursion_calc and level >= max_level:
-            continue
-        file_path = os.path.join(path, file)
-        if os.path.isdir(file_path):
-            parent = None
-            if level < max_level:
-                parent = tree.add(f"[magenta]{file}")
-            size = walk_dir(file_path, parent, level + 1)
-            if size and parent:
-                parent.label += f"[yellow] [{format_file_size(size)}]"
-        else:
-            size = get_file_size(file_path)
-            if level < max_level:
-                text_filename = Text(file, "green")
-                text_filename.highlight_regex(r"\.[^.]+$", "")
-                text_filename.append(
-                    f" ({format_file_size(size)})", "\033[92m")
-                tree.add(text_filename)
-        if size:
-            total_size += size
-    return total_size
+  unit = ['B','KIB','MIB','GIB','TIB','PIB']
+  return f"{size:.2f}".rstrip(".0").zfill(1)+unit[num]
 
 
-max_level = None
-no_recursion_calc = None
-def tree_dir(path, m_level=7, no_calc=False):
+def walk_dir(path,tree,level=0):
   global max_level, no_recursion_calc
-  max_level = m_level
-  no_recursion_calc = no_calc
-  tree = "\033[92m{os.path.abspath(path)}"
-  size = walk_dir(path, tree)
-  tree.label += f"\033[92m[{format_file_size(size)}]"
-  print(tree)
+  try:
+    listdir = os.listdir(path)
+  except:
+    return 0
+  total_size = 0
+  for file in listdir:
+    if no_recursion_calc and level >= max_level:
+      continue
+    file_path = os.path.join(path, file)
+    if os.path.isdir(file_path):
+      parent = None
+      if level < max_level:
+        parent = tree.add(f'[bright_magenta]{file}')
+      size = walk_dir(file_path, parent, level + 1)
+      if size and parent:
+        parent.label += f'[bright_yellow] ({format_file_size(size)})'
+    else:
+      size = get_file_size(file_path)
+      if level < max_level:
+        text_filename = Text(file,'bright_green')
+        text_filename.highlight_regex(r'\.[^.]+$','bold blue')
+        text_filename.append(f' ({format_file_size(size)})','bright_cyan')
+        tree.add(text_filename)
+    if size:
+      total_size += size
+  return total_size
+
+def tree(path,m_level=7):
+  with console.status('\033[96mLoading paths …\033[0m'):
+    global max_level, no_recursion_calc
+    max_level = m_level
+    no_recursion_calc = False
+    tree = Tree(f'[bright_magenta]{os.path.abspath(path)}')
+    size = walk_dir(path, tree)
+    tree.label += f' [bright_yellow]({format_file_size(size)})'
+    rich.print(tree)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HOPYBOX-1.6.7/hopybox/filetoolbox.py` & `hopybox-1.7.0/hopybox/filetool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import os
 import os.path
 import filetype
 import zipfile,tarfile
 import time
 from rich import console,syntax
-from .hopter import Error_pta,Error_ptb,Tip_pta
-from .tree_dir import tree_dir
+from .hopter import error_cross,Error_ptb,Tip_pta
+from .tree_dir import tree
 
-def file_information(filename):
-  print('''File-Size:{}B
-File-Dev:{}
-Fie-Nlink:{}
-File-Ino:{}
-File-Mtime:{}
-File-Content:\033[0m'''.format(os.stat(filename).st_size,os.stat(filename).st_dev,os.stat(filename).st_nlink,os.stat(filename).st_ino,time.strftime("%Y/%m/%d %H:%M:%S",time.localtime(os.stat(filename).st_mtime))))
-  with console.Console().status("\033[96mLoading file …\033[0m"):
-    file_open(filename)
+class Filetool:
+  def view():
+    pass
+
+filetool = Filetool()
 
 def read_file(filename):
   if filename:
     try:
       filekind = filetype.guess(filename)
       if filekind is None:
         print('\033[92mFile-Type:text')
         mode = 'r'
         file_information(filename)
+        with console.Console().status("\033[96mLoading file …\033[0m"):
+          file_open(filename)
       else:
         file_type = filekind.extension
         print('\033[92mFile-Type:%s' % file_type)
         if file_type == 'png' or file_type == 'jpg':
           mode = 'rb'
           file_information(filename)
+          with console.Console().status("\033[96mLoading file …\033[0m"):
+            file_open(filename)
         elif file_type == 'zip':
           zip = zipfile.ZipFile(filename)
           print(zip.filename)
           for i in range(len(zip.namelist())):
             print('\033[94m├ '+zip.namelist()[i])
           unfile_answer = input('\033[94mDo you want to unzip to the current directory?(Y/n)')
           while True:
@@ -45,26 +45,25 @@
             elif unfile_answer == 'n':
               break
             else:
               Error_ptb(unfile_answer)
           else:
             pass
     except FileNotFoundError as e:
-      Error_pta('FileNotFoundError','Command',str(e),'open '+filename)
+      error_cross('FileNotFoundError','Command',str(e),'open '+filename)
     except UnicodeDecodeError as e:
-      Error_pta('UnicodeDecodeError','Command',str(e),'open '+filename)
+      error_cross('UnicodeDecodeError','Command',str(e),'open '+filename)
     except IsADirectoryError as e:
-      Error_pta('IsADirectoryError','Command',str(e),'open '+filename)
+      error_cross('IsADirectoryError','Command',str(e),'open '+filename)
     except PermissionError as e:
-      Error_pta('PermissionError','Command',str(e),'open '+filename)
+      error_cross('PermissionError','Command',str(e),'open '+filename)
   else:
-    Error_pta('FileNotFoundError','Command','Please enter a file name','open '+filename)
+    error_cross('FileNotFoundError','Command','Please enter a file name','open '+filename)
 
 def file_open(filename):
-  print('\033[92mFile-Content:\033[0m')
   Console = console.Console()
   file = open(filename,'rb')
   code = file.read().decode('utf-8')
   file.close()
   extension = os.path.splitext(filename)[1]
   if extension == '.py':
     Console.print(syntax.Syntax(code,'python',theme="ansi_dark", line_numbers=True))
@@ -81,11 +80,11 @@
   elif extension == '.js':
     Console.print(syntax.Syntax(code,'javascript',theme="ansi_dark", line_numbers=True))
   else:
     Console.print(syntax.Syntax(code,'text',theme="ansi_dark", line_numbers=True))
 
 def del_file(filename):
   os.system('rm -rf '+filename)
-  Tip_pta('successfully deleted')
+  Tip_pta('Successfully deleted')
 
 def file_size(file):
   tree_dir(file)
```

### Comparing `HOPYBOX-1.6.7/hopybox/headers.py` & `hopybox-1.7.0/hopybox/headers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 def headers_water():
   headers_list = [ 
   { 'User-Agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.5005.78 Safari/537.36' } ,
   { 'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.105 Safari/537.36 Accept ' },
   { 'User-Agent' : 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36' },
-  { 'User-Agent' : 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.64 Safari/537.36 Edg/101.0.1210.53' },  
+  { 'User-Agent' : 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.64 Safari/537.36 Edg/101.0.1210.53' }, 
+  { 'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.88 Safari/537.36' } 
 ]
   return random.choice(headers_list)
```

### Comparing `HOPYBOX-1.6.7/hopybox/helps.py` & `hopybox-1.7.0/hopybox/helps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from .version import version_code as vcd
-def helps_print():
-  return '''\033[96mHOPYBOX %s Helps Documentation\n(HOPYBOX %s 帮助文档)\033[0m
+print('''HOPYBOX %s Helps Documentation\n(HOPYBOX %s 帮助文档)\033[0m
   
-\033[94mEdited in August 20, 2022\n(编辑于2022年8月20日)\033[0m
+\033[94mEdited in June 19, 2023\n(编辑于2023年月19日)\033[0m
 
 \033[92mAll Chinese and English are translated by Google, and this program is written in UTF-8 encoding.\n(所有中英文均由谷歌翻译,并且本程序采用UTF-8编码编写)
 
 This program supports Chinese and English.\n(这个程序支持中文与英文)
 
-\033[93m[1]Command mode
+\033[93m[1]Command mode (指令模式)
 Initiate this mode method:Enter the command 'take command'
 (启动此模式方法:输入“take command”)\033[0m\033[95m
  ⎛ help {module/package} # Get helps of module
  ⎜ id {text} # Getting id of text
  ⎜ run {filename} # Running file of python
  ⎜ download {url} # Download web pages or files 
  ⎜ hoget {url} # Program url get 
  ⎜ bowget {url} # Initiate your browser and visit url 
  ⎜ qqname {qqnumber} # Get the name for the entered QQ 
  ⎜ qqhead {qqnumber} # Get the avatar of the input QQ 
- ⎜ email {mail} # Python send mail
+ ⎜ email {email address} # Use Python to send mail, '{}' fill in the email address of the person you want to send to
  ⎜ install {package} # Install the latest package on PyPI
  ⎜ uninstall {package} # Uninstall package
  ⎜ del {filename} # Delete file or path
  ⎜ check version # Check program version
  ⎜ ipget {ip} # Look for the IPV4's address 
- ⎜ weather {city} # Get the weather for the entered city
  ⎜ open {filename} # Open the file 
  ⎜ caculate {formula} # Even support absolute values and root calculations(√{x} and |{x}|) 
  ⎜ triangle {formula} # Trigonometric functions, Current supported recognition formats are sin, cos, tan, asin, acos and atan
  ⎜ pi # Return pi 
  ⎜ pkg list # List of installed packages
  ⎜ fps # Current equipment running speed 
  ⎜ translate {word} # YouDao translate 
@@ -38,25 +35,24 @@
  ⎜ tree {filename} # Display the file information in the directory in the form of a tree (Example:tree /sdcard)
  ⎜ scan {pathname} {extension} # Look for specified suffix files in the specified path directory (Example:scan /sdcard .apk)
  ⎜ clear {pathname} {extension} # Clean up all object files in this path (Example:clear /sdcard .cache)
  ⎜ update {version} To get a update log about the version object (Example:update %s)
  ⎜ clear # Clear console 
  ⎝ exit # Exit 
 
-\033[0m\033[93m[2]System mode
+\033[0m\033[93m[2]System mode (系统模式)
 Initiate this mode method:Enter the command 'take system'
 (启动此模式方法:输入“take system”)\033[0m\033[95m
  ⎛ {command} # Python terminal's command 
  ⎜ clear # Clear console 
  ⎝ exit # Exit 
 
-\033[0m\033[93m[3]Python mode 
-Initiate this mode method:Enter the command 'take python'
-(启动此模式方法:输入“take python”)\033[0m\033[95m
+\033[0m\033[93m[3]Python mode
+Initiate this mode method:Enter the command 'take python'\033[0m\033[95m
  ⎛ debug {command} # Debugging simple python code
  ⎜ clear # Clear console 
  ⎜ interpreter # interpreter of python
- ⎜ ipython # Interpreter of ipython
+ ⎜ python3 # interpreter of python
  ⎝ python # Interpreter of python
 
-\033[0m\033[92mAt last
-If you have any questions, please contact the developer as hostudio.hopybox@foxmail.com.''' % (vcd,vcd,vcd)
+\033[0m\033[92m[4]Others (其它)
+If you have any questions, please contact the developer as\033[1;93m hostudio.hopybox@foxmail.com \033[0m.\'\'' % (vcd,vcd,vcd)''')
```

### Comparing `HOPYBOX-1.6.7/hopybox/qqget.py` & `hopybox-1.7.0/hopybox/qqget.py`

 * *Files identical despite different names*

### Comparing `HOPYBOX-1.6.7/hopybox/scan.py` & `hopybox-1.7.0/hopybox/scan.py`

 * *Files identical despite different names*

### Comparing `HOPYBOX-1.6.7/hopybox/urlget.py` & `hopybox-1.7.0/hopybox/connect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 import os
 import time
 import chardet
-import requests as visit
 import webbrowser
-from requests.exceptions import *
-from .headers import headers_water
-from rich import console,syntax
-from .hopter import Error_pta,Error_ptb,Tip_pta
 import requests
+from rich import syntax
+from rich.console import Console
+from bs4 import BeautifulSoup as soup
+from .headers import headers_water
+from .prompt import tip_tick
+from .prompt import error_cross
+
+# Disable Security Request Warning
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
+from requests.packages.urllib3.exceptions import InsecurePlatformWarning
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
+requests.packages.urllib3.disable_warnings(InsecurePlatformWarning)
 
-CoCo = console.Console()
+console = Console()
 headers = headers_water()
 
+class Choget:
+  def __init__(self):
+    pass
+  def time(self,state):
+    if state:
+      start_time = time.time()
+    else:
+      return time.time() - start_time
+    
+    
 def hoget(url):
   global headers
-  res = 0
   start_time = time.time()
   try:
-    with console.Console().status("\033[96mLoading url …"):
-      res = visit.get(url,headers=headers,stream=True,verify=False)
+    with Console().status("\033[96mLoading URL …"):
+      res = requests.get(url,headers=headers,stream=True,verify=False)
     if res.status_code == 200:
       end_time = time.time()
       total_time = end_time - start_time
-      print('\033[32mUrl-Url:\033[0m\033[94m\n'+res.url) 
-      print('\033[32mUrl-Time:\033[0m\033[94m\n'+str(total_time)+'S')
-      with console.Console().status("\033[96mLoading information …"):
-        print('\033[32mUrl-Szie:\033[0m\033[94m\n'+str(len(res.text))+'B')
-      print('\033[32mUrl-Cookies:\033[0m\033[94m')
-      for name, value in visit.utils.dict_from_cookiejar(res.cookies).items():
-        print('├ %s:%s ' % (name, value))
-      if not visit.utils.dict_from_cookiejar(res.cookies):
+      print('\033[32mURL-URL:\033[0m\033[94m\n'+res.url) 
+      print('\033[32mURL-Time:\033[0m\033[94m\n'+str(total_time)+'S')
+      with Console().status("\033[96mLoading information …"):
+        print('\033[32mURL-Szie:\033[0m\033[94m\n'+str(len(res.text))+'B')
+      print('\033[32mURL-Cookies:\033[0m\033[94m')
+      for name, value in requests.utils.dict_from_cookiejar(res.cookies).items():
+        print('* %s:%s ' % (name, value))
+      if not requests.utils.dict_from_cookiejar(res.cookies):
         print(None)
-      print('\033[32mUrl-Headers:\033[0m\033[94m')
+      print('\033[32mURL-Headers:\033[0m\033[94m')
       for name, value in res.headers.items():
-        print('├ %s:%s ' % (name, value))
-      print('\033[32mUrl-Requests-Headers:\033[0m\033[94m')
+        print('* %s:%s ' % (name, value))
+      print('\033[32mURL-Requests-Headers:\033[0m\033[94m')
       for name, value in res.request.headers.items():
-        print('├ %s:%s ' % (name, value))
-      print('\033[92mUrl-Code-Coding:\033[0m\033[94m\n'+str(res.encoding))
+        print('* %s:%s ' % (name, value))
+      print(f'\033[92mURL-Code-Coding:\033[0m\033[94m\n{res.encoding}')
       if res.encoding != None:
-        print('\033[92mUrl-Code-Type:\033[0m\033[94m\nGeneral network\033[0m')
+        print('\033[92mURL-Code-Type:\033[0m\033[94m\nGeneral network\033[0m')
+        print()
         res.encoding = chardet.detect(res.content)['encoding']
-        with console.Console().status("\033[96mLoading text …\033[0m"):
-          print('\033[92mUrl-Code-Content:\033[0m')
-          CoCo.print(syntax.Syntax(res.text,'html',theme="ansi_dark", line_numbers=True))
+        print('\033[92mURL-Code-Content:\033[0m')
+        console.print(syntax.Syntax(res.text,'html',theme="ansi_dark", line_numbers=True))
       else:
-        print('\033[92mUrl-Code-Type:\033[0m\033[94m\nOther network')
-        with console.Console().status("\033[96mLoading text …\033[0m"):
-          print('\033[92mUrl-Code-Content:\033[0m')
-          CoCo.print(syntax.Syntax(str(res.content),'html',theme="ansi_dark", line_numbers=True))
+        print('\033[92mURL-Code-Type:\033[0m\033[94m\nOther network\033[0m')
+        print('\033[92mURL-Code-Content:\033[0m')
+        console.print(syntax.Syntax(str(res.text),'html',theme='ansi_dark', line_numbers=True))
     else:
-      Error_pta(str(res.status_code)+'Error','Command',str(res.status_code)+' Error in request','hoget …')
-  except HTTPError as e:
-    Error_pta('HTTPError','Command',str(e),'hoget …')
-  except SSLError as e:
-    Error_pta('SSLError','Command',str(e),'hoget …')
-  except ConnectionError as e:
-    Error_pta('ConnectionError','Command',str(e),'hoget …')
-  except RequestException as e:
-    Error_pta('RequestException','Command',str(e),'hoget …')
- 
-def browser_get(url):
-  webbrowser.open(url) 
-  Tip_pta('The program has opened the URL in the browser')
+      error_cross(f'{res.status_code} Error','Command',f'{res.status_code} Error in request',f'hoget {url}')
+  except Exception as e:
+    error_cross(e.__class__.__name__,'Command',e,f'hoget {url}')
+    
+def browser(url):
+  try:
+    webbrowser.open(url) 
+    tip_tick('The program has opened the URL in the browser')
+  except Exception as e:
+    error_cross('OpenBrowserError','Command',e,f'browget {url}')
```

### Comparing `HOPYBOX-1.6.7/setup.py` & `hopybox-1.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 '''
             Copyright (c) 2022 HOStudio123(ChenJinlin) ,
                       All Rights Reserved.
 '''
+
 # -*- coding:utf-8 -*-
+
 import setuptools
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name = 'HOPYBOX',
-    version = '1.6.7',
+    version = '1.7.0',
     author = 'ChenJinlin',
     author_email = 'hostudio.hopybox@foxmail.com',
-    description = 'This is an open source, practical command Python box',
+    description = 'This is an open source, practical command Python box.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/HOStudio123/HOPYBOX',
     packages = setuptools.find_packages(),
     license = 'GPL-3.0-or-later',
     classifiers = [
         'Programming Language :: Python :: 3',
@@ -24,14 +26,22 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
     entry_points = {
             "console_scripts":[
-                "hopybox = hopybox:pattern",
-                "HOPYBOX = hopybox:pattern",
+                "hopybox = hopybox.__main__:start",
+                "HOPYBOX = hopybox.__main__:start",
                 ]
             },
     python_requires = '>=3.7',
-    install_requires = ['wget>=3.2','bs4==0.0.1','requests','lxml>=4.6.3','filetype','yagmail','rich>=12.5.1','chardet>=4.0.0','ipython>=8.3.0']    
+    install_requires = [
+        'requests',
+        'filetype',
+        'yagmail',
+        'rich',
+        'bs4',
+        'chardet',
+        'psutil>=5.8.0'
+    ]    
 )
```

