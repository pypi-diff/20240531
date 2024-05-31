# Comparing `tmp/unreal-qt-0.0.1.tar.gz` & `tmp/unreal_qt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unreal-qt-0.0.1.tar", last modified: Tue Jul  4 14:53:11 2023, max compression
+gzip compressed data, was "unreal_qt-0.0.2.tar", last modified: Fri May 31 08:37:16 2024, max compression
```

## Comparing `unreal-qt-0.0.1.tar` & `unreal_qt-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.737172 unreal-qt-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.729172 unreal-qt-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.729172 unreal-qt-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 14:53:11.733172 unreal-qt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.733172 unreal-qt-0.0.1/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/basic_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/hello_world_unreal_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/slow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/samples/title_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:53:11.737172 unreal-qt-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.733172 unreal-qt-0.0.1/unreal_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/unreal_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-04 14:52:57.000000 unreal-qt-0.0.1/unreal_qt/dark_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:11.733172 unreal-qt-0.0.1/unreal_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 14:53:11.000000 unreal-qt-0.0.1/unreal_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-04 14:53:11.000000 unreal-qt-0.0.1/unreal_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:53:11.000000 unreal-qt-0.0.1/unreal_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 14:53:11.000000 unreal-qt-0.0.1/unreal_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 14:53:11.000000 unreal-qt-0.0.1/unreal_qt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.006461 unreal_qt-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.006461 unreal_qt-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.006461 unreal_qt-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/basic_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/hello_world_unreal_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/slow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/samples/title_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/unreal_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/unreal_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-31 08:37:11.000000 unreal_qt-0.0.2/unreal_qt/dark_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:16.010461 unreal_qt-0.0.2/unreal_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 08:37:15.000000 unreal_qt-0.0.2/unreal_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-31 08:37:16.000000 unreal_qt-0.0.2/unreal_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:37:15.000000 unreal_qt-0.0.2/unreal_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 08:37:15.000000 unreal_qt-0.0.2/unreal_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 08:37:15.000000 unreal_qt-0.0.2/unreal_qt.egg-info/top_level.txt
```

### Comparing `unreal-qt-0.0.1/.github/workflows/python-publish.yml` & `unreal_qt-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `unreal-qt-0.0.1/.gitignore` & `unreal_qt-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `unreal-qt-0.0.1/PKG-INFO` & `unreal_qt-0.0.2/docs/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-Metadata-Version: 2.1
-Name: unreal-qt
-Version: 0.0.1
-Summary: A Qt manager for Unreal that enables the use of PyQt & PySide in Unreal Engine
-Author: Hannes D
-Project-URL: Homepage, https://github.com/hannesdelbeke/unreal-qt
-Project-URL: Source, https://github.com/hannesdelbeke/unreal-qt
-Keywords: application,unreal,pyside,pyqt,qt,engine,unrealengine
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
+⚠️ This repo is for developers, artists and non-dev users can use the [Unreal Qt plugin](https://github.com/hannesdelbeke/unreal-qt-plugin) 
 
 # unreal qt
-QT PySide2 support for unreal engine 5 (likely works in unreal 4)
+QT PySide6 support for unreal engine 5 (likely works in unreal 4)
 - prevent widget from instantly dissapearing due to garbage collection
 - automatically style all Qt widgets using Xingyu Lei's [unreal_stylesheet](https://github.com/leixingyu/UnrealStylesheet)
 - dark window bar for a better visual match with Unreal
 - parent widget to Unreal's main window to stay on top
         
-
+## Install
+1. Copy the `unreal_qt` folder to Unreal's Python path. e.g. 
+- project `D:\Unreal Projects\MyProject\Content\Python\Lib`
+- or editor `D:\Program Files\Epic Games\UE_5.4\Engine\Binaries\ThirdParty\Python3\Win64\Lib\site-packages`
+2. Run the setup code on Unreal startup, e.g. with a plugin or `init_unreal.py` file. see [docs](https://dev.epicgames.com/documentation/en-us/unreal-engine/scripting-the-unreal-editor-using-python)
+  
 ## Quickstart
 
 this guide assumes you have PySide2 installed already!
 1. Add the unreal_qt folder in your python path. See [unreal docs](https://docs.unrealengine.com/4.27/en-US/ProductionPipelines/ScriptingAndAutomation/Python/#pythonpathsintheunrealeditor)
 2. Use the following code snippet to create `sample.py` and add it to unreal python path.
 ```python
 # 1. SETUP - this step can automatically run on editor startup when added to your init_unreal.py
 import unreal_qt
 unreal_qt.setup()  
 
 # 2. CREATE WIDGET - create your qt widget
 # every widget you make after setup won't block the editor & have unreal styling
-from PySide2.QtWidgets import QLabel, QWidget, QVBoxLayout
+from PySide6.QtWidgets import QLabel, QWidget, QVBoxLayout
 w = QWidget()
 layout = QVBoxLayout()
 w.setLayout(layout)
 layout.addWidget(QLabel("Hello World!"))
 
 # 3. WRAP WIDGET - (optional) manage garbage collection, add darkbar, stay on top
 unreal_qt.wrap(w)
@@ -45,14 +40,18 @@
 3. import script in unreal with the Python terminal to run it.
 ```python
 import sample
 ```
 
 ![image](https://user-images.githubusercontent.com/3758308/191580757-f3993797-da80-449e-b9d4-ad311b2f37c5.png)
 
+
+<details>
+ <summary>Dark title bar</summary>
+        
 ## Dark title bar
 The windows bar is by default white on Windows, and QT can't change the bar color.
 
 With unreal_qt you can add a custom bar.
 
 - default window bar & frame
 
@@ -62,14 +61,17 @@
 
 ![image](https://user-images.githubusercontent.com/3758308/191618309-13e7329f-4310-407a-9eef-383a113e1ac1.png)
 
 - custom bar, frame, no title bar (supports resize)
 
 ![image](https://user-images.githubusercontent.com/3758308/191618151-319b8530-addb-4b9a-a51f-5da0a90a4fd3.png)
 
+</details>
+
+
 
 ## community
 - tech-artists.org [PySide and Unreal5](https://discourse.techart.online/t/pyside-and-unreal5/15475/6) thread 
 - [ ]  TODO unreal forums thread
 
 ## similar to
 - https://github.com/FXTD-ODYSSEY/Unreal-PyToolkit
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unreal-qt-0.0.1/pyproject.toml` & `unreal_qt-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 requires-python = ">=3.4"
 keywords = ["application", "unreal", "pyside", "pyqt", "qt", "engine", "unrealengine"]
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
-dependencies = ['importlib-metadata; python_version<"3.7"']
+dependencies = ['importlib-metadata; python_version<"3.7"', "PySide6"]
 #dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `unreal-qt-0.0.1/samples/slow_task.py` & `unreal_qt-0.0.2/samples/slow_task.py`

 * *Files identical despite different names*

### Comparing `unreal-qt-0.0.1/samples/tick.py` & `unreal_qt-0.0.2/samples/tick.py`

 * *Files identical despite different names*

### Comparing `unreal-qt-0.0.1/samples/title_bar.py` & `unreal_qt-0.0.2/samples/title_bar.py`

 * *Files identical despite different names*

### Comparing `unreal-qt-0.0.1/unreal_qt/dark_bar.py` & `unreal_qt-0.0.2/unreal_qt/dark_bar.py`

 * *Files identical despite different names*

