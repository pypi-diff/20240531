# Comparing `tmp/mpremote-1.22.0.tar.gz` & `tmp/mpremote-1.23.0.tar.gz`

## Comparing `mpremote-1.22.0.tar` & `mpremote-1.23.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/__main__.py
--rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/commands.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/console.py
--rw-r--r--   0        0        0    17020 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/main.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/mip.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/repl.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/transport.py
--rw-r--r--   0        0        0    39533 2020-02-02 00:00:00.000000 mpremote-1.22.0/mpremote/transport_serial.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mpremote-1.22.0/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 mpremote-1.22.0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mpremote-1.22.0/LICENSE
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 mpremote-1.22.0/README.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 mpremote-1.22.0/pyproject.toml
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 mpremote-1.22.0/PKG-INFO
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/__main__.py
+-rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/commands.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/console.py
+-rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/main.py
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/mip.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/repl.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/transport.py
+-rw-r--r--   0        0        0    39533 2020-02-02 00:00:00.000000 mpremote-1.23.0/mpremote/transport_serial.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mpremote-1.23.0/requirements.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 mpremote-1.23.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mpremote-1.23.0/LICENSE
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 mpremote-1.23.0/README.md
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 mpremote-1.23.0/pyproject.toml
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 mpremote-1.23.0/PKG-INFO
```

### Comparing `mpremote-1.22.0/mpremote/commands.py` & `mpremote-1.23.0/mpremote/commands.py`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/mpremote/console.py` & `mpremote-1.23.0/mpremote/console.py`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/mpremote/main.py` & `mpremote-1.23.0/mpremote/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         required=False,
         help="package index to use (defaults to micropython-lib)",
     )
     cmd_parser.add_argument("command", nargs=1, help="mip command (e.g. install)")
     cmd_parser.add_argument(
         "packages",
         nargs="+",
-        help="list package specifications, e.g. name, name@version, github:org/repo, github:org/repo@branch",
+        help="list package specifications, e.g. name, name@version, github:org/repo, github:org/repo@branch, gitlab:org/repo, gitlab:org/repo@branch",
     )
     return cmd_parser
 
 
 def argparse_none(description):
     return lambda: argparse.ArgumentParser(description=description)
```

### Comparing `mpremote-1.22.0/mpremote/mip.py` & `mpremote-1.23.0/mpremote/mip.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,26 @@
             + "/"
             + url[1]
             + "/"
             + branch
             + "/"
             + "/".join(url[2:])
         )
+    elif url.startswith("gitlab:"):
+        url = url[7:].split("/")
+        url = (
+            "https://gitlab.com/"
+            + url[0]
+            + "/"
+            + url[1]
+            + "/-/raw/"
+            + branch
+            + "/"
+            + "/".join(url[2:])
+        )
     return url
 
 
 def _download_file(transport, url, dest):
     try:
         with urllib.request.urlopen(url) as src:
             fd, path = tempfile.mkstemp()
@@ -112,14 +124,15 @@
 
 
 def _install_package(transport, package, index, target, version, mpy):
     if (
         package.startswith("http://")
         or package.startswith("https://")
         or package.startswith("github:")
+        or package.startswith("gitlab:")
     ):
         if package.endswith(".py") or package.endswith(".mpy"):
             print(f"Downloading {package} to {target}")
             _download_file(
                 transport, _rewrite_url(package, version), target + "/" + package.rsplit("/")[-1]
             )
             return
```

### Comparing `mpremote-1.22.0/mpremote/repl.py` & `mpremote-1.23.0/mpremote/repl.py`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/mpremote/transport.py` & `mpremote-1.23.0/mpremote/transport.py`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/mpremote/transport_serial.py` & `mpremote-1.23.0/mpremote/transport_serial.py`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/LICENSE` & `mpremote-1.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/README.md` & `mpremote-1.23.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,7 +76,8 @@
     mpremote ls
     mpremote cat boot.py
     mpremote cp :main.py .
     mpremote cp main.py :
     mpremote cp -r dir/ :
     mpremote mip install aioble
     mpremote mip install github:org/repo@branch
+    mpremote mip install gitlab:org/repo@branch
```

### Comparing `mpremote-1.22.0/pyproject.toml` & `mpremote-1.23.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpremote-1.22.0/PKG-INFO` & `mpremote-1.23.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mpremote
-Version: 1.22.0
+Version: 1.23.0
 Summary: Tool for interacting remotely with MicroPython devices
 Project-URL: Homepage, https://github.com/micropython/micropython
 Author-email: Damien George <damien@micropython.org>
 License: MIT
 License-File: LICENSE
 Keywords: hardware,micropython
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.4
-Requires-Dist: importlib-metadata>=1.4
+Requires-Dist: importlib-metadata>=1.4; python_version < '3.8'
 Requires-Dist: pyserial>=3.3
 Description-Content-Type: text/markdown
 
 # mpremote -- MicroPython remote control
 
 This CLI tool provides an integrated set of utilities to remotely interact with
 and automate a MicroPython device over a serial connection.
@@ -96,7 +96,8 @@
     mpremote ls
     mpremote cat boot.py
     mpremote cp :main.py .
     mpremote cp main.py :
     mpremote cp -r dir/ :
     mpremote mip install aioble
     mpremote mip install github:org/repo@branch
+    mpremote mip install gitlab:org/repo@branch
```

