# Comparing `tmp/libschrodinger-1.1.0.tar.gz` & `tmp/libschrodinger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.1.0.tar", last modified: Thu May 30 20:46:35 2024, max compression
+gzip compressed data, was "libschrodinger-1.2.0.tar", last modified: Fri May 31 07:40:33 2024, max compression
```

## Comparing `libschrodinger-1.1.0.tar` & `libschrodinger-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:46:35.248407 libschrodinger-1.1.0/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.1.0/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1513 2024-05-30 20:46:35.248075 libschrodinger-1.1.0/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.1.0/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:46:35.245321 libschrodinger-1.1.0/libschrodinger/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      247 2024-05-30 20:13:20.000000 libschrodinger-1.1.0/libschrodinger/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.1.0/libschrodinger/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.1.0/libschrodinger/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.1.0/libschrodinger/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:46:35.247658 libschrodinger-1.1.0/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1513 2024-05-30 20:46:35.000000 libschrodinger-1.1.0/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-30 20:46:35.000000 libschrodinger-1.1.0/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:46:35.000000 libschrodinger-1.1.0/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-30 20:46:35.000000 libschrodinger-1.1.0/libschrodinger.egg-info/requires.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:46:35.000000 libschrodinger-1.1.0/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      850 2024-05-30 20:46:13.000000 libschrodinger-1.1.0/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:46:35.248481 libschrodinger-1.1.0/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.418643 libschrodinger-1.2.0/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.2.0/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:40:33.417851 libschrodinger-1.2.0/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1298 2024-05-31 07:32:02.000000 libschrodinger-1.2.0/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.413306 libschrodinger-1.2.0/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      859 2024-05-31 07:08:55.000000 libschrodinger-1.2.0/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.2.0/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      780 2024-05-31 07:18:53.000000 libschrodinger-1.2.0/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.2.0/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/potential.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.416751 libschrodinger-1.2.0/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/requires.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      850 2024-05-31 07:37:33.000000 libschrodinger-1.2.0/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-31 07:40:33.418815 libschrodinger-1.2.0/setup.cfg
```

### Comparing `libschrodinger-1.1.0/LICENSE` & `libschrodinger-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/PKG-INFO` & `libschrodinger-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,71 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.1.0
+Version: 1.2.0
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 
-# A Python script to solve the Schrodinger's equation in a 2D domain.
+# A Python library/web app to simulate quantum-scale physics
+
+Features include (but not limited to):
+
+- create particles in a simulated environment
+- create potential fields to account for external forces
+- propagate particles (using the titular Schrödinger's equation)
+- draw and animate graphs
+- ~~access boundary error, core dumped~~ totally not run out of memory
+  - on the other hand, Python.
+
+# Library
+
+[examples](./examples/README.md)
+
+## Instalation
+
+```
+pip install --upgrade libschrodinger
+```
+
+# Web UI
 
 ![schreenshot showing app UI where people can create and edit particles](https://github.com/1p22geo/schrodinger/raw/master/static/media/png/screenshot.png)
 
 ## Static deployment
 
 [github pages](https://1p22geo.github.io/schrodinger)
 
 [docs](https://1p22geo.github.io/schrodinger/doc/)
 
-Includes everything except for the customizable experiment engine.
+Includes everything except for the user experiment engine.
 All static files and tutorials included.
 
 ## Deploying it yourself
 
 - Install python 3.10 or newer
 - First install the required libraries:
   - flask
   - numpy
   - scipy
   - matplotlib
 - Install [ffmpeg](https://ffmpeg.org)
 - Run the app
 
 ```shell
-$ python -m flask run
+$ python -m flask run -h 0.0.0.0
 ```
 
 ## Running tests
 
 All the dependencies for regular running are needed, together with `pytest`.
 
 Run in your terminal:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `libschrodinger-1.1.0/README.md` & `libschrodinger-1.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,54 @@
-# A Python script to solve the Schrodinger's equation in a 2D domain.
+# A Python library/web app to simulate quantum-scale physics
+
+Features include (but not limited to):
+
+- create particles in a simulated environment
+- create potential fields to account for external forces
+- propagate particles (using the titular Schrödinger's equation)
+- draw and animate graphs
+- ~~access boundary error, core dumped~~ totally not run out of memory
+  - on the other hand, Python.
+
+# Library
+
+[examples](./examples/README.md)
+
+## Instalation
+
+```
+pip install --upgrade libschrodinger
+```
+
+# Web UI
 
 ![schreenshot showing app UI where people can create and edit particles](https://github.com/1p22geo/schrodinger/raw/master/static/media/png/screenshot.png)
 
 ## Static deployment
 
 [github pages](https://1p22geo.github.io/schrodinger)
 
 [docs](https://1p22geo.github.io/schrodinger/doc/)
 
-Includes everything except for the customizable experiment engine.
+Includes everything except for the user experiment engine.
 All static files and tutorials included.
 
 ## Deploying it yourself
 
 - Install python 3.10 or newer
 - First install the required libraries:
   - flask
   - numpy
   - scipy
   - matplotlib
 - Install [ffmpeg](https://ffmpeg.org)
 - Run the app
 
 ```shell
-$ python -m flask run
+$ python -m flask run -h 0.0.0.0
 ```
 
 ## Running tests
 
 All the dependencies for regular running are needed, together with `pytest`.
 
 Run in your terminal:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `libschrodinger-1.1.0/libschrodinger/config.py` & `libschrodinger-1.2.0/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/constants.py` & `libschrodinger-1.2.0/libschrodinger/constants.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/electron.py` & `libschrodinger-1.2.0/libschrodinger/electron.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/figlocation.py` & `libschrodinger-1.2.0/libschrodinger/figlocation.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,9 +26,10 @@
         self.num = num
 
     def spec(self) -> matplotlib.gridspec.SubplotSpec:
         """
         Creates a SubplotSpec which can then be passed to fig.add_subplot
         """
         return matplotlib.gridspec.SubplotSpec(
-            matplotlib.gridspec.GridSpec(self.x, self.y), self.num
+            # this is not a typo, matplotlib is stupid and has (y,x) coordinates
+            matplotlib.gridspec.GridSpec(self.y, self.x), self.num
         )
```

### Comparing `libschrodinger-1.1.0/libschrodinger/gauss.py` & `libschrodinger-1.2.0/libschrodinger/gauss.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/graphs.py` & `libschrodinger-1.2.0/libschrodinger/graphs.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/interaction.py` & `libschrodinger-1.2.0/libschrodinger/interaction.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/particle.py` & `libschrodinger-1.2.0/libschrodinger/particle.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/potential.py` & `libschrodinger-1.2.0/libschrodinger/potential.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger/waveutils.py` & `libschrodinger-1.2.0/libschrodinger/waveutils.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.2.0/libschrodinger.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,71 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.1.0
+Version: 1.2.0
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 
-# A Python script to solve the Schrodinger's equation in a 2D domain.
+# A Python library/web app to simulate quantum-scale physics
+
+Features include (but not limited to):
+
+- create particles in a simulated environment
+- create potential fields to account for external forces
+- propagate particles (using the titular Schrödinger's equation)
+- draw and animate graphs
+- ~~access boundary error, core dumped~~ totally not run out of memory
+  - on the other hand, Python.
+
+# Library
+
+[examples](./examples/README.md)
+
+## Instalation
+
+```
+pip install --upgrade libschrodinger
+```
+
+# Web UI
 
 ![schreenshot showing app UI where people can create and edit particles](https://github.com/1p22geo/schrodinger/raw/master/static/media/png/screenshot.png)
 
 ## Static deployment
 
 [github pages](https://1p22geo.github.io/schrodinger)
 
 [docs](https://1p22geo.github.io/schrodinger/doc/)
 
-Includes everything except for the customizable experiment engine.
+Includes everything except for the user experiment engine.
 All static files and tutorials included.
 
 ## Deploying it yourself
 
 - Install python 3.10 or newer
 - First install the required libraries:
   - flask
   - numpy
   - scipy
   - matplotlib
 - Install [ffmpeg](https://ffmpeg.org)
 - Run the app
 
 ```shell
-$ python -m flask run
+$ python -m flask run -h 0.0.0.0
 ```
 
 ## Running tests
 
 All the dependencies for regular running are needed, together with `pytest`.
 
 Run in your terminal:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `libschrodinger-1.1.0/libschrodinger.egg-info/SOURCES.txt` & `libschrodinger-1.2.0/libschrodinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.1.0/pyproject.toml` & `libschrodinger-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libschrodinger"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="1p22geo", email="1p22geodecki@gmail.com" },
   { name="KacperTZSTI", email="kacper.m.trzop@gmail.com" },
 ]
 description = "A small package for simulating quantum-scale physics."
 readme = "README.md"
 requires-python = ">=3.8"
```

