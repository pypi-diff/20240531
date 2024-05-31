# Comparing `tmp/almax_common-0.9.4.tar.gz` & `tmp/almax_common-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.9.4.tar", last modified: Wed May 29 22:35:05 2024, max compression
+gzip compressed data, was "almax_common-0.9.5.tar", last modified: Fri May 31 14:03:22 2024, max compression
```

## Comparing `almax_common-0.9.4.tar` & `almax_common-0.9.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:35:05.758096 almax_common-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:35:05.758096 almax_common-0.9.4/Common/
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-29 22:34:38.000000 almax_common-0.9.4/Common/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 22:34:38.000000 almax_common-0.9.4/Common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:35:05.758096 almax_common-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 22:34:38.000000 almax_common-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:35:05.758096 almax_common-0.9.4/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:35:05.000000 almax_common-0.9.4/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 22:35:05.000000 almax_common-0.9.4/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:35:05.000000 almax_common-0.9.4/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 22:35:05.000000 almax_common-0.9.4/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:35:05.758096 almax_common-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-29 22:34:38.000000 almax_common-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 14:03:22.778973 almax_common-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 14:02:58.000000 almax_common-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:03:22.778973 almax_common-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-31 14:02:58.000000 almax_common-0.9.5/setup.py
```

### Comparing `almax_common-0.9.4/Common/Utils.py` & `almax_common-0.9.5/Utils/FileSystem.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-import os;
-from datetime import datetime;
-
-now = datetime.now();
-
-def CalculateDestinationFolder(source: str) -> str:
-    destination = CleanPath(source, '/').split('/');
-
-    if  destination[0] == 'H:':
-        destination[0] = 'Q:';
-    elif destination[0] == 'C:':
-        destination[3] = "Test";
-    else:
-        return '';
-
-    return '/'.join(destination);
+import os, shutil;
 
 def CleanPath(path: str, cleanString: str) -> str:
     return path.replace("\\", cleanString).replace('/', cleanString);
 
 def GetSubFolders(folder: str) -> list:
     return [ f.path for f in os.scandir(folder) if f.is_dir() ];
 
@@ -62,73 +47,91 @@
 def GetFolderFiles(folder: str) -> list:
     return [ f.path for f in os.scandir(folder) if f.is_file() ];
 
 def HasFiles(folder: str) -> bool:
     files = os.listdir(folder);
     return len(files) > 0;
    
-def GetRobocopyCommand(source: str, elaboration: int, operation:int, onlyFiles=False, customFolder: str = '', checkIfExists: list = []) -> list:
-    destination = CalculateDestinationFolder(source);
+def GetRobocopyCommand(source: str, elaboration: int = 8, operation:int = 0, onlyFiles=False, customFolder: str = '', checkIfExists: list = [], CalculateDestinationFolder: function = None) -> list:
+    if CalculateDestinationFolder == None:
+        return None;
+    destination = lambda:CalculateDestinationFolder(source);
     destinationLog = destination.split("/");
     destinationLog = destinationLog[-1];
 
     logPath = f"{customFolder}{destinationLog.replace(":", "").replace("/", "_") + ("_Files" if onlyFiles else "") + ".log"}";
     i = 0;
     while logPath in checkIfExists:
         i+=1;
         logPath = f"{customFolder}{destinationLog.replace(":", "").replace("/", "_").replace(" ", "_") + ("_Files" if onlyFiles else "") + "_" + str(i) + ".log"}";
     checkIfExists.append(logPath);
 
-    command = [
-        "Robocopy",
-        source,
-        destination,
-        f"/LOG:{logPath}"
-    ];
-
-    if elaboration in [32, 64, 128]:
-        command.append(f"/MT:{elaboration}");
-    if not onlyFiles:
-        command.append("/E");
-    if operation == 1:
-        command.append("/MOVE");
+    if os.path.isfile(source):
+        source = source.split("/");
+        if source[-1] == '':
+            source = source[:-1];
+        fileName = source[-1];
+        source = source[:-1];
+        source = "/".join(source);
+
+        destination = destination.split("/");
+        if destination[-1] == '':
+            destination = destination[:-1];
+        destination = destination[:-1];
+        destination = "/".join(destination);
+
+        command = [
+            "Robocopy",
+            source,
+            destination,
+            fileName,
+            f"/LOG:{logPath}"
+        ];
+    else:
+        command = [
+            "Robocopy",
+            source,
+            destination,
+            f"/LOG:{logPath}"
+        ];
+
+        if elaboration in [32, 64, 128]:
+            command.append(f"/MT:{elaboration}");
+        if not onlyFiles:
+            command.append("/E");
+        if operation == 1:
+            command.append("/MOVE");
 
     return [command, checkIfExists];
 
-def PrintBytes(size: int) -> str:
-    if size > 1024:
-        size = round(size / 1024, 2);
-        if(size > 1024):
-            size = round(size / 1024, 4);
-            if(size > 1024):
-                size = round(size / 1024, 8);
-                if(size > 1024):
-                    size = round(size / 1024, 16);
-                    return f"{size} TB";
-                else:
-                    return f"{size} GB";
-            else:
-                return f"{size} MB";
-        else:
-            return f"{size} KB";
-   
-    return f"{size} B";
-
-def CalculateTime(start: datetime):
-    return datetime.now() - start;
-
-def TimeToString(time: datetime) -> str:
-    seconds = time.total_seconds();
-    minutes = seconds // 60;
-    hours = minutes // 60;
-    days = hours // 24;
-    return f"{round(days)} Days = {round(hours)} Hours = {round(minutes)} Minutes = {round(seconds, 2)} Seconds";
-
-def CheckStringInFile(file_path, target_string):
-    try:
-        with open(file_path, 'r') as file:
-            for line in file:
-                if target_string in line:
-                    return True;
+def GetHighestPaths(paths: list) -> list:
+    paths.sort();
+    highest_paths = [paths[0]];
+
+    for path in paths[1:]:
+        if not path.startswith(highest_paths[-1]):
+            highest_paths.append(path);
+
+    return highest_paths;
+
+def FolderHasContent(folder: str) -> bool:
+    if os.path.exists(folder) and os.listdir(folder):
+        return True;
+    else:
         return False;
-    except FileNotFoundError:
-        return False;
+
+def FolderDeleteContents(folder: str) -> list:
+    bytes(folder, "utf-8").decode("unicode_escape");
+    deleted = [];
+    fails = False;
+    for filename in os.listdir(folder):
+        try:
+            file_path = os.path.join(folder, filename);
+            if os.path.isfile(file_path) or os.path.islink(file_path):
+                os.unlink(file_path);
+            elif os.path.isdir(file_path):
+                shutil.rmtree(file_path);
+            deleted.append(f"Success: {file_path}");
+        except Exception as e:
+            deleted.append(f"Fail: {e}; Path: {file_path}");
+            fails = True;
+    return [fails, deleted];
```

