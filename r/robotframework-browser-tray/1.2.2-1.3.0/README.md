# Comparing `tmp/robotframework_browser_tray-1.2.2.tar.gz` & `tmp/robotframework_browser_tray-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_browser_tray-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "robotframework_browser_tray-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `robotframework_browser_tray-1.2.2.tar` & `robotframework_browser_tray-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1852 2024-01-24 14:43:36.776726 robotframework_browser_tray-1.2.2/README.md
--rw-r--r--   0        0        0      712 2024-01-24 14:43:23.611699 robotframework_browser_tray-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-10 16:56:23.262179 robotframework_browser_tray-1.2.2/src/BrowserTray/__init__.py
--rw-r--r--   0        0        0       30 2024-01-24 13:54:57.652941 robotframework_browser_tray-1.2.2/src/BrowserTray/__main__.py
--rw-r--r--   0        0        0    56248 2024-01-24 14:02:11.777949 robotframework_browser_tray-1.2.2/src/BrowserTray/chromium.png
--rw-r--r--   0        0        0     4605 2024-01-24 14:01:32.138192 robotframework_browser_tray-1.2.2/src/BrowserTray/tray.py
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 robotframework_browser_tray-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2897 2024-05-31 12:31:14.544119 robotframework_browser_tray-1.3.0/README.md
+-rw-r--r--   0        0        0      795 2024-05-31 12:28:57.019749 robotframework_browser_tray-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2024-05-31 11:29:07.799831 robotframework_browser_tray-1.3.0/src/BrowserTray/BrowserRepl/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-31 12:25:56.237011 robotframework_browser_tray-1.3.0/src/BrowserTray/BrowserRepl/__main__.py
+-rw-r--r--   0        0        0      607 2024-05-31 11:25:54.994552 robotframework_browser_tray-1.3.0/src/BrowserTray/BrowserRepl/jsextension.js
+-rw-r--r--   0        0        0     1540 2024-05-31 11:57:04.748328 robotframework_browser_tray-1.3.0/src/BrowserTray/BrowserRepl/repl.py
+-rw-r--r--   0        0        0        0 2024-01-10 16:56:23.262179 robotframework_browser_tray-1.3.0/src/BrowserTray/__init__.py
+-rw-r--r--   0        0        0       30 2024-01-24 13:54:57.652941 robotframework_browser_tray-1.3.0/src/BrowserTray/__main__.py
+-rw-r--r--   0        0        0    56248 2024-01-24 14:02:11.777949 robotframework_browser_tray-1.3.0/src/BrowserTray/chromium.png
+-rw-r--r--   0        0        0     4605 2024-05-31 12:26:07.686769 robotframework_browser_tray-1.3.0/src/BrowserTray/tray.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 robotframework_browser_tray-1.3.0/PKG-INFO
```

### Comparing `robotframework_browser_tray-1.2.2/pyproject.toml` & `robotframework_browser_tray-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [project]
 name = "robotframework-browser-tray"
-version = "1.2.2"
+version = "1.3.0"
 description = "Tray icon to start the Chromium installed by Browser Library"
 authors = [
     {name = "Marduk Bolaños", email = "marduk.bolanos@imbus.de"},
 ]
 urls = { homepage = "https://github.com/mardukbp/robotframework-browser-tray" }
 
 dependencies = [
     "pystray>=0.19.5",
     "robotframework-browser>=18.0.0",
+    "robotframework-debug>=4.5.0",
 ]
 requires-python = ">=3.8.2"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 
 [tool.flit.module]
 name = "BrowserTray"
 
 [project.scripts]
 browser-tray = "BrowserTray.tray:run"
+ibrowser = "BrowserTray.BrowserRepl.repl:run"
 
 [build-system]
 requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [tool.pdm]
```

### Comparing `robotframework_browser_tray-1.2.2/src/BrowserTray/chromium.png` & `robotframework_browser_tray-1.3.0/src/BrowserTray/chromium.png`

 * *Files identical despite different names*

### Comparing `robotframework_browser_tray-1.2.2/src/BrowserTray/tray.py` & `robotframework_browser_tray-1.3.0/src/BrowserTray/tray.py`

 * *Files identical despite different names*

### Comparing `robotframework_browser_tray-1.2.2/PKG-INFO` & `robotframework_browser_tray-1.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,100 @@
-Metadata-Version: 2.1
-Name: robotframework-browser-tray
-Version: 1.2.2
-Summary: Tray icon to start the Chromium installed by Browser Library
-Author-email: Marduk Bolaños <marduk.bolanos@imbus.de>
-Requires-Python: >=3.8.2
-Description-Content-Type: text/markdown
-Requires-Dist: pystray>=0.19.5
-Requires-Dist: robotframework-browser>=18.0.0
-Project-URL: homepage, https://github.com/mardukbp/robotframework-browser-tray
-
-# robotframework-browser-tray
-
-A tray icon for starting the Chromium installed by [Browser Library](https://robotframework-browser.org/)
-
-**Requirements**
-
-- NodeJS >= 18
-- Windows
-
-
-## Use Cases
-
-- Execute tests incrementally using e.g. [RobotCode](https://github.com/d-biehl/robotcode)
-
-- Test selectors in an open web page interactively using [irobot](https://pypi.org/project/robotframework-debug/)
-
-
-## How to use it
-
-1. Install the package
-
-```bash
-pip install robotframework-browser-tray
-```
-
-2. Execute `browser-tray`
-
-**Hint**: In case your environment does not allow executing browser-tray, call the Python module directly:
-
-```bash
-python -m BrowserTray
-```
-
-3a. Click on the tray icon with the Chromium logo and select `Open Chromium`
-
-3b. If Microsoft Edge is installed on your machine:
-
-1. Close all instances of Microsoft Edge
-
-```powershell
-taskkill /F /IM msedge.exe
-```
-
-2. Start Microsoft Edge with `Windows + R`
-
-```powershell
-msedge.exe --remote-debugging-port=1234
-```
-
-4. Add these lines to the top of the .robot file with your tests:
-
-```robotframework
-Library       Browser               playwright_process_port=55555
-Test Setup    Connect To Browser    http://localhost:1234            chromium    use_cdp=True
-```
-
-In order to use other ports execute:
-
-```bash
-browser-tray --pw-port=XXXX --cdp-port=XXXX
-``` 
-
-## How it works
-
-On start up it checks whether `rfbrowser init chromium` has been executed in the current environment.
-
-If this requirement is met the Playwright wrapper is started with `node site-packages/Browser/wrapper/index.js 55555`.
-
-Selecting "Open Chromium" in the tray icon executes `site-packages/Browser/wrapper/node_modules/playwright-core/.local-browsers/chromium-XX/chrome-win/chrome.exe --remote-debugging-port=1234 --test-type`.
-
+# robotframework-browser-tray
+
+A tray icon for starting the Chromium installed by [Browser Library](https://robotframework-browser.org/)
+
+**Requirements**
+
+- NodeJS >= 18
+- Windows
+
+
+## Use Cases
+
+- Execute tests incrementally using e.g. [RobotCode](https://github.com/d-biehl/robotcode)
+
+- Test selectors in an open web page interactively using [irobot](https://pypi.org/project/robotframework-debug/)
+
+
+## How to use it
+
+1. Install the package
+
+```bash
+pip install robotframework-browser-tray
+```
+
+2. Execute `browser-tray`
+
+**Hint**: In case your environment does not allow executing browser-tray, call the Python module directly:
+
+```bash
+python -m BrowserTray
+```
+
+3. Click on the tray icon with the Chromium logo
+
+4. Open a Terminal and execute `ibrowser`
+
+**Hint**: In case your environment does not allow executing ibrowser, call the Python module directly:
+
+```bash
+python -m BrowserTray.BrowserRepl
+```
+
+### ibrowser
+
+ibrowser allows testing selectors in an open web page interactively. In addition to the selectors supported by Browser library,
+it adds the selector `role` for selecting elements using their ARIA role.
+
+The role of an element can be easily obtained from the Accessibility Tree. To open the tree follow these steps:
+
+1. Press F12 to open the DevTools
+2. Select the Elements tab
+3. In the right panel click on the Accessibility tab
+4. In the section "Accessibility Tree" check "Enable full-page accessibility tree"
+5. Click the button "Reload DevTools"
+6. In the left panel click on the person icon to toggle the Accessibility Tree view
+
+
+### Usage in a Robot Framework Test Suite
+
+Add these lines to the top of the .robot file:
+
+```robotframework
+Library       Browser               playwright_process_port=55555
+Test Setup    Connect To Browser    http://localhost:1234            chromium    use_cdp=True
+```
+
+In order to use other ports execute:
+
+```bash
+browser-tray --pw-port=XXXX --cdp-port=XXXX
+``` 
+
+
+### Using Microsoft Edge
+
+If Microsoft Edge is installed on your machine:
+
+1. Close all instances of Microsoft Edge
+
+```powershell
+taskkill /F /IM msedge.exe
+```
+
+2. Start Microsoft Edge with `Windows + R`
+
+```powershell
+msedge.exe --remote-debugging-port=1234
+```
+
+
+## How it works
+
+On start up it checks whether `rfbrowser init chromium` has been executed in the current environment.
+
+If this requirement is met the Playwright wrapper is started with `node site-packages/Browser/wrapper/index.js 55555`.
+
+Selecting "Open Chromium" in the tray icon executes `site-packages/Browser/wrapper/node_modules/playwright-core/.local-browsers/chromium-XX/chrome-win/chrome.exe --remote-debugging-port=1234 --test-type`.
+
+`ibrowser` is a batteries-included irobot that imports Browser library, connects to Chromium (if it is running) and adds some convenient selectors.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

