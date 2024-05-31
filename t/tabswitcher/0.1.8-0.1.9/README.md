# Comparing `tmp/tabswitcher-0.1.8.tar.gz` & `tmp/tabswitcher-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.8.tar", last modified: Wed May 29 20:56:24 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.9.tar", last modified: Thu May 30 06:13:42 2024, max compression
```

## Comparing `tabswitcher-0.1.8.tar` & `tabswitcher-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.205737 tabswitcher-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.209737 tabswitcher-0.1.8/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/runLogger.vbs
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:13:42.615339 tabswitcher-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-30 06:13:42.615339 tabswitcher-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:13:42.615339 tabswitcher-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:13:42.611339 tabswitcher-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:13:42.611339 tabswitcher-0.1.9/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:13:42.615339 tabswitcher-0.1.9/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/runLogger.vbs
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/assets/uninstall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 06:13:38.000000 tabswitcher-0.1.9/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:13:42.615339 tabswitcher-0.1.9/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 06:13:42.000000 tabswitcher-0.1.9/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.8/LICENCE` & `tabswitcher-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/PKG-INFO` & `tabswitcher-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.8/README.md` & `tabswitcher-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/setup.py` & `tabswitcher-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.8',
+    version='0.1.9',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.1.8/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.9/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.9/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/Settings.py` & `tabswitcher-0.1.9/src/tabswitcher/Settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,19 +90,19 @@
     
     def get_load_bookmarks(self):
         try:
             return self.config.getboolean('Functions', 'LoadBookmarks')
         except:
             return self.defaults['Functions']['LoadBookmarks']
     
-    def get_use_hotkey(self):
+    def get_use_hotkeys(self):
         try:
-            return self.config.getboolean('Functions', 'UseHotKey')
+            return self.config.getboolean('Functions', 'UseHotKeys')
         except:
-            return self.defaults['Functions']['UseHotKey']
+            return self.defaults['Functions']['UseHotKeys']
     
     def get_hotkey_open(self):
         try:
             return self.config.get('Functions', 'HotkeyOpen')
         except:
             return self.defaults['Functions']['HotkeyOpen']
```

### Comparing `tabswitcher-0.1.8/src/tabswitcher/Tab.py` & `tabswitcher-0.1.9/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/TabList.py` & `tabswitcher-0.1.9/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.9/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/__main__.py` & `tabswitcher-0.1.9/src/tabswitcher/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -324,24 +324,33 @@
             vbs_path = os.path.join(startup_folder, "runLogger.vbs")
             shutil.copy2(startup_script, vbs_path)
             subprocess.Popen(["cscript", vbs_path])
         else:
             batch_script = os.path.join(script_dir, "assets", "install.sh")
             subprocess.run(["sh", batch_script])
 
-
+    elif len(sys.argv) > 1 and sys.argv[1] == "--uninstall":
+        if platform.system() == "Windows":
+            startup_folder = os.path.join(os.environ["APPDATA"], r"Microsoft\Windows\Start Menu\Programs\Startup")
+            vbs_path = os.path.join(startup_folder, "runLogger.vbs")
+            if os.path.exists(vbs_path):
+                os.remove(vbs_path)
+        else:
+            batch_script = os.path.join(script_dir, "assets", "uninstall.sh")
+            subprocess.run(["sh", batch_script])
     elif len(sys.argv) > 1 and sys.argv[1] == "--version":
         version = pkg_resources.get_distribution("tabswitcher").version
         print(f"Version: {version}")
     elif len(sys.argv) > 1 and sys.argv[1] == "--settings":
         open_settings()
     elif len(sys.argv) > 1 and sys.argv[1] == "--help":
         print("tabswitcher: No arguments will just open the switcher window")
         print("--startlogger\tRun the tab logger that will save the currenlty active tab")
         print("--install\tWill make sure the logger is startet on system start")
+        print("--uninstall\tWill make sure remove the logger from the start of the system")
         print("--latest\tWill return of the tab id of the last 10 active tabs you can also add a index as secons parameter")
         print("--version\tGet the version number")
         print("--help\t\tSee this page")
     else:
         open_tabswitcher()
 
 if __name__ == "__main__":
```

### Comparing `tabswitcher-0.1.8/src/tabswitcher/actions.py` & `tabswitcher-0.1.9/src/tabswitcher/actions.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.9/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.9/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.9/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/brotab.py` & `tabswitcher-0.1.9/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/colors.py` & `tabswitcher-0.1.9/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/focusWindow.py` & `tabswitcher-0.1.9/src/tabswitcher/focusWindow.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.9/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.9/src/tabswitcher/loadBookmarks.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.9/src/tabswitcher/logTabs.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # Clear the history file
     if os.path.exists(tab_history_path):
         os.remove(tab_history_path)
 
     # define when to check the active tab and how often
     schedule.every(settings.get_tab_logging_interval()).seconds.do(check_active_tab)
 
-    if platform.system() == "Windows" and settings.get_use_hotkey():
+    if platform.system() == "Windows" and settings.get_use_hotkeys():
         import keyboard
         
         hotkey = settings.get_hotkey_open()
         keyboard.add_hotkey(hotkey, runTabSwitcher, suppress=True)
 
         hotkey = settings.get_hotkey_last()
         keyboard.add_hotkey(hotkey, focusLastTab, suppress=True)
```

### Comparing `tabswitcher-0.1.8/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.9/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.8/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.9/tabswitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.8/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.9/tabswitcher.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,13 +18,14 @@
 src/tabswitcher/shortcuts.py
 src/tabswitcher/assets/Icon.ico
 src/tabswitcher/assets/install.sh
 src/tabswitcher/assets/runLogger.vbs
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
 src/tabswitcher/assets/tabswitcher_service.xml
+src/tabswitcher/assets/uninstall.sh
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
 tabswitcher.egg-info/entry_points.txt
 tabswitcher.egg-info/requires.txt
 tabswitcher.egg-info/top_level.txt
```

