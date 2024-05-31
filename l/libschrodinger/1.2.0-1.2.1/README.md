# Comparing `tmp/libschrodinger-1.2.0.tar.gz` & `tmp/libschrodinger-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.2.0.tar", last modified: Fri May 31 07:40:33 2024, max compression
+gzip compressed data, was "libschrodinger-1.2.1.tar", last modified: Fri May 31 07:53:53 2024, max compression
```

## Comparing `libschrodinger-1.2.0.tar` & `libschrodinger-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.418643 libschrodinger-1.2.0/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.2.0/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:40:33.417851 libschrodinger-1.2.0/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1298 2024-05-31 07:32:02.000000 libschrodinger-1.2.0/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.413306 libschrodinger-1.2.0/libschrodinger/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      859 2024-05-31 07:08:55.000000 libschrodinger-1.2.0/libschrodinger/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.2.0/libschrodinger/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      780 2024-05-31 07:18:53.000000 libschrodinger-1.2.0/libschrodinger/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.2.0/libschrodinger/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.2.0/libschrodinger/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:40:33.416751 libschrodinger-1.2.0/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/requires.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-31 07:40:33.000000 libschrodinger-1.2.0/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      850 2024-05-31 07:37:33.000000 libschrodinger-1.2.0/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-31 07:40:33.418815 libschrodinger-1.2.0/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:53:53.915348 libschrodinger-1.2.1/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.2.1/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:53:53.915017 libschrodinger-1.2.1/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1298 2024-05-31 07:32:02.000000 libschrodinger-1.2.1/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:53:53.912442 libschrodinger-1.2.1/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1000 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.2.1/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.2.1/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5046 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      793 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2825 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4710 2024-05-31 07:49:59.000000 libschrodinger-1.2.1/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      991 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2078 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-31 07:49:59.000000 libschrodinger-1.2.1/libschrodinger/potential.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      905 2024-05-31 07:49:50.000000 libschrodinger-1.2.1/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 07:53:53.914605 libschrodinger-1.2.1/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1962 2024-05-31 07:53:53.000000 libschrodinger-1.2.1/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-31 07:53:53.000000 libschrodinger-1.2.1/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-31 07:53:53.000000 libschrodinger-1.2.1/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-31 07:53:53.000000 libschrodinger-1.2.1/libschrodinger.egg-info/requires.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-31 07:53:53.000000 libschrodinger-1.2.1/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      850 2024-05-31 07:52:55.000000 libschrodinger-1.2.1/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-31 07:53:53.915429 libschrodinger-1.2.1/setup.cfg
```

### Comparing `libschrodinger-1.2.0/LICENSE` & `libschrodinger-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/PKG-INFO` & `libschrodinger-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.2.0/README.md` & `libschrodinger-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/libschrodinger/__init__.py` & `libschrodinger-1.2.1/libschrodinger/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Use links on the left for all functions and classes
 of the main package.
 
 Subpackages available:
 ---
 `libschrodinger.quark` - package related to quarks and particles composed of quarks
 """
+
 import libschrodinger.quark.hadron
 import libschrodinger.quark.baryon
 import libschrodinger.quark.meson
 import libschrodinger.quark.color
 import libschrodinger.quark.quark
 import libschrodinger.waveutils
 import libschrodinger.potential
@@ -23,9 +24,14 @@
 import libschrodinger.graphs
 import libschrodinger.constants
 import libschrodinger.config
 import libschrodinger.electron
 import libschrodinger.figlocation
 import libschrodinger.gauss
 from importlib.metadata import version
-__version__ = version('libschrodinger')
-print(f"Starting libschrodinger v{__version__}")
+
+try:
+    __version__ = version("libschrodinger")
+    print(f"Starting libschrodinger v{__version__}")
+except:
+    print("[WARNING] failed to fetch package metadata")
+    print("libschrodinger might be installed incorrectly...")
```

### Comparing `libschrodinger-1.2.0/libschrodinger/config.py` & `libschrodinger-1.2.1/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/libschrodinger/constants.py` & `libschrodinger-1.2.1/libschrodinger/constants.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/libschrodinger/electron.py` & `libschrodinger-1.2.1/libschrodinger/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,30 +123,32 @@
             )
             * self.config.dt
         )
         self.psi = np.fft.ifft2(self.psi)
         self.psi = self.psi * np.exp(-1j * (V) * self.config.dt / 2)
         if not (self.config.interactions_enabled):
             return
-        if ((frame * self.config.dt) % self.T > 0)\
-                and ((frame * self.config.dt) % self.T < 1)\
-                and self._cycle == 0:
+        if (
+            ((frame * self.config.dt) % self.T > 0)
+            and ((frame * self.config.dt) % self.T < 1)
+            and self._cycle == 0
+        ):
             if self.principal_quantum < 2:
                 # broke-ass electron, can't even afford a photon xd
                 return
             self._cycle = 1
             p = libschrodinger.gauss.WavePacket(
                 self.config,
                 0.3,
                 2,
                 2,
                 self.potential.x_center,
                 self.potential.y_center,
                 0,
-                self.config.Ly
+                self.config.Ly,
                 # The photon has to run 1 Ly in 1 dt of time
                 # No, Ly is not light-year. It's the width of the simulation.
             )
             particles.append(p)
             self._photon = p._id
             self.principal_quantum -= 1
             self.psi = self.calculate_psi(self.potential)
```

### Comparing `libschrodinger-1.2.0/libschrodinger/figlocation.py` & `libschrodinger-1.2.1/libschrodinger/figlocation.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 
     def spec(self) -> matplotlib.gridspec.SubplotSpec:
         """
         Creates a SubplotSpec which can then be passed to fig.add_subplot
         """
         return matplotlib.gridspec.SubplotSpec(
             # this is not a typo, matplotlib is stupid and has (y,x) coordinates
-            matplotlib.gridspec.GridSpec(self.y, self.x), self.num
+            matplotlib.gridspec.GridSpec(self.y, self.x),
+            self.num,
         )
```

### Comparing `libschrodinger-1.2.0/libschrodinger/gauss.py` & `libschrodinger-1.2.1/libschrodinger/gauss.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
         - `particles: list[libschrodinger.particle.Particle]`
             - an array of other particles
             for inter-particle interactions
 
         """
 
         self.psi = libschrodinger.waveutils.rollwave(
-            self.config, self.psi, self.vx, self.vy)
+            self.config, self.psi, self.vx, self.vy
+        )
 
         self.psi = self.psi * np.exp(-1j * (V) * self.config.dt / 2)
         self.psi = np.fft.fft2(self.psi)
         self.psi = self.psi * np.exp(
             -1j
             * (
                 np.fft.fftfreq(self.config.Nx, self.config.dx) ** 2
```

### Comparing `libschrodinger-1.2.0/libschrodinger/graphs.py` & `libschrodinger-1.2.1/libschrodinger/graphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 
     Defaults to None, in which case the graph doesn't display the frame number.
 
     Otherwise it displays the given frame number for this figure.
     """
 
     def __init__(
-        self, config: libschrodinger.config.Config, figsize=(12, 8), frameno: int | None = None
+        self,
+        config: libschrodinger.config.Config,
+        figsize=(12, 8),
+        frameno: int | None = None,
     ):
         self.config = config
         self.frameno = frameno
         self.fig = plt.figure(figsize=figsize)
 
     def save(self, filename: str):
         """Save the animation frame as an image file.
@@ -72,15 +75,19 @@
         """
         Draws the frame number on the graph.
 
         No need to call it, `GraphDisplay.save()` calls it automagically
             if `frameno` is not None
         """
         self.fig.text(
-            0, 0, "frame " + str(self.frameno), fontsize=10, **libschrodinger.constants.PLT_FONT
+            0,
+            0,
+            "frame " + str(self.frameno),
+            fontsize=10,
+            **libschrodinger.constants.PLT_FONT,
         )
 
     def add_figure(
         self,
         location: libschrodinger.figlocation.FigureLocation,
         function: np.array,
         title: str = "",
```

### Comparing `libschrodinger-1.2.0/libschrodinger/interaction.py` & `libschrodinger-1.2.1/libschrodinger/interaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,25 @@
 import libschrodinger.potential
 
 
 class Interactions:
     """
     Static class with methods for interactions between particles.
     """
-    def get_relative_potential(config: libschrodinger.config.Config,
-                               particle1: libschrodinger.particle.Particle,
-                               particle2: libschrodinger.particle.Particle) -> np.array:
+
+    def get_relative_potential(
+        config: libschrodinger.config.Config,
+        particle1: libschrodinger.particle.Particle,
+        particle2: libschrodinger.particle.Particle,
+    ) -> np.array:
         if not config.interactions_enabled:
             return np.zeros((config.Nx, config.Ny))
         if isinstance(particle1, libschrodinger.electron.Electron):
             if isinstance(particle2, libschrodinger.electron.Electron):
-                return - 0.2 * libschrodinger.potential.MeanFieldPotential(config, particle1).V * particle1.principal_quantum * particle2.principal_quantum
+                return (
+                    -0.2
+                    * libschrodinger.potential.MeanFieldPotential(config, particle1).V
+                    * particle1.principal_quantum
+                    * particle2.principal_quantum
+                )
 
         return np.zeros((config.Nx, config.Ny))
```

### Comparing `libschrodinger-1.2.0/libschrodinger/particle.py` & `libschrodinger-1.2.1/libschrodinger/particle.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
     def __init__(self, config):
         self.config = config
         self.psi = np.zeros((config.Nx, config.Ny))
         self._fig_opts = {}
 
     def propagate(
-        self, V: np.array, particles: list["libschrodinger.particle.Particle"], frame: int
+        self,
+        V: np.array,
+        particles: list["libschrodinger.particle.Particle"],
+        frame: int,
     ):
         """
         propagate the wave function in a potential field
 
         Parameters
         ----------
         - `V: np.array`
```

### Comparing `libschrodinger-1.2.0/libschrodinger/potential.py` & `libschrodinger-1.2.1/libschrodinger/potential.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/libschrodinger/waveutils.py` & `libschrodinger-1.2.1/libschrodinger/waveutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 
 import libschrodinger.config
 
 
-def rollwave(config: libschrodinger.config.Config, wave: np.array, vx: float, vy: float):
+def rollwave(
+    config: libschrodinger.config.Config, wave: np.array, vx: float, vy: float
+):
     """
     Move a wave linearily forward by `(vx, vy)` within experiment coordinates.
     Might not work well with small distances.
 
     Parameters
     ----------
     - `config: libschrodinger.config.Config`: the domain config
```

### Comparing `libschrodinger-1.2.0/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.2.1/libschrodinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.2.0/libschrodinger.egg-info/SOURCES.txt` & `libschrodinger-1.2.1/libschrodinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.0/pyproject.toml` & `libschrodinger-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libschrodinger"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="1p22geo", email="1p22geodecki@gmail.com" },
   { name="KacperTZSTI", email="kacper.m.trzop@gmail.com" },
 ]
 description = "A small package for simulating quantum-scale physics."
 readme = "README.md"
 requires-python = ">=3.8"
```

