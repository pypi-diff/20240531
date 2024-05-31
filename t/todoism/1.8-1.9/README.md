# Comparing `tmp/todoism-1.8.tar.gz` & `tmp/todoism-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoism-1.8.tar", last modified: Mon Mar 18 17:49:37 2024, max compression
+gzip compressed data, was "todoism-1.9.tar", last modified: Mon Mar 18 18:45:56 2024, max compression
```

## Comparing `todoism-1.8.tar` & `todoism-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 17:49:37.166793 todoism-1.8/
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      205 2024-03-18 17:49:37.165794 todoism-1.8/PKG-INFO
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       49 2024-03-11 12:32:59.000000 todoism-1.8/README.md
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       38 2024-03-18 17:49:37.166793 todoism-1.8/setup.cfg
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      527 2024-03-18 17:49:32.000000 todoism-1.8/setup.py
-drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 17:49:37.159793 todoism-1.8/test/
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     1518 2024-03-15 15:40:49.000000 todoism-1.8/test/test.py
-drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 17:49:37.162793 todoism-1.8/todoism/
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-17 03:45:13.000000 todoism-1.8/todoism/__init__.py
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     6143 2024-03-18 17:32:55.000000 todoism-1.8/todoism/main.py
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     3197 2024-03-18 17:46:08.000000 todoism-1.8/todoism/print.py
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     1271 2024-03-16 15:18:54.000000 todoism-1.8/todoism/task.py
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     4448 2024-03-18 17:32:19.000000 todoism-1.8/todoism/utils.py
-drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 17:49:37.164794 todoism-1.8/todoism.egg-info/
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      205 2024-03-18 17:49:37.000000 todoism-1.8/todoism.egg-info/PKG-INFO
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      275 2024-03-18 17:49:37.000000 todoism-1.8/todoism.egg-info/SOURCES.txt
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        1 2024-03-18 17:49:37.000000 todoism-1.8/todoism.egg-info/dependency_links.txt
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       71 2024-03-18 17:49:37.000000 todoism-1.8/todoism.egg-info/entry_points.txt
--rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        8 2024-03-18 17:49:37.000000 todoism-1.8/todoism.egg-info/top_level.txt
+drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 18:45:56.626452 todoism-1.9/
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      205 2024-03-18 18:45:56.624452 todoism-1.9/PKG-INFO
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       49 2024-03-11 12:32:59.000000 todoism-1.9/README.md
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       38 2024-03-18 18:45:56.627452 todoism-1.9/setup.cfg
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      527 2024-03-18 18:45:52.000000 todoism-1.9/setup.py
+drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 18:45:56.619452 todoism-1.9/test/
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     1518 2024-03-15 15:40:49.000000 todoism-1.9/test/test.py
+drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 18:45:56.621452 todoism-1.9/todoism/
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-17 03:45:13.000000 todoism-1.9/todoism/__init__.py
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     6367 2024-03-18 18:43:20.000000 todoism-1.9/todoism/main.py
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     3197 2024-03-18 17:46:08.000000 todoism-1.9/todoism/print.py
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     1271 2024-03-16 15:18:54.000000 todoism-1.9/todoism/task.py
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)     4484 2024-03-18 18:44:27.000000 todoism-1.9/todoism/utils.py
+drwxr-xr-x   0 qichenliu  (1000) qichenliu  (1000)        0 2024-03-18 18:45:56.623452 todoism-1.9/todoism.egg-info/
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      205 2024-03-18 18:45:56.000000 todoism-1.9/todoism.egg-info/PKG-INFO
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)      275 2024-03-18 18:45:56.000000 todoism-1.9/todoism.egg-info/SOURCES.txt
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        1 2024-03-18 18:45:56.000000 todoism-1.9/todoism.egg-info/dependency_links.txt
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)       71 2024-03-18 18:45:56.000000 todoism-1.9/todoism.egg-info/entry_points.txt
+-rw-r--r--   0 qichenliu  (1000) qichenliu  (1000)        8 2024-03-18 18:45:56.000000 todoism-1.9/todoism.egg-info/top_level.txt
```

### Comparing `todoism-1.8/setup.py` & `todoism-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='todoism',
-    version='1.8',
+    version='1.9',
     packages=find_packages(exclude=['test']),
     package_dir={'todoism': 'todoism'},
     entry_points={
         'console_scripts': [
             'todo=todoism.main:main',
             'todoism=todoism.main:main',
         ],
```

### Comparing `todoism-1.8/test/test.py` & `todoism-1.9/test/test.py`

 * *Files identical despite different names*

### Comparing `todoism-1.8/todoism/main.py` & `todoism-1.9/todoism/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 start = task_cnt - (end - start - 1)
                 end = task_cnt
             else:
                 end = end + 1
             stdscr.erase()
             print_status_bar(stdscr, done_cnt, task_cnt)
             print_tasks(stdscr, task_list, current_id, start, end)
-            stdscr.addstr(window_height - 1 if task_cnt >= window_height - 1 else task_cnt + 1, 3, f"{task_cnt + 1}. ")
+            stdscr.addstr(window_height - 1 if task_cnt >= window_height - 1 else task_cnt + 1, 3, f"{task_cnt + 1}.{' ' if task_cnt + 1 >= 10 else ' ' * 2}")
             stdscr.refresh()
             
             # Add a new task
             new_task_description = edit(stdscr, create_new_task(task_cnt + 1), add_mode)               
             if new_task_description:
                 new_id = task_cnt + 1
                 task_list = add_new_task(task_list, new_id, new_task_description)
@@ -87,17 +87,21 @@
             if task_list:
                 done_list.append(task_list[current_id - 1])
                 task_list[current_id - 1]['status'] = not task_list[current_id - 1]['status']  
                 done_cnt = done_cnt + 1 if task_list[current_id - 1]['status'] is True else done_cnt - 1
                 save_tasks(task_list, tasks_file_path)
         elif key == ord('e'):
             curses.echo()
-            curses.curs_set(1)            
+            curses.curs_set(1)
             stdscr.move(current_id if current_id <= window_height - 1 else window_height - 1, len(task_list[current_id - 1]['description']) + indent)
             task_list[current_id - 1]['description'] = edit(stdscr, task_list[current_id - 1], edit_mode)
+            # delete the task if it was edited to empty
+            if task_list[current_id - 1]['description'] == "":
+                del task_list[current_id - 1]
+                reid(task_list)
             save_tasks(task_list, tasks_file_path)
             curses.curs_set(0)
             curses.noecho()        
         elif key == ord('f'):
             task_list[current_id - 1]['flagged'] = not task_list[current_id - 1]['flagged'] 
         elif key == ord('h'):
             stdscr.addstr(len(done_list) + 1, 0, "Completed Tasks:")
```

### Comparing `todoism-1.8/todoism/print.py` & `todoism-1.9/todoism/print.py`

 * *Files identical despite different names*

### Comparing `todoism-1.8/todoism/task.py` & `todoism-1.9/todoism/task.py`

 * *Files identical despite different names*

### Comparing `todoism-1.8/todoism/utils.py` & `todoism-1.9/todoism/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import curses
 from datetime import datetime
 from .task import *
 from .print import *
 
 
-indent = 6
+indent = 7
 description_length = 75
 task_highlighting_color = curses.COLOR_BLUE
 
 def get_arg(argv):
     if len(argv) > 1:
         return argv[1]
     else:
@@ -58,23 +58,25 @@
             not_flagged = []
             for t in task_list:
                 if t['flagged'] is True:
                     flagged_tasks.append(t)
                 else:
                     not_flagged.append(t)
             task_list = flagged_tasks + not_flagged
+            reid(task_list)
         elif category == 'd':
             done_tasks = []
             not_done = []
             for t in task_list:
                 if t['status'] == True:
                     done_tasks.append(t)
                 else:
                     not_done.append(t)
             task_list = not_done + done_tasks
+            reid(task_list)
     elif command == "group":
         pass
     elif command.startswith("setcolor "):
         color = command[9:]
         if color == "red":
             task_highlighting_color = curses.COLOR_RED
         elif color == "blue":
@@ -103,23 +105,22 @@
         if ch == 10: # Enter to complete
             break
         elif ch == curses.KEY_LEFT:
             stdscr.move(y, indent if x <= indent else x - 1) # cursor remains still
         elif ch == curses.KEY_RIGHT:
             stdscr.move(y, x + 1 if x < indent + len(task['description']) else indent + len(task['description']))
         elif ch == curses.KEY_BACKSPACE or ch == 127: # delete
-            if x <= 6:
+            if x <= 7:
                 stdscr.move(y, indent) # cursor remains still
                 continue
             # -1 because i am deleting the char before the cursor
             task['description'] = task['description'][:x - indent - 1] + task['description'][x - indent:]
             print_task_mode(stdscr, task, y, mode)
             stdscr.move(y, x - 1)
         elif 32 <= ch < 127: # printable char
             task['description'] = task['description'][:x - indent] + chr(ch) + task['description'][x - indent:]
             print_task_mode(stdscr, task, y, mode)
             stdscr.move(y, x + 1)        
         elif ch == 27 and mode == add_mode: # todo: too slow
             return ""
     return task['description']
     # todo sound
-    # selected color
```

